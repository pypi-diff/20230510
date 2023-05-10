# Comparing `tmp/libNeuroML-0.4.1.tar.gz` & `tmp/libNeuroML-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libNeuroML-0.4.1.tar", last modified: Mon Oct 17 14:53:29 2022, max compression
+gzip compressed data, was "libNeuroML-0.5.1.tar", last modified: Wed May 10 10:15:48 2023, max compression
```

## Comparing `libNeuroML-0.4.1.tar` & `libNeuroML-0.5.1.tar`

### file list

```diff
@@ -1,82 +1,70 @@
-drwxr-xr-x   0 padraig    (501) staff       (20)        0 2022-10-17 14:53:29.000000 libNeuroML-0.4.1/
--rw-r--r--   0 padraig    (501) staff       (20)      314 2017-01-07 12:43:01.000000 libNeuroML-0.4.1/AUTHORS
--rw-r--r--   0 padraig    (501) staff       (20)     1501 2017-01-07 12:43:01.000000 libNeuroML-0.4.1/LICENSE
--rw-r--r--   0 padraig    (501) staff       (20)      251 2019-11-06 11:28:50.000000 libNeuroML-0.4.1/MANIFEST.in
--rw-r--r--   0 padraig    (501) staff       (20)     6945 2022-10-17 14:53:29.000000 libNeuroML-0.4.1/PKG-INFO
--rw-r--r--   0 padraig    (501) staff       (20)     5051 2022-05-19 09:52:56.000000 libNeuroML-0.4.1/README.md
-drwxr-xr-x   0 padraig    (501) staff       (20)        0 2022-10-17 14:53:28.000000 libNeuroML-0.4.1/doc/
--rw-r--r--   0 padraig    (501) staff       (20)     5943 2022-10-13 16:12:26.000000 libNeuroML-0.4.1/doc/Makefile
--rw-r--r--   0 padraig    (501) staff       (20)    12803 2022-10-14 10:36:58.000000 libNeuroML-0.4.1/doc/conf.py
--rw-r--r--   0 padraig    (501) staff       (20)       41 2021-12-17 11:12:10.000000 libNeuroML-0.4.1/doc/requirements.txt
-drwxr-xr-x   0 padraig    (501) staff       (20)        0 2022-10-17 14:53:28.000000 libNeuroML-0.4.1/libNeuroML.egg-info/
--rw-r--r--   0 padraig    (501) staff       (20)     6945 2022-10-17 14:53:28.000000 libNeuroML-0.4.1/libNeuroML.egg-info/PKG-INFO
--rw-r--r--   0 padraig    (501) staff       (20)     2003 2022-10-17 14:53:28.000000 libNeuroML-0.4.1/libNeuroML.egg-info/SOURCES.txt
--rw-r--r--   0 padraig    (501) staff       (20)        1 2022-10-17 14:53:28.000000 libNeuroML-0.4.1/libNeuroML.egg-info/dependency_links.txt
--rw-r--r--   0 padraig    (501) staff       (20)       52 2022-10-17 14:53:28.000000 libNeuroML-0.4.1/libNeuroML.egg-info/requires.txt
--rw-r--r--   0 padraig    (501) staff       (20)        8 2022-10-17 14:53:28.000000 libNeuroML-0.4.1/libNeuroML.egg-info/top_level.txt
-drwxr-xr-x   0 padraig    (501) staff       (20)        0 2022-10-17 14:53:28.000000 libNeuroML-0.4.1/neuroml/
--rw-r--r--   0 padraig    (501) staff       (20)      259 2022-10-13 16:12:26.000000 libNeuroML-0.4.1/neuroml/__init__.py
--rw-r--r--   0 padraig    (501) staff       (20)      247 2022-10-13 16:12:26.000000 libNeuroML-0.4.1/neuroml/__version__.py
--rw-r--r--   0 padraig    (501) staff       (20)     9631 2021-12-17 11:12:10.000000 libNeuroML-0.4.1/neuroml/arraymorph.py
--rw-r--r--   0 padraig    (501) staff       (20)     1960 2021-12-17 11:12:10.000000 libNeuroML-0.4.1/neuroml/arraymorph_load_time_benchmark.py
-drwxr-xr-x   0 padraig    (501) staff       (20)        0 2022-10-17 14:53:28.000000 libNeuroML-0.4.1/neuroml/hdf5/
--rw-r--r--   0 padraig    (501) staff       (20)     7824 2021-12-17 11:12:10.000000 libNeuroML-0.4.1/neuroml/hdf5/DefaultNetworkHandler.py
--rw-r--r--   0 padraig    (501) staff       (20)    15739 2022-08-23 16:17:44.000000 libNeuroML-0.4.1/neuroml/hdf5/NetworkBuilder.py
--rw-r--r--   0 padraig    (501) staff       (20)    16653 2022-08-23 16:17:44.000000 libNeuroML-0.4.1/neuroml/hdf5/NetworkContainer.py
--rw-r--r--   0 padraig    (501) staff       (20)    29546 2022-08-23 16:17:44.000000 libNeuroML-0.4.1/neuroml/hdf5/NeuroMLHdf5Parser.py
--rw-r--r--   0 padraig    (501) staff       (20)    21712 2021-12-17 11:12:10.000000 libNeuroML-0.4.1/neuroml/hdf5/NeuroMLXMLParser.py
--rw-r--r--   0 padraig    (501) staff       (20)      618 2021-12-17 11:12:10.000000 libNeuroML-0.4.1/neuroml/hdf5/__init__.py
--rw-r--r--   0 padraig    (501) staff       (20)    12164 2022-10-13 16:12:26.000000 libNeuroML-0.4.1/neuroml/loaders.py
--rw-r--r--   0 padraig    (501) staff       (20)      589 2022-10-13 16:12:26.000000 libNeuroML-0.4.1/neuroml/neuro_lex_ids.py
-drwxr-xr-x   0 padraig    (501) staff       (20)        0 2022-10-17 14:53:28.000000 libNeuroML-0.4.1/neuroml/nml/
--rw-r--r--   0 padraig    (501) staff       (20)   137302 2020-04-08 18:07:10.000000 libNeuroML-0.4.1/neuroml/nml/NeuroML_v2.0.xsd
--rw-r--r--   0 padraig    (501) staff       (20)   137302 2021-03-22 15:36:59.000000 libNeuroML-0.4.1/neuroml/nml/NeuroML_v2.1.xsd
--rw-r--r--   0 padraig    (501) staff       (20)   169821 2021-12-17 11:12:10.000000 libNeuroML-0.4.1/neuroml/nml/NeuroML_v2.2.xsd
--rw-r--r--   0 padraig    (501) staff       (20)   175271 2022-09-05 11:47:42.000000 libNeuroML-0.4.1/neuroml/nml/NeuroML_v2.3.xsd
--rw-r--r--   0 padraig    (501) staff       (20)    73810 2017-01-07 12:43:01.000000 libNeuroML-0.4.1/neuroml/nml/NeuroML_v2beta1.xsd
--rw-r--r--   0 padraig    (501) staff       (20)    79479 2017-01-07 12:43:01.000000 libNeuroML-0.4.1/neuroml/nml/NeuroML_v2beta2.xsd
--rw-r--r--   0 padraig    (501) staff       (20)    84413 2017-01-07 12:43:01.000000 libNeuroML-0.4.1/neuroml/nml/NeuroML_v2beta3.xsd
--rw-r--r--   0 padraig    (501) staff       (20)   129617 2017-01-07 12:43:01.000000 libNeuroML-0.4.1/neuroml/nml/NeuroML_v2beta4.xsd
--rw-r--r--   0 padraig    (501) staff       (20)   137302 2019-11-06 11:28:50.000000 libNeuroML-0.4.1/neuroml/nml/NeuroML_v2beta5.xsd
--rw-r--r--   0 padraig    (501) staff       (20)        0 2017-01-07 12:43:01.000000 libNeuroML-0.4.1/neuroml/nml/__init__.py
--rw-r--r--   0 padraig    (501) staff       (20)     1994 2022-10-14 10:36:58.000000 libNeuroML-0.4.1/neuroml/nml/annotate_nml.py
--rw-r--r--   0 padraig    (501) staff       (20)       48 2021-12-17 11:12:10.000000 libNeuroML-0.4.1/neuroml/nml/config.py
--rw-r--r--   0 padraig    (501) staff       (20)     4535 2021-12-17 11:12:10.000000 libNeuroML-0.4.1/neuroml/nml/generateds_config.py
--rw-r--r--   0 padraig    (501) staff       (20)     1171 2022-10-14 10:36:58.000000 libNeuroML-0.4.1/neuroml/nml/generatedscollector.py
--rw-r--r--   0 padraig    (501) staff       (20)    23727 2022-10-13 16:12:26.000000 libNeuroML-0.4.1/neuroml/nml/generatedssupersuper.py
--rw-r--r--   0 padraig    (501) staff       (20)    90048 2022-10-13 16:12:26.000000 libNeuroML-0.4.1/neuroml/nml/helper_methods.py
--rw-r--r--   0 padraig    (501) staff       (20)  2323160 2022-10-14 10:36:58.000000 libNeuroML-0.4.1/neuroml/nml/nml.py
-drwxr-xr-x   0 padraig    (501) staff       (20)        0 2022-10-17 14:53:29.000000 libNeuroML-0.4.1/neuroml/test/
--rw-r--r--   0 padraig    (501) staff       (20)       56 2021-03-22 15:36:59.000000 libNeuroML-0.4.1/neuroml/test/README
--rw-r--r--   0 padraig    (501) staff       (20)        0 2017-01-07 12:43:01.000000 libNeuroML-0.4.1/neuroml/test/__init__.py
--rw-r--r--   0 padraig    (501) staff       (20)      137 2021-07-27 14:34:20.000000 libNeuroML-0.4.1/neuroml/test/__init__.pyc
--rw-r--r--   0 padraig    (501) staff       (20)      771 2021-12-17 11:12:10.000000 libNeuroML-0.4.1/neuroml/test/misc_tests.py
--rw-r--r--   0 padraig    (501) staff       (20)     1193 2021-07-27 14:34:20.000000 libNeuroML-0.4.1/neuroml/test/misc_tests.pyc
--rw-r--r--   0 padraig    (501) staff       (20)    14468 2021-12-17 11:12:10.000000 libNeuroML-0.4.1/neuroml/test/test_arraymorph.py
--rw-r--r--   0 padraig    (501) staff       (20)    15691 2021-07-27 14:34:20.000000 libNeuroML-0.4.1/neuroml/test/test_arraymorph.pyc
--rw-r--r--   0 padraig    (501) staff       (20)     6583 2022-08-23 16:17:44.000000 libNeuroML-0.4.1/neuroml/test/test_cell.py
--rw-r--r--   0 padraig    (501) staff       (20)     5598 2021-07-27 14:34:20.000000 libNeuroML-0.4.1/neuroml/test/test_cell.pyc
--rw-r--r--   0 padraig    (501) staff       (20)     2453 2021-12-17 11:12:10.000000 libNeuroML-0.4.1/neuroml/test/test_hdf5_optimized.py
--rw-r--r--   0 padraig    (501) staff       (20)     2336 2021-07-27 14:34:20.000000 libNeuroML-0.4.1/neuroml/test/test_hdf5_optimized.pyc
--rw-r--r--   0 padraig    (501) staff       (20)     2104 2021-12-17 11:12:10.000000 libNeuroML-0.4.1/neuroml/test/test_hdf5_parser.py
--rw-r--r--   0 padraig    (501) staff       (20)     2530 2021-07-27 14:34:20.000000 libNeuroML-0.4.1/neuroml/test/test_hdf5_parser.pyc
--rw-r--r--   0 padraig    (501) staff       (20)     1376 2021-12-17 11:12:10.000000 libNeuroML-0.4.1/neuroml/test/test_integration.py
--rw-r--r--   0 padraig    (501) staff       (20)     2217 2021-07-27 14:34:20.000000 libNeuroML-0.4.1/neuroml/test/test_integration.pyc
--rw-r--r--   0 padraig    (501) staff       (20)     1849 2022-10-13 16:12:26.000000 libNeuroML-0.4.1/neuroml/test/test_loaders.py
--rw-r--r--   0 padraig    (501) staff       (20)     1274 2021-07-27 14:34:20.000000 libNeuroML-0.4.1/neuroml/test/test_loaders.pyc
--rw-r--r--   0 padraig    (501) staff       (20)      684 2021-12-17 11:12:10.000000 libNeuroML-0.4.1/neuroml/test/test_morphology.py
--rw-r--r--   0 padraig    (501) staff       (20)     1440 2021-07-27 14:34:20.000000 libNeuroML-0.4.1/neuroml/test/test_morphology.pyc
--rw-r--r--   0 padraig    (501) staff       (20)    24218 2022-10-14 10:36:58.000000 libNeuroML-0.4.1/neuroml/test/test_nml.py
--rw-r--r--   0 padraig    (501) staff       (20)     7461 2022-08-23 16:17:44.000000 libNeuroML-0.4.1/neuroml/test/test_segment.py
--rw-r--r--   0 padraig    (501) staff       (20)     9713 2021-07-27 14:34:20.000000 libNeuroML-0.4.1/neuroml/test/test_segment.pyc
--rw-r--r--   0 padraig    (501) staff       (20)     1031 2022-10-13 16:12:26.000000 libNeuroML-0.4.1/neuroml/test/test_utils.py
--rw-r--r--   0 padraig    (501) staff       (20)     4176 2021-12-17 11:12:10.000000 libNeuroML-0.4.1/neuroml/test/test_writers.py
--rw-r--r--   0 padraig    (501) staff       (20)     8294 2021-07-27 14:34:20.000000 libNeuroML-0.4.1/neuroml/test/test_writers.pyc
--rw-r--r--   0 padraig    (501) staff       (20)     2100 2021-12-17 11:12:10.000000 libNeuroML-0.4.1/neuroml/test/test_xml_parser.py
--rw-r--r--   0 padraig    (501) staff       (20)     2970 2021-07-27 14:34:20.000000 libNeuroML-0.4.1/neuroml/test/test_xml_parser.pyc
--rw-r--r--   0 padraig    (501) staff       (20)        0 2020-06-12 12:28:03.000000 libNeuroML-0.4.1/neuroml/test/tmpfile
--rw-r--r--   0 padraig    (501) staff       (20)     7652 2022-10-13 16:12:26.000000 libNeuroML-0.4.1/neuroml/utils.py
--rw-r--r--   0 padraig    (501) staff       (20)     6112 2021-12-17 11:12:10.000000 libNeuroML-0.4.1/neuroml/writers.py
--rw-r--r--   0 padraig    (501) staff       (20)       61 2022-05-19 09:52:56.000000 libNeuroML-0.4.1/requirements.txt
--rw-r--r--   0 padraig    (501) staff       (20)      184 2022-10-17 14:53:29.000000 libNeuroML-0.4.1/setup.cfg
--rw-r--r--   0 padraig    (501) staff       (20)     1634 2022-10-13 16:12:26.000000 libNeuroML-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:15:48.215885 libNeuroML-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-10 10:15:48.215885 libNeuroML-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:15:48.207885 libNeuroML-0.5.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    12802 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:15:48.207885 libNeuroML-0.5.1/libNeuroML.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-10 10:15:48.000000 libNeuroML-0.5.1/libNeuroML.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-10 10:15:48.000000 libNeuroML-0.5.1/libNeuroML.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 10:15:48.000000 libNeuroML-0.5.1/libNeuroML.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-10 10:15:48.000000 libNeuroML-0.5.1/libNeuroML.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 10:15:48.000000 libNeuroML-0.5.1/libNeuroML.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:15:48.207885 libNeuroML-0.5.1/neuroml/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/arraymorph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/arraymorph_load_time_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:15:48.207885 libNeuroML-0.5.1/neuroml/hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/hdf5/DefaultNetworkHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15728 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/hdf5/NetworkBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16632 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/hdf5/NetworkContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29523 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/hdf5/NeuroMLHdf5Parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21689 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/hdf5/NeuroMLXMLParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/hdf5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/neuro_lex_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:15:48.211885 libNeuroML-0.5.1/neuroml/nml/
+-rw-r--r--   0 runner    (1001) docker     (123)   137302 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/NeuroML_v2.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   137302 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/NeuroML_v2.1.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   169821 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/NeuroML_v2.2.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   178637 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/NeuroML_v2.3.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    73810 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/NeuroML_v2beta1.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    79479 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/NeuroML_v2beta2.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    84413 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/NeuroML_v2beta3.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   129617 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/NeuroML_v2beta4.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)   137302 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/NeuroML_v2beta5.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/annotate_nml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/gds_imports-template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/generateds_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/generatedscollector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23753 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/generatedssupersuper.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107919 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2412988 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/nml/nml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:15:48.215885 libNeuroML-0.5.1/neuroml/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/README
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/misc_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_arraymorph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15013 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_hdf5_optimized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_hdf5_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25543 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_nml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_writers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/test/test_xml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/neuroml/writers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-10 10:15:48.215885 libNeuroML-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-10 10:15:37.000000 libNeuroML-0.5.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `libNeuroML-0.4.1/LICENSE` & `libNeuroML-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.4.1/PKG-INFO` & `libNeuroML-0.5.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,136 +1,159 @@
 Metadata-Version: 2.1
 Name: libNeuroML
-Version: 0.4.1
+Version: 0.5.1
 Summary: A Python library for working with NeuroML descriptions of neuronal models
 Home-page: http://libneuroml.readthedocs.org/en/latest/
 Author: libNeuroML authors and contributors
 Author-email: vellamike@gmail.com, p.gleeson@gmail.com
 License: BSD
-Description: ## Introduction
-        
-        [![GH Build](https://github.com/NeuralEnsemble/libNeuroML/actions/workflows/ci.yml/badge.svg)](https://github.com/NeuralEnsemble/libNeuroML/actions/workflows/ci.yml)
-        [![Documentation Status](https://readthedocs.org/projects/libneuroml/badge/?version=latest)](https://libneuroml.readthedocs.io/en/latest/?badge=latest)
-        [![PyPI](https://img.shields.io/pypi/v/libNeuroML)](https://pypi.org/project/libNeuroML/)
-        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/libNeuroML)](https://pypi.org/project/libNeuroML/)
-        [![GitHub](https://img.shields.io/github/license/NeuralEnsemble/libNeuroML)](https://github.com/NeuralEnsemble/libNeuroML/blob/master/LICENSE)
-        [![GitHub pull requests](https://img.shields.io/github/issues-pr/NeuralEnsemble/libNeuroML)](https://github.com/NeuralEnsemble/libNeuroML/pulls)
-        [![GitHub issues](https://img.shields.io/github/issues/NeuralEnsemble/libNeuroML)](https://github.com/NeuralEnsemble/libNeuroML/issues)
-        [![GitHub Org's stars](https://img.shields.io/github/stars/NeuralEnsemble?style=social)](https://github.com/NeuralEnsemble)
-        [![Twitter Follow](https://img.shields.io/twitter/follow/NeuroML?style=social)](https://twitter.com/NeuroML)
-        [![Gitter](https://badges.gitter.im/NeuroML/community.svg)](https://gitter.im/NeuroML/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
-        
-        This package provides Python libNeuroML, for working with neuronal models specified in [NeuroML 2](http://neuroml.org/neuromlv2).
-        
-        For more about libNeuroML see:
-        
-        Michael Vella, Robert C. Cannon, Sharon Crook, Andrew P. Davison, Gautham Ganapathy, Hugh P. C. Robinson, R. Angus Silver and Padraig Gleeson,
-        **libNeuroML and PyLEMS: using Python to combine procedural and declarative modeling approaches in computational neuroscience**
-        [Frontiers in Neuroinformatics 2014](http://journal.frontiersin.org/Journal/10.3389/fninf.2014.00038/abstract), doi: 10.3389/fninf.2014.00038
-        
-        _**PLEASE CITE THE PAPER ABOVE IF YOU USE libNeuroML!**_
-        
-        Documentation is available at http://readthedocs.org/docs/libneuroml/en/latest/
-        
-        For installation instructions, see http://readthedocs.org/docs/libneuroml/en/latest/install.html
-        
-        For an overview of all NeuroML related libraries/documentation/publications see https://docs.neuroml.org
-        
-        ## pyNeuroML
-        
-        A related package, **[pyNeuroML](https://github.com/NeuroML/pyNeuroML)** builds on this and provides functionality, scripts and modules for reading, writing, **simulating** and analysing NeuroML2/LEMS models.
-        
-        pyNeuroML builds on: [libNeuroML](https://github.com/NeuralEnsemble/libNeuroML) & [PyLEMS](https://github.com/LEMS/pylems) and wraps functionality from [jNeuroML](https://github.com/NeuroML/jNeuroML).
-        
-        
-        ## Development process for libNeuroML
-        
-        Most of the work happens in the [development branch](https://github.com/NeuralEnsemble/libNeuroML/tree/development).
-        That branch is kept up to date with the development branches for [NeuroML 2](https://github.com/NeuroML/NeuroML2/tree/development) and related libraries.
-        See https://docs.neuroml.org/ for an overview of the various NeuroML libraries.
-        
-        ## Changelog
-        ### version 0.2.57 (dev)
-        
-        - Enable Python 3.10 support
-        - Regenerate nml.py with generateDS using Python 3
-        - Add generic `add` method to all NeuroML ComponentType classes that allows users to easily construct their NeuroML documents.
-        - Improve unit tests
-        - DEPRECATION notice: `append_to_element` will be deprecated in future releases, please use the `add` method instead
-        
-        ### version 0.2.56
-        
-        - Documentation updates for RTD and other minor fixes.
-        
-        ### version 0.2.55
-        
-        - Patch release with minor changes under the hood.
-        - Use PyTest for testing.
-        - Enable CI on GitHub Actions
-        
-        ### version 0.2.54
-        
-        - Using Schema for NeuroML v2.1. Better compatibility with Python 3
-        
-        ### version 0.2.50
-        
-        - Updated to use the final stable Schema for NeuroML v2.0
-        
-        ### version 0.2.47
-        
-        - Updated to use the final stable Schema for NeuroML v2beta5
-        
-        ### version 0.2.18
-        
-        - Updated to use the final stable Schema for NeuroML v2beta4
-        - Tested with Python 3
-        
-        ### version 0.2.4
-        
-        - Updated to use the Schema for NeuroML v2beta4
-        
-        ### version 0.2.2
-        
-        - Updated to use the Schema for NeuroML v2beta3
-        - Ensures numpy & pytables are only required when using non-XML loaders/writers
-        
-        ### version 0.2.0
-        
-        - Updated to use the Schema for NeuroML v2beta2
-        
-        ### version 0.1.9
-        
-        - Minor release: Update to latest schema
-        
-        ### version 0.1.8
-        
-        - Several Bug fixes and small enhamcements
-        - Support for latest NeuroML schema (see change outline)
-        - JSON serialization
-        - MongoDB backend
-        - HDF5 serialization
-        - Improved installation process
-        - All usage examples are now run on the Travis-CI continuous integration server to confirm that that they do not error.
-        - Schema validation utility
-        - Improved documentation and documentation new look
-        
-        
-        :copyright: Copyright 2021 by the libNeuroML team, see [AUTHORS](AUTHORS). Modified BSD License, see [LICENSE](LICENSE) for details.
-        
-        
-        [![Build Status](https://api.travis-ci.org/NeuralEnsemble/libNeuroML.png)](https://travis-ci.org/NeuralEnsemble/libNeuroML)
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 Provides-Extra: full
+License-File: LICENSE
+License-File: AUTHORS
+
+## Introduction
+
+[![GH Build](https://github.com/NeuralEnsemble/libNeuroML/actions/workflows/ci.yml/badge.svg)](https://github.com/NeuralEnsemble/libNeuroML/actions/workflows/ci.yml)
+[![Documentation Status](https://readthedocs.org/projects/libneuroml/badge/?version=latest)](https://libneuroml.readthedocs.io/en/latest/?badge=latest)
+[![PyPI](https://img.shields.io/pypi/v/libNeuroML)](https://pypi.org/project/libNeuroML/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/libNeuroML)](https://pypi.org/project/libNeuroML/)
+[![GitHub](https://img.shields.io/github/license/NeuralEnsemble/libNeuroML)](https://github.com/NeuralEnsemble/libNeuroML/blob/master/LICENSE)
+[![GitHub pull requests](https://img.shields.io/github/issues-pr/NeuralEnsemble/libNeuroML)](https://github.com/NeuralEnsemble/libNeuroML/pulls)
+[![GitHub issues](https://img.shields.io/github/issues/NeuralEnsemble/libNeuroML)](https://github.com/NeuralEnsemble/libNeuroML/issues)
+[![GitHub Org's stars](https://img.shields.io/github/stars/NeuralEnsemble?style=social)](https://github.com/NeuralEnsemble)
+[![Twitter Follow](https://img.shields.io/twitter/follow/NeuroML?style=social)](https://twitter.com/NeuroML)
+[![Gitter](https://badges.gitter.im/NeuroML/community.svg)](https://gitter.im/NeuroML/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
+
+This package provides Python libNeuroML, for working with neuronal models specified in [NeuroML 2](http://neuroml.org/neuromlv2).
+
+For more about libNeuroML see:
+
+Michael Vella, Robert C. Cannon, Sharon Crook, Andrew P. Davison, Gautham Ganapathy, Hugh P. C. Robinson, R. Angus Silver and Padraig Gleeson,
+**libNeuroML and PyLEMS: using Python to combine procedural and declarative modeling approaches in computational neuroscience**
+[Frontiers in Neuroinformatics 2014](http://journal.frontiersin.org/Journal/10.3389/fninf.2014.00038/abstract), doi: 10.3389/fninf.2014.00038
+
+_**PLEASE CITE THE PAPER ABOVE IF YOU USE libNeuroML!**_
+
+Documentation is available at http://readthedocs.org/docs/libneuroml/en/latest/
+
+For installation instructions, see http://readthedocs.org/docs/libneuroml/en/latest/install.html
+
+For an overview of all NeuroML related libraries/documentation/publications see https://docs.neuroml.org
+
+## pyNeuroML
+
+A related package, **[pyNeuroML](https://github.com/NeuroML/pyNeuroML)** builds on this and provides functionality, scripts and modules for reading, writing, **simulating** and analysing NeuroML2/LEMS models.
+
+pyNeuroML builds on: [libNeuroML](https://github.com/NeuralEnsemble/libNeuroML) & [PyLEMS](https://github.com/LEMS/pylems) and wraps functionality from [jNeuroML](https://github.com/NeuroML/jNeuroML).
+
+
+## Development process for libNeuroML
+
+Most of the work happens in the [development branch](https://github.com/NeuralEnsemble/libNeuroML/tree/development).
+That branch is kept up to date with the development branches for [NeuroML 2](https://github.com/NeuroML/NeuroML2/tree/development) and related libraries.
+See https://docs.neuroml.org/ for an overview of the various NeuroML libraries.
+
+## Changelog
+### version 0.4.1
+
+- add multiple cell builder utility functions
+- performance improvements in generic helper functions
+- documentation fixes/improvements
+- add type annotations to all nml classes to aid users
+- add level 1 validation method
+- add generic component inspection methods
+
+### version 0.4.0
+
+- update to use schema version 2.3
+- drop python 2 support
+
+### version 0.3.1
+
+- include schema documentation in generated `nml.py` API
+- introduce generic methods to add child/children elements to components
+
+### version 0.2.58
+
+- multiple documentation fixes
+
+### version 0.2.57
+
+- Enable Python 3.10 support
+- Regenerate nml.py with generateDS using Python 3
+- Add generic `add` method to all NeuroML ComponentType classes that allows users to easily construct their NeuroML documents.
+- Improve unit tests
+- DEPRECATION notice: `append_to_element` will be deprecated in future releases, please use the `add` method instead
+
+### version 0.2.56
+
+- Documentation updates for RTD and other minor fixes.
+
+### version 0.2.55
+
+- Patch release with minor changes under the hood.
+- Use PyTest for testing.
+- Enable CI on GitHub Actions
+
+### version 0.2.54
+
+- Using Schema for NeuroML v2.1. Better compatibility with Python 3
+
+### version 0.2.50
+
+- Updated to use the final stable Schema for NeuroML v2.0
+
+### version 0.2.47
+
+- Updated to use the final stable Schema for NeuroML v2beta5
+
+### version 0.2.18
+
+- Updated to use the final stable Schema for NeuroML v2beta4
+- Tested with Python 3
+
+### version 0.2.4
+
+- Updated to use the Schema for NeuroML v2beta4
+
+### version 0.2.2
+
+- Updated to use the Schema for NeuroML v2beta3
+- Ensures numpy & pytables are only required when using non-XML loaders/writers
+
+### version 0.2.0
+
+- Updated to use the Schema for NeuroML v2beta2
+
+### version 0.1.9
+
+- Minor release: Update to latest schema
+
+### version 0.1.8
+
+- Several Bug fixes and small enhamcements
+- Support for latest NeuroML schema (see change outline)
+- JSON serialization
+- MongoDB backend
+- HDF5 serialization
+- Improved installation process
+- All usage examples are now run on the Travis-CI continuous integration server to confirm that that they do not error.
+- Schema validation utility
+- Improved documentation and documentation new look
+
+
+:copyright: Copyright 2023 by the libNeuroML team, see [AUTHORS](AUTHORS). Modified BSD License, see [LICENSE](LICENSE) for details.
+
```

### Comparing `libNeuroML-0.4.1/README.md` & `libNeuroML-0.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,38 @@
 ## Development process for libNeuroML
 
 Most of the work happens in the [development branch](https://github.com/NeuralEnsemble/libNeuroML/tree/development).
 That branch is kept up to date with the development branches for [NeuroML 2](https://github.com/NeuroML/NeuroML2/tree/development) and related libraries.
 See https://docs.neuroml.org/ for an overview of the various NeuroML libraries.
 
 ## Changelog
-### version 0.2.57 (dev)
+### version 0.4.1
+
+- add multiple cell builder utility functions
+- performance improvements in generic helper functions
+- documentation fixes/improvements
+- add type annotations to all nml classes to aid users
+- add level 1 validation method
+- add generic component inspection methods
+
+### version 0.4.0
+
+- update to use schema version 2.3
+- drop python 2 support
+
+### version 0.3.1
+
+- include schema documentation in generated `nml.py` API
+- introduce generic methods to add child/children elements to components
+
+### version 0.2.58
+
+- multiple documentation fixes
+
+### version 0.2.57
 
 - Enable Python 3.10 support
 - Regenerate nml.py with generateDS using Python 3
 - Add generic `add` method to all NeuroML ComponentType classes that allows users to easily construct their NeuroML documents.
 - Improve unit tests
 - DEPRECATION notice: `append_to_element` will be deprecated in future releases, please use the `add` method instead
 
@@ -102,11 +125,9 @@
 - HDF5 serialization
 - Improved installation process
 - All usage examples are now run on the Travis-CI continuous integration server to confirm that that they do not error.
 - Schema validation utility
 - Improved documentation and documentation new look
 
 
-:copyright: Copyright 2021 by the libNeuroML team, see [AUTHORS](AUTHORS). Modified BSD License, see [LICENSE](LICENSE) for details.
-
+:copyright: Copyright 2023 by the libNeuroML team, see [AUTHORS](AUTHORS). Modified BSD License, see [LICENSE](LICENSE) for details.
 
-[![Build Status](https://api.travis-ci.org/NeuralEnsemble/libNeuroML.png)](https://travis-ci.org/NeuralEnsemble/libNeuroML)
```

### Comparing `libNeuroML-0.4.1/doc/Makefile` & `libNeuroML-0.5.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.4.1/doc/conf.py` & `libNeuroML-0.5.1/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,16 +50,16 @@
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
-project = u"libNeuroML"
-copyright = u"2021, libNeuroML authors and contributors"
+project = "libNeuroML"
+copyright = "2023, libNeuroML authors and contributors"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = ""
@@ -74,15 +74,16 @@
 autodoc_class_signature = "mixed"
 autoclass_content = "class"
 
 # gds specific members to exclude from nml.py doc
 # grep -io "def gds_.*(" nml.py  | sed -e 's/def //' -e 's/($//' | sort -u | tr '\n' ',' | sed 's/,/, /g'
 # grep -io "def .*_(" nml.py  | sed -e 's/def //' -e 's/($//' | sort -u | tr '\n' ',' | sed 's/,/, /g'
 autodoc_default_options = {
-    "exclude-members": "build, buildAttributes, buildChildren, exportAttributes, export, exportChildren, factory, hasContent_, member_data_items_, subclass, superclass, warn_count, validate_allowedSpaces, validate_BlockTypes, validate_channelTypes, validate_DoubleGreaterThanZero, validate_gateTypes, validate_MetaId, validate_MetaId_patterns_, validate_Metric, validate_networkTypes, validate_NeuroLexId, validate_NeuroLexId_patterns_, validate_Nml2Quantity, validate_Nml2Quantity_capacitance, validate_Nml2Quantity_capacitance_patterns_, validate_Nml2Quantity_concentration, validate_Nml2Quantity_concentration_patterns_, validate_Nml2Quantity_conductance, validate_Nml2Quantity_conductanceDensity, validate_Nml2Quantity_conductanceDensity_patterns_, validate_Nml2Quantity_conductance_patterns_, validate_Nml2Quantity_conductancePerVoltage, validate_Nml2Quantity_conductancePerVoltage_patterns_, validate_Nml2Quantity_current, validate_Nml2Quantity_currentDensity, validate_Nml2Quantity_currentDensity_patterns_, validate_Nml2Quantity_current_patterns_, validate_Nml2Quantity_length, validate_Nml2Quantity_length_patterns_, validate_Nml2Quantity_none, validate_Nml2Quantity_none_patterns_, validate_Nml2Quantity_patterns_, validate_Nml2Quantity_permeability, validate_Nml2Quantity_permeability_patterns_, validate_Nml2Quantity_pertime, validate_Nml2Quantity_pertime_patterns_, validate_Nml2Quantity_resistance, validate_Nml2Quantity_resistance_patterns_, validate_Nml2Quantity_rhoFactor, validate_Nml2Quantity_rhoFactor_patterns_, validate_Nml2Quantity_specificCapacitance, validate_Nml2Quantity_specificCapacitance_patterns_, validate_Nml2Quantity_temperature, validate_Nml2Quantity_temperature_patterns_, validate_Nml2Quantity_time, validate_Nml2Quantity_time_patterns_, validate_Nml2Quantity_voltage, validate_Nml2Quantity_voltage_patterns_, validate_NmlId, validate_NmlId_patterns_, validate_NonNegativeInteger, validate_Notes, validate_PlasticityTypes, validate_populationTypes, validate_PositiveInteger, validate_ZeroOrOne, validate_ZeroToOne, gds_build_any, gds_check_cardinality_, gds_djo_etl_transform, gds_djo_etl_transform_db_obj, gds_encode, gds_format_base64, gds_format_boolean, gds_format_boolean_list, gds_format_date, gds_format_datetime, gds_format_decimal, gds_format_decimal_list, gds_format_double, gds_format_double_list, gds_format_float, gds_format_float_list, gds_format_integer, gds_format_integer_list, gds_format_string, gds_format_time, gds_get_node_lineno_, gds_parse_boolean, gds_parse_date, gds_parse_datetime, gds_parse_decimal, gds_parse_double, gds_parse_float, gds_parse_integer, gds_parse_string, gds_parse_time, gds_reverse_node_mapping, gds_sqa_etl_transform, gds_sqa_etl_transform_db_obj, gds_str_lower, gds_validate_base64, gds_validate_boolean, gds_validate_boolean_list, gds_validate_builtin_ST_, gds_validate_date, gds_validate_datetime, gds_validate_decimal, gds_validate_decimal_list, gds_validate_defined_ST_, gds_validate_double, gds_validate_double_list, gds_validate_float, gds_validate_float_list, gds_validate_integer, gds_validate_integer_list, gds_validate_simple_patterns, gds_validate_string, gds_validate_time, excl_select_objs_, find_attr_value_, gds_check_cardinality_, gds_get_node_lineno_, gds_validate_builtin_ST_, gds_validate_defined_ST_, get_all_text_, get_class_obj_, get_path_, get_path_list_, getSubclassFromModule_, parsexml_, parsexmlstring_, validate_, convert_unicode, Tag_strip_pattern_, tzoff_pattern"}
+    "exclude-members": "build, buildAttributes, buildChildren, exportAttributes, export, exportChildren, factory, hasContent_, member_data_items_, subclass, superclass, warn_count, validate_allowedSpaces, validate_BlockTypes, validate_channelTypes, validate_DoubleGreaterThanZero, validate_gateTypes, validate_MetaId, validate_MetaId_patterns_, validate_Metric, validate_networkTypes, validate_NeuroLexId, validate_NeuroLexId_patterns_, validate_Nml2Quantity, validate_Nml2Quantity_capacitance, validate_Nml2Quantity_capacitance_patterns_, validate_Nml2Quantity_concentration, validate_Nml2Quantity_concentration_patterns_, validate_Nml2Quantity_conductance, validate_Nml2Quantity_conductanceDensity, validate_Nml2Quantity_conductanceDensity_patterns_, validate_Nml2Quantity_conductance_patterns_, validate_Nml2Quantity_conductancePerVoltage, validate_Nml2Quantity_conductancePerVoltage_patterns_, validate_Nml2Quantity_current, validate_Nml2Quantity_currentDensity, validate_Nml2Quantity_currentDensity_patterns_, validate_Nml2Quantity_current_patterns_, validate_Nml2Quantity_length, validate_Nml2Quantity_length_patterns_, validate_Nml2Quantity_none, validate_Nml2Quantity_none_patterns_, validate_Nml2Quantity_patterns_, validate_Nml2Quantity_permeability, validate_Nml2Quantity_permeability_patterns_, validate_Nml2Quantity_pertime, validate_Nml2Quantity_pertime_patterns_, validate_Nml2Quantity_resistance, validate_Nml2Quantity_resistance_patterns_, validate_Nml2Quantity_rhoFactor, validate_Nml2Quantity_rhoFactor_patterns_, validate_Nml2Quantity_specificCapacitance, validate_Nml2Quantity_specificCapacitance_patterns_, validate_Nml2Quantity_temperature, validate_Nml2Quantity_temperature_patterns_, validate_Nml2Quantity_time, validate_Nml2Quantity_time_patterns_, validate_Nml2Quantity_voltage, validate_Nml2Quantity_voltage_patterns_, validate_NmlId, validate_NmlId_patterns_, validate_NonNegativeInteger, validate_Notes, validate_PlasticityTypes, validate_populationTypes, validate_PositiveInteger, validate_ZeroOrOne, validate_ZeroToOne, gds_build_any, gds_check_cardinality_, gds_djo_etl_transform, gds_djo_etl_transform_db_obj, gds_encode, gds_format_base64, gds_format_boolean, gds_format_boolean_list, gds_format_date, gds_format_datetime, gds_format_decimal, gds_format_decimal_list, gds_format_double, gds_format_double_list, gds_format_float, gds_format_float_list, gds_format_integer, gds_format_integer_list, gds_format_string, gds_format_time, gds_get_node_lineno_, gds_parse_boolean, gds_parse_date, gds_parse_datetime, gds_parse_decimal, gds_parse_double, gds_parse_float, gds_parse_integer, gds_parse_string, gds_parse_time, gds_reverse_node_mapping, gds_sqa_etl_transform, gds_sqa_etl_transform_db_obj, gds_str_lower, gds_validate_base64, gds_validate_boolean, gds_validate_boolean_list, gds_validate_builtin_ST_, gds_validate_date, gds_validate_datetime, gds_validate_decimal, gds_validate_decimal_list, gds_validate_defined_ST_, gds_validate_double, gds_validate_double_list, gds_validate_float, gds_validate_float_list, gds_validate_integer, gds_validate_integer_list, gds_validate_simple_patterns, gds_validate_string, gds_validate_time, excl_select_objs_, find_attr_value_, gds_check_cardinality_, gds_get_node_lineno_, gds_validate_builtin_ST_, gds_validate_defined_ST_, get_all_text_, get_class_obj_, get_path_, get_path_list_, getSubclassFromModule_, parsexml_, parsexmlstring_, validate_, convert_unicode, Tag_strip_pattern_, tzoff_pattern"
+}
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `libNeuroML-0.4.1/libNeuroML.egg-info/PKG-INFO` & `libNeuroML-0.5.1/libNeuroML.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,136 +1,159 @@
 Metadata-Version: 2.1
 Name: libNeuroML
-Version: 0.4.1
+Version: 0.5.1
 Summary: A Python library for working with NeuroML descriptions of neuronal models
 Home-page: http://libneuroml.readthedocs.org/en/latest/
 Author: libNeuroML authors and contributors
 Author-email: vellamike@gmail.com, p.gleeson@gmail.com
 License: BSD
-Description: ## Introduction
-        
-        [![GH Build](https://github.com/NeuralEnsemble/libNeuroML/actions/workflows/ci.yml/badge.svg)](https://github.com/NeuralEnsemble/libNeuroML/actions/workflows/ci.yml)
-        [![Documentation Status](https://readthedocs.org/projects/libneuroml/badge/?version=latest)](https://libneuroml.readthedocs.io/en/latest/?badge=latest)
-        [![PyPI](https://img.shields.io/pypi/v/libNeuroML)](https://pypi.org/project/libNeuroML/)
-        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/libNeuroML)](https://pypi.org/project/libNeuroML/)
-        [![GitHub](https://img.shields.io/github/license/NeuralEnsemble/libNeuroML)](https://github.com/NeuralEnsemble/libNeuroML/blob/master/LICENSE)
-        [![GitHub pull requests](https://img.shields.io/github/issues-pr/NeuralEnsemble/libNeuroML)](https://github.com/NeuralEnsemble/libNeuroML/pulls)
-        [![GitHub issues](https://img.shields.io/github/issues/NeuralEnsemble/libNeuroML)](https://github.com/NeuralEnsemble/libNeuroML/issues)
-        [![GitHub Org's stars](https://img.shields.io/github/stars/NeuralEnsemble?style=social)](https://github.com/NeuralEnsemble)
-        [![Twitter Follow](https://img.shields.io/twitter/follow/NeuroML?style=social)](https://twitter.com/NeuroML)
-        [![Gitter](https://badges.gitter.im/NeuroML/community.svg)](https://gitter.im/NeuroML/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
-        
-        This package provides Python libNeuroML, for working with neuronal models specified in [NeuroML 2](http://neuroml.org/neuromlv2).
-        
-        For more about libNeuroML see:
-        
-        Michael Vella, Robert C. Cannon, Sharon Crook, Andrew P. Davison, Gautham Ganapathy, Hugh P. C. Robinson, R. Angus Silver and Padraig Gleeson,
-        **libNeuroML and PyLEMS: using Python to combine procedural and declarative modeling approaches in computational neuroscience**
-        [Frontiers in Neuroinformatics 2014](http://journal.frontiersin.org/Journal/10.3389/fninf.2014.00038/abstract), doi: 10.3389/fninf.2014.00038
-        
-        _**PLEASE CITE THE PAPER ABOVE IF YOU USE libNeuroML!**_
-        
-        Documentation is available at http://readthedocs.org/docs/libneuroml/en/latest/
-        
-        For installation instructions, see http://readthedocs.org/docs/libneuroml/en/latest/install.html
-        
-        For an overview of all NeuroML related libraries/documentation/publications see https://docs.neuroml.org
-        
-        ## pyNeuroML
-        
-        A related package, **[pyNeuroML](https://github.com/NeuroML/pyNeuroML)** builds on this and provides functionality, scripts and modules for reading, writing, **simulating** and analysing NeuroML2/LEMS models.
-        
-        pyNeuroML builds on: [libNeuroML](https://github.com/NeuralEnsemble/libNeuroML) & [PyLEMS](https://github.com/LEMS/pylems) and wraps functionality from [jNeuroML](https://github.com/NeuroML/jNeuroML).
-        
-        
-        ## Development process for libNeuroML
-        
-        Most of the work happens in the [development branch](https://github.com/NeuralEnsemble/libNeuroML/tree/development).
-        That branch is kept up to date with the development branches for [NeuroML 2](https://github.com/NeuroML/NeuroML2/tree/development) and related libraries.
-        See https://docs.neuroml.org/ for an overview of the various NeuroML libraries.
-        
-        ## Changelog
-        ### version 0.2.57 (dev)
-        
-        - Enable Python 3.10 support
-        - Regenerate nml.py with generateDS using Python 3
-        - Add generic `add` method to all NeuroML ComponentType classes that allows users to easily construct their NeuroML documents.
-        - Improve unit tests
-        - DEPRECATION notice: `append_to_element` will be deprecated in future releases, please use the `add` method instead
-        
-        ### version 0.2.56
-        
-        - Documentation updates for RTD and other minor fixes.
-        
-        ### version 0.2.55
-        
-        - Patch release with minor changes under the hood.
-        - Use PyTest for testing.
-        - Enable CI on GitHub Actions
-        
-        ### version 0.2.54
-        
-        - Using Schema for NeuroML v2.1. Better compatibility with Python 3
-        
-        ### version 0.2.50
-        
-        - Updated to use the final stable Schema for NeuroML v2.0
-        
-        ### version 0.2.47
-        
-        - Updated to use the final stable Schema for NeuroML v2beta5
-        
-        ### version 0.2.18
-        
-        - Updated to use the final stable Schema for NeuroML v2beta4
-        - Tested with Python 3
-        
-        ### version 0.2.4
-        
-        - Updated to use the Schema for NeuroML v2beta4
-        
-        ### version 0.2.2
-        
-        - Updated to use the Schema for NeuroML v2beta3
-        - Ensures numpy & pytables are only required when using non-XML loaders/writers
-        
-        ### version 0.2.0
-        
-        - Updated to use the Schema for NeuroML v2beta2
-        
-        ### version 0.1.9
-        
-        - Minor release: Update to latest schema
-        
-        ### version 0.1.8
-        
-        - Several Bug fixes and small enhamcements
-        - Support for latest NeuroML schema (see change outline)
-        - JSON serialization
-        - MongoDB backend
-        - HDF5 serialization
-        - Improved installation process
-        - All usage examples are now run on the Travis-CI continuous integration server to confirm that that they do not error.
-        - Schema validation utility
-        - Improved documentation and documentation new look
-        
-        
-        :copyright: Copyright 2021 by the libNeuroML team, see [AUTHORS](AUTHORS). Modified BSD License, see [LICENSE](LICENSE) for details.
-        
-        
-        [![Build Status](https://api.travis-ci.org/NeuralEnsemble/libNeuroML.png)](https://travis-ci.org/NeuralEnsemble/libNeuroML)
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 Provides-Extra: full
+License-File: LICENSE
+License-File: AUTHORS
+
+## Introduction
+
+[![GH Build](https://github.com/NeuralEnsemble/libNeuroML/actions/workflows/ci.yml/badge.svg)](https://github.com/NeuralEnsemble/libNeuroML/actions/workflows/ci.yml)
+[![Documentation Status](https://readthedocs.org/projects/libneuroml/badge/?version=latest)](https://libneuroml.readthedocs.io/en/latest/?badge=latest)
+[![PyPI](https://img.shields.io/pypi/v/libNeuroML)](https://pypi.org/project/libNeuroML/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/libNeuroML)](https://pypi.org/project/libNeuroML/)
+[![GitHub](https://img.shields.io/github/license/NeuralEnsemble/libNeuroML)](https://github.com/NeuralEnsemble/libNeuroML/blob/master/LICENSE)
+[![GitHub pull requests](https://img.shields.io/github/issues-pr/NeuralEnsemble/libNeuroML)](https://github.com/NeuralEnsemble/libNeuroML/pulls)
+[![GitHub issues](https://img.shields.io/github/issues/NeuralEnsemble/libNeuroML)](https://github.com/NeuralEnsemble/libNeuroML/issues)
+[![GitHub Org's stars](https://img.shields.io/github/stars/NeuralEnsemble?style=social)](https://github.com/NeuralEnsemble)
+[![Twitter Follow](https://img.shields.io/twitter/follow/NeuroML?style=social)](https://twitter.com/NeuroML)
+[![Gitter](https://badges.gitter.im/NeuroML/community.svg)](https://gitter.im/NeuroML/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
+
+This package provides Python libNeuroML, for working with neuronal models specified in [NeuroML 2](http://neuroml.org/neuromlv2).
+
+For more about libNeuroML see:
+
+Michael Vella, Robert C. Cannon, Sharon Crook, Andrew P. Davison, Gautham Ganapathy, Hugh P. C. Robinson, R. Angus Silver and Padraig Gleeson,
+**libNeuroML and PyLEMS: using Python to combine procedural and declarative modeling approaches in computational neuroscience**
+[Frontiers in Neuroinformatics 2014](http://journal.frontiersin.org/Journal/10.3389/fninf.2014.00038/abstract), doi: 10.3389/fninf.2014.00038
+
+_**PLEASE CITE THE PAPER ABOVE IF YOU USE libNeuroML!**_
+
+Documentation is available at http://readthedocs.org/docs/libneuroml/en/latest/
+
+For installation instructions, see http://readthedocs.org/docs/libneuroml/en/latest/install.html
+
+For an overview of all NeuroML related libraries/documentation/publications see https://docs.neuroml.org
+
+## pyNeuroML
+
+A related package, **[pyNeuroML](https://github.com/NeuroML/pyNeuroML)** builds on this and provides functionality, scripts and modules for reading, writing, **simulating** and analysing NeuroML2/LEMS models.
+
+pyNeuroML builds on: [libNeuroML](https://github.com/NeuralEnsemble/libNeuroML) & [PyLEMS](https://github.com/LEMS/pylems) and wraps functionality from [jNeuroML](https://github.com/NeuroML/jNeuroML).
+
+
+## Development process for libNeuroML
+
+Most of the work happens in the [development branch](https://github.com/NeuralEnsemble/libNeuroML/tree/development).
+That branch is kept up to date with the development branches for [NeuroML 2](https://github.com/NeuroML/NeuroML2/tree/development) and related libraries.
+See https://docs.neuroml.org/ for an overview of the various NeuroML libraries.
+
+## Changelog
+### version 0.4.1
+
+- add multiple cell builder utility functions
+- performance improvements in generic helper functions
+- documentation fixes/improvements
+- add type annotations to all nml classes to aid users
+- add level 1 validation method
+- add generic component inspection methods
+
+### version 0.4.0
+
+- update to use schema version 2.3
+- drop python 2 support
+
+### version 0.3.1
+
+- include schema documentation in generated `nml.py` API
+- introduce generic methods to add child/children elements to components
+
+### version 0.2.58
+
+- multiple documentation fixes
+
+### version 0.2.57
+
+- Enable Python 3.10 support
+- Regenerate nml.py with generateDS using Python 3
+- Add generic `add` method to all NeuroML ComponentType classes that allows users to easily construct their NeuroML documents.
+- Improve unit tests
+- DEPRECATION notice: `append_to_element` will be deprecated in future releases, please use the `add` method instead
+
+### version 0.2.56
+
+- Documentation updates for RTD and other minor fixes.
+
+### version 0.2.55
+
+- Patch release with minor changes under the hood.
+- Use PyTest for testing.
+- Enable CI on GitHub Actions
+
+### version 0.2.54
+
+- Using Schema for NeuroML v2.1. Better compatibility with Python 3
+
+### version 0.2.50
+
+- Updated to use the final stable Schema for NeuroML v2.0
+
+### version 0.2.47
+
+- Updated to use the final stable Schema for NeuroML v2beta5
+
+### version 0.2.18
+
+- Updated to use the final stable Schema for NeuroML v2beta4
+- Tested with Python 3
+
+### version 0.2.4
+
+- Updated to use the Schema for NeuroML v2beta4
+
+### version 0.2.2
+
+- Updated to use the Schema for NeuroML v2beta3
+- Ensures numpy & pytables are only required when using non-XML loaders/writers
+
+### version 0.2.0
+
+- Updated to use the Schema for NeuroML v2beta2
+
+### version 0.1.9
+
+- Minor release: Update to latest schema
+
+### version 0.1.8
+
+- Several Bug fixes and small enhamcements
+- Support for latest NeuroML schema (see change outline)
+- JSON serialization
+- MongoDB backend
+- HDF5 serialization
+- Improved installation process
+- All usage examples are now run on the Travis-CI continuous integration server to confirm that that they do not error.
+- Schema validation utility
+- Improved documentation and documentation new look
+
+
+:copyright: Copyright 2023 by the libNeuroML team, see [AUTHORS](AUTHORS). Modified BSD License, see [LICENSE](LICENSE) for details.
+
```

### Comparing `libNeuroML-0.4.1/neuroml/arraymorph.py` & `libNeuroML-0.5.1/neuroml/arraymorph.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         connectivity=[],
         id=None,
         node_types=None,
         name=None,
         physical_mask=None,
         fractions_along=None,
     ):
-
         super(ArrayMorphology, self).__init__()
 
         self.connectivity = np.array(connectivity)
         self.vertices = np.array(vertices)
 
         self.id = id
 
@@ -168,15 +167,14 @@
         for i in self.connectivity:
             if i >= index:
                 self.connectivity[k] = i - 1
             k += 1
         pass
 
     def to_neuroml_morphology(self, id=""):
-
         morphology = neuroml.Morphology()
         morphology.id = id
 
         # need to traverse the tree:
         for index in range(self.num_vertices - 1):
             seg = self.segment_from_vertex_index(index)
             morphology.segments.append(seg)
@@ -251,15 +249,14 @@
 
     def __iadd__(self, segment_list):
         for segment in segment_list:
             self.append(segment)
         return self
 
     def __getitem__(self, segment_index):
-
         if segment_index in self.instantiated_segments:
             neuroml_segment = self.instantiated_segments[segment_index]
         else:
             vertex_index = self.__vertex_index_from_segment_index__(segment_index)
             neuroml_segment = self.arraymorph.segment_from_vertex_index(vertex_index)
             self.instantiated_segments[segment_index] = neuroml_segment
         return neuroml_segment
```

### Comparing `libNeuroML-0.4.1/neuroml/arraymorph_load_time_benchmark.py` & `libNeuroML-0.5.1/neuroml/arraymorph_load_time_benchmark.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.4.1/neuroml/hdf5/DefaultNetworkHandler.py` & `libNeuroML-0.5.1/neuroml/hdf5/DefaultNetworkHandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 #
 
 
 import logging
 
 
 class DefaultNetworkHandler:
-
     log = logging.getLogger("DefaultNetworkHandler")
 
     isParallel = 0
 
     #
     #  Internal info method, can be reused in overriding classes for debugging
     #
@@ -97,24 +96,22 @@
     def printInputInformation(self, inputName, population_id, component, size=-1):
         return self.print_input_information(inputName, population_id, component, size)
 
     #
     #  Should be overridden
     #
     def handle_document_start(self, id, notes):
-
         self.log.debug("Document: %s" % id)
         if notes:
             self.log.debug("  Notes: " + notes)
 
     #
     #  Should be overridden to create network
     #
     def handle_network(self, network_id, notes, temperature=None):
-
         self.log.debug("Network: %s" % network_id)
         if temperature:
             self.log.debug("  Temperature: " + temperature)
         if notes:
             self.log.debug("  Notes: " + notes)
 
     #
@@ -167,15 +164,14 @@
         synapse,
         hasWeights=False,
         hasDelays=False,
         type="projection",
         synapse_obj=None,
         pre_synapse_obj=None,
     ):
-
         synInfo = ""
         if synapse_obj:
             synInfo += " (syn: %s)" % synapse_obj.__class__.__name__
 
         if pre_synapse_obj:
             synInfo += " (pre comp: %s)" % pre_synapse_obj.__class__.__name__
 
@@ -206,15 +202,14 @@
         preSegId=0,
         preFract=0.5,
         postSegId=0,
         postFract=0.5,
         delay=0,
         weight=1,
     ):
-
         self.print_connection_information(
             projName, id, prePop, postPop, synapseType, preCellId, postCellId, weight
         )
         if preSegId != 0 or postSegId != 0 or preFract != 0.5 or postFract != 0.5:
             self.log.debug(
                 "Src cell: %d, seg: %f, fract: %f -> Tgt cell %d, seg: %f, fract: %f; weight %s, delay: %s ms"
                 % (
@@ -231,15 +226,14 @@
 
     #
     #  Should be overridden to handle end of network connection
     #
     def finalise_projection(
         self, projName, prePop, postPop, synapse=None, type="projection"
     ):
-
         self.log.debug(
             "Projection: "
             + projName
             + " from "
             + prePop
             + " to "
             + postPop
@@ -248,30 +242,28 @@
 
     #
     #  Should be overridden to create input source array
     #
     def handle_input_list(
         self, inputListId, population_id, component, size, input_comp_obj=None
     ):
-
         self.print_input_information(inputListId, population_id, component, size)
 
         if size < 0:
             self.log.error(
                 "Error! Need a size attribute in sites element to create spike source!"
             )
             return
 
     #
     #  Should be overridden to to connect each input to the target cell
     #
     def handle_single_input(
         self, inputListId, id, cellId, segId=0, fract=0.5, weight=1
     ):
-
         self.log.debug(
             "Input: %s[%s], cellId: %i, seg: %i, fract: %f, weight: %f"
             % (inputListId, id, cellId, segId, fract, weight)
         )
 
     #
     #  Should be overridden to to connect each input to the target cell
```

### Comparing `libNeuroML-0.4.1/neuroml/hdf5/NetworkBuilder.py` & `libNeuroML-0.5.1/neuroml/hdf5/NetworkBuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 from neuroml.hdf5.DefaultNetworkHandler import DefaultNetworkHandler
 
 import neuroml
 
 
 class NetworkBuilder(DefaultNetworkHandler):
-
     log = logging.getLogger("NetworkBuilder")
 
     populations = {}
     projections = {}
     projection_syns = {}
     projection_types = {}
     projection_syns_pre = {}
@@ -44,15 +43,14 @@
         if notes and len(notes) > 0:
             self.nml_doc.notes = notes
 
     #
     #  Overridden from DefaultNetworkHandler
     #
     def handle_network(self, network_id, notes, temperature=None):
-
         self.network = neuroml.Network(id=network_id)
         self.nml_doc.networks.append(self.network)
         if notes and len(notes) > 0:
             self.network.notes = notes
         if temperature is not None:
             self.network.temperature = temperature
             self.network.type = "networkWithTemperature"
@@ -65,15 +63,14 @@
         population_id,
         component,
         size,
         component_obj=None,
         properties={},
         notes=None,
     ):
-
         if component_obj:
             self.nml_doc.append(component_obj)
 
         pop = neuroml.Population(id=population_id, component=component, size=size)
 
         if notes and len(notes) > 0:
             pop.notes = notes
@@ -134,15 +131,14 @@
         synapse,
         hasWeights=False,
         hasDelays=False,
         type="projection",
         synapse_obj=None,
         pre_synapse_obj=None,
     ):
-
         if synapse_obj:
             self.nml_doc.append(synapse_obj)
         if pre_synapse_obj:
             self.nml_doc.append(pre_synapse_obj)
 
         proj = None
 
@@ -243,15 +239,14 @@
         preSegId=0,
         preFract=0.5,
         postSegId=0,
         postFract=0.5,
         delay=0,
         weight=1,
     ):
-
         # self.printConnectionInformation(proj_id, conn_id, prePop, postPop, synapseType, preCellId, postCellId, weight)
 
         pre_cell_path = "../%s/%i/%s" % (
             prePop,
             preCellId,
             self.populations[prePop].component,
         )
@@ -263,15 +258,14 @@
             postCellId,
             self.populations[postPop].component,
         )
         if self.populations[postPop].type == None:
             post_cell_path = "../%s[%i]" % (postPop, postCellId)
 
         if isinstance(self.projections[proj_id], neuroml.ElectricalProjection):
-
             instances = False
             if (
                 len(self.populations[prePop].instances) > 0
                 or len(self.populations[postPop].instances) > 0
             ):
                 instances = True
 
@@ -319,15 +313,14 @@
                     )
 
                     self.projections[proj_id].electrical_connection_instance_ws.append(
                         conn
                     )
 
         elif isinstance(self.projections[proj_id], neuroml.ContinuousProjection):
-
             instances = False
             if (
                 len(self.populations[prePop].instances) > 0
                 or len(self.populations[postPop].instances) > 0
             ):
                 instances = True
 
@@ -383,17 +376,15 @@
                     )
 
                     self.projections[proj_id].continuous_connection_instance_ws.append(
                         conn
                     )
 
         else:
-
             if not self.weightDelays[proj_id] and delay == 0 and weight == 1:
-
                 connection = neuroml.Connection(
                     id=conn_id,
                     pre_cell_id=pre_cell_path,
                     pre_segment_id=preSegId,
                     pre_fraction_along=preFract,
                     post_cell_id=post_cell_path,
                     post_segment_id=postSegId,
@@ -419,15 +410,14 @@
 
     #
     #  Overridden from DefaultNetworkHandler
     #
     def handle_input_list(
         self, inputListId, population_id, component, size, input_comp_obj=None
     ):
-
         if input_comp_obj:
             self.nml_doc.append(input_comp_obj)
 
         input_list = neuroml.InputList(
             id=inputListId, component=component, populations=population_id
         )
 
@@ -437,15 +427,14 @@
 
     #
     #  Overridden from DefaultNetworkHandler
     #
     def handle_single_input(
         self, inputListId, id, cellId, segId=0, fract=0.5, weight=1.0
     ):
-
         input_list = self.input_lists[inputListId]
         target_path = "../%s/%i/%s" % (
             input_list.populations,
             cellId,
             self.populations[input_list.populations].component,
         )
```

### Comparing `libNeuroML-0.4.1/neuroml/hdf5/NetworkContainer.py` & `libNeuroML-0.5.1/neuroml/hdf5/NetworkContainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,22 +4,20 @@
 """
 
 import neuroml
 import numpy as np
 
 
 class NetworkContainer(neuroml.Network):
-
     pass
     # def __getattr__(self,name):
     #    print('Requesting in NC: %s'%name)
 
 
 class OptimizedList(object):
-
     array = None
     cursor = 0
 
     def __init__(self, array=None, indices={}):
         self.array = array
         self.indices = indices
         # print("Created %s with %s"% (self,indices))
@@ -35,15 +33,14 @@
         if not name in self.indices:
             return default_value
         else:
             return self.array[i][self.indices[name]]
 
     def _add_index_information(self, hdf5_array):
         for name in self.indices.keys():
-
             n = "column_%i" % self.indices[name]
             # print("Adding attribute to H5 array: %s = %s"%(n,name))
             hdf5_array._f_setattr(n, name)
 
     def __len__(self):
         length = self.array.shape[0] if isinstance(self.array, np.ndarray) else 0
         # print('Getting length (%s) of %s'%(length,self.__class__.__name__,))
@@ -66,33 +63,29 @@
 
     def __iadd__(self, i_list):
         for i in i_list:
             self.append(i)
         return self
 
     def __delitem__(self, index):
-
         raise NotImplementedError(
             "__delitem__ is not implemented (yet) in HDF5 based optimized list"
         )
 
     def __setitem__(self, index, instance):
-
         raise NotImplementedError(
             "__setitem__() is not implemented (yet) in HDF5 based instance list"
         )
 
     def __str__(self):
-
         return "%s (optimized) with %s entries" % (self.__class__.__name__, len(self))
 
 
 class InstanceList(OptimizedList):
     def __getitem__(self, index):
-
         if len(self.array[index]) == 4:
             id = self.array[index][self._get_index_or_add("id", 0)]
             # print('    Getting instance %s in %s (%s)'%(index,self,id))
             assert id == index
         else:
             id = index
 
@@ -102,25 +95,23 @@
             y=self.array[index][self._get_index_or_add("y", 2)],
             z=self.array[index][self._get_index_or_add("z", 3)],
         )
 
         return instance
 
     def append(self, instance):
-
         # print('Adding instance: %s'%instance)
         l = instance.location
         i = np.array([[instance.id, l.x, l.y, l.z]], np.float32)
         if len(self) == 0:
             self.array = i
         else:
             self.array = np.concatenate((self.array, i))
 
     def add_instance(self, id, x, y, z):
-
         i = np.array([[id, x, y, z]], np.float32)
         if len(self) == 0:
             self.array = i
         else:
             self.array = np.concatenate((self.array, i))
 
 
@@ -156,15 +147,14 @@
         )
 
         self.instances = InstanceList()
 
         # print("PopulationContainer created")
 
     def __str__(self):
-
         return (
             "Population (optimized): "
             + str(self.id)
             + " with "
             + str(self.get_size())
             + " components of type "
             + (self.component if self.component else "???")
@@ -177,15 +167,14 @@
         popGroup._f_setattr("id", self.id)
         popGroup._f_setattr("component", self.component)
 
         for p in self.properties:
             popGroup._f_setattr("property:%s" % p.tag, p)
 
         if len(self.instances) > 0:
-
             popGroup._f_setattr("size", len(self.instances))
             popGroup._f_setattr("type", "populationList")
 
             h5array = h5file.create_carray(
                 popGroup,
                 self.id,
                 obj=self.instances.array,
@@ -205,15 +194,14 @@
         id=None,
         presynaptic_population=None,
         postsynaptic_population=None,
         synapse=None,
         connections=None,
         connection_wds=None,
     ):
-
         super(self.__class__, self).__init__(
             neuro_lex_id=neuro_lex_id,
             id=id,
             presynaptic_population=presynaptic_population,
             postsynaptic_population=postsynaptic_population,
             synapse=synapse,
             connections=connections,
@@ -268,15 +256,14 @@
         neuro_lex_id=None,
         id=None,
         presynaptic_population=None,
         postsynaptic_population=None,
         electrical_connections=None,
         electrical_connection_instances=None,
     ):
-
         super(self.__class__, self).__init__(
             neuro_lex_id=neuro_lex_id,
             id=id,
             presynaptic_population=presynaptic_population,
             postsynaptic_population=postsynaptic_population,
             electrical_connections=electrical_connections,
             electrical_connection_instances=electrical_connection_instances,
@@ -318,20 +305,18 @@
             title="Connections of cells in " + self.id,
         )
 
         self.connections._add_index_information(h5array)
 
 
 class ConnectionList(OptimizedList):
-
     presynaptic_population = None
     postsynaptic_population = None
 
     def __getitem__(self, index):
-
         id_index = self._get_index_or_add("id", -1)
         if id_index > 0:
             id = int(self.array[index][id_index])
             assert self.array[index][0] == index
         else:
             id = index
 
@@ -353,15 +338,14 @@
             pre_fraction_along=pre_fraction_along,
             post_fraction_along=post_fraction_along,
         )
 
         return input
 
     def append(self, conn):
-
         i = np.array(
             [[conn.id, conn.get_pre_cell_id(), conn.get_post_cell_id()]], np.float32
         )
 
         if len(self) == 0:
             self.array = i
         else:
@@ -383,15 +367,14 @@
         assert input == None
         self.input = InputsList()
         self.input.target_population = populations
 
         # print("InputListContainer %s created"%self.id)
 
     def __str__(self):
-
         return (
             "Input list (optimized): "
             + self.id
             + " to "
             + self.populations
             + ", component "
             + self.component
@@ -412,19 +395,17 @@
             title="Locations of inputs in " + self.id,
         )
 
         self.input._add_index_information(h5array)
 
 
 class InputsList(OptimizedList):
-
     target_population = None
 
     def __getitem__(self, index):
-
         # print('    Getting instance %s'%(index))
         # print self.array
 
         id = self.array[index][self._get_index_or_add("id", 0)]
         assert id == index
 
         target_cell_id = int(
@@ -442,15 +423,14 @@
             segment_id=segment_id,
             fraction_along=fraction_along,
         )
 
         return input
 
     def append(self, input):
-
         # print('Adding input: %s'%input)
 
         i = np.array(
             [
                 [
                     input.id,
                     input.get_target_cell_id(),
@@ -464,15 +444,14 @@
         if len(self) == 0:
             self.array = i
         else:
             self.array = np.concatenate((self.array, i))
 
 
 if __name__ == "__main__":
-
     from neuroml.loaders import read_neuroml2_file
 
     file_name = "../examples/test_files/MediumNet.net.nml"
 
     nml_doc = read_neuroml2_file(file_name, include_includes=True)
 
     print(nml_doc.summary())
```

### Comparing `libNeuroML-0.4.1/neuroml/hdf5/NeuroMLHdf5Parser.py` & `libNeuroML-0.5.1/neuroml/hdf5/NeuroMLHdf5Parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 
 from neuroml.loaders import read_neuroml2_string
 from neuroml.utils import add_all_to_document
 import os.path
 
 
 class NeuroMLHdf5Parser:
-
     log = logging.getLogger("NeuroMLHdf5Parser")
 
     currPopulation = ""
     currentComponent = ""
     totalInstances = 0
 
     currentProjectionId = ""
@@ -109,15 +108,14 @@
                 self.netHandler, "finaliseInputSource"
             ):
                 self.netHandler.finalise_input_source = (
                     self.netHandler.finaliseInputSource
                 )
 
     def parse(self, filename):
-
         h5file = tables.open_file(filename, mode="r")
 
         self.log.info(
             "Opened HDF5 file: %s; id=%s"
             % (h5file.filename, h5file.root.neuroml._v_attrs.id)
         )
 
@@ -142,22 +140,20 @@
             )
 
         self.parse_group(h5file.root.neuroml)
 
         h5file.close()
 
     def get_nml_doc(self):
-
         if not self.optimized:
             nml2_doc = nmlHandler.get_nml_doc()
             if self.nml_doc_extra_elements:
                 add_all_to_document(self.nml_doc_extra_elements, nml2_doc)
             return nml2_doc
         else:
-
             nml_doc = neuroml.NeuroMLDocument(id=self.doc_id, notes=self.doc_notes)
             if self.nml_doc_extra_elements:
                 add_all_to_document(self.nml_doc_extra_elements, nml_doc)
             nml_doc.networks.append(self.optimizedNetwork)
 
             return nml_doc
 
@@ -169,22 +165,20 @@
 
         self.start_group(g)
 
         # Note this ensures groups are parsed before datasets. Important for synapse props
 
         # Ensure populations parsed first!
         for node in g:
-
             if node._c_classid == "GROUP" and node._v_name.count("population_") >= 1:
                 self.log.debug("Sub node: " + str(node) + ", class: " + node._c_classid)
                 self.parse_group(node)
 
         # Non populations!
         for node in g:
-
             if node._c_classid == "GROUP" and node._v_name.count("population_") == 0:
                 self.log.debug(
                     "Sub node (ng): " + str(node) + ", class: " + node._c_classid
                 )
                 self.parse_group(node)
 
         for node in g:
@@ -192,19 +186,17 @@
 
             if self._is_dataset(node):
                 self.parse_dataset(node)
 
         self.end_group(g)
 
     def _extract_named_indices(self, d):
-
         named_indices = {}
 
         for attrName in d.attrs._v_attrnames:
-
             if "column_" in attrName:
                 val = d.attrs.__getattr__(attrName)
                 if isinstance(val, str):
                     name = val
                 else:
                     name = val[0]
 
@@ -224,15 +216,14 @@
                 + str(d.shape[0])
                 + " rows of: "
                 + str(d.shape[1])
                 + " entries"
             )
 
             if not self.optimized:
-
                 indexId = -1
                 indexX = -1
                 indexY = -1
                 indexZ = -1
 
                 for attrName in d.attrs._v_attrnames:
                     val = d.attrs.__getattr__(attrName)
@@ -262,25 +253,23 @@
                 if indexZ < 0:
                     if len(d[0]) == 3:
                         indexZ = 2
                     if len(d[0]) == 4:
                         indexY = 3
 
                 for i in range(0, d.shape[0]):
-
                     self.netHandler.handle_location(
                         int(d[i, indexId]) if indexId >= 0 else i,
                         self.currPopulation,
                         self.currentComponent,
                         float(d[i, indexX]),
                         float(d[i, indexY]),
                         float(d[i, indexZ]),
                     )
             else:
-
                 # TODO: a better way to convert???
                 a = np.array(d)
                 self.currOptPopulation.instances = InstanceList(
                     array=a, indices=self._extract_named_indices(d)
                 )
 
         elif self.currentProjectionId != "":
@@ -290,15 +279,14 @@
                 + str(d.shape[0])
                 + " rows of: "
                 + str(d.shape[1])
                 + " entries"
             )
 
             if not self.optimized:
-
                 indexId = -1
                 indexPreCellId = -1
                 indexPreSegId = -1
                 indexPreFractAlong = -1
                 indexPostCellId = -1
                 indexPostSegId = -1
                 indexPostFractAlong = -1
@@ -445,15 +433,14 @@
                 + str(d.shape[0])
                 + " rows of: "
                 + str(d.shape[1])
                 + " entries"
             )
 
             if not self.optimized:
-
                 indexId = -1
                 indexTargetCellId = -1
                 indexSegId = -1
                 indexFractAlong = -1
                 indexWeight = -1
 
                 segId = 0
@@ -475,15 +462,14 @@
                         indexSegId = int(attrName[len("column_") :])
                     elif val == "fraction_along" or val[0] == "fraction_along":
                         indexFractAlong = int(attrName[len("column_") :])
                     elif val == "weight" or val[0] == "weight":
                         indexWeight = int(attrName[len("column_") :])
 
                 for i in range(0, d.shape[0]):
-
                     if indexId >= 0:
                         id_ = int(d[i, indexId])
                     else:
                         id_ = i
 
                     tid = int(d[i, indexTargetCellId])
 
@@ -506,23 +492,21 @@
                         fract=fractAlong,
                         weight=weight,
                     )
 
                 self.netHandler.finalise_input_source(self.currInputList)
 
             else:
-
                 # TODO: a better way to convert???
                 a = np.array(d)
                 self.currOptInputList.input = InputsList(
                     array=a, indices=self._extract_named_indices(d)
                 )
 
     def _get_node_size(self, g, name):
-
         size = -1
         # Peek ahead for size...
         for node in g:
             if self._is_dataset(node) and node.name == name:
                 size = node.shape[0]
 
         if size == -1:
@@ -530,26 +514,24 @@
 
         return size
 
     def start_group(self, g):
         self.log.debug("Going into a group: " + g._v_name)
 
         if g._v_name == "neuroml":
-
             if not self.optimized:
                 self.netHandler.handle_document_start(
                     get_str_attribute_group(g, "id"),
                     get_str_attribute_group(g, "notes"),
                 )
             else:
                 self.doc_id = get_str_attribute_group(g, "id")
                 self.doc_notes = get_str_attribute_group(g, "notes")
 
         if g._v_name == "network":
-
             if not self.optimized:
                 self.netHandler.handle_network(
                     get_str_attribute_group(g, "id"),
                     get_str_attribute_group(g, "notes"),
                     temperature=get_str_attribute_group(g, "temperature"),
                 )
             else:
@@ -616,15 +598,14 @@
                     self.currOptPopulation.properties.append(
                         neuroml.Property(tag=p, value=properties[p])
                     )
 
                 self.optimizedNetwork.populations.append(self.currOptPopulation)
 
         if g._v_name.count("projection_") >= 1:
-
             self.currentProjectionId = get_str_attribute_group(g, "id")
             pt = get_str_attribute_group(g, "type")
             self.currentProjectionType = pt if pt else "projection"
             self.currentProjectionPrePop = get_str_attribute_group(
                 g, "presynapticPopulation"
             )
             self.currentProjectionPostPop = get_str_attribute_group(
@@ -646,15 +627,14 @@
                         self.currentProjectionId,
                         self.currentProjectionPrePop,
                         self.currentProjectionPostPop,
                         self.currentSynapse,
                     )
                 )
             else:
-
                 if self.currentProjectionType == "electricalProjection":
                     raise Exception(
                         "Cannot yet export electricalProjections to optimized HDF5 format"
                     )
                     self.currOptProjection = ElectricalProjectionContainer(
                         id=self.currentProjectionId,
                         presynaptic_population=self.currentProjectionPrePop,
@@ -662,15 +642,14 @@
                     )
 
                     self.optimizedNetwork.electrical_projections.append(
                         self.currOptProjection
                     )
 
                 elif self.currentProjectionType == "continuousProjection":
-
                     raise Exception(
                         "Cannot yet export continuousProjections to optimized HDF5 format"
                     )
 
                     self.optimizedNetwork.continuous_projections.append(
                         self.currOptProjection
                     )
@@ -735,15 +714,14 @@
                 + ", cell type: "
                 + self.currentComponent
             )
             self.currPopulation = ""
             self.currentComponent = ""
 
         if g._v_name.count("projection_") >= 1:
-
             if not self.optimized:
                 self.netHandler.finalise_projection(
                     self.currentProjectionId,
                     self.currentProjectionPrePop,
                     self.currentProjectionPostPop,
                     synapse=self.currentSynapse,
                     type=self.currentProjectionType,
@@ -757,15 +735,14 @@
             self.currentPreSynapse = ""
 
         if g._v_name.count("inputList_") >= 1 or g._v_name.count("input_list_") >= 1:
             self.currInputList = ""
 
 
 if __name__ == "__main__":
-
     file_name = "../examples/test_files/complete.nml.h5"
     # file_name = '../../../neuroConstruct/osb/showcase/NetPyNEShowcase/NeuroML2/scaling/Balanced.net.nml.h5'
 
     logging.basicConfig(
         level=logging.DEBUG, format="%(name)-19s %(levelname)-5s - %(message)s"
     )
```

### Comparing `libNeuroML-0.4.1/neuroml/hdf5/NeuroMLXMLParser.py` & `libNeuroML-0.5.1/neuroml/hdf5/NeuroMLXMLParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,26 @@
 #
 
 import logging
 import inspect
 
 
 class NeuroMLXMLParser:
-
     log = logging.getLogger("NeuroMLXMLParser")
 
     currPopulation = ""
     currentComponent = ""
     totalInstances = 0
 
     currentProjectionId = ""
     currentProjectionPrePop = ""
     currentProjectionPostPop = ""
     currentSynapse = ""
 
     def __init__(self, netHandler):
-
         self.netHandler = netHandler
 
         # For continued use with old API
         if not hasattr(self.netHandler, "handle_network") or hasattr(
             self.netHandler, "handleNetwork"
         ):
             self.netHandler.handle_network = self.netHandler.handleNetwork
@@ -82,45 +80,41 @@
         elif delay_string.endswith("s"):
             return float(delay_string[:-1].strip()) * 1000.0
         else:
             print("Can't parse string for delay: %s" % delay_string)
             exit(1)
 
     def parse(self, filename):
-
         print("Parsing: %s" % filename)
 
         import neuroml.loaders as loaders
 
         self.nml_doc = loaders.read_neuroml2_file(
             filename, include_includes=True, already_included=[]
         )
 
         print("Loaded: %s as NeuroMLDocument" % filename)
 
         self.netHandler.handle_document_start(self.nml_doc.id, self.nml_doc.notes)
 
         for network in self.nml_doc.networks:
-
             self.netHandler.handle_network(
                 network.id, network.notes, temperature=network.temperature
             )
 
             for population in network.populations:
-
                 component_obj = self.nml_doc.get_by_id(population.component)
                 properties = {}
                 for p in population.properties:
                     properties[p.tag] = p.value
 
                 if (
                     len(population.instances) > 0
                     and population.type == "populationList"
                 ):
-
                     # Try for Python3
                     try:
                         args = inspect.getfullargspec(
                             self.netHandler.handle_population
                         )[0]
                     except AttributeError:
                         # Fall back for Python 2
@@ -139,15 +133,14 @@
                             population.id,
                             population.component,
                             len(population.instances),
                             component_obj=component_obj,
                         )
 
                     for inst in population.instances:
-
                         loc = inst.location
                         self.netHandler.handle_location(
                             inst.id,
                             population.id,
                             population.component,
                             loc.x,
                             loc.y,
@@ -181,27 +174,25 @@
 
                     for i in range(population.size):
                         self.netHandler.handle_location(
                             i, population.id, population.component, None, None, None
                         )
 
             for projection in network.projections:
-
                 synapse_obj = self.nml_doc.get_by_id(projection.synapse)
 
                 self.netHandler.handle_projection(
                     projection.id,
                     projection.presynaptic_population,
                     projection.postsynaptic_population,
                     projection.synapse,
                     synapse_obj=synapse_obj,
                 )
 
                 for connection in projection.connections:
-
                     self.netHandler.handle_connection(
                         projection.id,
                         connection.id,
                         projection.presynaptic_population,
                         projection.postsynaptic_population,
                         projection.synapse,
                         preCellId=connection.get_pre_cell_id(),
@@ -211,15 +202,14 @@
                         preFract=float(connection.pre_fraction_along),
                         postFract=float(connection.post_fraction_along),
                         delay=0,
                         weight=1,
                     )
 
                 for connection in projection.connection_wds:
-
                     self.netHandler.handle_connection(
                         projection.id,
                         connection.id,
                         projection.presynaptic_population,
                         projection.postsynaptic_population,
                         projection.synapse,
                         preCellId=connection.get_pre_cell_id(),
@@ -229,15 +219,14 @@
                         preFract=float(connection.pre_fraction_along),
                         postFract=float(connection.post_fraction_along),
                         delay=self._parse_delay(connection.delay),
                         weight=float(connection.weight),
                     )
 
             for ep in network.electrical_projections:
-
                 synapse = None
 
                 for connection in ep.electrical_connections:
                     if synapse != None and synapse != connection.synapse:
                         raise Exception(
                             "There are different synapses for connections inside: %s!"
                             % ep
@@ -266,15 +255,14 @@
                     ep.postsynaptic_population,
                     synapse,
                     type="electricalProjection",
                     synapse_obj=synapse_obj,
                 )
 
                 for connection in ep.electrical_connections:
-
                     self.netHandler.handle_connection(
                         ep.id,
                         connection.id,
                         ep.presynaptic_population,
                         ep.postsynaptic_population,
                         connection.synapse,
                         preCellId=connection.get_pre_cell_id(),
@@ -282,15 +270,14 @@
                         preSegId=int(connection.pre_segment),
                         postSegId=int(connection.post_segment),
                         preFract=float(connection.pre_fraction_along),
                         postFract=float(connection.post_fraction_along),
                     )
 
                 for connection in ep.electrical_connection_instances:
-
                     self.netHandler.handle_connection(
                         ep.id,
                         connection.id,
                         ep.presynaptic_population,
                         ep.postsynaptic_population,
                         connection.synapse,
                         preCellId=connection.get_pre_cell_id(),
@@ -298,15 +285,14 @@
                         preSegId=int(connection.pre_segment),
                         postSegId=int(connection.post_segment),
                         preFract=float(connection.pre_fraction_along),
                         postFract=float(connection.post_fraction_along),
                     )
 
                 for connection in ep.electrical_connection_instance_ws:
-
                     self.netHandler.handle_connection(
                         ep.id,
                         connection.id,
                         ep.presynaptic_population,
                         ep.postsynaptic_population,
                         connection.synapse,
                         preCellId=connection.get_pre_cell_id(),
@@ -315,15 +301,14 @@
                         postSegId=int(connection.post_segment),
                         preFract=float(connection.pre_fraction_along),
                         postFract=float(connection.post_fraction_along),
                         weight=connection.get_weight(),
                     )
 
             for cp in network.continuous_projections:
-
                 pre_comp = None
                 post_comp = None
 
                 for connection in cp.continuous_connections:
                     if pre_comp != None and pre_comp != connection.pre_component:
                         raise Exception(
                             "There are different pre components for connections inside: %s!"
@@ -377,15 +362,14 @@
                     synapse,
                     type="continuousProjection",
                     pre_synapse_obj=pre_obj,
                     synapse_obj=post_obj,
                 )
 
                 for connection in cp.continuous_connections:
-
                     self.netHandler.handle_connection(
                         cp.id,
                         connection.id,
                         cp.presynaptic_population,
                         cp.postsynaptic_population,
                         synapseType=None,
                         preCellId=connection.get_pre_cell_id(),
@@ -393,15 +377,14 @@
                         preSegId=int(connection.pre_segment),
                         postSegId=int(connection.post_segment),
                         preFract=float(connection.pre_fraction_along),
                         postFract=float(connection.post_fraction_along),
                     )
 
                 for connection in cp.continuous_connection_instances:
-
                     self.netHandler.handle_connection(
                         cp.id,
                         connection.id,
                         cp.presynaptic_population,
                         cp.postsynaptic_population,
                         synapseType=None,
                         preCellId=connection.get_pre_cell_id(),
@@ -409,15 +392,14 @@
                         preSegId=int(connection.pre_segment),
                         postSegId=int(connection.post_segment),
                         preFract=float(connection.pre_fraction_along),
                         postFract=float(connection.post_fraction_along),
                     )
 
                 for connection in cp.continuous_connection_instance_ws:
-
                     self.netHandler.handle_connection(
                         cp.id,
                         connection.id,
                         cp.presynaptic_population,
                         cp.postsynaptic_population,
                         synapseType=None,
                         preCellId=connection.get_pre_cell_id(),
@@ -426,49 +408,45 @@
                         postSegId=int(connection.post_segment),
                         preFract=float(connection.pre_fraction_along),
                         postFract=float(connection.post_fraction_along),
                         weight=connection.get_weight(),
                     )
 
             for input_list in network.input_lists:
-
                 input_comp_obj = self.nml_doc.get_by_id(input_list.component)
 
                 self.netHandler.handle_input_list(
                     input_list.id,
                     input_list.populations,
                     input_list.component,
                     len(input_list.input),
                     input_comp_obj=input_comp_obj,
                 )
 
                 for input in input_list.input:
-
                     self.netHandler.handle_single_input(
                         input_list.id,
                         input.id,
                         cellId=input.get_target_cell_id(),
                         segId=input.get_segment_id(),
                         fract=input.get_fraction_along(),
                     )
                 for input_w in input_list.input_ws:
-
                     self.netHandler.handle_single_input(
                         input_list.id,
                         input_w.id,
                         cellId=input_w.get_target_cell_id(),
                         segId=input_w.get_segment_id(),
                         fract=input_w.get_fraction_along(),
                         weight=input_w.get_weight(),
                     )
 
                 self.netHandler.finalise_input_source(input_list.id)
 
             for explicitInput in network.explicit_inputs:
-
                 list_name = "INPUT_%s_%s" % (
                     explicitInput.input,
                     explicitInput.target.replace("[", "_").replace("]", "_"),
                 )
                 if list_name.endswith("_"):
                     list_name = list_name[:-1]
 
@@ -492,15 +470,14 @@
                     fract=0.5,
                 )
 
                 self.netHandler.finalise_input_source(list_name)
 
 
 if __name__ == "__main__":
-
     file_name = "../examples/tmp/testh5.nml"
 
     logging.basicConfig(
         level=logging.INFO, format="%(name)-19s %(levelname)-5s - %(message)s"
     )
 
     from neuroml.hdf5.DefaultNetworkHandler import DefaultNetworkHandler
```

### Comparing `libNeuroML-0.4.1/neuroml/loaders.py` & `libNeuroML-0.5.1/neuroml/loaders.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,23 +10,14 @@
 import warnings
 
 from typing import Callable, Optional
 
 supressGeneratedsWarnings = True
 
 
-def print_(text, verbose=True):
-    if verbose:
-        prefix = "libNeuroML >>> "
-        # if not isinstance(text, str): text = text.decode('ascii')
-        if verbose:
-
-            print("%s%s" % (prefix, text.replace("\n", "\n" + prefix)))
-
-
 class NeuroMLLoader(object):
     @classmethod
     def load(cls, src):
         doc = cls.__nml2_doc(src)
         if isinstance(doc, neuroml.nml.nml.NeuroMLDocument):
             return doc
         else:
@@ -35,15 +26,14 @@
                     src
                 )
             )
 
     @classmethod
     def __nml2_doc(cls, file_name):
         try:
-
             if supressGeneratedsWarnings:
                 warnings.simplefilter("ignore")
             nml2_doc = nmlparse(file_name, silence=True)
             if supressGeneratedsWarnings:
                 warnings.resetwarnings()
         except Exception as e:
             raise Exception("Not a valid NeuroML 2 doc (%s): %s" % (file_name, e), e)
@@ -64,22 +54,20 @@
         logging.basicConfig(
             level=logging.INFO, format="%(name)-19s %(levelname)-5s - %(message)s"
         )
 
         from neuroml.hdf5.NeuroMLHdf5Parser import NeuroMLHdf5Parser
 
         if optimized:
-
             currParser = NeuroMLHdf5Parser(None, optimized=True)
 
             currParser.parse(file_name)
 
             return currParser.get_nml_doc()
         else:
-
             from neuroml.hdf5.NetworkBuilder import NetworkBuilder
 
             nmlHandler = NetworkBuilder()
 
             currParser = NeuroMLHdf5Parser(nmlHandler)
 
             currParser.parse(file_name)
@@ -89,19 +77,26 @@
                 utils.add_all_to_document(currParser.nml_doc_extra_elements, nml2_doc)
 
             return nml2_doc
 
 
 class SWCLoader(object):
     """
-    WARNING: Class defunct
+    This class is deprecated and will be removed in a future release. Please
+    refer to https://docs.neuroml.org/Userdocs/ImportingMorphologyFiles.html
+    for information on importing/converting morphology files to NeuroML2.
     """
 
     @classmethod
     def load_swc_single(cls, src, name=None):
+        warnings.warn(
+            "This method/class is deprecated and will be removed in a future release. Please see https://docs.neuroml.org/Userdocs/ImportingMorphologyFiles.html",
+            FutureWarning,
+            stacklevel=2,
+        )
 
         import numpy as np
         from neuroml import arraymorph
 
         dtype = {
             "names": ("id", "type", "x", "y", "z", "r", "pid"),
             "formats": ("int32", "int32", "f4", "f4", "f4", "f4", "int32"),
@@ -150,15 +145,14 @@
             name=name,
         )
 
 
 class ArrayMorphLoader(object):
     @classmethod
     def __extract_morphology(cls, node):
-
         from neuroml import arraymorph
 
         loaded_morphology = arraymorph.ArrayMorphology()
         loaded_morphology.physical_mask = node.physical_mask[:]
         loaded_morphology.vertices = node.vertices[:]
         loaded_morphology.connectivity = node.connectivity[:]
 
@@ -169,15 +163,14 @@
         """
         Right now this load method isn't done in a very nice way.
         TODO: Complete refactoring.
         """
         import tables
 
         with tables.open_file(filepath, mode="r") as file:
-
             document = neuroml.NeuroMLDocument()
 
             for node in file.root:
                 if hasattr(node, "vertices"):
                     loaded_morphology = cls.__extract_morphology(node)
                     document.morphology.append(loaded_morphology)
                 else:
@@ -189,15 +182,15 @@
 
 
 def read_neuroml2_file(
     nml2_file_name: str,
     include_includes: bool = False,
     verbose: bool = False,
     already_included: list = None,
-    print_method: Callable = print_,
+    print_method: Callable = neuroml.print_,
     optimized: bool = False,
 ) -> neuroml.nml.nml.NeuroMLDocument:
     """
     Read a NeuroML2 file into a NeuroMLDocument object
 
     :param nml2_file_name: name of NeuroML file to read
     :type nml2_file_name: str
@@ -234,15 +227,15 @@
 
 
 def read_neuroml2_string(
     nml2_string: str,
     include_includes: bool = False,
     verbose: bool = False,
     already_included: list = [],
-    print_method: Callable = print_,
+    print_method: Callable = neuroml.print_,
     optimized: bool = False,
     base_path: Optional[str] = None,
 ) -> neuroml.nml.nml.NeuroMLDocument:
     """
     Read a NeuroML2 string into a NeuroMLDocument object
 
     :param nml2_string: NeuroML string to load
@@ -277,15 +270,15 @@
 
 
 def _read_neuroml2(
     nml2_file_name_or_string: str,
     include_includes: bool = False,
     verbose: bool = False,
     already_included: list = [],
-    print_method: Callable = print_,
+    print_method: Callable = neuroml.print_,
     optimized: bool = False,
     base_path: Optional[str] = None,
 ) -> neuroml.nml.nml.NeuroMLDocument:
     """
     Read a NeuroML2 file or string into a NeuroMLDocument object.
 
     Internal method, please use `read_neuroml2_file` or `read_neuroml2_string`
@@ -333,15 +326,15 @@
         nml2_doc = NeuroMLLoader.load(nml2_file_name_or_string)
 
     if supressGeneratedsWarnings:
         warnings.resetwarnings()
 
     if include_includes:
         print_method(
-            "Including included files (included already: %s)" % already_included,
+            "Including the included files (included already: %s)" % already_included,
             verbose,
         )
 
         for include in nml2_doc.includes:
             incl_loc = os.path.abspath(os.path.join(base_path_to_use, include.href))
             if incl_loc not in already_included:
                 print_method(
@@ -369,21 +362,19 @@
                     raise Exception("Unrecognised extension on file: %s" % incl_loc)
 
         nml2_doc.includes = []
 
     else:
         if len(nml2_doc.includes) > 0:
             print_method(
-                "NOT including included files, even though %s are included!"
+                "NOT processing included files, even though %s are included!"
                 % len(nml2_doc.includes),
                 verbose,
             )
 
-        nml2_doc.includes = []
-
     return nml2_doc
 
 
 if __name__ == "__main__":
     f = sys.argv[1]
     nml_doc = read_neuroml2_file(f)
     print("Read in %s" % f)
```

### Comparing `libNeuroML-0.4.1/neuroml/neuro_lex_ids.py` & `libNeuroML-0.5.1/neuroml/neuro_lex_ids.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 """
 NeuroLex Ids
 
 File: neuroml/neuro_lex_ids.py
 
-Copyright 2022 NeuroML contributors
+Copyright 2023 NeuroML contributors
 """
 
 neuro_lex_ids = {
     # https://scicrunch.org/scicrunch/interlex/view/ilx_0101043?searchTerm=GO:0030424
     "axon": "GO:0030424",
     # https://scicrunch.org/scicrunch/interlex/view/ilx_0103021?searchTerm=GO:0030425
     "dend": "GO:0030425",
```

### Comparing `libNeuroML-0.4.1/neuroml/nml/NeuroML_v2.0.xsd` & `libNeuroML-0.5.1/neuroml/nml/NeuroML_v2.0.xsd`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.4.1/neuroml/nml/NeuroML_v2.1.xsd` & `libNeuroML-0.5.1/neuroml/nml/NeuroML_v2.1.xsd`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.4.1/neuroml/nml/NeuroML_v2.2.xsd` & `libNeuroML-0.5.1/neuroml/nml/NeuroML_v2.2.xsd`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.4.1/neuroml/nml/NeuroML_v2.3.xsd` & `libNeuroML-0.5.1/neuroml/nml/NeuroML_v2.3.xsd`

 * *Files 2% similar despite different names*

#### Comparing `libNeuroML-0.4.1/neuroml/nml/NeuroML_v2.3.xsd` & `libNeuroML-0.5.1/neuroml/nml/NeuroML_v2.3.xsd`

```diff
@@ -219,14 +219,15 @@
   <xs:complexType name="ComponentType">
     <xs:annotation>
       <xs:documentation>Contains an extension to NeuroML by creating custom LEMS ComponentType.</xs:documentation>
     </xs:annotation>
     <xs:sequence>
       <xs:element name="Property" type="LEMS_Property" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="Parameter" type="Parameter" minOccurs="0" maxOccurs="unbounded"/>
+      <xs:element name="DerivedParameter" type="DerivedParameter" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="Constant" type="Constant" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="Exposure" type="Exposure" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="Requirement" type="Requirement" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="InstanceRequirement" type="InstanceRequirement" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="Dynamics" type="Dynamics" minOccurs="0" maxOccurs="unbounded"/>
     </xs:sequence>
     <xs:attribute name="name" type="xs:string" use="required"/>
@@ -281,14 +282,24 @@
   </xs:complexType>
   <xs:complexType name="Parameter">
     <!-- For language binding generators, so there will be a class of this name... -->
     <xs:complexContent>
       <xs:extension base="NamedDimensionalType"/>
     </xs:complexContent>
   </xs:complexType>
+  <xs:complexType name="DerivedParameter">
+    <xs:annotation>
+      <xs:documentation>LEMS DerivedParamter element</xs:documentation>
+    </xs:annotation>
+    <xs:complexContent>
+      <xs:extension base="NamedDimensionalType">
+        <xs:attribute name="value" type="xs:string" use="required"/>
+      </xs:extension>
+    </xs:complexContent>
+  </xs:complexType>
   <xs:complexType name="LEMS_Property">
     <xs:complexContent>
       <xs:extension base="NamedDimensionalType">
         <xs:attribute name="defaultValue" type="xs:double" use="optional"/>
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
@@ -308,14 +319,18 @@
       <xs:documentation>LEMS ComponentType for Dynamics</xs:documentation>
     </xs:annotation>
     <xs:sequence>
       <xs:element name="StateVariable" type="StateVariable" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="DerivedVariable" type="DerivedVariable" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="ConditionalDerivedVariable" type="ConditionalDerivedVariable" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="TimeDerivative" type="TimeDerivative" minOccurs="0" maxOccurs="unbounded"/>
+      <xs:element name="OnStart" type="OnStart" minOccurs="0" maxOccurs="1"/>
+      <xs:element name="OnEvent" type="OnEvent" minOccurs="0" maxOccurs="unbounded"/>
+      <xs:element name="OnCondition" type="OnCondition" minOccurs="0" maxOccurs="unbounded"/>
+      <xs:element name="Regime" type="Regime" minOccurs="0" maxOccurs="unbounded"/>
     </xs:sequence>
   </xs:complexType>
   <xs:complexType name="DerivedVariable">
     <xs:annotation>
       <xs:documentation>LEMS ComponentType for DerivedVariable</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
@@ -346,14 +361,65 @@
     <xs:attribute name="condition" type="xs:string" use="optional"/>
     <xs:attribute name="value" type="xs:string" use="required"/>
   </xs:complexType>
   <xs:complexType name="TimeDerivative">
     <xs:attribute name="variable" type="xs:string" use="required"/>
     <xs:attribute name="value" type="xs:string" use="required"/>
   </xs:complexType>
+  <xs:complexType name="OnStart">
+    <xs:sequence>
+      <xs:element name="StateAssignment" type="StateAssignment" minOccurs="1" maxOccurs="unbounded"/>
+    </xs:sequence>
+  </xs:complexType>
+  <xs:complexType name="StateAssignment">
+    <xs:attribute name="variable" type="xs:string" use="required"/>
+    <xs:attribute name="value" type="xs:string" use="required"/>
+  </xs:complexType>
+  <xs:complexType name="OnEvent">
+    <xs:sequence>
+      <xs:element name="StateAssignment" type="StateAssignment" minOccurs="0" maxOccurs="unbounded"/>
+      <xs:element name="EventOut" type="EventOut" minOccurs="0" maxOccurs="unbounded"/>
+    </xs:sequence>
+    <xs:attribute name="port" type="xs:string" use="required"/>
+  </xs:complexType>
+  <xs:complexType name="EventOut">
+    <xs:attribute name="port" type="xs:string" use="required"/>
+  </xs:complexType>
+  <xs:complexType name="OnCondition">
+    <xs:sequence>
+      <xs:element name="StateAssignment" type="StateAssignment" minOccurs="0" maxOccurs="unbounded"/>
+      <xs:element name="EventOut" type="EventOut" minOccurs="0" maxOccurs="unbounded"/>
+      <xs:element name="Transition" type="Transition" minOccurs="0" maxOccurs="1"/>
+      <!-- only on OnCondition inside Regime... -->
+    </xs:sequence>
+    <xs:attribute name="test" type="xs:string" use="required"/>
+  </xs:complexType>
+  <xs:complexType name="Transition">
+    <xs:attribute name="regime" type="xs:string" use="required"/>
+  </xs:complexType>
+  <xs:complexType name="Regime">
+    <xs:sequence>
+      <xs:element name="TimeDerivative" type="TimeDerivative" minOccurs="0" maxOccurs="unbounded"/>
+      <xs:element name="OnEntry" type="OnEntry" minOccurs="0" maxOccurs="1"/>
+      <xs:element name="OnCondition" type="OnCondition" minOccurs="0" maxOccurs="unbounded"/>
+    </xs:sequence>
+    <xs:attribute name="name" type="xs:string" use="required"/>
+    <xs:attribute name="initial" type="TrueOrFalse" use="optional"/>
+  </xs:complexType>
+  <xs:complexType name="OnEntry">
+    <xs:sequence>
+      <xs:element name="StateAssignment" type="StateAssignment" minOccurs="1" maxOccurs="unbounded"/>
+    </xs:sequence>
+  </xs:complexType>
+  <xs:simpleType name="TrueOrFalse">
+    <xs:restriction base="xs:string">
+      <xs:enumeration value="true"/>
+      <xs:enumeration value="false"/>
+    </xs:restriction>
+  </xs:simpleType>
   <xs:simpleType name="ZeroToOne">
     <xs:annotation>
       <xs:documentation>Float value restricted to between 1 and 0</xs:documentation>
     </xs:annotation>
     <xs:restriction base="xs:float">
       <xs:minInclusive value="0"/>
       <xs:maxInclusive value="1"/>
@@ -521,15 +587,15 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="IonChannelKS">
     <xs:annotation>
       <xs:documentation>A kinetic scheme based ion channel with multiple  **gateKS** s, each of which consists of multiple  **KSState** s and  **KSTransition** s giving the rates of transition between them
 \n
-:param conductance:
+:param conductance: 
 :type conductance: conductance</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="Standalone">
         <xs:sequence>
           <xs:element name="gateKS" type="GateKS" minOccurs="0" maxOccurs="unbounded"/>
         </xs:sequence>
@@ -539,15 +605,15 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="IonChannel">
     <xs:annotation>
       <xs:documentation>Note  **ionChannel**  and  **ionChannelHH**  are currently functionally identical. This is needed since many existing examples use ionChannel, some use ionChannelHH. NeuroML v2beta4 should remove one of these, probably ionChannelHH.
 \n
-:param conductance:
+:param conductance: 
 :type conductance: conductance</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="IonChannelScalable">
         <xs:choice>
           <xs:element name="gate" type="GateHHUndetermined" minOccurs="0" maxOccurs="unbounded"/>
           <xs:element name="gateHHrates" type="GateHHRates" minOccurs="0" maxOccurs="unbounded"/>
@@ -564,28 +630,28 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="IonChannelHH">
     <xs:annotation>
       <xs:documentation>Note  **ionChannel**  and  **ionChannelHH**  are currently functionally identical. This is needed since many existing examples use ionChannel, some use ionChannelHH. NeuroML v2beta4 should remove one of these, probably ionChannelHH.
 \n
-:param conductance:
+:param conductance: 
 :type conductance: conductance</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="IonChannel"/>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="IonChannelVShift">
     <xs:annotation>
       <xs:documentation>Same as  **ionChannel** , but with a **vShift**  parameter to change voltage activation of gates. The exact usage of **vShift**  in expressions for rates is determined by the individual gates.
 \n
-:param vShift:
+:param vShift: 
 :type vShift: voltage
-:param conductance:
+:param conductance: 
 :type conductance: conductance</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="IonChannel">
         <xs:attribute name="vShift" type="Nml2Quantity_voltage" use="required"/>
       </xs:extension>
     </xs:complexContent>
@@ -597,17 +663,17 @@
       <!--<xs:enumeration value="ionChannelKS"/> use an explicit <ionChannelKS ... > element, not <ionChannel type="ionChannelKS" ..> -->
     </xs:restriction>
   </xs:simpleType>
   <xs:complexType name="Q10ConductanceScaling">
     <xs:annotation>
       <xs:documentation>A value for the conductance scaling which varies as a standard function of the difference between the current temperature, **temperature,**  and the temperature at which the conductance was originally determined, **experimentalTemp**
 \n
-:param q10Factor:
+:param q10Factor: 
 :type q10Factor: none
-:param experimentalTemp:
+:param experimentalTemp: 
 :type experimentalTemp: temperature</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="BaseWithoutId">
         <xs:attribute name="q10Factor" type="Nml2Quantity_none" use="required"/>
         <xs:attribute name="experimentalTemp" type="Nml2Quantity_temperature" use="required"/>
       </xs:extension>
@@ -625,28 +691,28 @@
       <xs:enumeration value="gateFractional"/>
     </xs:restriction>
   </xs:simpleType>
   <xs:complexType name="ClosedState">
     <xs:annotation>
       <xs:documentation>A  **KSState**  with **relativeConductance**  of 0
 \n
-:param relativeConductance:
+:param relativeConductance: 
 :type relativeConductance: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="Base">
         <!-- Only has id...-->
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="OpenState">
     <xs:annotation>
       <xs:documentation>A  **KSState**  with **relativeConductance**  of 1
 \n
-:param relativeConductance:
+:param relativeConductance: 
 :type relativeConductance: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="Base">
         <!-- Only has id...-->
       </xs:extension>
     </xs:complexContent>
@@ -702,15 +768,15 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="GateKS">
     <xs:annotation>
       <xs:documentation>A gate which consists of multiple  **KSState** s and  **KSTransition** s giving the rates of transition between them
 \n
-:param instances:
+:param instances: 
 :type instances: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="Base">
         <xs:sequence>
           <xs:element name="notes" type="Notes" minOccurs="0"/>
           <xs:element name="q10Settings" type="Q10Settings" minOccurs="0"/>
@@ -746,15 +812,15 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="GateHHRates">
     <xs:annotation>
       <xs:documentation>Gate which follows the general Hodgkin Huxley formalism
 \n
-:param instances:
+:param instances: 
 :type instances: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="Base">
         <xs:all>
           <xs:element name="notes" type="Notes" minOccurs="0"/>
           <xs:element name="q10Settings" type="Q10Settings" minOccurs="0"/>
@@ -766,15 +832,15 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="GateHHTauInf">
     <xs:annotation>
       <xs:documentation>Gate which follows the general Hodgkin Huxley formalism
 \n
-:param instances:
+:param instances: 
 :type instances: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="Base">
         <xs:all>
           <xs:element name="notes" type="Notes" minOccurs="0"/>
           <xs:element name="q10Settings" type="Q10Settings" minOccurs="0"/>
@@ -786,15 +852,15 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="GateHHRatesTauInf">
     <xs:annotation>
       <xs:documentation>Gate which follows the general Hodgkin Huxley formalism
 \n
-:param instances:
+:param instances: 
 :type instances: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="Base">
         <xs:all>
           <xs:element name="notes" type="Notes" minOccurs="0"/>
           <xs:element name="q10Settings" type="Q10Settings" minOccurs="0"/>
@@ -808,15 +874,15 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="GateHHRatesTau">
     <xs:annotation>
       <xs:documentation>Gate which follows the general Hodgkin Huxley formalism
 \n
-:param instances:
+:param instances: 
 :type instances: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="Base">
         <xs:all>
           <xs:element name="notes" type="Notes" minOccurs="0"/>
           <xs:element name="q10Settings" type="Q10Settings" minOccurs="0"/>
@@ -829,15 +895,15 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="GateHHRatesInf">
     <xs:annotation>
       <xs:documentation>Gate which follows the general Hodgkin Huxley formalism
 \n
-:param instances:
+:param instances: 
 :type instances: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="Base">
         <xs:all>
           <xs:element name="notes" type="Notes" minOccurs="0"/>
           <xs:element name="q10Settings" type="Q10Settings" minOccurs="0"/>
@@ -850,15 +916,15 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="GateHHInstantaneous">
     <xs:annotation>
       <xs:documentation>Gate which follows the general Hodgkin Huxley formalism but is instantaneous, so tau = 0 and gate follows exactly inf value
 \n
-:param instances:
+:param instances: 
 :type instances: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="Base">
         <xs:all>
           <xs:element name="notes" type="Notes" minOccurs="0"/>
           <xs:element name="steadyState" type="HHVariable" minOccurs="1"/>
@@ -868,15 +934,15 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="GateFractional">
     <xs:annotation>
       <xs:documentation>Gate composed of subgates contributing with fractional conductance
 \n
-:param instances:
+:param instances: 
 :type instances: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="Base">
         <xs:sequence>
           <xs:element name="notes" type="Notes" minOccurs="0"/>
           <xs:element name="q10Settings" type="Q10Settings" minOccurs="0"/>
@@ -944,19 +1010,19 @@
   <!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
   <!--      Concentration Model types                        -->
   <!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
   <xs:complexType name="DecayingPoolConcentrationModel">
     <xs:annotation>
       <xs:documentation>Model of an intracellular buffering mechanism for **ion**  ( currently hard Coded to be calcium, due to requirement for **iCa**  ) which has a baseline level **restingConc**  and tends to this value with time course **decayConstant.**  The ion is assumed to occupy a shell inside the membrane of thickness **shellThickness.**
 \n
-:param restingConc:
+:param restingConc: 
 :type restingConc: concentration
-:param decayConstant:
+:param decayConstant: 
 :type decayConstant: time
-:param shellThickness:
+:param shellThickness: 
 :type shellThickness: length</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="Standalone">
         <xs:attribute name="ion" type="NmlId" use="required">
           <xs:annotation/>
         </xs:attribute>
@@ -966,19 +1032,19 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="FixedFactorConcentrationModel">
     <xs:annotation>
       <xs:documentation>Model of buffering of concentration of an ion ( currently hard coded to be calcium, due to requirement for **iCa**  ) which has a baseline level **restingConc**  and tends to this value with time course **decayConstant.**  A fixed factor **rho**  is used to scale the incoming current *independently of the size of the compartment* to produce a concentration change.
 \n
-:param restingConc:
+:param restingConc: 
 :type restingConc: concentration
-:param decayConstant:
+:param decayConstant: 
 :type decayConstant: time
-:param rho:
+:param rho: 
 :type rho: rho_factor</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="Standalone">
         <xs:attribute name="ion" type="NmlId" use="required">
           <xs:annotation/>
         </xs:attribute>
@@ -1052,15 +1118,15 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="GapJunction">
     <xs:annotation>
       <xs:documentation>Gap junction/single electrical connection
 \n
-:param conductance:
+:param conductance: 
 :type conductance: conductance</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="BaseSynapse">
         <xs:attribute name="conductance" type="Nml2Quantity_conductance" use="required"/>
       </xs:extension>
     </xs:complexContent>
@@ -1073,28 +1139,28 @@
       <xs:extension base="BaseSynapse"/>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="LinearGradedSynapse">
     <xs:annotation>
       <xs:documentation>Behaves just like a one way gap junction.
 \n
-:param conductance:
+:param conductance: 
 :type conductance: conductance</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="BaseSynapse">
         <xs:attribute name="conductance" type="Nml2Quantity_conductance" use="required"/>
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="GradedSynapse">
     <xs:annotation>
       <xs:documentation>Graded/analog synapse. Based on synapse in Methods of http://www. nature.com/neuro/journal/v7/n12/abs/nn1352.html
 \n
-:param conductance:
+:param conductance: 
 :type conductance: conductance
 :param delta: Slope of the activation curve
 :type delta: voltage
 :param k: Rate constant for transmitter-receptor dissociation rate
 :type k: per_time
 :param Vth: The half-activation voltage of the synapse
 :type Vth: voltage
@@ -1161,17 +1227,17 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="ExpTwoSynapse">
     <xs:annotation>
       <xs:documentation>Ohmic synapse model whose conductance waveform on receiving an event has a rise time of **tauRise**  and a decay time of **tauDecay.**  Max conductance reached during this time ( assuming zero conductance before ) is **gbase**  * **weight.**
 \n
-:param tauRise:
+:param tauRise: 
 :type tauRise: time
-:param tauDecay:
+:param tauDecay: 
 :type tauDecay: time
 :param gbase: Baseline conductance, generally the maximum conductance following a single spike
 :type gbase: conductance
 :param erev: Reversal potential of the synapse
 :type erev: voltage</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
@@ -1181,19 +1247,19 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="ExpThreeSynapse">
     <xs:annotation>
       <xs:documentation>Ohmic synapse similar to expTwoSynapse but consisting of two components that can differ in decay times and max conductances but share the same rise time.
 \n
-:param tauRise:
+:param tauRise: 
 :type tauRise: time
-:param tauDecay1:
+:param tauDecay1: 
 :type tauDecay1: time
-:param tauDecay2:
+:param tauDecay2: 
 :type tauDecay2: time
 :param gbase1: Baseline conductance 1
 :type gbase1: conductance
 :param gbase2: Baseline conductance 2
 :type gbase2: conductance
 :param erev: Reversal potential of the synapse
 :type erev: voltage</xs:documentation>
@@ -1219,17 +1285,17 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="BlockingPlasticSynapse">
     <xs:annotation>
       <xs:documentation>Biexponential synapse that allows for optional block and plasticity mechanisms, which can be expressed as child elements.
 \n
-:param tauRise:
+:param tauRise: 
 :type tauRise: time
-:param tauDecay:
+:param tauDecay: 
 :type tauDecay: time
 :param gbase: Baseline conductance, generally the maximum conductance following a single spike
 :type gbase: conductance
 :param erev: Reversal potential of the synapse
 :type erev: voltage</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
@@ -1286,17 +1352,17 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="IafTauCell">
     <xs:annotation>
       <xs:documentation>Integrate and fire cell which returns to its leak reversal potential of **leakReversal**  with a time constant **tau**
 \n
-:param leakReversal:
+:param leakReversal: 
 :type leakReversal: voltage
-:param tau:
+:param tau: 
 :type tau: time
 :param thresh: The membrane potential at which to emit a spiking event and reset voltage
 :type thresh: voltage
 :param reset: The value the membrane potential is reset to on spiking
 :type reset: voltage</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
@@ -1308,19 +1374,19 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="IafTauRefCell">
     <xs:annotation>
       <xs:documentation>Integrate and fire cell which returns to its leak reversal potential of **leakReversal**  with a time course **tau.**  It has a refractory period of **refract**  after spiking
 \n
-:param refract:
+:param refract: 
 :type refract: time
-:param leakReversal:
+:param leakReversal: 
 :type leakReversal: voltage
-:param tau:
+:param tau: 
 :type tau: time
 :param thresh: The membrane potential at which to emit a spiking event and reset voltage
 :type thresh: voltage
 :param reset: The value the membrane potential is reset to on spiking
 :type reset: voltage</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
@@ -1329,21 +1395,21 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="IafCell">
     <xs:annotation>
       <xs:documentation>Integrate and fire cell with capacitance **C,**  **leakConductance**  and **leakReversal**
 \n
-:param leakConductance:
+:param leakConductance: 
 :type leakConductance: conductance
-:param leakReversal:
+:param leakReversal: 
 :type leakReversal: voltage
-:param thresh:
+:param thresh: 
 :type thresh: voltage
-:param reset:
+:param reset: 
 :type reset: voltage
 :param C: Total capacitance of the cell membrane
 :type C: capacitance</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="BaseCell">
         <xs:attribute name="leakReversal" type="Nml2Quantity_voltage" use="required"/>
@@ -1354,23 +1420,23 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="IafRefCell">
     <xs:annotation>
       <xs:documentation>Integrate and fire cell with capacitance **C,**  **leakConductance,**  **leakReversal**  and refractory period **refract**
 \n
-:param refract:
+:param refract: 
 :type refract: time
-:param leakConductance:
+:param leakConductance: 
 :type leakConductance: conductance
-:param leakReversal:
+:param leakReversal: 
 :type leakReversal: voltage
-:param thresh:
+:param thresh: 
 :type thresh: voltage
-:param reset:
+:param reset: 
 :type reset: voltage
 :param C: Total capacitance of the cell membrane
 :type C: capacitance</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="IafCell">
         <xs:attribute name="refract" type="Nml2Quantity_time" use="required"/>
@@ -1424,31 +1490,31 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="Izhikevich2007Cell">
     <xs:annotation>
       <xs:documentation>Cell based on the modified Izhikevich model in Izhikevich 2007, Dynamical systems in neuroscience, MIT Press
 \n
-:param v0:
+:param v0: 
 :type v0: voltage
-:param k:
+:param k: 
 :type k: conductance_per_voltage
-:param vr:
+:param vr: 
 :type vr: voltage
-:param vt:
+:param vt: 
 :type vt: voltage
-:param vpeak:
+:param vpeak: 
 :type vpeak: voltage
-:param a:
+:param a: 
 :type a: per_time
-:param b:
+:param b: 
 :type b: conductance
-:param c:
+:param c: 
 :type c: voltage
-:param d:
+:param d: 
 :type d: current
 :param C: Total capacitance of the cell membrane
 :type C: capacitance</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="BaseCellMembPotCap">
         <xs:attribute name="v0" type="Nml2Quantity_voltage" use="required"/>
@@ -1463,33 +1529,33 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="AdExIaFCell">
     <xs:annotation>
       <xs:documentation>Model based on Brette R and Gerstner W ( 2005 ) Adaptive Exponential Integrate-and-Fire Model as an Effective Description of Neuronal Activity. J Neurophysiol 94:3637-3642
 \n
-:param gL:
+:param gL: 
 :type gL: conductance
-:param EL:
+:param EL: 
 :type EL: voltage
-:param VT:
+:param VT: 
 :type VT: voltage
-:param thresh:
+:param thresh: 
 :type thresh: voltage
-:param reset:
+:param reset: 
 :type reset: voltage
-:param delT:
+:param delT: 
 :type delT: voltage
-:param tauw:
+:param tauw: 
 :type tauw: time
-:param refract:
+:param refract: 
 :type refract: time
-:param a:
+:param a: 
 :type a: conductance
-:param b:
+:param b: 
 :type b: current
 :param C: Total capacitance of the cell membrane
 :type C: capacitance</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="BaseCellMembPotCap">
         <xs:attribute name="gL" type="Nml2Quantity_conductance" use="required"/>
@@ -1505,38 +1571,38 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="FitzHughNagumoCell">
     <xs:annotation>
       <xs:documentation>Simple dimensionless model of spiking cell from FitzHugh and Nagumo. Superseded by **fitzHughNagumo1969Cell**  ( See https://github.com/NeuroML/NeuroML2/issues/42 )
 \n
-:param I:
+:param I: 
 :type I: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="BaseCell">
         <xs:attribute name="I" type="Nml2Quantity_none" use="required"/>
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="FitzHughNagumo1969Cell">
     <xs:annotation>
       <xs:documentation>The Fitzhugh Nagumo model is a two-dimensional simplification of the Hodgkin-Huxley model of spike generation in squid giant axons. This system was suggested by FitzHugh ( FitzHugh R. [1961]: Impulses and physiological states in theoretical models of nerve membrane. Biophysical J. 1:445-466 ), who called it &quot; Bonhoeffer-van der Pol model &quot;, and the equivalent circuit by Nagumo et al. ( Nagumo J. , Arimoto S. , and Yoshizawa S. [1962] An active pulse transmission line simulating nerve axon. Proc IRE. 50:2061-2070. 1962 ). This version corresponds to the one described in FitzHugh R. [1969]: Mathematical models of excitation and propagation in nerve. Chapter 1 ( pp. 1-85 in H. P. Schwan, ed. Biological Engineering, McGraw-Hill Book Co. , N. Y. )
 \n
-:param a:
+:param a: 
 :type a: none
-:param b:
+:param b: 
 :type b: none
 :param I: plays the role of an external injected current
 :type I: none
-:param phi:
+:param phi: 
 :type phi: none
-:param V0:
+:param V0: 
 :type V0: none
-:param W0:
+:param W0: 
 :type W0: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="BaseCell">
         <xs:attribute name="a" type="Nml2Quantity_none" use="required"/>
         <xs:attribute name="b" type="Nml2Quantity_none" use="required"/>
         <xs:attribute name="I" type="Nml2Quantity_none" use="required"/>
@@ -1546,55 +1612,55 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="PinskyRinzelCA3Cell">
     <xs:annotation>
       <xs:documentation>Reduced CA3 cell model from Pinsky and Rinzel 1994. See https://github.com/OpenSourceBrain/PinskyRinzelModel
 \n
-:param iSoma:
+:param iSoma: 
 :type iSoma: currentDensity
-:param iDend:
+:param iDend: 
 :type iDend: currentDensity
-:param gLs:
+:param gLs: 
 :type gLs: conductanceDensity
-:param gLd:
+:param gLd: 
 :type gLd: conductanceDensity
-:param gNa:
+:param gNa: 
 :type gNa: conductanceDensity
-:param gKdr:
+:param gKdr: 
 :type gKdr: conductanceDensity
-:param gCa:
+:param gCa: 
 :type gCa: conductanceDensity
-:param gKahp:
+:param gKahp: 
 :type gKahp: conductanceDensity
-:param gKC:
+:param gKC: 
 :type gKC: conductanceDensity
-:param gc:
+:param gc: 
 :type gc: conductanceDensity
-:param eNa:
+:param eNa: 
 :type eNa: voltage
-:param eCa:
+:param eCa: 
 :type eCa: voltage
-:param eK:
+:param eK: 
 :type eK: voltage
-:param eL:
+:param eL: 
 :type eL: voltage
-:param pp:
+:param pp: 
 :type pp: none
-:param cm:
+:param cm: 
 :type cm: specificCapacitance
-:param alphac:
+:param alphac: 
 :type alphac: none
-:param betac:
+:param betac: 
 :type betac: none
-:param gNmda:
+:param gNmda: 
 :type gNmda: conductanceDensity
-:param gAmpa:
+:param gAmpa: 
 :type gAmpa: conductanceDensity
-:param qd0:
+:param qd0: 
 :type qd0: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="BaseCell">
         <xs:attribute name="iSoma" type="Nml2Quantity_currentDensity" use="required"/>
         <xs:attribute name="iDend" type="Nml2Quantity_currentDensity" use="required"/>
         <xs:attribute name="gc" type="Nml2Quantity_conductanceDensity" use="required"/>
@@ -1889,57 +1955,57 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="SpikeThresh">
     <xs:annotation>
       <xs:documentation>Membrane potential at which to emit a spiking event. Note, usually the spiking event will not be emitted again until the membrane potential has fallen below this value and rises again to cross it in a positive direction
 \n
-:param value:
+:param value: 
 :type value: voltage</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="BaseWithoutId">
         <xs:attribute name="value" type="Nml2Quantity_voltage" use="required"/>
         <xs:attribute name="segmentGroup" type="NmlId" use="optional" default="all"/>
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="SpecificCapacitance">
     <xs:annotation>
       <xs:documentation>Capacitance per unit area
 \n
-:param value:
+:param value: 
 :type value: specificCapacitance</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="BaseWithoutId">
         <xs:attribute name="value" type="Nml2Quantity_specificCapacitance" use="required"/>
         <xs:attribute name="segmentGroup" type="NmlId" use="optional" default="all"/>
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="InitMembPotential">
     <xs:annotation>
       <xs:documentation>Explicitly set initial membrane potential for the cell
 \n
-:param value:
+:param value: 
 :type value: voltage</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="BaseWithoutId">
         <xs:attribute name="value" type="Nml2Quantity_voltage" use="required"/>
         <xs:attribute name="segmentGroup" type="NmlId" use="optional" default="all"/>
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="Resistivity">
     <xs:annotation>
       <xs:documentation>The resistivity, or specific axial resistance, of the cytoplasm
 \n
-:param value:
+:param value: 
 :type value: resistivity</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="BaseWithoutId">
         <xs:attribute name="value" type="Nml2Quantity_resistivity" use="required"/>
         <xs:attribute name="segmentGroup" type="NmlId" use="optional" default="all"/>
       </xs:extension>
@@ -2025,15 +2091,15 @@
   </xs:complexType>
   <xs:complexType name="ChannelDensity">
     <xs:annotation>
       <xs:documentation>Specifies a time varying ohmic conductance density, **gDensity,**  which is distributed on an area of the **cell**  ( specified in  **membraneProperties**  ) with fixed reversal potential **erev**  producing a current density **iDensity**
 \n
 :param erev: The reversal potential of the current produced
 :type erev: voltage
-:param condDensity:
+:param condDensity: 
 :type condDensity: conductanceDensity</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="Base">
         <xs:sequence>
           <xs:element name="variableParameter" type="VariableParameter" minOccurs="0" maxOccurs="unbounded"/>
         </xs:sequence>
@@ -2049,32 +2115,32 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="ChannelDensityVShift">
     <xs:annotation>
       <xs:documentation>Same as  **channelDensity** , but with a **vShift**  parameter to change voltage activation of gates. The exact usage of **vShift**  in expressions for rates is determined by the individual gates.
 \n
-:param vShift:
+:param vShift: 
 :type vShift: voltage
 :param erev: The reversal potential of the current produced
 :type erev: voltage
-:param condDensity:
+:param condDensity: 
 :type condDensity: conductanceDensity</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="ChannelDensity">
         <xs:attribute name="vShift" type="Nml2Quantity_voltage" use="required"/>
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="ChannelDensityNernst">
     <xs:annotation>
       <xs:documentation>Specifies a time varying conductance density, **gDensity,**  which is distributed on an area of the **cell,**  producing a current density **iDensity**  and whose reversal potential is calculated from the Nernst equation. Hard coded for Ca only! See https://github.com/OpenSourceBrain/ghk-nernst.
 \n
-:param condDensity:
+:param condDensity: 
 :type condDensity: conductanceDensity</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="Base">
         <xs:sequence>
           <xs:element name="variableParameter" type="VariableParameter" minOccurs="0" maxOccurs="unbounded"/>
         </xs:sequence>
@@ -2089,28 +2155,28 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="ChannelDensityNernstCa2">
     <xs:annotation>
       <xs:documentation>This component is similar to the original component type  **channelDensityNernst**  but it is changed in order to have a reversal potential that depends on a second independent Ca++ pool ( ca2 ). See https://github.com/OpenSourceBrain/ghk-nernst.
 \n
-:param condDensity:
+:param condDensity: 
 :type condDensity: conductanceDensity</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="ChannelDensityNernst">
         <!-- No difference in structure. Specifying an independent complexType ensures generated APIs create a class for this-->
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="ChannelDensityGHK">
     <xs:annotation>
       <xs:documentation>Specifies a time varying conductance density, **gDensity,**  which is distributed on an area of the cell, producing a current density **iDensity**  and whose reversal potential is calculated from the Goldman Hodgkin Katz equation. Hard coded for Ca only! See https://github.com/OpenSourceBrain/ghk-nernst.
 \n
-:param permeability:
+:param permeability: 
 :type permeability: permeability</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="Base">
         <xs:attribute name="ionChannel" type="NmlId" use="required"/>
         <xs:attribute name="permeability" type="Nml2Quantity_permeability" use="required"/>
         <!-- Note: only one of the following should be used!! -->
@@ -2122,15 +2188,15 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="ChannelDensityGHK2">
     <xs:annotation>
       <xs:documentation>Time varying conductance density, **gDensity,**  which is distributed on an area of the cell, producing a current density **iDensity.**  Modified version of Jaffe et al. 1994 ( used also in Lawrence et al. 2006 ). See https://github.com/OpenSourceBrain/ghk-nernst.
 \n
-:param condDensity:
+:param condDensity: 
 :type condDensity: conductanceDensity</xs:documentation>
     </xs:annotation>
     <!--
             See https://github.com/OpenSourceBrain/ghk-nernst.
         -->
     <xs:complexContent>
       <xs:extension base="Base">
@@ -2176,17 +2242,17 @@
         </xs:complexContent>
 
     </xs:complexType> -->
   <xs:complexType name="Species">
     <xs:annotation>
       <xs:documentation>Description of a chemical species identified by **ion,**  which has internal, **concentration,**  and external, **extConcentration**  values for its concentration
 \n
-:param initialConcentration:
+:param initialConcentration: 
 :type initialConcentration: concentration
-:param initialExtConcentration:
+:param initialExtConcentration: 
 :type initialExtConcentration: concentration</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="Base">
         <xs:attribute name="concentrationModel" type="NmlId" use="required"/>
         <xs:attribute name="ion" type="NmlId" use="optional">
           <xs:annotation/>
@@ -2596,19 +2662,19 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="TransientPoissonFiringSynapse">
     <xs:annotation>
       <xs:documentation>Poisson spike generator firing at **averageRate**  after a **delay**  and for a **duration,**  connected to single **synapse**  that is triggered every time a spike is generated, providing an input current. Similar to ComponentType  **poissonFiringSynapse** .
 \n
-:param averageRate:
+:param averageRate: 
 :type averageRate: per_time
-:param delay:
+:param delay: 
 :type delay: time
-:param duration:
+:param duration: 
 :type duration: time</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="Standalone">
         <xs:attribute name="averageRate" type="Nml2Quantity_pertime" use="required"/>
         <xs:attribute name="delay" type="Nml2Quantity_time" use="required"/>
         <xs:attribute name="duration" type="Nml2Quantity_time" use="required"/>
@@ -2791,19 +2857,19 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="Location">
     <xs:annotation>
       <xs:documentation>Specifies the ( x, y, z ) location of a single  **instance**  of a component in a  **population**
 \n
-:param x:
+:param x: 
 :type x: none
-:param y:
+:param y: 
 :type y: none
-:param z:
+:param z: 
 :type z: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="BaseWithoutId">
         <xs:attribute name="x" type="xs:float" use="required"/>
         <xs:attribute name="y" type="xs:float" use="required"/>
         <xs:attribute name="z" type="xs:float" use="required"/>
@@ -2911,17 +2977,17 @@
       <xs:extension base="BaseConnectionOldFormat"/>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="ConnectionWD">
     <xs:annotation>
       <xs:documentation>Event connection between named components, which gets processed via a new instance of a synapse component which is created on the target component, includes setting of **weight**  and **delay**  for the synaptic connection
 \n
-:param weight:
+:param weight: 
 :type weight: none
-:param delay:
+:param delay: 
 :type delay: time</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="BaseConnectionOldFormat">
         <xs:attribute name="weight" type="xs:float" use="required"/>
         <xs:attribute name="delay" type="Nml2Quantity_time" use="required"/>
       </xs:extension>
@@ -2959,15 +3025,15 @@
       <xs:extension base="ElectricalConnection"/>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="ElectricalConnectionInstanceW">
     <xs:annotation>
       <xs:documentation>To enable connections between populations through gap junctions. Populations need to be of type  **populationList**  and contain  **instance**  and  **location**  elements. Includes setting of **weight**  for the connection
 \n
-:param weight:
+:param weight: 
 :type weight: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="ElectricalConnectionInstance">
         <xs:attribute name="weight" type="xs:float" use="required"/>
       </xs:extension>
     </xs:complexContent>
@@ -3005,15 +3071,15 @@
       <xs:extension base="ContinuousConnection"/>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="ContinuousConnectionInstanceW">
     <xs:annotation>
       <xs:documentation>An instance of a connection in a  **continuousProjection**  between **presynapticPopulation**  to another **postsynapticPopulation**  through a **preComponent**  at the start and **postComponent**  at the end. Populations need to be of type  **populationList**  and contain  **instance**  and  **location**  elements. Can be used for analog synapses. Includes setting of **weight**  for the connection
 \n
-:param weight:
+:param weight: 
 :type weight: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="ContinuousConnectionInstance">
         <xs:attribute name="weight" type="xs:float" use="required"/>
       </xs:extension>
     </xs:complexContent>
@@ -3058,15 +3124,15 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="InputW">
     <xs:annotation>
       <xs:documentation>Specifies input lists. Can set **weight**  to scale individual inputs.
 \n
-:param weight:
+:param weight: 
 :type weight: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="Input">
         <xs:attribute name="weight" type="xs:float" use="required"/>
       </xs:extension>
     </xs:complexContent>
@@ -3074,23 +3140,23 @@
   <!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
   <!--      PyNN standard cell & synapse definitions         -->
   <!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
   <xs:complexType name="basePyNNCell">
     <xs:annotation>
       <xs:documentation>Base type of any PyNN standard cell model. Note: membrane potential **v**  has dimensions voltage, but all other parameters are dimensionless. This is to facilitate translation to and from PyNN scripts in Python, where these parameters have implicit units, see http://neuralensemble.org/trac/PyNN/wiki/StandardModels
 \n
-:param cm:
+:param cm: 
 :type cm: none
-:param i_offset:
+:param i_offset: 
 :type i_offset: none
 :param tau_syn_E: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type tau_syn_E: none
 :param tau_syn_I: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type tau_syn_I: none
-:param v_init:
+:param v_init: 
 :type v_init: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="BaseCell">
         <xs:attribute name="cm" type="xs:float" use="required"/>
         <xs:attribute name="i_offset" type="xs:float" use="required"/>
         <xs:attribute name="tau_syn_E" type="xs:float" use="required"/>
@@ -3099,33 +3165,33 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="basePyNNIaFCell">
     <xs:annotation>
       <xs:documentation>Base type of any PyNN standard integrate and fire model
 \n
-:param tau_refrac:
+:param tau_refrac: 
 :type tau_refrac: none
-:param v_thresh:
+:param v_thresh: 
 :type v_thresh: none
-:param tau_m:
+:param tau_m: 
 :type tau_m: none
-:param v_rest:
+:param v_rest: 
 :type v_rest: none
-:param v_reset:
+:param v_reset: 
 :type v_reset: none
-:param cm:
+:param cm: 
 :type cm: none
-:param i_offset:
+:param i_offset: 
 :type i_offset: none
 :param tau_syn_E: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type tau_syn_E: none
 :param tau_syn_I: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type tau_syn_I: none
-:param v_init:
+:param v_init: 
 :type v_init: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="basePyNNCell">
         <xs:attribute name="tau_m" type="xs:float" use="required"/>
         <xs:attribute name="tau_refrac" type="xs:float" use="required"/>
         <xs:attribute name="v_reset" type="xs:float" use="required"/>
@@ -3138,203 +3204,203 @@
     <xs:annotation>
       <xs:documentation>Base type of conductance based PyNN IaF cell models
 \n
 :param e_rev_E: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type e_rev_E: none
 :param e_rev_I: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type e_rev_I: none
-:param tau_refrac:
+:param tau_refrac: 
 :type tau_refrac: none
-:param v_thresh:
+:param v_thresh: 
 :type v_thresh: none
-:param tau_m:
+:param tau_m: 
 :type tau_m: none
-:param v_rest:
+:param v_rest: 
 :type v_rest: none
-:param v_reset:
+:param v_reset: 
 :type v_reset: none
-:param cm:
+:param cm: 
 :type cm: none
-:param i_offset:
+:param i_offset: 
 :type i_offset: none
 :param tau_syn_E: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type tau_syn_E: none
 :param tau_syn_I: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type tau_syn_I: none
-:param v_init:
+:param v_init: 
 :type v_init: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="basePyNNIaFCell">
         <xs:attribute name="e_rev_E" type="xs:float" use="required"/>
         <xs:attribute name="e_rev_I" type="xs:float" use="required"/>
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="IF_curr_alpha">
     <xs:annotation>
       <xs:documentation>Leaky integrate and fire model with fixed threshold and alpha-function-shaped post-synaptic current
 \n
-:param tau_refrac:
+:param tau_refrac: 
 :type tau_refrac: none
-:param v_thresh:
+:param v_thresh: 
 :type v_thresh: none
-:param tau_m:
+:param tau_m: 
 :type tau_m: none
-:param v_rest:
+:param v_rest: 
 :type v_rest: none
-:param v_reset:
+:param v_reset: 
 :type v_reset: none
-:param cm:
+:param cm: 
 :type cm: none
-:param i_offset:
+:param i_offset: 
 :type i_offset: none
 :param tau_syn_E: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type tau_syn_E: none
 :param tau_syn_I: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type tau_syn_I: none
-:param v_init:
+:param v_init: 
 :type v_init: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="basePyNNIaFCell"/>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="IF_curr_exp">
     <xs:annotation>
       <xs:documentation>Leaky integrate and fire model with fixed threshold and decaying-exponential post-synaptic current
 \n
-:param tau_refrac:
+:param tau_refrac: 
 :type tau_refrac: none
-:param v_thresh:
+:param v_thresh: 
 :type v_thresh: none
-:param tau_m:
+:param tau_m: 
 :type tau_m: none
-:param v_rest:
+:param v_rest: 
 :type v_rest: none
-:param v_reset:
+:param v_reset: 
 :type v_reset: none
-:param cm:
+:param cm: 
 :type cm: none
-:param i_offset:
+:param i_offset: 
 :type i_offset: none
 :param tau_syn_E: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type tau_syn_E: none
 :param tau_syn_I: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type tau_syn_I: none
-:param v_init:
+:param v_init: 
 :type v_init: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="basePyNNIaFCell"/>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="IF_cond_alpha">
     <xs:annotation>
       <xs:documentation>Leaky integrate and fire model with fixed threshold and alpha-function-shaped post-synaptic conductance
 \n
 :param e_rev_E: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type e_rev_E: none
 :param e_rev_I: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type e_rev_I: none
-:param tau_refrac:
+:param tau_refrac: 
 :type tau_refrac: none
-:param v_thresh:
+:param v_thresh: 
 :type v_thresh: none
-:param tau_m:
+:param tau_m: 
 :type tau_m: none
-:param v_rest:
+:param v_rest: 
 :type v_rest: none
-:param v_reset:
+:param v_reset: 
 :type v_reset: none
-:param cm:
+:param cm: 
 :type cm: none
-:param i_offset:
+:param i_offset: 
 :type i_offset: none
 :param tau_syn_E: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type tau_syn_E: none
 :param tau_syn_I: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type tau_syn_I: none
-:param v_init:
+:param v_init: 
 :type v_init: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="basePyNNIaFCondCell"/>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="IF_cond_exp">
     <xs:annotation>
       <xs:documentation>Leaky integrate and fire model with fixed threshold and exponentially-decaying post-synaptic conductance
 \n
 :param e_rev_E: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type e_rev_E: none
 :param e_rev_I: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type e_rev_I: none
-:param tau_refrac:
+:param tau_refrac: 
 :type tau_refrac: none
-:param v_thresh:
+:param v_thresh: 
 :type v_thresh: none
-:param tau_m:
+:param tau_m: 
 :type tau_m: none
-:param v_rest:
+:param v_rest: 
 :type v_rest: none
-:param v_reset:
+:param v_reset: 
 :type v_reset: none
-:param cm:
+:param cm: 
 :type cm: none
-:param i_offset:
+:param i_offset: 
 :type i_offset: none
 :param tau_syn_E: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type tau_syn_E: none
 :param tau_syn_I: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type tau_syn_I: none
-:param v_init:
+:param v_init: 
 :type v_init: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="basePyNNIaFCondCell"/>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="EIF_cond_exp_isfa_ista">
     <xs:annotation>
       <xs:documentation>Adaptive exponential integrate and fire neuron according to Brette R and Gerstner W ( 2005 ) with exponentially-decaying post-synaptic conductance
 \n
-:param v_spike:
+:param v_spike: 
 :type v_spike: none
-:param delta_T:
+:param delta_T: 
 :type delta_T: none
-:param tau_w:
+:param tau_w: 
 :type tau_w: none
-:param a:
+:param a: 
 :type a: none
-:param b:
+:param b: 
 :type b: none
 :param e_rev_E: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type e_rev_E: none
 :param e_rev_I: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type e_rev_I: none
-:param tau_refrac:
+:param tau_refrac: 
 :type tau_refrac: none
-:param v_thresh:
+:param v_thresh: 
 :type v_thresh: none
-:param tau_m:
+:param tau_m: 
 :type tau_m: none
-:param v_rest:
+:param v_rest: 
 :type v_rest: none
-:param v_reset:
+:param v_reset: 
 :type v_reset: none
-:param cm:
+:param cm: 
 :type cm: none
-:param i_offset:
+:param i_offset: 
 :type i_offset: none
 :param tau_syn_E: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type tau_syn_E: none
 :param tau_syn_I: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type tau_syn_I: none
-:param v_init:
+:param v_init: 
 :type v_init: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="basePyNNIaFCondCell">
         <xs:attribute name="a" type="xs:float" use="required"/>
         <xs:attribute name="b" type="xs:float" use="required"/>
         <xs:attribute name="delta_T" type="xs:float" use="required"/>
@@ -3343,84 +3409,84 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="EIF_cond_alpha_isfa_ista">
     <xs:annotation>
       <xs:documentation>Adaptive exponential integrate and fire neuron according to Brette R and Gerstner W ( 2005 ) with alpha-function-shaped post-synaptic conductance
 \n
-:param v_spike:
+:param v_spike: 
 :type v_spike: none
-:param delta_T:
+:param delta_T: 
 :type delta_T: none
-:param tau_w:
+:param tau_w: 
 :type tau_w: none
-:param a:
+:param a: 
 :type a: none
-:param b:
+:param b: 
 :type b: none
 :param e_rev_E: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type e_rev_E: none
 :param e_rev_I: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type e_rev_I: none
-:param tau_refrac:
+:param tau_refrac: 
 :type tau_refrac: none
-:param v_thresh:
+:param v_thresh: 
 :type v_thresh: none
-:param tau_m:
+:param tau_m: 
 :type tau_m: none
-:param v_rest:
+:param v_rest: 
 :type v_rest: none
-:param v_reset:
+:param v_reset: 
 :type v_reset: none
-:param cm:
+:param cm: 
 :type cm: none
-:param i_offset:
+:param i_offset: 
 :type i_offset: none
 :param tau_syn_E: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type tau_syn_E: none
 :param tau_syn_I: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type tau_syn_I: none
-:param v_init:
+:param v_init: 
 :type v_init: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="EIF_cond_exp_isfa_ista"/>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="HH_cond_exp">
     <xs:annotation>
       <xs:documentation>Single-compartment Hodgkin-Huxley-type neuron with transient sodium and delayed-rectifier potassium currents using the ion channel models from Traub.
 \n
-:param gbar_K:
+:param gbar_K: 
 :type gbar_K: none
-:param gbar_Na:
+:param gbar_Na: 
 :type gbar_Na: none
-:param g_leak:
+:param g_leak: 
 :type g_leak: none
-:param e_rev_K:
+:param e_rev_K: 
 :type e_rev_K: none
-:param e_rev_Na:
+:param e_rev_Na: 
 :type e_rev_Na: none
-:param e_rev_leak:
+:param e_rev_leak: 
 :type e_rev_leak: none
-:param v_offset:
+:param v_offset: 
 :type v_offset: none
-:param e_rev_E:
+:param e_rev_E: 
 :type e_rev_E: none
-:param e_rev_I:
+:param e_rev_I: 
 :type e_rev_I: none
-:param cm:
+:param cm: 
 :type cm: none
-:param i_offset:
+:param i_offset: 
 :type i_offset: none
 :param tau_syn_E: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type tau_syn_E: none
 :param tau_syn_I: This parameter is never used in the NeuroML2 description of this cell! Any synapse producing a current can be placed on this cell
 :type tau_syn_I: none
-:param v_init:
+:param v_init: 
 :type v_init: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="basePyNNCell">
         <xs:attribute name="v_offset" type="xs:float" use="required"/>
         <xs:attribute name="e_rev_E" type="xs:float" use="required"/>
         <xs:attribute name="e_rev_I" type="xs:float" use="required"/>
@@ -3433,84 +3499,84 @@
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="BasePynnSynapse">
     <xs:annotation>
       <xs:documentation>Base type for all PyNN synapses. Note, the current **I**  produced is dimensionless, but it requires a membrane potential **v**  with dimension voltage
 \n
-:param tau_syn:
+:param tau_syn: 
 :type tau_syn: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="BaseSynapse">
         <xs:attribute name="tau_syn" type="xs:float" use="required"/>
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="ExpCondSynapse">
     <xs:annotation>
       <xs:documentation>Conductance based synapse with instantaneous rise and single exponential decay ( with time constant tau_syn )
 \n
-:param e_rev:
+:param e_rev: 
 :type e_rev: none
-:param tau_syn:
+:param tau_syn: 
 :type tau_syn: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="BasePynnSynapse">
         <xs:attribute name="e_rev" type="xs:float" use="required"/>
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="AlphaCondSynapse">
     <xs:annotation>
       <xs:documentation>Alpha synapse: rise time and decay time are both tau_syn. Conductance based synapse.
 \n
-:param e_rev:
+:param e_rev: 
 :type e_rev: none
-:param tau_syn:
+:param tau_syn: 
 :type tau_syn: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="BasePynnSynapse">
         <xs:attribute name="e_rev" type="xs:float" use="required"/>
       </xs:extension>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="ExpCurrSynapse">
     <xs:annotation>
       <xs:documentation>Current based synapse with instantaneous rise and single exponential decay ( with time constant tau_syn )
 \n
-:param tau_syn:
+:param tau_syn: 
 :type tau_syn: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="BasePynnSynapse"/>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="AlphaCurrSynapse">
     <xs:annotation>
       <xs:documentation>Alpha synapse: rise time and decay time are both tau_syn. Current based synapse.
 \n
-:param tau_syn:
+:param tau_syn: 
 :type tau_syn: none</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="BasePynnSynapse"/>
     </xs:complexContent>
   </xs:complexType>
   <xs:complexType name="SpikeSourcePoisson">
     <xs:annotation>
       <xs:documentation>Spike source, generating spikes according to a Poisson process.
 \n
-:param start:
+:param start: 
 :type start: time
-:param duration:
+:param duration: 
 :type duration: time
-:param rate:
+:param rate: 
 :type rate: per_time</xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="Standalone">
         <xs:attribute name="start" type="Nml2Quantity_time" use="required"/>
         <xs:attribute name="duration" type="Nml2Quantity_time" use="required"/>
         <xs:attribute name="rate" type="Nml2Quantity_pertime" use="required"/>
```

### Comparing `libNeuroML-0.4.1/neuroml/nml/NeuroML_v2beta1.xsd` & `libNeuroML-0.5.1/neuroml/nml/NeuroML_v2beta1.xsd`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.4.1/neuroml/nml/NeuroML_v2beta2.xsd` & `libNeuroML-0.5.1/neuroml/nml/NeuroML_v2beta2.xsd`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.4.1/neuroml/nml/NeuroML_v2beta3.xsd` & `libNeuroML-0.5.1/neuroml/nml/NeuroML_v2beta3.xsd`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.4.1/neuroml/nml/NeuroML_v2beta4.xsd` & `libNeuroML-0.5.1/neuroml/nml/NeuroML_v2beta4.xsd`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.4.1/neuroml/nml/NeuroML_v2beta5.xsd` & `libNeuroML-0.5.1/neuroml/nml/NeuroML_v2beta5.xsd`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.4.1/neuroml/nml/annotate_nml.py` & `libNeuroML-0.5.1/neuroml/nml/annotate_nml.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,35 +6,35 @@
 
 This must be run from the project root for all the imports to work correctly:
 
 python -m neuroml.nml.annotate_nml
 
 File: annotate_nml.py
 
-Copyright 2022 NeuroML contributors
+Copyright 2023 NeuroML contributors
 """
 
 
 import inspect
 from . import nml
 
 
 ignorelist = [
     "GeneratedsSuper",
     "GeneratedsSuperSuper",
 ]
 
 
 def pred(c):
-    return (inspect.isclass(c) and (c.__name__ not in ignorelist))
+    return inspect.isclass(c) and (c.__name__ not in ignorelist)
 
 
 classes = inspect.getmembers(nml, pred)
 
-with open("sed-script.txt", 'w') as f:
+with open("sed-script.txt", "w") as f:
     for aclass, atype in classes:
         # print(f"Processing {aclass}")
         member_types = {}
         if getattr(atype, "_get_members", False):
             members = atype()._get_members()
             for amember in members:
                 dtype = amember.get_data_type().replace("xs:", "")
@@ -48,14 +48,14 @@
                 # understand what needs to be used.
 
                 # must be run on unblacked file because we are relying on all
                 # arguments to be in the same line as init
                 if amember.get_container() == 0:
                     print(
                         f"""/{regexstart}/,/{regexend}/ s/\\(def __init__.* {dname}\\)=\\([[:alnum:]\\._ ']*\\),/\\1: "a {dtype} ({dreq})" = \\2,/""",
-                        file=f
+                        file=f,
                     )
                 else:
                     print(
                         f"""/{regexstart}/,/{regexend}/ s/\\(def __init__.* {dname}\\)=\\([[:alnum:]\\._ ']*\\),/\\1: "list of {dtype}(s) ({dreq})" = \\2,/""",
-                        file=f
+                        file=f,
                     )
```

### Comparing `libNeuroML-0.4.1/neuroml/nml/generateds_config.py` & `libNeuroML-0.5.1/neuroml/nml/generateds_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,14 @@
     elif re.search("[^aeiou]y$", noun):
         return re.sub("y$", "ies", noun)
     else:
         return noun + "s"
 
 
 def _node_to_python(node):
-
     pluralize_flag = "maxOccurs" in node.attrib
 
     for attribute in node.attrib:
         nml_attribute = node.attrib.pop(attribute)
         if nml_attribute[0].islower():
             renamed_attribute = to_lowercase_with_underscores(nml_attribute)
             if pluralize_flag:
```

### Comparing `libNeuroML-0.4.1/neuroml/nml/generatedscollector.py` & `libNeuroML-0.5.1/neuroml/nml/generatedscollector.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,37 +3,35 @@
 Implementation of generateds collector.
 
 This has been split out from nml.py so that the collector can be used in
 generatedssupersuper.py
 
 File: neuroml/nml.py/generatedscollector.py
 
-Copyright 2022 Ankur Sinha
+Copyright 2023 Ankur Sinha
 Author: Ankur Sinha <sanjay DOT ankur AT gmail DOT com>
 """
 
 import inspect
 
 
 class GdsCollector(object):
     def __init__(self, messages=None):
         if messages is None:
             self.messages = []
         else:
             self.messages = messages
 
     def add_message(self, msg):
-        caller = inspect.stack()[1].frame.f_locals['self']
+        caller = inspect.stack()[1].frame.f_locals["self"]
         try:
             caller_id_str = f" ({caller.id})"
         except AttributeError:
             caller_id_str = ""
-        self.messages.append(
-            f"{caller.__class__.__name__}{caller_id_str}: {msg}"
-        )
+        self.messages.append(f"{caller.__class__.__name__}{caller_id_str}: {msg}")
 
     def get_messages(self):
         return self.messages
 
     def clear_messages(self):
         self.messages = []
```

### Comparing `libNeuroML-0.4.1/neuroml/nml/generatedssupersuper.py` & `libNeuroML-0.5.1/neuroml/nml/generatedssupersuper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 """
 Super class for GeneratedsSuper
 
 File: neuroml/nml/generatedssupersuper.py
 
-Copyright 2022 NeuroML contributors
+Copyright 2023 NeuroML contributors
 """
 
 
 import sys
 
 from .generatedscollector import GdsCollector
 
@@ -448,14 +448,15 @@
             "channelTypes",
             "gateTypes",
             "networkTypes",
             "populationTypes",
             "_FixedOffsetTZ",
             "GdsCollector_",
             "GeneratedsSuperSuper",
+            "attrgetter",
         ]
 
         # do not show parameters here, they are indicated by members below
         # some classes may not have doc strings, do nothing if they don't
         try:
             info_str = "{}\n\n".format(
                 self.__class__.__doc__.split(":param")[0].strip()
```

### Comparing `libNeuroML-0.4.1/neuroml/nml/helper_methods.py` & `libNeuroML-0.5.1/neuroml/nml/helper_methods.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
 import re
 
+
 #
 # You must include the following class definition at the top of
 #   your method specification file.
 #
 class MethodSpec(object):
     def __init__(self, name="", source="", class_names="", class_names_compiled=None):
         """MethodSpec -- A specification of a method.
@@ -153,16 +154,14 @@
     @property
     def volume(self):
         """Get the volume of the segment.
 
         :returns: volume of segment
         :rtype: float
         """
-
-        from math import pi
         if self.proximal==None:
             raise Exception('Cannot get volume of segment '+str(self.id)+' using the volume property, since no proximal point is set on it (the proximal point comes from the parent segment). Use the method get_segment_volume(segment_id) on the cell instead.')
 
         prox_rad = self.proximal.diameter/2.0
         dist_rad = self.distal.diameter/2.0
 
         if self.proximal.x == self.distal.x and \
@@ -191,17 +190,14 @@
     @property
     def surface_area(self):
         """Get the surface area of the segment.
 
         :returns: surface area of segment
         :rtype: float
         """
-        from math import pi
-        from math import sqrt
-
         if self.proximal==None:
             raise Exception('Cannot get surface area of segment '+str(self.id)+' using the surface_area property, since no proximal point is set on it (the proximal point comes from the parent segment). Use the method get_segment_surface_area(segment_id) on the cell instead.')
 
         prox_rad = self.proximal.diameter/2.0
         dist_rad = self.distal.diameter/2.0
 
         if self.proximal.x == self.distal.x and \
@@ -756,15 +752,14 @@
     def summary(self, show_includes=True, show_non_network=True):
         """Get a pretty-printed summary of the complete NeuroMLDocument.
 
         This includes information on the various Components included in the
         NeuroMLDocument: networks, cells, projections, synapses, and so on.
         """
 
-        import inspect
 
         info = "*******************************************************\\n"
         info+="* NeuroMLDocument: "+self.id+"\\n*\\n"
         post = ""
         membs = inspect.getmembers(self)
         for memb in membs:
             if isinstance(memb[1], list) and len(memb[1])>0 and not memb[0].endswith('_') and not memb[0] == 'networks':
@@ -888,15 +883,14 @@
         """Get a component by specifying its ID.
 
         :param id: id of Component to get
         :type id: str
         :returns: Component with given ID or None if no Component with provided ID was found
         """
         if len(id)==0:
-            import inspect
             callframe = inspect.getouterframes(inspect.currentframe(), 2)
             print('Method: '+ callframe[1][3] + ' is asking for an element with no id...')
 
             return None
         all_ids = []
         for ms in self.member_data_items_:
             mlist = getattr(self, ms.get_name())
@@ -905,20 +899,19 @@
                 continue
             for m in mlist:
                 if hasattr(m,"id"):
                     if m.id == id:
                         return m
                     else:
                         all_ids.append(m.id)
-        from neuroml.loaders import print_
         if self.warn_count<10:
-            print_("Id "+id+" not found in <neuroml> element. All ids: "+str(sorted(all_ids)))
+            neuroml.print_("Id "+id+" not found in <neuroml> element. All ids: "+str(sorted(all_ids)))
             self.warn_count+=1
         elif self.warn_count==10:
-            print_(" - Suppressing further warnings about id not found...")
+            neuroml.print_(" - Suppressing further warnings about id not found...")
         return None
 
     def append(self, element):
         """Append an element
 
         :param element: element to append
         :type element: Object
@@ -951,20 +944,19 @@
                 continue
             for m in mlist:
                 if hasattr(m,"id"):
                     if m.id == id:
                         return m
                     else:
                         all_ids.append(m.id)
-        from neuroml.loaders import print_
         if self.warn_count<10:
-            print_("Id "+id+" not found in <network> element. All ids: "+str(sorted(all_ids)))
+            neuroml.print_("Id "+id+" not found in <network> element. All ids: "+str(sorted(all_ids)))
             self.warn_count+=1
         elif self.warn_count==10:
-            print_(" - Suppressing further warnings about id not found...")
+            neuroml.print_(" - Suppressing further warnings about id not found...")
         return None
 
 
     def __str__(self):
 
         return "Network "+str(self.id)+" with "+str(len(self.populations))+" population(s)"
 
@@ -975,16 +967,14 @@
 METHOD_SPECS += (network_get_by_id,)
 
 
 cell_methods = MethodSpec(
     name="cell_methods",
     source='''\
 
-    from ..neuro_lex_ids import neuro_lex_ids
-
     # Get segment object by its id
     def get_segment(self, segment_id):
         # type: (int) -> Segment
         """Get segment object by its id
 
         :param segment_id: ID of segment
         :return: segment
@@ -1160,43 +1150,67 @@
 
     def get_ordered_segments_in_groups(self,
                                        group_list,
                                        check_parentage=False,
                                        include_cumulative_lengths=False,
                                        include_path_lengths=False,
                                        path_length_metric="Path Length from root"): # Only option supported
-        # type: (List, bool, bool, bool, str) -> Dict
+        # type: (List, bool, bool, bool, str) -> Any
         """
-        Get ordered list of segments in specified groups
+        Get ordered list of segments in specified groups, with additional
+        information.
+
+        Note that this method orders segments by id, so the assumption is that
+        all segment with id `N + m` will be a descendent of segment with id `N`
+        in the segment group.
 
-        :param group_list: a group id or list of groups to get segments from
-        :type group_list: str or list
+        :param group_list: a group id or list of group ids to get segments from
+        :type group_list: str or list(str)
         :param check_parentage: verify parentage
         :type check_parentage: bool
-        :param include_commulative_lengths: also include cummulative lengths
+        :param include_cumulative_lengths: also include cummulative length of
+            each segment from root
         :type include_cumulative_lengths: bool
-        :param include_path_lengths: also include path lengths
+        :param include_path_lengths: also include path lengths from segment
+            group's root segment to proximal and distal points of each segment
         :type include_path_lengths: bool
         :param path_length_metric: metric to use for path length ("Path Length
             from root" is currently the only supported option, and the default)
         :type path_length_metric: str
 
-        :return: dictionary of segments with additional information depending
-            on what parameters were used:
+        :returns: depending on provided arguments:
+
+                - if no additional options are provided, returns a dictionary
+                  with segment group ids as keys, and lists of ordered segments
+                  in those segment groups as values (`ord_segs`)
+                - if only `include_path_lengths` is set, returns a tuple:
+                  `[ord_segs, path_lengths_to_proximal ,
+                  path_lengths_to_distal]`
+                - if only `include_cumulative_lengths` is set, returns a tuple:
+                  `[ord_segs, cumulative_lengths]`
+                - if both `include_path_lengths` and
+                  `include_cumulative_lengths` are set, returns a tuple:
+                  `[ord_segs, cumulative_lengths, path_lengths_to_proximal ,
+                  path_lengths_to_distal]`
 
         :raises: Exception if check_parentage is True and parentage cannot be verified
         """
 
         unord_segs = {}
         other_segs = {}
 
         # convert to list if a single segment group ID has been provided
         if isinstance(group_list, str):
             group_list = [group_list]
 
+        # populate the dict to ensure that the order of segment groups is
+        # maintained in the returned result
+        for sgid in group_list:
+            unord_segs[sgid] = None
+
         # get a dict of all segments in the cell, with their ids as keys
         segments = self.get_segment_ids_vs_segments()
 
         # get list of segments in all segment groups
         # and store this information in two dicts:
         # - unord_segs: for segment groups in group_list
         # - other_segs: for segment groups not in group_list
@@ -1208,37 +1222,34 @@
                 unord_segs[sg.id] = [segments[s] for s in all_segs_here]
             else:
                 other_segs[sg.id] = [segments[s] for s in all_segs_here]
 
         ord_segs = {}
 
         # sort unord_segs by id to get an ordered list in ord_segs
-        from operator import attrgetter
-        for key in unord_segs.keys():
-            segs = unord_segs[key]
-            if len(segs)==1 or len(segs)==0:
-                ord_segs[key]=segs
-            else:
-                ord_segs[key]=sorted(segs,key=attrgetter('id'),reverse=False)
+        for key, segs in unord_segs.items():
+            if segs is not None:
+                if len(segs)==1 or len(segs)==0:
+                    ord_segs[key]=segs
+                else:
+                    ord_segs[key]=sorted(segs,key=attrgetter('id'),reverse=False)
 
         if check_parentage:
             # check parent ordering
 
             for key in ord_segs.keys():
                 existing_ids = []
                 for s in ord_segs[key]:
                     if s.id != ord_segs[key][0].id:
                         if not s.parent or not s.parent.segments in existing_ids:
                             raise Exception("Problem with finding parent of seg: "+str(s)+" in list: "+str(ord_segs))
                     existing_ids.append(s.id)
 
 
         if include_cumulative_lengths or include_path_lengths:
-            import math
-
             cumulative_lengths = {}
             path_lengths_to_proximal = {}
             path_lengths_to_distal = {}
 
             for key in ord_segs.keys():
                 cumulative_lengths[key] = []
                 path_lengths_to_proximal[key] = {}
@@ -1253,22 +1264,15 @@
 
                         path_lengths_to_proximal[key][seg.id] = 0
                         last_seg = seg
                         par_seg_element = seg.parent
                         while par_seg_element!=None:
 
                             par_seg = segments[par_seg_element.segments]
-                            d = par_seg.distal
-                            p = par_seg.proximal
-
-                            if not p:
-                                par_seg_parent_seg = segments[par_seg.parent.segments]
-                                p = par_seg_parent_seg.distal
-
-                            par_length = math.sqrt( (d.x-p.x)**2 + (d.y-p.y)**2 + (d.z-p.z)**2 )
+                            par_length = self.get_segment_length(par_seg.id)
 
                             fract = float(last_seg.parent.fraction_along)
                             path_lengths_to_proximal[key][seg.id] += par_length*fract
 
                             last_seg = par_seg
                             par_seg_element = par_seg.parent
 
@@ -1330,49 +1334,150 @@
             if substring in sg.id:
                 sgs[sg.id] = sg
         if len(sgs) == 0:
             raise ValueError("Segment group with id matching "+str(substring)+" not found in cell "+str(self.id))
         return sgs
 
 
-    def summary(self):
+    def summary(self, morph=True, biophys=True):
         """Print cell summary.
 
-        Currently prints:
+        Shows the number of segments and segment groups, and information on the
+        biophysical properties of the cell. See the `morphinfo` and
+        `biophysinfo` methods for more details.
+
+        :param morph: toggle showing/hiding morphology information
+        :type morph: bool
+        :param biophys: toggle showing/hiding biophysology information
+        :type biophys: bool
+        :returns: None
+        """
 
-        - id of cell
-        - any notes
-        - number of segments
-        - number of segment groups
+        print(f"*********** Summary ({self.id}) ************")
+        print("* Notes: "+str(self.notes))
+        print()
 
-        TODO: extend to show more information about the cell that may be useful
-        to users.
+        if morph:
+            print(f"*********** Morphology summary ({self.id}) ************")
+            self.morphinfo()
+            print("*******************************************************")
+            print("Tip: use morphinfo(True) to see more detailed information.")
+
+        if biophys:
+            print(f"*********** Biophys summary ({self.id}) ************")
+            self.biophysinfo()
+            print("*******************************************************")
+
+
+    def morphinfo(self, segment_detail=False):
+        """Show info on morphology of the cell.
+        By default, since cells can have large numbers of segments and segment
+        groups, it only provides metrics on the total numbers. To see details,
+        pass `segment_detail=True`.
+
+        See also: `get_segment_group_info`.
+
+        :param segment_detail: toggle whether to show detailed information on
+            segment groups and their segments
+        :type segment_detail: bool
+        :returns: None
 
         """
-
-        print("*******************************************************")
-        print("* Cell: "+str(self.id))
-        print("* Notes: "+str(self.notes))
         print("* Segments: "+str(len(self.morphology.segments)))
         print("* SegmentGroups: "+str(len(self.morphology.segment_groups)))
-        print("*******************************************************")
 
+        if segment_detail:
+            for sg in self.morphology.segment_groups:
+                self.get_segment_group_info(sg.id)
+
+
+    def biophysinfo(self):
+        """Get information on the biophysical properties of the cell.
+        :returns: None
+
+        """
+        bp = None
+        mp = None
+        ip = None
+        if self.__class__.__name__ == "Cell":
+            bp = self.biophysical_properties
+            mp = bp.membrane_properties
+            ip = bp.intracellular_properties
+        elif self.__class__.__name__ == "Cell2CaPools":
+            bp = self.biophysical_properties2_ca_pools
+            mp = bp.membrane_properties2_ca_pools
+            ip = bp.intracellular_properties2_ca_pools
+
+        membp = mp.info(show_contents=True, return_format="dict")
+        # check if there are any membrane properties
+        for prop, val in membp.items():
+            if len(val['members']) > 0:
+                print(f"* Membrane properties")
+                break
+
+        for prop, val in membp.items():
+            ctype = val['type']
+            # objects
+            ms = val['members']
+            if len(ms) > 0:
+                print(f"\t* {ctype}:")
+                for am in ms:
+                    inf = am.info(show_contents=True, return_format="dict")
+                    for p, v in inf.items():
+                        print(f"\t\t* {p}: {v['members']}")
+
+                    print()
+
+        intp = ip.info(show_contents=True, return_format="dict")
+        for prop, val in intp.items():
+            if len(val['members']) > 0:
+                print(f"* Intracellular properties")
+                break
+
+        for prop, val in intp.items():
+            ctype = val['type']
+            # objects
+            ms = val['members']
+            if len(ms) > 0:
+                print(f"\t* {ctype}:")
+                for am in ms:
+                    inf = am.info(show_contents=True, return_format="dict")
+                    for p, v in inf.items():
+                        print(f"\t\t* {p}: {v['members']}")
+
+                    print()
+
+    def get_segment_group_info(self, group_id):
+        """Get information about a segment group
+
+        :param group_id: id of segment group
+        :type group_id: int
+        :returns: None
+
+        """
+        print(f"* Segment group: {group_id}:")
+        segs = self.get_all_segments_in_group(segment_group=group_id)
+        for s in segs:
+            sinfo = self.get_segment(s)
+            print(f"\t * {s} (Parent: {sinfo.parent.segments if sinfo.parent else '-'}; {self.get_actual_proximal(s)} -> {sinfo.distal})")
 
     def add_segment(
         self,
         prox,
         dist,
         seg_id=None,
         name=None,
         parent=None,
         fraction_along=1.0,
         group_id=None,
         use_convention=True,
         seg_type=None,
         reorder_segment_groups=True,
+        optimise_segment_groups=True
+
     ):
         """Add a segment to the cell, to the provided segment group, creating
         it if required.
 
         :param prox: proximal segment information
         :type prox: list with 4 float entries: [x, y, z, diameter]
         :param dist: dist segment information
@@ -1397,16 +1502,16 @@
             If `use_convention` is `True`, and a `group_id` is provided, the
             segment group will also be added to the default segment groups if
             it has not been previously added. If `group_id` is `None`, the
             segment will be added to the default groups instead.
 
             If `use_convention` is `False`, this is unused.
         :type seg_type: str
-        :param parent: parent segment
-        :type parent: SegmentParent
+        :param parent: parent segment object
+        :type parent: Segment
         :param fraction_along: where the new segment is connected to the parent (0: distal point, 1: proximal point)
         :type fraction_along: float
         :param group_id: id of segment group to add the segment to
             If a segment group with this id does not exist, a new segment group
             will be created.
 
             The suggested convention is: `axon_`, `soma_`, `dend_` for axonal,
@@ -1428,14 +1533,17 @@
             included in the default groups should be declared before they are
             used in the default groups. When adding lots of segments, one may
             want to only reorder at the end of the process instead of after
             each segment is added.
 
             This is only relevant if `use_convention=True`.
         :type reorder_segment_groups: bool
+        :param optimise_segment_groups: toggle whether segment groups should be
+            optimised after operation
+        :type optimise_segment_groups: bool
         :returns: the created segment
         :rtype: Segment
         :raises ValueError: if `seg_id` is provided and a segment with this ID
             already exists
 
         """
         try:
@@ -1469,15 +1577,15 @@
         )
 
         if seg_id:
             try:
                 seg = None
                 seg = self.get_segment(seg_id)
                 if seg:
-                    raise ValueError("A segment with provided id f{seg_id} already exists")
+                    raise ValueError(f"A segment with provided id {seg_id} already exists")
             except ValueError:
                 # a segment with this ID does not already exist
                 pass
         else:
             seg_id = segid
 
         segment = self.component_factory("Segment", id=seg_id, proximal=p, distal=d, parent=sp)
@@ -1498,35 +1606,30 @@
                 )
             seg_group.members.append(Member(segments=segment.id))
 
         if use_convention:
             if not seg_type:
                 raise ValueError("Please provide a seg_type")
             if seg_type == "axon":
-                seg_group_default = self.get_segment_group("axon_group")
+                [seg_group_all, seg_group_default] = self.setup_default_segment_groups(use_convention=True, default_groups=["all", "axon_group"])
             elif seg_type == "soma":
-                seg_group_default = self.get_segment_group("soma_group")
+                [seg_group_all, seg_group_default] = self.setup_default_segment_groups(use_convention=True, default_groups=["all", "soma_group"])
             elif seg_type == "dendrite":
-                seg_group_default = self.get_segment_group("dendrite_group")
+                [seg_group_all, seg_group_default] = self.setup_default_segment_groups(use_convention=True, default_groups=["all", "dendrite_group"])
             else:
                 raise ValueError(f"Invalid segment type provided: {seg_type}")
 
-            seg_group_all = self.get_segment_group("all")
-
-            # get_segment_group raises a ValueError, so won't get here if one
-            # is not found
-
             # Now add the segment group that contains this segment if it exists
             # to the global groups. If a segment group does not exist for this
             # segment, add the segment itself to the global groups
 
             # Do not use add here, we do not need it's extra features (and
             # their performance costs)
             # De-duplicate/optimise later if required
-            if seg_group:
+            if seg_group and seg_group.id != seg_group_default.id:
                 seg_group_default.includes.append(Include(segment_groups=seg_group.id))
                 seg_group_all.includes.append(Include(segment_groups=seg_group.id))
             else:
                 seg_group_default.members.append(Member(segments=segment.id))
                 seg_group_all.members.append(Member(segments=segment.id))
 
             if reorder_segment_groups:
@@ -1545,53 +1648,75 @@
             else:
                 # if it doesn't belong to a group, use the type to indicate
                 # what kind of segment this is
                 segment_name = f"Seg{seg_id}"
             segment.name = segment_name
 
         self.morphology.segments.append(segment)
+
+        if optimise_segment_groups:
+            self.optimise_segment_groups()
+
         return segment
 
-    def add_segment_group(self, group_id):
+    def add_segment_group(self, group_id, neuro_lex_id=None, notes=None):
         """Add a new general segment group.
 
         The segments included in this group do not need to be contiguous. This
-        segment group will not be marked as a section using the required
-        NeuroLex ID.
+        segment group will not be automatically marked as a section using the
+        required NeuroLex ID.
+
+        If a segment group with provided ID already exists, it will not be
+        overwritten.
 
         :param group_id: ID of segment group
         :type group_id: str
+        :param neuro_lex_id: NeuroLex ID to use for segment group
+        :type neuro_lex_id: str
+        :param notes: Notes text to add
+        :type notes: str
         :returns: new segment group
         :rtype: SegmentGroup
 
         """
-        seg_group = self.component_factory(
-            "SegmentGroup", id=group_id
-        )
-        self.morphology.segment_groups.append(seg_group)
+        seg_group = None
+        try:
+            seg_group = self.get_segment_group(group_id)
+        except ValueError:
+            seg_group = self.morphology.add(
+                "SegmentGroup", id=group_id,
+                neuro_lex_id=neuro_lex_id,
+                notes=notes, validate=False
+            )
+        else:
+            print(f"Warning: Segment group {seg_group.id} already exists.")
+
         return seg_group
 
 
-    def add_unbranched_segment_group(self, group_id):
+    def add_unbranched_segment_group(self, group_id, notes=None):
         """Add a new unbranched segment group.
 
         This is similar to the `add_segment_group` method, but this segment
         group will be used to store contiguous segments, which form an
-        unbranched section of a cell.
+        unbranched section of a cell. It adds the NeuroLex ID for a neuronal
+        branch to the segment group.
 
         :param group_id: ID of segment group
         :type group_id: str
+        :param notes: notes to add
+        :type notes: str
         :returns: new segment group
         :rtype: SegmentGroup
 
         """
-        seg_group = self.component_factory(
-            "SegmentGroup", id=group_id, neuro_lex_id=self.neuro_lex_ids["section"]
+        seg_group = self.add_segment_group(
+            group_id=group_id, neuro_lex_id=neuroml.neuro_lex_ids.neuro_lex_ids["section"],
+            notes=notes
         )
-        self.morphology.segment_groups.append(seg_group)
         return seg_group
 
 
     def reorder_segment_groups(self):
         """Move default segment groups to the end.
 
         This is required so that the segment groups included in the default
@@ -1600,18 +1725,18 @@
         :returns: None
 
         """
         seg_groups = self.morphology.segment_groups
         for group in ["soma_group", "axon_group", "dendrite_group", "all"]:
             try:
                 sg = self.get_segment_group(group)
+                seg_groups.append(seg_groups.pop(seg_groups.index(sg)))
             except ValueError:
                 pass
 
-            seg_groups.append(seg_groups.pop(seg_groups.index(sg)))
 
     def optimise_segment_groups(self):
         """Optimise all segment groups in the cell.
 
         This will:
 
         - deduplicate members and includes in segment groups
@@ -1664,73 +1789,75 @@
         """Set the spike threshold of the cell.
 
         :param v: value to set for spike threshold with units
         :type v: str
         :param group_id: id of segment group to modify
         :type group_id: str
         """
-        self.biophysical_properties.membrane_properties.add(
+        self.add_membrane_property(
             "SpikeThresh", value=v, segment_groups=group_id
         )
 
 
     def set_init_memb_potential(self, v, group_id="all"):
         """Set the initial membrane potential of the cell.
 
         :param v: value to set for membrane potential with units
         :type v: str
         :param group_id: id of segment group to modify
         :type group_id: str
         """
-        self.biophysical_properties.membrane_properties.add(
+        self.add_membrane_property(
             "InitMembPotential", value=v, segment_groups=group_id
         )
 
 
     def set_resistivity(self, resistivity, group_id="all") -> None:
         """Set the resistivity of the cell
 
         :type resistivity: str
         :param group_id: segment group to modify
         :type group_id: str
         """
-        self.biophysical_properties.intracellular_properties.add(
+        self.add_intracellular_property(
             "Resistivity", value=resistivity, segment_groups=group_id
         )
 
 
     def set_specific_capacitance(
         self, spec_cap, group_id="all"
     ):
         """Set the specific capacitance for the cell.
 
         :param spec_cap: value of specific capacitance with units
         :type spec_cap: str
         :param group_id: segment group to modify
         :type group_id: str
         """
-        self.biophysical_properties.membrane_properties.add(
+        self.add_membrane_property(
             "SpecificCapacitance", value=spec_cap, segment_groups=group_id
         )
 
 
     def add_intracellular_property(self, property_name, **kwargs):
         """Generic function to add an intracellular property to the cell.
 
         For a full list of membrane properties, see:
         https://docs.neuroml.org/Userdocs/Schemas/Cells.html?#intracellularproperties
 
         :param property_name: name of intracellular property to add
         :type property_name: str
         :param kwargs: named arguments for intracellular property to be added
         :type kwargs: Any
-        :returns: None
+        :returns: added property
 
         """
-        self.biophysical_properties.intracellular_properties.add(property_name, **kwargs)
+        self.setup_nml_cell(use_convention=False)
+        prop = self.biophysical_properties.intracellular_properties.add(property_name, **kwargs)
+        return prop
 
 
     def add_membrane_property(self, property_name, **kwargs):
         """Generic function to add a membrane property to the cell.
 
         For a full list of membrane properties, see:
         https://docs.neuroml.org/Userdocs/Schemas/Cells.html?#membraneproperties
@@ -1738,18 +1865,20 @@
         Please also see specific functions in this module, which are designed to be
         easier to use than this generic function.
 
         :param property_name: name of membrane to add
         :type property_name: str
         :param kwargs: named arguments for membrane property to be added
         :type kwargs: Any
-        :returns: None
+        :returns: added property
 
         """
-        self.biophysical_properties.membrane_properties.add(property_name, **kwargs)
+        self.setup_nml_cell(use_convention=False)
+        prop = self.biophysical_properties.membrane_properties.add(property_name, **kwargs)
+        return prop
 
 
     def add_channel_density_v(
         self,
         channel_density_type,
         nml_cell_doc,
         ion_chan_def_file="",
@@ -1763,26 +1892,28 @@
         :type channel_density_type: str
         :param nml_cell_doc: cell NeuroML document to which channel density is to be added
         :type nml_cell_doc: NeuroMLDocument
         :param ion_chan_def_file: path to NeuroML2 file defining the ion channel, if empty, it assumes the channel is defined in the same file
         :type ion_chan_def_file: str
         :param kwargs: named arguments for required channel density type
         :type kwargs: Any
-        :returns: None
+        :returns: added channel density
         """
 
-        self.add_membrane_property(channel_density_type, **kwargs)
+        cd = self.add_membrane_property(channel_density_type, **kwargs)
 
         if len(ion_chan_def_file) > 0:
             if (
                 self.component_factory("IncludeType", href=ion_chan_def_file)
                 not in nml_cell_doc.includes
             ):
                 nml_cell_doc.add("IncludeType", href=ion_chan_def_file)
 
+        return cd
+
 
     def add_channel_density(
         self,
         nml_cell_doc,
         cd_id,
         ion_channel,
         cond_density,
@@ -1805,16 +1936,18 @@
         :type erev: str
         :param group_id: segment groups to add to
         :type group_id: str
         :param ion: name of ion
         :type ion: str
         :param ion_chan_def_file: path to NeuroML2 file defining the ion channel, if empty, it assumes the channel is defined in the same file
         :type ion_chan_def_file: str
+        :returns: added channel density
+        :rtype: ChannelDensity
         """
-        cd = self.biophysical_properties.membrane_properties.add(
+        cd = self.add_membrane_property(
             "ChannelDensity",
             id=cd_id,
             segment_groups=group_id,
             ion=ion,
             ion_channel=ion_channel,
             erev=erev,
             cond_density=cond_density,
@@ -1823,90 +1956,119 @@
         if len(ion_chan_def_file) > 0:
             if (
                 self.component_factory("IncludeType", href=ion_chan_def_file)
                 not in nml_cell_doc.includes
             ):
                 nml_cell_doc.add("IncludeType", href=ion_chan_def_file)
 
-    def setup_nml_cell(self, use_convention=True, overwrite=False):
+        return cd
+
+    def setup_nml_cell(self, use_convention=True, overwrite=False, default_groups=["all", "soma_group"]):
         """Correctly initialise a NeuroML cell.
 
         To be called after a new component has been created to initialise the
         cell with these properties:
 
         - Morphology: id="morphology"
         - BiophysicalProperties: id="biophys":
 
           - MembraneProperties
           - IntracellularProperties
 
-        If `use_convention` is True, it also creates some default SegmentGroups for
-        convenience:
-
-        - "all", "soma_group", "dendrite_group", "axon_group" which
-          are used by other helper functions to include all, soma, dendrite, and
-          axon segments respectively.
+        If `use_convention` is True, it also creates the provided
+        `default_groups` SegmentGroups for convenience. By default, it creates
+        the "all", and "soma_group" groups since each cell must at least have a
+        soma.
+
+        When dendritic and axonal segments are added, the `add_segment`
+        function will create `dendrite_group` and `axon_group` groups as
+        required.
 
         Note that since this cell does not currently include a segment in its
         morphology, it is *not* a valid NeuroML construct. Use the `add_segment`
         and `add_unbranched_segments` functions to add segments and branches.
         They will also populate the default segment groups.
 
         :param id: id of the cell
         :type id: str
         :param use_convention: whether helper segment groups should be created using the default convention
         :type use_convention: bool
         :param overwrite: overwrite existing components
         :type overwrite: bool
+        :param default_groups: list of default segment groups to create
+        :type default_groups: list of strings
         :returns: None
         :rtype: None
 
         """
         # do not validate yet, because segments are required
         self.add("Morphology", id="morphology", validate=False, force=overwrite)
 
         # add does not overwrite existing values
         self.add("BiophysicalProperties", id="biophys", validate=False, force=overwrite)
         self.biophysical_properties.add("IntracellularProperties", validate=False, force=overwrite)
         self.biophysical_properties.add("MembraneProperties", validate=False, force=overwrite)
 
+        self.setup_default_segment_groups(use_convention, default_groups)
+
+
+    def setup_default_segment_groups(self, use_convention=True, default_groups=["all", "soma_group"]):
+        """Create default segment groups for the cell.
+
+        If `use_convention` is True, it also creates the provided
+        `default_groups` SegmentGroups for convenience. By default, it creates
+        the "all", and "soma_group" groups since each cell must at least have a
+        soma. Allowed values are: "all", "soma_group", "axon_group", "dendrite_group".
+
+        :param use_convention: whether helper segment groups should be created using the default convention
+        :type use_convention: bool
+        :param default_groups: list of default segment groups to create
+        :type default_groups: list of strings
+        :returns: list of created segment groups (or empty list if none created)
+        :rtype: list
+        """
+        new_groups = []
         if use_convention:
-            seg_group_all = self.component_factory("SegmentGroup", id="all")
-            seg_group_soma = self.component_factory(
-                "SegmentGroup",
-                id="soma_group",
-                neuro_lex_id=self.neuro_lex_ids["soma"],
-                notes="Default soma segment group for the cell",
-            )
-            seg_group_axon = self.component_factory(
-                "SegmentGroup",
-                id="axon_group",
-                neuro_lex_id=self.neuro_lex_ids["axon"],
-                notes="Default axon segment group for the cell",
-            )
-            seg_group_dend = self.component_factory(
-                "SegmentGroup",
-                id="dendrite_group",
-                neuro_lex_id=self.neuro_lex_ids["dend"],
-                notes="Default dendrite segment group for the cell",
-            )
-            # skip validation: segments etc needed, cell is invalid
-            self.morphology.add(seg_group_all, validate=False, force=overwrite)
-            self.morphology.add(seg_group_soma, validate=False, force=overwrite)
-            self.morphology.add(seg_group_axon, validate=False, force=overwrite)
-            self.morphology.add(seg_group_dend, validate=False, force=overwrite)
+            for grp in default_groups:
+                neuro_lex_id = None
+                notes = None
+
+                if grp == "soma_group":
+                    neuro_lex_id=neuroml.neuro_lex_ids.neuro_lex_ids["soma"]
+                    notes="Default soma segment group for the cell"
+                elif grp == "axon_group":
+                    neuro_lex_id=neuroml.neuro_lex_ids.neuro_lex_ids["axon"]
+                    notes="Default axon segment group for the cell"
+                elif grp == "dendrite_group":
+                    neuro_lex_id=neuroml.neuro_lex_ids.neuro_lex_ids["dend"]
+                    notes="Default dendrite segment group for the cell"
+                elif grp == "all":
+                    neuro_lex_id=None
+                    notes="Default segment group for all segments in the cell"
+                else:
+                    print(f"Error: only 'all', 'soma_group', 'dendrite_group', and 'axon_group' are supported. Received {grp}")
+                    return []
+
+                seg_group = self.add_segment_group(group_id=grp, neuro_lex_id=neuro_lex_id, notes=notes)
+                new_groups.append(seg_group)
+
+            self.reorder_segment_groups()
+
+        return new_groups
 
     def add_unbranched_segments(
         self,
         points,
         parent=None,
         fraction_along=1.0,
         group_id=None,
         use_convention=True,
-        seg_type=None
+        seg_type=None,
+        reorder_segment_groups=True,
+        optimise_segment_groups=True
     ):
         """Add an unbranched list of segments to the cell.
 
         The list of points will include the first proximal point where this
         should be joined to the cell, followed by a list of distal points:
 
         ::
@@ -1936,14 +2098,28 @@
         :type group_id: SegmentGroup
         :param use_convention: whether helper segment groups should be created using the default convention
             See the documentation of the `add_segment` method for more information
             on the convention
         :type use_convention: bool
         :param seg_type: type of segments ("axon", "soma", "dendrite")
         :type seg_type: str
+        :param reorder_segment_groups: whether the groups should be reordered
+            to put the default segment groups last after the segment has been
+            added.
+            This is required for a valid NeuroML file because segment groups
+            included in the default groups should be declared before they are
+            used in the default groups. When adding lots of segments, one may
+            want to only reorder at the end of the process instead of after
+            each segment is added.
+
+            This is only relevant if `use_convention=True`.
+        :type reorder_segment_groups: bool
+        :param optimise_segment_groups: toggle whether segment groups should be
+            optimised after operation
+        :type optimise_segment_groups: bool
         :returns: the segment group containing this new list of segments
         :rtype: SegmentGroup
 
         """
         prox = points[0]
         dist = points[1]
 
@@ -1963,18 +2139,23 @@
             seg = self.add_segment(prox=prox, dist=dist, name=None, parent=seg,
                                    fraction_along=1.0, group_id=group_id,
                                    use_convention=use_convention,
                                    seg_type=seg_type,
                                    reorder_segment_groups=False)
             prox = dist
 
-        self.reorder_segment_groups()
+        if reorder_segment_groups:
+            self.reorder_segment_groups()
+
+        if optimise_segment_groups:
+            self.optimise_segment_groups()
+
         return self.get_segment_group(group_id)
 
-    def create_unbranched_segment_group_branches(self, root_segment_id: int, use_convention: bool=True):
+    def create_unbranched_segment_group_branches(self, root_segment_id: int, use_convention: bool=True, reorder_segment_groups=True, optimise_segment_groups=True):
         """Organise the segments of the cell into new segment groups that each
         form a single contiguous unbranched cell branch.
 
         Note that the first segment (root segment) of a branch must have a proximal
         point that connects it to the rest of the neuronal morphology. If, when
         constructing these branches, a root segment is found that does not include
         a proximal point, one will be added using the `get_actual_proximal` method.
@@ -1983,29 +2164,53 @@
         segment groups.
 
         :param root_segment_id: id of segment considered the root of the tree,
             generally the first soma segment
         :type root_segment_id: int
         :param use_convention: toggle using NeuroML convention for segment groups
         :type use_convention: bool
+        :param reorder_segment_groups: whether the groups should be reordered
+            to put the default segment groups last after the segment has been
+            added.
+            This is required for a valid NeuroML file because segment groups
+            included in the default groups should be declared before they are
+            used in the default groups. When adding lots of segments, one may
+            want to only reorder at the end of the process instead of after
+            each segment is added.
+
+            This is only relevant if `use_convention=True`.
+        :type reorder_segment_groups: bool
+        :param optimise_segment_groups: toggle whether segment groups should be
+            optimised after operation
+        :type optimise_segment_groups: bool
         :returns: modified cell with new section groups
         :rtype: neuroml.Cell
 
         """
+        # don't recompute if already exists
         # get morphology tree
-        morph_tree = self.get_segment_adjacency_list()
+        morph_tree = getattr(self, "adjacency_list", None)
+        if morph_tree is None:
+            morph_tree = self.get_segment_adjacency_list()
 
         # initialise root segment and first segment group
         seg = self.get_segment(root_segment_id)
         group_name = f"seg_group_{len(self.morphology.segment_groups) - 1}_seg_{seg.id}"
         new_seg_group = self.add_unbranched_segment_group(group_name)
 
         # run recursive function
         self.__sectionise(root_segment_id, new_seg_group, morph_tree)
 
+        if reorder_segment_groups:
+            self.reorder_segment_groups()
+
+        if optimise_segment_groups:
+            self.optimise_segment_groups()
+
+
 
     def __sectionise(self, root_segment_id, seg_group, morph_tree):
         """Main recursive sectionising method.
 
         :param root_segment_id: id of root of branch
         :type root_segment_id: int
         :returns: TODO
@@ -2053,45 +2258,301 @@
         """Get the adjacency list of all segments in the cell morphology.
         Returns a dict where each key is a parent segment, and the value is the
         list of its children segments.
 
         Segment without children (leaf segments) are not included as parents in the
         adjacency list.
 
-        :returns: dict with parent segments as keys and their children as values
-        :rtype: dict
+        This method also stores the computed adjacency list in
+        `self.adjacency_list` for future use by other methods.
+
+        `self.adjacency_list` is populated each time this method is run, to
+        ensure that users can regenerate it after making modifications to the
+        cell morphology. If the morphology has not changed, one only needs to
+        populate it once and then re-use it as required.
+
+        :returns: dict with parent segment ids as keys and ids of their children as values
+        :rtype: dict[int, list[int]]
 
         """
         # create data structure holding list of children for each segment
         child_lists = {}
         for segment in self.morphology.segments:
             try:
                 parent = segment.parent.segments
                 if parent not in child_lists:
                     child_lists[parent] = []
                 child_lists[parent].append(segment.id)
             except AttributeError:
                 print(f"Warning: Segment: {segment} has no parent")
 
+        self.adjacency_list = child_lists
         return child_lists
 
+    def get_graph(self):
+        """Get a networkx DiGraph of the morphology of the cell with distances
+        between the proximal point of a parent and the point where a child
+        connects to it as the weights of the edges of the graph.
+
+        Please see https://networkx.org/documentation/stable/reference
+        for information on networkx routines that can be used on this graph.
+
+        This method also stores the graph in the `self.cell_graph` attribute
+        for future use.
+
+        :returns: networkx.Graph
+
+        """
+        cell_graph = nx.DiGraph()
+
+        # don't recompute if already exists
+        adlist = getattr(self, "adjacency_list", None)
+        if adlist is None:
+            adlist = self.get_segment_adjacency_list()
+
+        for parid, childrenids in adlist.items():
+
+            par_length = self.get_segment_length(parid)
+
+            for cid in childrenids:
+                child = self.get_segment(cid)
+
+                fract = float(child.parent.fraction_along)
+                len_to_proximal = par_length*fract
+
+                cell_graph.add_edge(parid, cid, weight=len_to_proximal)
+
+        self.cell_graph = cell_graph
+        return cell_graph
+
+    def get_distance(self, dest, source = 0):
+        """Get path length between between two segments on a cell.
+
+        Uses `networkx.dijkstra_path_length` to compute the shortest
+        path between source and dest
+
+        :param from: id of segment to get distance from
+        :type from: int
+        :param to: id of segment to get distance to
+        :type to: int
+        :returns: float
+        """
+        graph = getattr(self, "cell_graph", None)
+        if graph is None:
+            graph = self.get_graph()
+        return nx.dijkstra_path_length(graph, source, dest)
+
+    def get_all_distances_from_segment(self, seg_id = 0):
+        """Get distances of all segments from the segment with id seg_id.
+
+        Useful to get distances of segments from the soma.
+
+        Uses networkx.single_source_dijkstra on the cell graph, without a
+        target.
+
+        :param seg_id: id of segment to get distances from
+        :type seg_id: int
+        :returns: pair of dictionaries for distance, path
+            The return value is a tuple of two dictionaries keyed by target
+            nodes. The first dictionary stores distance to each target node.
+            The second stores the path to each target node.
+
+        """
+        graph = getattr(self, "cell_graph", None)
+        if graph is None:
+            graph = self.get_graph()
+        return(nx.single_source_dijkstra(graph, source=seg_id))
+
+    def get_segments_at_distance(self, distance, src_seg = 0):
+        """Get all segments at distance from the provided `src_seg`.
+
+        For each segment, it returns the fraction along the segment that the
+        provided distance is at. For example, if segment N is 500 units long,
+        and the `distance` cut-off is at 200, the fraction along is: 200/500.
+
+        :param src_seg: id of segment to get distances from
+        :type src_seg: int
+        :param distance: distance to get segments at
+        :type distance: float
+        :returns: dict with segment ids as keys, and fraction along at which
+            the cut off is as values
+
+        """
+        graph = getattr(self, "cell_graph", None)
+        if graph is None:
+            graph = self.get_graph()
+        # returns all segments that are less than `distance` away.
+        (target_dict, path_dict) = (nx.single_source_dijkstra(graph, source=src_seg, cutoff=distance))
+
+        segs_frac_alongs = {}
+
+        for tgt, dist in target_dict.items():
+            try:
+                frac_along = ((distance - dist) / self.get_segment_length(tgt))
+            except ZeroDivisionError:
+                # ignore zero length segments
+                print(f"Warning: encountered zero length segment: {tgt}")
+                continue
+
+            if frac_along > 1.0:
+                # not in this segment
+                continue
+            else:
+                segs_frac_alongs[tgt] = frac_along
+
+        return segs_frac_alongs
+
+
+    def get_branching_points(self):
+        """Get segments where the cell morphology branches.
+
+        That is, the out-degree of the segment is > 1
+
+        :returns: list of segment ids
+
+        """
+        graph = getattr(self, "cell_graph", None)
+        if graph is None:
+            graph = self.get_graph()
+
+        segs = [n for (n, d) in graph.out_degree if d > 1]
+        return segs
+
+
+    def get_extremeties(self):
+        """Get segments that are at the ends/tips of the neuronal morphology,
+        with their distances from the soma.
+
+        :returns: dict of segment ids and their distances from cell root as values
+
+        """
+        graph = getattr(self, "cell_graph", None)
+        if graph is None:
+            graph = self.get_graph()
+        segs = [n for (n, d) in graph.out_degree if d == 0]
+
+        res = {}
+        for s in segs:
+            res[s] = self.get_distance(s)
+        return res
+
+
+    def get_segment_location_info(self, seg_id):
+        """Get location information about a particular segment.
+
+        :param seg_id: id of segment to get information for
+        :type seg_id: int
+        :returns: a dictionary with various metrics about the segment
+
+            - length of segment
+            - distance from cell root
+            - distance from nearest branching point
+            - name of unbranched segment group segment belongs to (if any)
+            - id of root segment of the unbranched segment group
+            - distance from the segment group root segment
+
+        """
+        soma_id = self.get_morphology_root()
+        distance_from_soma = self.get_distance(seg_id, source=soma_id)
+        in_sg = None
+        sg_segs = None
+        sg_root = None
+        distance_from_sg_root = None
+        distance_from_bpt = None
+
+        # get the unbranched segment group that this segment is in
+        for sg in self.morphology.segment_groups:
+            if sg.neuro_lex_id == neuroml.neuro_lex_ids.neuro_lex_ids["section"]:
+                sg_segs = self.get_all_segments_in_group(sg)
+                if seg_id in sg_segs:
+                    in_sg = sg
+
+                    # break out of loop
+                    break
+
+        graph = getattr(self, "cell_graph", None)
+        if graph is None:
+            graph = self.get_graph()
+
+        # find first ancestral branching point
+        # (a segment with more than one child)
+        current = seg_id
+        sg_root = current
+        parent = list(graph.predecessors(current))[0]
+        children = list(graph.successors(parent))
+
+        while len(children) == 1:
+            # the root of the segment group may not be at a
+            # branching point: an unbranched cell branch can consist of
+            # multiple unbranched segment groups
+            if in_sg is not None:
+                if current in sg_segs:
+                    sg_root = current
+
+            current = parent
+            parent = list(graph.predecessors(current))[0]
+            children = list(graph.successors(parent))
+
+        distance_from_bpt = self.get_distance(seg_id, source=current)
+
+        res = {}
+        res['id'] = seg_id
+        res['length'] = self.get_segment_length(seg_id)
+        res['distance_from_cell_root'] = distance_from_soma
+        res['distance_from_nearest_branching_point'] = distance_from_bpt
+
+        # at unbranched segment root
+        if in_sg is not None:
+            res['in_unbranched_segment_group'] = in_sg.id
+            res['unbranched_segment_group_root'] = sg_root
+            distance_from_sg_root = self.get_distance(seg_id, source=sg_root)
+            res['distance_from_segment_group_root'] = distance_from_sg_root
+
+        return res
+
+
+    def get_morphology_root(self):
+        """Return the root of the complete cell morphology.
+
+        This is usually the first segment of the soma, and there should only be
+        one such segment.
+
+        :returns: id of the root segment
+
+        """
+        # check if convention was followed and segment id 0 is root (has no
+        # parents)
+        try:
+            root_seg = self.get_segment(0)
+            if root_seg.parent is None:
+                return 0
+        except ValueError:
+            pass
+
+        graph = getattr(self, "cell_graph", None)
+        if graph is None:
+            graph = self.get_graph()
+        segs = [n for (n, d) in graph.in_degree if d == 0]
+        # there should only be one segment with 0 indegree
+        assert len(segs) == 1
+        return segs[0]
+
     ''',
     class_names=("Cell"),
 )
 
 METHOD_SPECS += (cell_methods,)
 
 
 inserts = {}
 
 inserts[
     "Network"
 ] = """
 
-        import numpy
 
         netGroup = h5file.create_group(h5Group, 'network')
         netGroup._f_setattr("id", self.id)
         netGroup._f_setattr("notes", self.notes)
         if self.temperature:
             netGroup._f_setattr("temperature", self.temperature)
 
@@ -2118,16 +2579,14 @@
 
 """
 
 inserts[
     "Population"
 ] = """
 
-        import numpy
-
         popGroup = h5file.create_group(h5Group, 'population_'+self.id)
         popGroup._f_setattr("id", self.id)
         popGroup._f_setattr("component", self.component)
         for p in self.properties:
             popGroup._f_setattr("property:"+p.tag, p.value)
 
 
@@ -2164,16 +2623,14 @@
 
 """
 
 inserts[
     "Projection"
 ] = """
 
-        import numpy
-
         projGroup = h5file.create_group(h5Group, 'projection_'+self.id)
         projGroup._f_setattr("id", self.id)
         projGroup._f_setattr("type", "projection")
         projGroup._f_setattr("presynapticPopulation", self.presynaptic_population)
         projGroup._f_setattr("postsynapticPopulation", self.postsynaptic_population)
         projGroup._f_setattr("synapse", self.synapse)
 
@@ -2181,17 +2638,15 @@
 
         connection_wds = len(self.connection_wds) > 0
 
         cols = 2
 
         extra_cols = {}
 
-        from neuroml.utils import has_segment_fraction_info
-
-        include_segment_fraction = has_segment_fraction_info(self.connections) or has_segment_fraction_info(self.connection_wds)
+        include_segment_fraction = neuroml.utils.has_segment_fraction_info(self.connections) or neuroml.utils.has_segment_fraction_info(self.connection_wds)
 
         if include_segment_fraction:
             extra_cols["column_"+str(cols)] = "pre_segment_id"
             extra_cols["column_"+str(cols+1)] = "post_segment_id"
             extra_cols["column_"+str(cols+2)] = "pre_fraction_along"
             extra_cols["column_"+str(cols+3)] = "post_fraction_along"
             cols +=4
@@ -2257,16 +2712,14 @@
 
 """
 
 inserts[
     "ElectricalProjection"
 ] = """
 
-        import numpy
-
         projGroup = h5file.create_group(h5Group, 'projection_'+self.id)
         projGroup._f_setattr("id", self.id)
         projGroup._f_setattr("type", "electricalProjection")
         projGroup._f_setattr("presynapticPopulation", self.presynaptic_population)
         projGroup._f_setattr("postsynapticPopulation", self.postsynaptic_population)
 
         syn = self.electrical_connections[0].synapse if len(self.electrical_connections)>0 else \
@@ -2334,16 +2787,14 @@
 """
 
 
 inserts[
     "ContinuousProjection"
 ] = """
 
-        import numpy
-
         projGroup = h5file.create_group(h5Group, 'projection_'+self.id)
         projGroup._f_setattr("id", self.id)
         projGroup._f_setattr("type", "continuousProjection")
         projGroup._f_setattr("presynapticPopulation", self.presynaptic_population)
         projGroup._f_setattr("postsynapticPopulation", self.postsynaptic_population)
 
         pre_comp = self.continuous_connections[0].pre_component if len(self.continuous_connections)>0 else \
@@ -2417,16 +2868,14 @@
 """
 
 
 inserts[
     "InputList"
 ] = """
 
-        import numpy
-
         ilGroup = h5file.create_group(h5Group, 'inputList_'+self.id)
         ilGroup._f_setattr("id", self.id)
         ilGroup._f_setattr("component", self.component)
         ilGroup._f_setattr("population", self.populations)
 
         cols = 4
```

### Comparing `libNeuroML-0.4.1/neuroml/nml/nml.py` & `libNeuroML-0.5.1/neuroml/nml/nml.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #
-# Generated Tue Oct 11 14:23:30 2022 by generateDS.py version 2.40.13.
-# Python 3.10.7 (main, Sep  7 2022, 00:00:00) [GCC 12.2.1 20220819 (Red Hat 12.2.1-1)]
+# Generated Wed May  3 13:39:08 2023 by generateDS.py version 2.41.3.
+# Python 3.10.11 (main, Apr  5 2023, 00:00:00) [GCC 13.0.1 20230404 (Red Hat 13.0.1-0)]
 #
 # Command line options:
 #   ('-o', 'nml.py')
 #   ('--use-getter-setter', 'none')
 #   ('--user-methods', 'helper_methods.py')
 #   ('--export', 'write validate')
+#   ('--custom-imports-template', 'gds_imports-template.py')
 #
 # Command line arguments:
 #   NeuroML_v2.3.xsd
 #
 # Command line:
-#   /home/asinha/.local/share/virtualenvs/neuroml-dev/bin/generateDS -o "nml.py" --use-getter-setter="none" --user-methods="helper_methods.py" --export="write validate" NeuroML_v2.3.xsd
+#   /home/asinha/.local/share/virtualenvs/neuroml-310/bin/generateDS -o "nml.py" --use-getter-setter="none" --user-methods="helper_methods.py" --export="write validate" --custom-imports-template="gds_imports-template.py" NeuroML_v2.3.xsd
 #
 # Current working directory (os.getcwd()):
 #   nml
 #
 
 import sys
 
@@ -31,14 +32,30 @@
 import os
 import re as re_
 import base64
 import datetime as datetime_
 import decimal as decimal_
 from lxml import etree as etree_
 
+import math
+
+from math import pi, sqrt
+
+from operator import attrgetter
+
+import inspect
+
+import networkx as nx
+
+import numpy
+
+
+import neuroml
+
+import neuroml.neuro_lex_ids
 
 Validate_simpletypes_ = True
 SaveElementTreeNode = True
 TagNamePrefix = ""
 if sys.version_info.major == 2:
     BaseStrType_ = basestring
 else:
@@ -1164,14 +1181,19 @@
 
 
 class PlasticityTypes(str, Enum):
     TSODYKS_MARKRAM_DEP_MECHANISM = "tsodyksMarkramDepMechanism"
     TSODYKS_MARKRAM_DEP_FAC_MECHANISM = "tsodyksMarkramDepFacMechanism"
 
 
+class TrueOrFalse(str, Enum):
+    TRUE = "true"
+    FALSE = "false"
+
+
 class ZeroOrOne(str, Enum):
     """ZeroOrOne -- Value which is either 0 or 1"""
 
     _0 = "0"
     _1 = "1"
 
 
@@ -1245,14 +1267,27 @@
                 "minOccurs": "0",
                 "name": "Parameter",
                 "type": "Parameter",
             },
             None,
         ),
         MemberSpec_(
+            "DerivedParameter",
+            "DerivedParameter",
+            1,
+            1,
+            {
+                "maxOccurs": "unbounded",
+                "minOccurs": "0",
+                "name": "DerivedParameter",
+                "type": "DerivedParameter",
+            },
+            None,
+        ),
+        MemberSpec_(
             "Constant",
             "Constant",
             1,
             1,
             {
                 "maxOccurs": "unbounded",
                 "minOccurs": "0",
@@ -1320,14 +1355,15 @@
     def __init__(
         self,
         name: "a string (required)" = None,
         extends: "a string (optional)" = None,
         description: "a string (optional)" = None,
         Property: "list of Property(s) (optional)" = None,
         Parameter: "list of Parameter(s) (optional)" = None,
+        DerivedParameter: "list of DerivedParameter(s) (optional)" = None,
         Constant: "list of Constant(s) (optional)" = None,
         Exposure: "list of Exposure(s) (optional)" = None,
         Requirement: "list of Requirement(s) (optional)" = None,
         InstanceRequirement: "list of InstanceRequirement(s) (optional)" = None,
         Dynamics: "list of Dynamics(s) (optional)" = None,
         gds_collector_=None,
         **kwargs_,
@@ -1349,14 +1385,19 @@
             self.Property = Property
         self.Property_nsprefix_ = None
         if Parameter is None:
             self.Parameter = []
         else:
             self.Parameter = Parameter
         self.Parameter_nsprefix_ = None
+        if DerivedParameter is None:
+            self.DerivedParameter = []
+        else:
+            self.DerivedParameter = DerivedParameter
+        self.DerivedParameter_nsprefix_ = None
         if Constant is None:
             self.Constant = []
         else:
             self.Constant = Constant
         self.Constant_nsprefix_ = None
         if Exposure is None:
             self.Exposure = []
@@ -1391,14 +1432,15 @@
 
     factory = staticmethod(factory)
 
     def _hasContent(self):
         if (
             self.Property
             or self.Parameter
+            or self.DerivedParameter
             or self.Constant
             or self.Exposure
             or self.Requirement
             or self.InstanceRequirement
             or self.Dynamics
         ):
             return True
@@ -1536,14 +1578,28 @@
                 outfile,
                 level,
                 namespaceprefix_,
                 namespacedef_="",
                 name_="Parameter",
                 pretty_print=pretty_print,
             )
+        for DerivedParameter_ in self.DerivedParameter:
+            namespaceprefix_ = (
+                self.DerivedParameter_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.DerivedParameter_nsprefix_)
+                else ""
+            )
+            DerivedParameter_.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="DerivedParameter",
+                pretty_print=pretty_print,
+            )
         for Constant_ in self.Constant:
             namespaceprefix_ = (
                 self.Constant_nsprefix_ + ":"
                 if (UseCapturedNS_ and self.Constant_nsprefix_)
                 else ""
             )
             Constant_.export(
@@ -1628,14 +1684,17 @@
         self.gds_check_cardinality_(
             self.Property, "Property", min_occurs=0, max_occurs=9999999
         )
         self.gds_check_cardinality_(
             self.Parameter, "Parameter", min_occurs=0, max_occurs=9999999
         )
         self.gds_check_cardinality_(
+            self.DerivedParameter, "DerivedParameter", min_occurs=0, max_occurs=9999999
+        )
+        self.gds_check_cardinality_(
             self.Constant, "Constant", min_occurs=0, max_occurs=9999999
         )
         self.gds_check_cardinality_(
             self.Exposure, "Exposure", min_occurs=0, max_occurs=9999999
         )
         self.gds_check_cardinality_(
             self.Requirement, "Requirement", min_occurs=0, max_occurs=9999999
@@ -1650,14 +1709,16 @@
             self.Dynamics, "Dynamics", min_occurs=0, max_occurs=9999999
         )
         if recursive:
             for item in self.Property:
                 item.validate_(gds_collector, recursive=True)
             for item in self.Parameter:
                 item.validate_(gds_collector, recursive=True)
+            for item in self.DerivedParameter:
+                item.validate_(gds_collector, recursive=True)
             for item in self.Constant:
                 item.validate_(gds_collector, recursive=True)
             for item in self.Exposure:
                 item.validate_(gds_collector, recursive=True)
             for item in self.Requirement:
                 item.validate_(gds_collector, recursive=True)
             for item in self.InstanceRequirement:
@@ -1701,14 +1762,19 @@
             self.Property.append(obj_)
             obj_.original_tagname_ = "Property"
         elif nodeName_ == "Parameter":
             obj_ = Parameter.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.Parameter.append(obj_)
             obj_.original_tagname_ = "Parameter"
+        elif nodeName_ == "DerivedParameter":
+            obj_ = DerivedParameter.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            self.DerivedParameter.append(obj_)
+            obj_.original_tagname_ = "DerivedParameter"
         elif nodeName_ == "Constant":
             obj_ = Constant.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.Constant.append(obj_)
             obj_.original_tagname_ = "Constant"
         elif nodeName_ == "Exposure":
             obj_ = Exposure.factory(parent_object_=self)
@@ -1975,24 +2041,75 @@
                 "maxOccurs": "unbounded",
                 "minOccurs": "0",
                 "name": "TimeDerivative",
                 "type": "TimeDerivative",
             },
             None,
         ),
+        MemberSpec_(
+            "OnStart",
+            "OnStart",
+            0,
+            1,
+            {"maxOccurs": "1", "minOccurs": "0", "name": "OnStart", "type": "OnStart"},
+            None,
+        ),
+        MemberSpec_(
+            "OnEvent",
+            "OnEvent",
+            1,
+            1,
+            {
+                "maxOccurs": "unbounded",
+                "minOccurs": "0",
+                "name": "OnEvent",
+                "type": "OnEvent",
+            },
+            None,
+        ),
+        MemberSpec_(
+            "OnCondition",
+            "OnCondition",
+            1,
+            1,
+            {
+                "maxOccurs": "unbounded",
+                "minOccurs": "0",
+                "name": "OnCondition",
+                "type": "OnCondition",
+            },
+            None,
+        ),
+        MemberSpec_(
+            "Regime",
+            "Regime",
+            1,
+            1,
+            {
+                "maxOccurs": "unbounded",
+                "minOccurs": "0",
+                "name": "Regime",
+                "type": "Regime",
+            },
+            None,
+        ),
     ]
     subclass = None
     superclass = None
 
     def __init__(
         self,
         StateVariable: "list of StateVariable(s) (optional)" = None,
         DerivedVariable: "list of DerivedVariable(s) (optional)" = None,
         ConditionalDerivedVariable: "list of ConditionalDerivedVariable(s) (optional)" = None,
         TimeDerivative: "list of TimeDerivative(s) (optional)" = None,
+        OnStart: "a OnStart (optional)" = None,
+        OnEvent: "list of OnEvent(s) (optional)" = None,
+        OnCondition: "list of OnCondition(s) (optional)" = None,
+        Regime: "list of Regime(s) (optional)" = None,
         gds_collector_=None,
         **kwargs_,
     ):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get("parent_object_")
@@ -2013,14 +2130,31 @@
             self.ConditionalDerivedVariable = ConditionalDerivedVariable
         self.ConditionalDerivedVariable_nsprefix_ = None
         if TimeDerivative is None:
             self.TimeDerivative = []
         else:
             self.TimeDerivative = TimeDerivative
         self.TimeDerivative_nsprefix_ = None
+        self.OnStart = OnStart
+        self.OnStart_nsprefix_ = None
+        if OnEvent is None:
+            self.OnEvent = []
+        else:
+            self.OnEvent = OnEvent
+        self.OnEvent_nsprefix_ = None
+        if OnCondition is None:
+            self.OnCondition = []
+        else:
+            self.OnCondition = OnCondition
+        self.OnCondition_nsprefix_ = None
+        if Regime is None:
+            self.Regime = []
+        else:
+            self.Regime = Regime
+        self.Regime_nsprefix_ = None
 
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(CurrentSubclassModule_, Dynamics)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
         if Dynamics.subclass:
@@ -2032,14 +2166,18 @@
 
     def _hasContent(self):
         if (
             self.StateVariable
             or self.DerivedVariable
             or self.ConditionalDerivedVariable
             or self.TimeDerivative
+            or self.OnStart is not None
+            or self.OnEvent
+            or self.OnCondition
+            or self.Regime
         ):
             return True
         else:
             return False
 
     def export(
         self,
@@ -2160,14 +2298,70 @@
                 outfile,
                 level,
                 namespaceprefix_,
                 namespacedef_="",
                 name_="TimeDerivative",
                 pretty_print=pretty_print,
             )
+        if self.OnStart is not None:
+            namespaceprefix_ = (
+                self.OnStart_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.OnStart_nsprefix_)
+                else ""
+            )
+            self.OnStart.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="OnStart",
+                pretty_print=pretty_print,
+            )
+        for OnEvent_ in self.OnEvent:
+            namespaceprefix_ = (
+                self.OnEvent_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.OnEvent_nsprefix_)
+                else ""
+            )
+            OnEvent_.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="OnEvent",
+                pretty_print=pretty_print,
+            )
+        for OnCondition_ in self.OnCondition:
+            namespaceprefix_ = (
+                self.OnCondition_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.OnCondition_nsprefix_)
+                else ""
+            )
+            OnCondition_.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="OnCondition",
+                pretty_print=pretty_print,
+            )
+        for Regime_ in self.Regime:
+            namespaceprefix_ = (
+                self.Regime_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.Regime_nsprefix_)
+                else ""
+            )
+            Regime_.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="Regime",
+                pretty_print=pretty_print,
+            )
 
     def validate_(self, gds_collector, recursive=False):
         self.gds_collector_ = gds_collector
         message_count = len(self.gds_collector_.get_messages())
         # validate simple type attributes
         # validate simple type children
         # validate complex type children
@@ -2182,23 +2376,41 @@
             "ConditionalDerivedVariable",
             min_occurs=0,
             max_occurs=9999999,
         )
         self.gds_check_cardinality_(
             self.TimeDerivative, "TimeDerivative", min_occurs=0, max_occurs=9999999
         )
+        self.gds_check_cardinality_(self.OnStart, "OnStart", min_occurs=0, max_occurs=1)
+        self.gds_check_cardinality_(
+            self.OnEvent, "OnEvent", min_occurs=0, max_occurs=9999999
+        )
+        self.gds_check_cardinality_(
+            self.OnCondition, "OnCondition", min_occurs=0, max_occurs=9999999
+        )
+        self.gds_check_cardinality_(
+            self.Regime, "Regime", min_occurs=0, max_occurs=9999999
+        )
         if recursive:
             for item in self.StateVariable:
                 item.validate_(gds_collector, recursive=True)
             for item in self.DerivedVariable:
                 item.validate_(gds_collector, recursive=True)
             for item in self.ConditionalDerivedVariable:
                 item.validate_(gds_collector, recursive=True)
             for item in self.TimeDerivative:
                 item.validate_(gds_collector, recursive=True)
+            if self.OnStart is not None:
+                self.OnStart.validate_(gds_collector, recursive=True)
+            for item in self.OnEvent:
+                item.validate_(gds_collector, recursive=True)
+            for item in self.OnCondition:
+                item.validate_(gds_collector, recursive=True)
+            for item in self.Regime:
+                item.validate_(gds_collector, recursive=True)
         return message_count == len(self.gds_collector_.get_messages())
 
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
@@ -2231,14 +2443,34 @@
             self.ConditionalDerivedVariable.append(obj_)
             obj_.original_tagname_ = "ConditionalDerivedVariable"
         elif nodeName_ == "TimeDerivative":
             obj_ = TimeDerivative.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.TimeDerivative.append(obj_)
             obj_.original_tagname_ = "TimeDerivative"
+        elif nodeName_ == "OnStart":
+            obj_ = OnStart.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            self.OnStart = obj_
+            obj_.original_tagname_ = "OnStart"
+        elif nodeName_ == "OnEvent":
+            obj_ = OnEvent.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            self.OnEvent.append(obj_)
+            obj_.original_tagname_ = "OnEvent"
+        elif nodeName_ == "OnCondition":
+            obj_ = OnCondition.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            self.OnCondition.append(obj_)
+            obj_.original_tagname_ = "OnCondition"
+        elif nodeName_ == "Regime":
+            obj_ = Regime.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            self.Regime.append(obj_)
+            obj_.original_tagname_ = "Regime"
 
 
 # end class Dynamics
 
 
 class Case(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
@@ -2601,14 +2833,1717 @@
     ):
         pass
 
 
 # end class TimeDerivative
 
 
+class OnStart(GeneratedsSuper):
+    __hash__ = GeneratedsSuper.__hash__
+    member_data_items_ = [
+        MemberSpec_(
+            "StateAssignment",
+            "StateAssignment",
+            1,
+            0,
+            {
+                "maxOccurs": "unbounded",
+                "minOccurs": "1",
+                "name": "StateAssignment",
+                "type": "StateAssignment",
+            },
+            None,
+        ),
+    ]
+    subclass = None
+    superclass = None
+
+    def __init__(
+        self,
+        StateAssignment: "list of StateAssignment(s) (required)" = None,
+        gds_collector_=None,
+        **kwargs_,
+    ):
+        self.gds_collector_ = gds_collector_
+        self.gds_elementtree_node_ = None
+        self.original_tagname_ = None
+        self.parent_object_ = kwargs_.get("parent_object_")
+        self.ns_prefix_ = None
+        if StateAssignment is None:
+            self.StateAssignment = []
+        else:
+            self.StateAssignment = StateAssignment
+        self.StateAssignment_nsprefix_ = None
+
+    def factory(*args_, **kwargs_):
+        if CurrentSubclassModule_ is not None:
+            subclass = getSubclassFromModule_(CurrentSubclassModule_, OnStart)
+            if subclass is not None:
+                return subclass(*args_, **kwargs_)
+        if OnStart.subclass:
+            return OnStart.subclass(*args_, **kwargs_)
+        else:
+            return OnStart(*args_, **kwargs_)
+
+    factory = staticmethod(factory)
+
+    def _hasContent(self):
+        if self.StateAssignment:
+            return True
+        else:
+            return False
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="http://www.neuroml.org/schema/neuroml2" ',
+        name_="OnStart",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("OnStart")
+        if imported_ns_def_ is not None:
+            namespacedef_ = imported_ns_def_
+        if pretty_print:
+            eol_ = "\n"
+        else:
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "OnStart":
+            name_ = self.original_tagname_
+        if UseCapturedNS_ and self.ns_prefix_:
+            namespaceprefix_ = self.ns_prefix_ + ":"
+        showIndent(outfile, level, pretty_print)
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
+        already_processed = set()
+        self._exportAttributes(
+            outfile, level, already_processed, namespaceprefix_, name_="OnStart"
+        )
+        if self._hasContent():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="OnStart",
+                pretty_print=pretty_print,
+            )
+            showIndent(outfile, level, pretty_print)
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
+        else:
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self, outfile, level, already_processed, namespaceprefix_="", name_="OnStart"
+    ):
+        pass
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="http://www.neuroml.org/schema/neuroml2" ',
+        name_="OnStart",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
+        if pretty_print:
+            eol_ = "\n"
+        else:
+            eol_ = ""
+        for StateAssignment_ in self.StateAssignment:
+            namespaceprefix_ = (
+                self.StateAssignment_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.StateAssignment_nsprefix_)
+                else ""
+            )
+            StateAssignment_.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="StateAssignment",
+                pretty_print=pretty_print,
+            )
+
+    def validate_(self, gds_collector, recursive=False):
+        self.gds_collector_ = gds_collector
+        message_count = len(self.gds_collector_.get_messages())
+        # validate simple type attributes
+        # validate simple type children
+        # validate complex type children
+        self.gds_check_cardinality_(
+            self.StateAssignment, "StateAssignment", min_occurs=1, max_occurs=9999999
+        )
+        if recursive:
+            for item in self.StateAssignment:
+                item.validate_(gds_collector, recursive=True)
+        return message_count == len(self.gds_collector_.get_messages())
+
+    def build(self, node, gds_collector_=None):
+        self.gds_collector_ = gds_collector_
+        if SaveElementTreeNode:
+            self.gds_elementtree_node_ = node
+        already_processed = set()
+        self.ns_prefix_ = node.prefix
+        self._buildAttributes(node, node.attrib, already_processed)
+        for child in node:
+            nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
+            self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+        return self
+
+    def _buildAttributes(self, node, attrs, already_processed):
+        pass
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "StateAssignment":
+            obj_ = StateAssignment.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            self.StateAssignment.append(obj_)
+            obj_.original_tagname_ = "StateAssignment"
+
+
+# end class OnStart
+
+
+class StateAssignment(GeneratedsSuper):
+    __hash__ = GeneratedsSuper.__hash__
+    member_data_items_ = [
+        MemberSpec_(
+            "variable", "xs:string", 0, 0, {"use": "required", "name": "variable"}
+        ),
+        MemberSpec_("value", "xs:string", 0, 0, {"use": "required", "name": "value"}),
+    ]
+    subclass = None
+    superclass = None
+
+    def __init__(
+        self,
+        variable: "a string (required)" = None,
+        value: "a string (required)" = None,
+        gds_collector_=None,
+        **kwargs_,
+    ):
+        self.gds_collector_ = gds_collector_
+        self.gds_elementtree_node_ = None
+        self.original_tagname_ = None
+        self.parent_object_ = kwargs_.get("parent_object_")
+        self.ns_prefix_ = None
+        self.variable = _cast(None, variable)
+        self.variable_nsprefix_ = None
+        self.value = _cast(None, value)
+        self.value_nsprefix_ = None
+
+    def factory(*args_, **kwargs_):
+        if CurrentSubclassModule_ is not None:
+            subclass = getSubclassFromModule_(CurrentSubclassModule_, StateAssignment)
+            if subclass is not None:
+                return subclass(*args_, **kwargs_)
+        if StateAssignment.subclass:
+            return StateAssignment.subclass(*args_, **kwargs_)
+        else:
+            return StateAssignment(*args_, **kwargs_)
+
+    factory = staticmethod(factory)
+
+    def _hasContent(self):
+        if ():
+            return True
+        else:
+            return False
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_="",
+        name_="StateAssignment",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("StateAssignment")
+        if imported_ns_def_ is not None:
+            namespacedef_ = imported_ns_def_
+        if pretty_print:
+            eol_ = "\n"
+        else:
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "StateAssignment":
+            name_ = self.original_tagname_
+        if UseCapturedNS_ and self.ns_prefix_:
+            namespaceprefix_ = self.ns_prefix_ + ":"
+        showIndent(outfile, level, pretty_print)
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
+        already_processed = set()
+        self._exportAttributes(
+            outfile, level, already_processed, namespaceprefix_, name_="StateAssignment"
+        )
+        if self._hasContent():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="StateAssignment",
+                pretty_print=pretty_print,
+            )
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
+        else:
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self,
+        outfile,
+        level,
+        already_processed,
+        namespaceprefix_="",
+        name_="StateAssignment",
+    ):
+        if self.variable is not None and "variable" not in already_processed:
+            already_processed.add("variable")
+            outfile.write(
+                " variable=%s"
+                % (
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_attrib(self.variable), input_name="variable"
+                        )
+                    ),
+                )
+            )
+        if self.value is not None and "value" not in already_processed:
+            already_processed.add("value")
+            outfile.write(
+                " value=%s"
+                % (
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_attrib(self.value), input_name="value"
+                        )
+                    ),
+                )
+            )
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_="",
+        name_="StateAssignment",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
+        pass
+
+    def validate_(self, gds_collector, recursive=False):
+        self.gds_collector_ = gds_collector
+        message_count = len(self.gds_collector_.get_messages())
+        # validate simple type attributes
+        self.gds_validate_builtin_ST_(
+            self.gds_validate_string, self.variable, "variable"
+        )
+        self.gds_check_cardinality_(self.variable, "variable", required=True)
+        self.gds_validate_builtin_ST_(self.gds_validate_string, self.value, "value")
+        self.gds_check_cardinality_(self.value, "value", required=True)
+        # validate simple type children
+        # validate complex type children
+        if recursive:
+            pass
+        return message_count == len(self.gds_collector_.get_messages())
+
+    def build(self, node, gds_collector_=None):
+        self.gds_collector_ = gds_collector_
+        if SaveElementTreeNode:
+            self.gds_elementtree_node_ = node
+        already_processed = set()
+        self.ns_prefix_ = node.prefix
+        self._buildAttributes(node, node.attrib, already_processed)
+        for child in node:
+            nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
+            self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+        return self
+
+    def _buildAttributes(self, node, attrs, already_processed):
+        value = find_attr_value_("variable", node)
+        if value is not None and "variable" not in already_processed:
+            already_processed.add("variable")
+            self.variable = value
+        value = find_attr_value_("value", node)
+        if value is not None and "value" not in already_processed:
+            already_processed.add("value")
+            self.value = value
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        pass
+
+
+# end class StateAssignment
+
+
+class OnEvent(GeneratedsSuper):
+    __hash__ = GeneratedsSuper.__hash__
+    member_data_items_ = [
+        MemberSpec_("port", "xs:string", 0, 0, {"use": "required", "name": "port"}),
+        MemberSpec_(
+            "StateAssignment",
+            "StateAssignment",
+            1,
+            1,
+            {
+                "maxOccurs": "unbounded",
+                "minOccurs": "0",
+                "name": "StateAssignment",
+                "type": "StateAssignment",
+            },
+            None,
+        ),
+        MemberSpec_(
+            "EventOut",
+            "EventOut",
+            1,
+            1,
+            {
+                "maxOccurs": "unbounded",
+                "minOccurs": "0",
+                "name": "EventOut",
+                "type": "EventOut",
+            },
+            None,
+        ),
+    ]
+    subclass = None
+    superclass = None
+
+    def __init__(
+        self,
+        port: "a string (required)" = None,
+        StateAssignment: "list of StateAssignment(s) (optional)" = None,
+        EventOut: "list of EventOut(s) (optional)" = None,
+        gds_collector_=None,
+        **kwargs_,
+    ):
+        self.gds_collector_ = gds_collector_
+        self.gds_elementtree_node_ = None
+        self.original_tagname_ = None
+        self.parent_object_ = kwargs_.get("parent_object_")
+        self.ns_prefix_ = None
+        self.port = _cast(None, port)
+        self.port_nsprefix_ = None
+        if StateAssignment is None:
+            self.StateAssignment = []
+        else:
+            self.StateAssignment = StateAssignment
+        self.StateAssignment_nsprefix_ = None
+        if EventOut is None:
+            self.EventOut = []
+        else:
+            self.EventOut = EventOut
+        self.EventOut_nsprefix_ = None
+
+    def factory(*args_, **kwargs_):
+        if CurrentSubclassModule_ is not None:
+            subclass = getSubclassFromModule_(CurrentSubclassModule_, OnEvent)
+            if subclass is not None:
+                return subclass(*args_, **kwargs_)
+        if OnEvent.subclass:
+            return OnEvent.subclass(*args_, **kwargs_)
+        else:
+            return OnEvent(*args_, **kwargs_)
+
+    factory = staticmethod(factory)
+
+    def _hasContent(self):
+        if self.StateAssignment or self.EventOut:
+            return True
+        else:
+            return False
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="http://www.neuroml.org/schema/neuroml2" ',
+        name_="OnEvent",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("OnEvent")
+        if imported_ns_def_ is not None:
+            namespacedef_ = imported_ns_def_
+        if pretty_print:
+            eol_ = "\n"
+        else:
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "OnEvent":
+            name_ = self.original_tagname_
+        if UseCapturedNS_ and self.ns_prefix_:
+            namespaceprefix_ = self.ns_prefix_ + ":"
+        showIndent(outfile, level, pretty_print)
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
+        already_processed = set()
+        self._exportAttributes(
+            outfile, level, already_processed, namespaceprefix_, name_="OnEvent"
+        )
+        if self._hasContent():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="OnEvent",
+                pretty_print=pretty_print,
+            )
+            showIndent(outfile, level, pretty_print)
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
+        else:
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self, outfile, level, already_processed, namespaceprefix_="", name_="OnEvent"
+    ):
+        if self.port is not None and "port" not in already_processed:
+            already_processed.add("port")
+            outfile.write(
+                " port=%s"
+                % (
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_attrib(self.port), input_name="port"
+                        )
+                    ),
+                )
+            )
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="http://www.neuroml.org/schema/neuroml2" ',
+        name_="OnEvent",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
+        if pretty_print:
+            eol_ = "\n"
+        else:
+            eol_ = ""
+        for StateAssignment_ in self.StateAssignment:
+            namespaceprefix_ = (
+                self.StateAssignment_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.StateAssignment_nsprefix_)
+                else ""
+            )
+            StateAssignment_.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="StateAssignment",
+                pretty_print=pretty_print,
+            )
+        for EventOut_ in self.EventOut:
+            namespaceprefix_ = (
+                self.EventOut_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.EventOut_nsprefix_)
+                else ""
+            )
+            EventOut_.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="EventOut",
+                pretty_print=pretty_print,
+            )
+
+    def validate_(self, gds_collector, recursive=False):
+        self.gds_collector_ = gds_collector
+        message_count = len(self.gds_collector_.get_messages())
+        # validate simple type attributes
+        self.gds_validate_builtin_ST_(self.gds_validate_string, self.port, "port")
+        self.gds_check_cardinality_(self.port, "port", required=True)
+        # validate simple type children
+        # validate complex type children
+        self.gds_check_cardinality_(
+            self.StateAssignment, "StateAssignment", min_occurs=0, max_occurs=9999999
+        )
+        self.gds_check_cardinality_(
+            self.EventOut, "EventOut", min_occurs=0, max_occurs=9999999
+        )
+        if recursive:
+            for item in self.StateAssignment:
+                item.validate_(gds_collector, recursive=True)
+            for item in self.EventOut:
+                item.validate_(gds_collector, recursive=True)
+        return message_count == len(self.gds_collector_.get_messages())
+
+    def build(self, node, gds_collector_=None):
+        self.gds_collector_ = gds_collector_
+        if SaveElementTreeNode:
+            self.gds_elementtree_node_ = node
+        already_processed = set()
+        self.ns_prefix_ = node.prefix
+        self._buildAttributes(node, node.attrib, already_processed)
+        for child in node:
+            nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
+            self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+        return self
+
+    def _buildAttributes(self, node, attrs, already_processed):
+        value = find_attr_value_("port", node)
+        if value is not None and "port" not in already_processed:
+            already_processed.add("port")
+            self.port = value
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "StateAssignment":
+            obj_ = StateAssignment.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            self.StateAssignment.append(obj_)
+            obj_.original_tagname_ = "StateAssignment"
+        elif nodeName_ == "EventOut":
+            obj_ = EventOut.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            self.EventOut.append(obj_)
+            obj_.original_tagname_ = "EventOut"
+
+
+# end class OnEvent
+
+
+class EventOut(GeneratedsSuper):
+    __hash__ = GeneratedsSuper.__hash__
+    member_data_items_ = [
+        MemberSpec_("port", "xs:string", 0, 0, {"use": "required", "name": "port"}),
+    ]
+    subclass = None
+    superclass = None
+
+    def __init__(
+        self, port: "a string (required)" = None, gds_collector_=None, **kwargs_
+    ):
+        self.gds_collector_ = gds_collector_
+        self.gds_elementtree_node_ = None
+        self.original_tagname_ = None
+        self.parent_object_ = kwargs_.get("parent_object_")
+        self.ns_prefix_ = None
+        self.port = _cast(None, port)
+        self.port_nsprefix_ = None
+
+    def factory(*args_, **kwargs_):
+        if CurrentSubclassModule_ is not None:
+            subclass = getSubclassFromModule_(CurrentSubclassModule_, EventOut)
+            if subclass is not None:
+                return subclass(*args_, **kwargs_)
+        if EventOut.subclass:
+            return EventOut.subclass(*args_, **kwargs_)
+        else:
+            return EventOut(*args_, **kwargs_)
+
+    factory = staticmethod(factory)
+
+    def _hasContent(self):
+        if ():
+            return True
+        else:
+            return False
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_="",
+        name_="EventOut",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("EventOut")
+        if imported_ns_def_ is not None:
+            namespacedef_ = imported_ns_def_
+        if pretty_print:
+            eol_ = "\n"
+        else:
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "EventOut":
+            name_ = self.original_tagname_
+        if UseCapturedNS_ and self.ns_prefix_:
+            namespaceprefix_ = self.ns_prefix_ + ":"
+        showIndent(outfile, level, pretty_print)
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
+        already_processed = set()
+        self._exportAttributes(
+            outfile, level, already_processed, namespaceprefix_, name_="EventOut"
+        )
+        if self._hasContent():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="EventOut",
+                pretty_print=pretty_print,
+            )
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
+        else:
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self, outfile, level, already_processed, namespaceprefix_="", name_="EventOut"
+    ):
+        if self.port is not None and "port" not in already_processed:
+            already_processed.add("port")
+            outfile.write(
+                " port=%s"
+                % (
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_attrib(self.port), input_name="port"
+                        )
+                    ),
+                )
+            )
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_="",
+        name_="EventOut",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
+        pass
+
+    def validate_(self, gds_collector, recursive=False):
+        self.gds_collector_ = gds_collector
+        message_count = len(self.gds_collector_.get_messages())
+        # validate simple type attributes
+        self.gds_validate_builtin_ST_(self.gds_validate_string, self.port, "port")
+        self.gds_check_cardinality_(self.port, "port", required=True)
+        # validate simple type children
+        # validate complex type children
+        if recursive:
+            pass
+        return message_count == len(self.gds_collector_.get_messages())
+
+    def build(self, node, gds_collector_=None):
+        self.gds_collector_ = gds_collector_
+        if SaveElementTreeNode:
+            self.gds_elementtree_node_ = node
+        already_processed = set()
+        self.ns_prefix_ = node.prefix
+        self._buildAttributes(node, node.attrib, already_processed)
+        for child in node:
+            nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
+            self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+        return self
+
+    def _buildAttributes(self, node, attrs, already_processed):
+        value = find_attr_value_("port", node)
+        if value is not None and "port" not in already_processed:
+            already_processed.add("port")
+            self.port = value
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        pass
+
+
+# end class EventOut
+
+
+class OnCondition(GeneratedsSuper):
+    __hash__ = GeneratedsSuper.__hash__
+    member_data_items_ = [
+        MemberSpec_("test", "xs:string", 0, 0, {"use": "required", "name": "test"}),
+        MemberSpec_(
+            "StateAssignment",
+            "StateAssignment",
+            1,
+            1,
+            {
+                "maxOccurs": "unbounded",
+                "minOccurs": "0",
+                "name": "StateAssignment",
+                "type": "StateAssignment",
+            },
+            None,
+        ),
+        MemberSpec_(
+            "EventOut",
+            "EventOut",
+            1,
+            1,
+            {
+                "maxOccurs": "unbounded",
+                "minOccurs": "0",
+                "name": "EventOut",
+                "type": "EventOut",
+            },
+            None,
+        ),
+        MemberSpec_(
+            "Transition",
+            "Transition",
+            0,
+            1,
+            {
+                "maxOccurs": "1",
+                "minOccurs": "0",
+                "name": "Transition",
+                "type": "Transition",
+            },
+            None,
+        ),
+    ]
+    subclass = None
+    superclass = None
+
+    def __init__(
+        self,
+        test: "a string (required)" = None,
+        StateAssignment: "list of StateAssignment(s) (optional)" = None,
+        EventOut: "list of EventOut(s) (optional)" = None,
+        Transition: "a Transition (optional)" = None,
+        gds_collector_=None,
+        **kwargs_,
+    ):
+        self.gds_collector_ = gds_collector_
+        self.gds_elementtree_node_ = None
+        self.original_tagname_ = None
+        self.parent_object_ = kwargs_.get("parent_object_")
+        self.ns_prefix_ = None
+        self.test = _cast(None, test)
+        self.test_nsprefix_ = None
+        if StateAssignment is None:
+            self.StateAssignment = []
+        else:
+            self.StateAssignment = StateAssignment
+        self.StateAssignment_nsprefix_ = None
+        if EventOut is None:
+            self.EventOut = []
+        else:
+            self.EventOut = EventOut
+        self.EventOut_nsprefix_ = None
+        self.Transition = Transition
+        self.Transition_nsprefix_ = None
+
+    def factory(*args_, **kwargs_):
+        if CurrentSubclassModule_ is not None:
+            subclass = getSubclassFromModule_(CurrentSubclassModule_, OnCondition)
+            if subclass is not None:
+                return subclass(*args_, **kwargs_)
+        if OnCondition.subclass:
+            return OnCondition.subclass(*args_, **kwargs_)
+        else:
+            return OnCondition(*args_, **kwargs_)
+
+    factory = staticmethod(factory)
+
+    def _hasContent(self):
+        if self.StateAssignment or self.EventOut or self.Transition is not None:
+            return True
+        else:
+            return False
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="http://www.neuroml.org/schema/neuroml2" ',
+        name_="OnCondition",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("OnCondition")
+        if imported_ns_def_ is not None:
+            namespacedef_ = imported_ns_def_
+        if pretty_print:
+            eol_ = "\n"
+        else:
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "OnCondition":
+            name_ = self.original_tagname_
+        if UseCapturedNS_ and self.ns_prefix_:
+            namespaceprefix_ = self.ns_prefix_ + ":"
+        showIndent(outfile, level, pretty_print)
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
+        already_processed = set()
+        self._exportAttributes(
+            outfile, level, already_processed, namespaceprefix_, name_="OnCondition"
+        )
+        if self._hasContent():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="OnCondition",
+                pretty_print=pretty_print,
+            )
+            showIndent(outfile, level, pretty_print)
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
+        else:
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self,
+        outfile,
+        level,
+        already_processed,
+        namespaceprefix_="",
+        name_="OnCondition",
+    ):
+        if self.test is not None and "test" not in already_processed:
+            already_processed.add("test")
+            outfile.write(
+                " test=%s"
+                % (
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_attrib(self.test), input_name="test"
+                        )
+                    ),
+                )
+            )
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="http://www.neuroml.org/schema/neuroml2" ',
+        name_="OnCondition",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
+        if pretty_print:
+            eol_ = "\n"
+        else:
+            eol_ = ""
+        for StateAssignment_ in self.StateAssignment:
+            namespaceprefix_ = (
+                self.StateAssignment_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.StateAssignment_nsprefix_)
+                else ""
+            )
+            StateAssignment_.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="StateAssignment",
+                pretty_print=pretty_print,
+            )
+        for EventOut_ in self.EventOut:
+            namespaceprefix_ = (
+                self.EventOut_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.EventOut_nsprefix_)
+                else ""
+            )
+            EventOut_.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="EventOut",
+                pretty_print=pretty_print,
+            )
+        if self.Transition is not None:
+            namespaceprefix_ = (
+                self.Transition_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.Transition_nsprefix_)
+                else ""
+            )
+            self.Transition.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="Transition",
+                pretty_print=pretty_print,
+            )
+
+    def validate_(self, gds_collector, recursive=False):
+        self.gds_collector_ = gds_collector
+        message_count = len(self.gds_collector_.get_messages())
+        # validate simple type attributes
+        self.gds_validate_builtin_ST_(self.gds_validate_string, self.test, "test")
+        self.gds_check_cardinality_(self.test, "test", required=True)
+        # validate simple type children
+        # validate complex type children
+        self.gds_check_cardinality_(
+            self.StateAssignment, "StateAssignment", min_occurs=0, max_occurs=9999999
+        )
+        self.gds_check_cardinality_(
+            self.EventOut, "EventOut", min_occurs=0, max_occurs=9999999
+        )
+        self.gds_check_cardinality_(
+            self.Transition, "Transition", min_occurs=0, max_occurs=1
+        )
+        if recursive:
+            for item in self.StateAssignment:
+                item.validate_(gds_collector, recursive=True)
+            for item in self.EventOut:
+                item.validate_(gds_collector, recursive=True)
+            if self.Transition is not None:
+                self.Transition.validate_(gds_collector, recursive=True)
+        return message_count == len(self.gds_collector_.get_messages())
+
+    def build(self, node, gds_collector_=None):
+        self.gds_collector_ = gds_collector_
+        if SaveElementTreeNode:
+            self.gds_elementtree_node_ = node
+        already_processed = set()
+        self.ns_prefix_ = node.prefix
+        self._buildAttributes(node, node.attrib, already_processed)
+        for child in node:
+            nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
+            self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+        return self
+
+    def _buildAttributes(self, node, attrs, already_processed):
+        value = find_attr_value_("test", node)
+        if value is not None and "test" not in already_processed:
+            already_processed.add("test")
+            self.test = value
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "StateAssignment":
+            obj_ = StateAssignment.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            self.StateAssignment.append(obj_)
+            obj_.original_tagname_ = "StateAssignment"
+        elif nodeName_ == "EventOut":
+            obj_ = EventOut.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            self.EventOut.append(obj_)
+            obj_.original_tagname_ = "EventOut"
+        elif nodeName_ == "Transition":
+            obj_ = Transition.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            self.Transition = obj_
+            obj_.original_tagname_ = "Transition"
+
+
+# end class OnCondition
+
+
+class Transition(GeneratedsSuper):
+    __hash__ = GeneratedsSuper.__hash__
+    member_data_items_ = [
+        MemberSpec_("regime", "xs:string", 0, 0, {"use": "required", "name": "regime"}),
+    ]
+    subclass = None
+    superclass = None
+
+    def __init__(
+        self, regime: "a string (required)" = None, gds_collector_=None, **kwargs_
+    ):
+        self.gds_collector_ = gds_collector_
+        self.gds_elementtree_node_ = None
+        self.original_tagname_ = None
+        self.parent_object_ = kwargs_.get("parent_object_")
+        self.ns_prefix_ = None
+        self.regime = _cast(None, regime)
+        self.regime_nsprefix_ = None
+
+    def factory(*args_, **kwargs_):
+        if CurrentSubclassModule_ is not None:
+            subclass = getSubclassFromModule_(CurrentSubclassModule_, Transition)
+            if subclass is not None:
+                return subclass(*args_, **kwargs_)
+        if Transition.subclass:
+            return Transition.subclass(*args_, **kwargs_)
+        else:
+            return Transition(*args_, **kwargs_)
+
+    factory = staticmethod(factory)
+
+    def _hasContent(self):
+        if ():
+            return True
+        else:
+            return False
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_="",
+        name_="Transition",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("Transition")
+        if imported_ns_def_ is not None:
+            namespacedef_ = imported_ns_def_
+        if pretty_print:
+            eol_ = "\n"
+        else:
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "Transition":
+            name_ = self.original_tagname_
+        if UseCapturedNS_ and self.ns_prefix_:
+            namespaceprefix_ = self.ns_prefix_ + ":"
+        showIndent(outfile, level, pretty_print)
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
+        already_processed = set()
+        self._exportAttributes(
+            outfile, level, already_processed, namespaceprefix_, name_="Transition"
+        )
+        if self._hasContent():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="Transition",
+                pretty_print=pretty_print,
+            )
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
+        else:
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self, outfile, level, already_processed, namespaceprefix_="", name_="Transition"
+    ):
+        if self.regime is not None and "regime" not in already_processed:
+            already_processed.add("regime")
+            outfile.write(
+                " regime=%s"
+                % (
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_attrib(self.regime), input_name="regime"
+                        )
+                    ),
+                )
+            )
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_="",
+        name_="Transition",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
+        pass
+
+    def validate_(self, gds_collector, recursive=False):
+        self.gds_collector_ = gds_collector
+        message_count = len(self.gds_collector_.get_messages())
+        # validate simple type attributes
+        self.gds_validate_builtin_ST_(self.gds_validate_string, self.regime, "regime")
+        self.gds_check_cardinality_(self.regime, "regime", required=True)
+        # validate simple type children
+        # validate complex type children
+        if recursive:
+            pass
+        return message_count == len(self.gds_collector_.get_messages())
+
+    def build(self, node, gds_collector_=None):
+        self.gds_collector_ = gds_collector_
+        if SaveElementTreeNode:
+            self.gds_elementtree_node_ = node
+        already_processed = set()
+        self.ns_prefix_ = node.prefix
+        self._buildAttributes(node, node.attrib, already_processed)
+        for child in node:
+            nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
+            self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+        return self
+
+    def _buildAttributes(self, node, attrs, already_processed):
+        value = find_attr_value_("regime", node)
+        if value is not None and "regime" not in already_processed:
+            already_processed.add("regime")
+            self.regime = value
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        pass
+
+
+# end class Transition
+
+
+class Regime(GeneratedsSuper):
+    __hash__ = GeneratedsSuper.__hash__
+    member_data_items_ = [
+        MemberSpec_("name", "xs:string", 0, 0, {"use": "required", "name": "name"}),
+        MemberSpec_(
+            "initial", "TrueOrFalse", 0, 1, {"use": "optional", "name": "initial"}
+        ),
+        MemberSpec_(
+            "TimeDerivative",
+            "TimeDerivative",
+            1,
+            1,
+            {
+                "maxOccurs": "unbounded",
+                "minOccurs": "0",
+                "name": "TimeDerivative",
+                "type": "TimeDerivative",
+            },
+            None,
+        ),
+        MemberSpec_(
+            "OnEntry",
+            "OnEntry",
+            0,
+            1,
+            {"maxOccurs": "1", "minOccurs": "0", "name": "OnEntry", "type": "OnEntry"},
+            None,
+        ),
+        MemberSpec_(
+            "OnCondition",
+            "OnCondition",
+            1,
+            1,
+            {
+                "maxOccurs": "unbounded",
+                "minOccurs": "0",
+                "name": "OnCondition",
+                "type": "OnCondition",
+            },
+            None,
+        ),
+    ]
+    subclass = None
+    superclass = None
+
+    def __init__(
+        self,
+        name: "a string (required)" = None,
+        initial: "a TrueOrFalse (optional)" = None,
+        TimeDerivative: "list of TimeDerivative(s) (optional)" = None,
+        OnEntry: "a OnEntry (optional)" = None,
+        OnCondition: "list of OnCondition(s) (optional)" = None,
+        gds_collector_=None,
+        **kwargs_,
+    ):
+        self.gds_collector_ = gds_collector_
+        self.gds_elementtree_node_ = None
+        self.original_tagname_ = None
+        self.parent_object_ = kwargs_.get("parent_object_")
+        self.ns_prefix_ = None
+        self.name = _cast(None, name)
+        self.name_nsprefix_ = None
+        self.initial = _cast(None, initial)
+        self.initial_nsprefix_ = None
+        if TimeDerivative is None:
+            self.TimeDerivative = []
+        else:
+            self.TimeDerivative = TimeDerivative
+        self.TimeDerivative_nsprefix_ = None
+        self.OnEntry = OnEntry
+        self.OnEntry_nsprefix_ = None
+        if OnCondition is None:
+            self.OnCondition = []
+        else:
+            self.OnCondition = OnCondition
+        self.OnCondition_nsprefix_ = None
+
+    def factory(*args_, **kwargs_):
+        if CurrentSubclassModule_ is not None:
+            subclass = getSubclassFromModule_(CurrentSubclassModule_, Regime)
+            if subclass is not None:
+                return subclass(*args_, **kwargs_)
+        if Regime.subclass:
+            return Regime.subclass(*args_, **kwargs_)
+        else:
+            return Regime(*args_, **kwargs_)
+
+    factory = staticmethod(factory)
+
+    def validate_TrueOrFalse(self, value):
+        # Validate type TrueOrFalse, a restriction on xs:string.
+        if (
+            value is not None
+            and Validate_simpletypes_
+            and self.gds_collector_ is not None
+        ):
+            if not isinstance(value, str):
+                lineno = self.gds_get_node_lineno_()
+                self.gds_collector_.add_message(
+                    'Value "%(value)s"%(lineno)s is not of the correct base simple type (str)'
+                    % {
+                        "value": value,
+                        "lineno": lineno,
+                    }
+                )
+                return False
+            value = value
+            enumerations = ["true", "false"]
+            if value not in enumerations:
+                lineno = self.gds_get_node_lineno_()
+                self.gds_collector_.add_message(
+                    'Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on TrueOrFalse'
+                    % {"value": encode_str_2_3(value), "lineno": lineno}
+                )
+                result = False
+
+    def _hasContent(self):
+        if self.TimeDerivative or self.OnEntry is not None or self.OnCondition:
+            return True
+        else:
+            return False
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="http://www.neuroml.org/schema/neuroml2" ',
+        name_="Regime",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("Regime")
+        if imported_ns_def_ is not None:
+            namespacedef_ = imported_ns_def_
+        if pretty_print:
+            eol_ = "\n"
+        else:
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "Regime":
+            name_ = self.original_tagname_
+        if UseCapturedNS_ and self.ns_prefix_:
+            namespaceprefix_ = self.ns_prefix_ + ":"
+        showIndent(outfile, level, pretty_print)
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
+        already_processed = set()
+        self._exportAttributes(
+            outfile, level, already_processed, namespaceprefix_, name_="Regime"
+        )
+        if self._hasContent():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="Regime",
+                pretty_print=pretty_print,
+            )
+            showIndent(outfile, level, pretty_print)
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
+        else:
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self, outfile, level, already_processed, namespaceprefix_="", name_="Regime"
+    ):
+        if self.name is not None and "name" not in already_processed:
+            already_processed.add("name")
+            outfile.write(
+                " name=%s"
+                % (
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_attrib(self.name), input_name="name"
+                        )
+                    ),
+                )
+            )
+        if self.initial is not None and "initial" not in already_processed:
+            already_processed.add("initial")
+            outfile.write(
+                " initial=%s"
+                % (
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_attrib(self.initial), input_name="initial"
+                        )
+                    ),
+                )
+            )
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="http://www.neuroml.org/schema/neuroml2" ',
+        name_="Regime",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
+        if pretty_print:
+            eol_ = "\n"
+        else:
+            eol_ = ""
+        for TimeDerivative_ in self.TimeDerivative:
+            namespaceprefix_ = (
+                self.TimeDerivative_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.TimeDerivative_nsprefix_)
+                else ""
+            )
+            TimeDerivative_.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="TimeDerivative",
+                pretty_print=pretty_print,
+            )
+        if self.OnEntry is not None:
+            namespaceprefix_ = (
+                self.OnEntry_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.OnEntry_nsprefix_)
+                else ""
+            )
+            self.OnEntry.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="OnEntry",
+                pretty_print=pretty_print,
+            )
+        for OnCondition_ in self.OnCondition:
+            namespaceprefix_ = (
+                self.OnCondition_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.OnCondition_nsprefix_)
+                else ""
+            )
+            OnCondition_.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="OnCondition",
+                pretty_print=pretty_print,
+            )
+
+    def validate_(self, gds_collector, recursive=False):
+        self.gds_collector_ = gds_collector
+        message_count = len(self.gds_collector_.get_messages())
+        # validate simple type attributes
+        self.gds_validate_builtin_ST_(self.gds_validate_string, self.name, "name")
+        self.gds_check_cardinality_(self.name, "name", required=True)
+        self.gds_validate_defined_ST_(
+            self.validate_TrueOrFalse, self.initial, "initial"
+        )
+        self.gds_check_cardinality_(self.initial, "initial", required=False)
+        # validate simple type children
+        # validate complex type children
+        self.gds_check_cardinality_(
+            self.TimeDerivative, "TimeDerivative", min_occurs=0, max_occurs=9999999
+        )
+        self.gds_check_cardinality_(self.OnEntry, "OnEntry", min_occurs=0, max_occurs=1)
+        self.gds_check_cardinality_(
+            self.OnCondition, "OnCondition", min_occurs=0, max_occurs=9999999
+        )
+        if recursive:
+            for item in self.TimeDerivative:
+                item.validate_(gds_collector, recursive=True)
+            if self.OnEntry is not None:
+                self.OnEntry.validate_(gds_collector, recursive=True)
+            for item in self.OnCondition:
+                item.validate_(gds_collector, recursive=True)
+        return message_count == len(self.gds_collector_.get_messages())
+
+    def build(self, node, gds_collector_=None):
+        self.gds_collector_ = gds_collector_
+        if SaveElementTreeNode:
+            self.gds_elementtree_node_ = node
+        already_processed = set()
+        self.ns_prefix_ = node.prefix
+        self._buildAttributes(node, node.attrib, already_processed)
+        for child in node:
+            nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
+            self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+        return self
+
+    def _buildAttributes(self, node, attrs, already_processed):
+        value = find_attr_value_("name", node)
+        if value is not None and "name" not in already_processed:
+            already_processed.add("name")
+            self.name = value
+        value = find_attr_value_("initial", node)
+        if value is not None and "initial" not in already_processed:
+            already_processed.add("initial")
+            self.initial = value
+            self.validate_TrueOrFalse(self.initial)  # validate type TrueOrFalse
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "TimeDerivative":
+            obj_ = TimeDerivative.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            self.TimeDerivative.append(obj_)
+            obj_.original_tagname_ = "TimeDerivative"
+        elif nodeName_ == "OnEntry":
+            obj_ = OnEntry.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            self.OnEntry = obj_
+            obj_.original_tagname_ = "OnEntry"
+        elif nodeName_ == "OnCondition":
+            obj_ = OnCondition.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            self.OnCondition.append(obj_)
+            obj_.original_tagname_ = "OnCondition"
+
+
+# end class Regime
+
+
+class OnEntry(GeneratedsSuper):
+    __hash__ = GeneratedsSuper.__hash__
+    member_data_items_ = [
+        MemberSpec_(
+            "StateAssignment",
+            "StateAssignment",
+            1,
+            0,
+            {
+                "maxOccurs": "unbounded",
+                "minOccurs": "1",
+                "name": "StateAssignment",
+                "type": "StateAssignment",
+            },
+            None,
+        ),
+    ]
+    subclass = None
+    superclass = None
+
+    def __init__(
+        self,
+        StateAssignment: "list of StateAssignment(s) (required)" = None,
+        gds_collector_=None,
+        **kwargs_,
+    ):
+        self.gds_collector_ = gds_collector_
+        self.gds_elementtree_node_ = None
+        self.original_tagname_ = None
+        self.parent_object_ = kwargs_.get("parent_object_")
+        self.ns_prefix_ = None
+        if StateAssignment is None:
+            self.StateAssignment = []
+        else:
+            self.StateAssignment = StateAssignment
+        self.StateAssignment_nsprefix_ = None
+
+    def factory(*args_, **kwargs_):
+        if CurrentSubclassModule_ is not None:
+            subclass = getSubclassFromModule_(CurrentSubclassModule_, OnEntry)
+            if subclass is not None:
+                return subclass(*args_, **kwargs_)
+        if OnEntry.subclass:
+            return OnEntry.subclass(*args_, **kwargs_)
+        else:
+            return OnEntry(*args_, **kwargs_)
+
+    factory = staticmethod(factory)
+
+    def _hasContent(self):
+        if self.StateAssignment:
+            return True
+        else:
+            return False
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="http://www.neuroml.org/schema/neuroml2" ',
+        name_="OnEntry",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("OnEntry")
+        if imported_ns_def_ is not None:
+            namespacedef_ = imported_ns_def_
+        if pretty_print:
+            eol_ = "\n"
+        else:
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "OnEntry":
+            name_ = self.original_tagname_
+        if UseCapturedNS_ and self.ns_prefix_:
+            namespaceprefix_ = self.ns_prefix_ + ":"
+        showIndent(outfile, level, pretty_print)
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
+        already_processed = set()
+        self._exportAttributes(
+            outfile, level, already_processed, namespaceprefix_, name_="OnEntry"
+        )
+        if self._hasContent():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="OnEntry",
+                pretty_print=pretty_print,
+            )
+            showIndent(outfile, level, pretty_print)
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
+        else:
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self, outfile, level, already_processed, namespaceprefix_="", name_="OnEntry"
+    ):
+        pass
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_=' xmlns:None="http://www.neuroml.org/schema/neuroml2" ',
+        name_="OnEntry",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
+        if pretty_print:
+            eol_ = "\n"
+        else:
+            eol_ = ""
+        for StateAssignment_ in self.StateAssignment:
+            namespaceprefix_ = (
+                self.StateAssignment_nsprefix_ + ":"
+                if (UseCapturedNS_ and self.StateAssignment_nsprefix_)
+                else ""
+            )
+            StateAssignment_.export(
+                outfile,
+                level,
+                namespaceprefix_,
+                namespacedef_="",
+                name_="StateAssignment",
+                pretty_print=pretty_print,
+            )
+
+    def validate_(self, gds_collector, recursive=False):
+        self.gds_collector_ = gds_collector
+        message_count = len(self.gds_collector_.get_messages())
+        # validate simple type attributes
+        # validate simple type children
+        # validate complex type children
+        self.gds_check_cardinality_(
+            self.StateAssignment, "StateAssignment", min_occurs=1, max_occurs=9999999
+        )
+        if recursive:
+            for item in self.StateAssignment:
+                item.validate_(gds_collector, recursive=True)
+        return message_count == len(self.gds_collector_.get_messages())
+
+    def build(self, node, gds_collector_=None):
+        self.gds_collector_ = gds_collector_
+        if SaveElementTreeNode:
+            self.gds_elementtree_node_ = node
+        already_processed = set()
+        self.ns_prefix_ = node.prefix
+        self._buildAttributes(node, node.attrib, already_processed)
+        for child in node:
+            nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
+            self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+        return self
+
+    def _buildAttributes(self, node, attrs, already_processed):
+        pass
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        if nodeName_ == "StateAssignment":
+            obj_ = StateAssignment.factory(parent_object_=self)
+            obj_.build(child_, gds_collector_=gds_collector_)
+            self.StateAssignment.append(obj_)
+            obj_.original_tagname_ = "StateAssignment"
+
+
+# end class OnEntry
+
+
 class IncludeType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     member_data_items_ = [
         MemberSpec_("href", "xs:anyURI", 0, 0, {"use": "required", "name": "href"}),
     ]
     subclass = None
     superclass = None
@@ -5047,15 +6982,14 @@
 
         Returns 0.5 is fraction_along was not set.
         """
 
         return float(self.fraction_along) if self.fraction_along else 0.5
 
     def __str__(self):
-
         return (
             "Input "
             + str(self.id)
             + ": "
             + str(self.get_target_cell_id())
             + ":"
             + str(self.get_segment_id())
@@ -5384,16 +7318,14 @@
             obj_.original_tagname_ = "inputW"
         super(InputList, self)._buildChildren(child_, node, nodeName_, True)
 
     def exportHdf5(self, h5file, h5Group):
         """Export to HDF5 file."""
         # print("Exporting InputList: "+str(self.id)+" as HDF5")
 
-        import numpy
-
         ilGroup = h5file.create_group(h5Group, "inputList_" + self.id)
         ilGroup._f_setattr("id", self.id)
         ilGroup._f_setattr("component", self.component)
         ilGroup._f_setattr("population", self.populations)
 
         cols = 4
 
@@ -5433,15 +7365,14 @@
         array._f_setattr("column_1", "target_cell_id")
         array._f_setattr("column_2", "segment_id")
         array._f_setattr("column_3", "fraction_along")
         for k in extra_cols:
             array._f_setattr(k, extra_cols[k])
 
     def __str__(self):
-
         return (
             "Input list: "
             + self.id
             + " to "
             + self.populations
             + ", component "
             + self.component
@@ -5693,15 +7624,14 @@
 
         Returns 0.5 is fraction_along was not set.
         """
 
         return float(self.fraction_along) if self.fraction_along else 0.5
 
     def __str__(self):
-
         return (
             "Input "
             + str(self.id)
             + ": "
             + str(self.get_target_cell_id())
             + ":"
             + str(self.get_segment_id())
@@ -5725,15 +7655,14 @@
         """Get target population."""
         if "[" in self.target:
             return self.target.split("[")[0]
         else:
             return self.target.split("/")[0]
 
     def __str__(self):
-
         dest = self.destination if self.destination else "unspecified"
         return (
             "Explicit Input of type "
             + str(self.input)
             + " to "
             + self.get_target_population()
             + "(cell "
@@ -6615,15 +8544,14 @@
         """Get population"""
         if "[" in ref:
             return ref.split("[")[0]
         else:
             return ref.split("/")[0]
 
     def __str__(self):
-
         dest = self.destination if self.destination else "unspecified"
         return (
             "Synaptic connection from "
             + str(self._get_population(self.from_))
             + "(cell "
             + str(self._get_cell_id(self.from_))
             + ") -> "
@@ -7025,34 +8953,31 @@
     def _buildChildren(
         self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
     ):
         super(Location, self)._buildChildren(child_, node, nodeName_, True)
         pass
 
     def _format(self, value):
-
         if int(value) == value:
             return str(int(value))
         else:
             return "%.4f" % value
 
     def __str__(self):
-
         return (
             "("
             + self._format(self.x)
             + ", "
             + self._format(self.y)
             + ", "
             + self._format(self.z)
             + ")"
         )
 
     def __repr__(self):
-
         return str(self)
 
 
 # end class Location
 
 
 class Instance(BaseWithoutId):
@@ -7299,23 +9224,21 @@
             obj_ = Location.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.location = obj_
             obj_.original_tagname_ = "location"
         super(Instance, self)._buildChildren(child_, node, nodeName_, True)
 
     def __str__(self):
-
         return (
             "Instance "
             + str(self.id)
             + (" at location: " + str(self.location) if self.location else "")
         )
 
     def __repr__(self):
-
         return str(self)
 
 
 # end class Instance
 
 
 class GridLayout(BaseWithoutId):
@@ -8737,24 +10660,21 @@
             obj_.original_tagname_ = "instance"
         super(Population, self)._buildChildren(child_, node, nodeName_, True)
 
     def exportHdf5(self, h5file, h5Group):
         """Export to HDF5 file."""
         # print("Exporting Population: "+str(self.id)+" as HDF5")
 
-        import numpy
-
         popGroup = h5file.create_group(h5Group, "population_" + self.id)
         popGroup._f_setattr("id", self.id)
         popGroup._f_setattr("component", self.component)
         for p in self.properties:
             popGroup._f_setattr("property:" + p.tag, p.value)
 
         if len(self.instances) > 0:
-
             colCount = 3
             a = numpy.zeros([len(self.instances), colCount], numpy.float32)
 
             count = 0
             for instance in self.instances:
                 a[count, 0] = instance.location.x
                 a[count, 1] = instance.location.y
@@ -8779,15 +10699,14 @@
         return (
             len(self.instances)
             if len(self.instances) > 0
             else (self.size if self.size else 0)
         )
 
     def __str__(self):
-
         return (
             "Population: "
             + str(self.id)
             + " with "
             + str(self.get_size())
             + " components of type "
             + (self.component if self.component else "???")
@@ -10380,44 +12299,39 @@
                 continue
             for m in mlist:
                 if hasattr(m, "id"):
                     if m.id == id:
                         return m
                     else:
                         all_ids.append(m.id)
-        from neuroml.loaders import print_
-
         if self.warn_count < 10:
-            print_(
+            neuroml.print_(
                 "Id "
                 + id
                 + " not found in <network> element. All ids: "
                 + str(sorted(all_ids))
             )
             self.warn_count += 1
         elif self.warn_count == 10:
-            print_(" - Suppressing further warnings about id not found...")
+            neuroml.print_(" - Suppressing further warnings about id not found...")
         return None
 
     def __str__(self):
-
         return (
             "Network "
             + str(self.id)
             + " with "
             + str(len(self.populations))
             + " population(s)"
         )
 
     def exportHdf5(self, h5file, h5Group):
         """Export to HDF5 file."""
         # print("Exporting Network: "+str(self.id)+" as HDF5")
 
-        import numpy
-
         netGroup = h5file.create_group(h5Group, "network")
         netGroup._f_setattr("id", self.id)
         netGroup._f_setattr("notes", self.notes)
         if self.temperature:
             netGroup._f_setattr("temperature", self.temperature)
 
         for pop in self.populations:
@@ -18040,16 +19954,15 @@
         pass
 
 
 # end class InhomogeneousValue
 
 
 class ChannelDensityGHK2(Base):
-    """ChannelDensityGHK2 -- Time varying conductance density, **gDensity,**  which is distributed on an area of the cel
-    l, producing a current density **iDensity.**  Modified version of Jaffe et al. 1994 ( used also in Lawrence et al. 2006 ). See https://github.com/OpenSourceBrain/ghk-nernst.
+    """ChannelDensityGHK2 -- Time varying conductance density, **gDensity,**  which is distributed on an area of the cell, producing a current density **iDensity.**  Modified version of Jaffe et al. 1994 ( used also in Lawrence et al. 2006 ). See https://github.com/OpenSourceBrain/ghk-nernst.
     \n
     :param condDensity:
     :type condDensity: conductanceDensity
 
     """
 
     __hash__ = GeneratedsSuper.__hash__
@@ -26039,27 +27952,25 @@
             obj_ = InhomogeneousParameter.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.inhomogeneous_parameters.append(obj_)
             obj_.original_tagname_ = "inhomogeneousParameter"
         super(SegmentGroup, self)._buildChildren(child_, node, nodeName_, True)
 
     def __str__(self):
-
         return (
             "SegmentGroup: "
             + str(self.id)
             + ", "
             + str(len(self.members))
             + " member(s), "
             + str(len(self.includes))
             + " included group(s)"
         )
 
     def __repr__(self):
-
         return str(self)
 
 
 # end class SegmentGroup
 
 
 class Point3DWithDiam(BaseWithoutId):
@@ -26315,29 +28226,27 @@
     def _buildChildren(
         self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
     ):
         super(Point3DWithDiam, self)._buildChildren(child_, node, nodeName_, True)
         pass
 
     def __str__(self):
-
         return (
             "("
             + str(self.x)
             + ", "
             + str(self.y)
             + ", "
             + str(self.z)
             + "), diam "
             + str(self.diameter)
             + "um"
         )
 
     def __repr__(self):
-
         return str(self)
 
     def distance_to(self, other_3d_point):
         """Find the distance between this point and another.
 
         :param other_3d_point: other 3D point to calculate distance to
         :type other_3d_point: Point3DWithDiam
@@ -26982,36 +28891,31 @@
         length = (
             (prox_x - dist_x) ** 2 + (prox_y - dist_y) ** 2 + (prox_z - dist_z) ** 2
         ) ** (0.5)
 
         return length
 
     def __str__(self):
-
         return (
             "<Segment|"
             + str(self.id)
             + ("|" + self.name if self.name is not None else "")
             + ">"
         )
 
     def __repr__(self):
-
         return str(self)
 
     @property
     def volume(self):
         """Get the volume of the segment.
 
         :returns: volume of segment
         :rtype: float
         """
-
-        from math import pi
-
         if self.proximal == None:
             raise Exception(
                 "Cannot get volume of segment "
                 + str(self.id)
                 + " using the volume property, since no proximal point is set on it (the proximal point comes from the parent segment). Use the method get_segment_volume(segment_id) on the cell instead."
             )
 
@@ -27019,15 +28923,14 @@
         dist_rad = self.distal.diameter / 2.0
 
         if (
             self.proximal.x == self.distal.x
             and self.proximal.y == self.distal.y
             and self.proximal.z == self.distal.z
         ):
-
             if prox_rad != dist_rad:
                 raise Exception(
                     "Cannot get volume of segment "
                     + str(self.id)
                     + ". The (x,y,z) coordinates of the proximal and distal points match (i.e. it is a sphere), but the diameters of these points are different, making the volume calculation ambiguous."
                 )
 
@@ -27044,17 +28947,14 @@
     @property
     def surface_area(self):
         """Get the surface area of the segment.
 
         :returns: surface area of segment
         :rtype: float
         """
-        from math import pi
-        from math import sqrt
-
         if self.proximal == None:
             raise Exception(
                 "Cannot get surface area of segment "
                 + str(self.id)
                 + " using the surface_area property, since no proximal point is set on it (the proximal point comes from the parent segment). Use the method get_segment_surface_area(segment_id) on the cell instead."
             )
 
@@ -27062,15 +28962,14 @@
         dist_rad = self.distal.diameter / 2.0
 
         if (
             self.proximal.x == self.distal.x
             and self.proximal.y == self.distal.y
             and self.proximal.z == self.distal.z
         ):
-
             if prox_rad != dist_rad:
                 raise Exception(
                     "Cannot get surface area of segment "
                     + str(self.id)
                     + ". The (x,y,z) coordinates of the proximal and distal points match (i.e. it is a sphere), but the diameters of these points are different, making the surface area calculation ambiguous."
                 )
 
@@ -40154,16 +42053,14 @@
     def summary(self, show_includes=True, show_non_network=True):
         """Get a pretty-printed summary of the complete NeuroMLDocument.
 
         This includes information on the various Components included in the
         NeuroMLDocument: networks, cells, projections, synapses, and so on.
         """
 
-        import inspect
-
         info = "*******************************************************\n"
         info += "* NeuroMLDocument: " + self.id + "\n*\n"
         post = ""
         membs = inspect.getmembers(self)
         for memb in membs:
             if (
                 isinstance(memb[1], list)
@@ -40399,16 +42296,14 @@
         """Get a component by specifying its ID.
 
         :param id: id of Component to get
         :type id: str
         :returns: Component with given ID or None if no Component with provided ID was found
         """
         if len(id) == 0:
-            import inspect
-
             callframe = inspect.getouterframes(inspect.currentframe(), 2)
             print(
                 "Method: " + callframe[1][3] + " is asking for an element with no id..."
             )
 
             return None
         all_ids = []
@@ -40419,26 +42314,24 @@
                 continue
             for m in mlist:
                 if hasattr(m, "id"):
                     if m.id == id:
                         return m
                     else:
                         all_ids.append(m.id)
-        from neuroml.loaders import print_
-
         if self.warn_count < 10:
-            print_(
+            neuroml.print_(
                 "Id "
                 + id
                 + " not found in <neuroml> element. All ids: "
                 + str(sorted(all_ids))
             )
             self.warn_count += 1
         elif self.warn_count == 10:
-            print_(" - Suppressing further warnings about id not found...")
+            neuroml.print_(" - Suppressing further warnings about id not found...")
         return None
 
     def append(self, element):
         """Append an element
 
         :param element: element to append
         :type element: Object
@@ -42535,15 +44428,14 @@
 
         If weight is not set, the default value of 1.0 is returned.
         """
 
         return float(self.weight) if self.weight != None else 1.0
 
     def __str__(self):
-
         return (
             "Input (weight) "
             + str(self.id)
             + ": "
             + str(self.get_target_cell_id())
             + ":"
             + str(self.get_segment_id())
@@ -42870,16 +44762,14 @@
             obj_.original_tagname_ = "continuousConnectionInstanceW"
         super(ContinuousProjection, self)._buildChildren(child_, node, nodeName_, True)
 
     def exportHdf5(self, h5file, h5Group):
         """Export to HDF5 file."""
         # print("Exporting ContinuousProjection: "+str(self.id)+" as HDF5")
 
-        import numpy
-
         projGroup = h5file.create_group(h5Group, "projection_" + self.id)
         projGroup._f_setattr("id", self.id)
         projGroup._f_setattr("type", "continuousProjection")
         projGroup._f_setattr("presynapticPopulation", self.presynaptic_population)
         projGroup._f_setattr("postsynapticPopulation", self.postsynaptic_population)
 
         pre_comp = (
@@ -43280,16 +45170,14 @@
             obj_.original_tagname_ = "electricalConnectionInstanceW"
         super(ElectricalProjection, self)._buildChildren(child_, node, nodeName_, True)
 
     def exportHdf5(self, h5file, h5Group):
         """Export to HDF5 file."""
         # print("Exporting ElectricalProjection: "+str(self.id)+" as HDF5")
 
-        import numpy
-
         projGroup = h5file.create_group(h5Group, "projection_" + self.id)
         projGroup._f_setattr("id", self.id)
         projGroup._f_setattr("type", "electricalProjection")
         projGroup._f_setattr("presynapticPopulation", self.presynaptic_population)
         projGroup._f_setattr("postsynapticPopulation", self.postsynaptic_population)
 
         syn = (
@@ -44515,16 +46403,14 @@
             obj_.original_tagname_ = "connectionWD"
         super(Projection, self)._buildChildren(child_, node, nodeName_, True)
 
     def exportHdf5(self, h5file, h5Group):
         """Export to HDF5 file."""
         # print("Exporting Projection: "+str(self.id)+" as HDF5")
 
-        import numpy
-
         projGroup = h5file.create_group(h5Group, "projection_" + self.id)
         projGroup._f_setattr("id", self.id)
         projGroup._f_setattr("type", "projection")
         projGroup._f_setattr("presynapticPopulation", self.presynaptic_population)
         projGroup._f_setattr("postsynapticPopulation", self.postsynaptic_population)
         projGroup._f_setattr("synapse", self.synapse)
 
@@ -44532,19 +46418,17 @@
 
         connection_wds = len(self.connection_wds) > 0
 
         cols = 2
 
         extra_cols = {}
 
-        from neuroml.utils import has_segment_fraction_info
-
-        include_segment_fraction = has_segment_fraction_info(
+        include_segment_fraction = neuroml.utils.has_segment_fraction_info(
             self.connections
-        ) or has_segment_fraction_info(self.connection_wds)
+        ) or neuroml.utils.has_segment_fraction_info(self.connection_wds)
 
         if include_segment_fraction:
             extra_cols["column_" + str(cols)] = "pre_segment_id"
             extra_cols["column_" + str(cols + 1)] = "post_segment_id"
             extra_cols["column_" + str(cols + 2)] = "pre_fraction_along"
             extra_cols["column_" + str(cols + 3)] = "post_fraction_along"
             cols += 4
@@ -46306,16 +48190,14 @@
         elif nodeName_ == "biophysicalProperties":
             obj_ = BiophysicalProperties.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.biophysical_properties = obj_
             obj_.original_tagname_ = "biophysicalProperties"
         super(Cell, self)._buildChildren(child_, node, nodeName_, True)
 
-    from ..neuro_lex_ids import neuro_lex_ids
-
     # Get segment object by its id
     def get_segment(self, segment_id):
         # type: (int) -> Segment
         """Get segment object by its id
 
         :param segment_id: ID of segment
         :return: segment
@@ -46471,15 +48353,14 @@
         """
 
         if isinstance(segment_group, str):
             for sg in self.morphology.segment_groups:
                 if sg.id == segment_group:
                     segment_group = sg
             if isinstance(segment_group, str):
-
                 if (
                     assume_all_means_all and segment_group == "all"
                 ):  # i.e. wasn't explicitly defined, but assume it means all segments
                     return [seg.id for seg in self.morphology.segments]
 
                 raise Exception(
                     "No segment group " + segment_group + " found in cell " + self.id
@@ -46503,43 +48384,67 @@
         self,
         group_list,
         check_parentage=False,
         include_cumulative_lengths=False,
         include_path_lengths=False,
         path_length_metric="Path Length from root",
     ):  # Only option supported
-        # type: (List, bool, bool, bool, str) -> Dict
+        # type: (List, bool, bool, bool, str) -> Any
         """
-        Get ordered list of segments in specified groups
+        Get ordered list of segments in specified groups, with additional
+        information.
 
-        :param group_list: a group id or list of groups to get segments from
-        :type group_list: str or list
+        Note that this method orders segments by id, so the assumption is that
+        all segment with id `N + m` will be a descendent of segment with id `N`
+        in the segment group.
+
+        :param group_list: a group id or list of group ids to get segments from
+        :type group_list: str or list(str)
         :param check_parentage: verify parentage
         :type check_parentage: bool
-        :param include_commulative_lengths: also include cummulative lengths
+        :param include_cumulative_lengths: also include cummulative length of
+            each segment from root
         :type include_cumulative_lengths: bool
-        :param include_path_lengths: also include path lengths
+        :param include_path_lengths: also include path lengths from segment
+            group's root segment to proximal and distal points of each segment
         :type include_path_lengths: bool
         :param path_length_metric: metric to use for path length ("Path Length
             from root" is currently the only supported option, and the default)
         :type path_length_metric: str
 
-        :return: dictionary of segments with additional information depending
-            on what parameters were used:
+        :returns: depending on provided arguments:
+
+                - if no additional options are provided, returns a dictionary
+                  with segment group ids as keys, and lists of ordered segments
+                  in those segment groups as values (`ord_segs`)
+                - if only `include_path_lengths` is set, returns a tuple:
+                  `[ord_segs, path_lengths_to_proximal ,
+                  path_lengths_to_distal]`
+                - if only `include_cumulative_lengths` is set, returns a tuple:
+                  `[ord_segs, cumulative_lengths]`
+                - if both `include_path_lengths` and
+                  `include_cumulative_lengths` are set, returns a tuple:
+                  `[ord_segs, cumulative_lengths, path_lengths_to_proximal ,
+                  path_lengths_to_distal]`
 
         :raises: Exception if check_parentage is True and parentage cannot be verified
         """
 
         unord_segs = {}
         other_segs = {}
 
         # convert to list if a single segment group ID has been provided
         if isinstance(group_list, str):
             group_list = [group_list]
 
+        # populate the dict to ensure that the order of segment groups is
+        # maintained in the returned result
+        for sgid in group_list:
+            unord_segs[sgid] = None
+
         # get a dict of all segments in the cell, with their ids as keys
         segments = self.get_segment_ids_vs_segments()
 
         # get list of segments in all segment groups
         # and store this information in two dicts:
         # - unord_segs: for segment groups in group_list
         # - other_segs: for segment groups not in group_list
@@ -46551,22 +48456,20 @@
                 unord_segs[sg.id] = [segments[s] for s in all_segs_here]
             else:
                 other_segs[sg.id] = [segments[s] for s in all_segs_here]
 
         ord_segs = {}
 
         # sort unord_segs by id to get an ordered list in ord_segs
-        from operator import attrgetter
-
-        for key in unord_segs.keys():
-            segs = unord_segs[key]
-            if len(segs) == 1 or len(segs) == 0:
-                ord_segs[key] = segs
-            else:
-                ord_segs[key] = sorted(segs, key=attrgetter("id"), reverse=False)
+        for key, segs in unord_segs.items():
+            if segs is not None:
+                if len(segs) == 1 or len(segs) == 0:
+                    ord_segs[key] = segs
+                else:
+                    ord_segs[key] = sorted(segs, key=attrgetter("id"), reverse=False)
 
         if check_parentage:
             # check parent ordering
 
             for key in ord_segs.keys():
                 existing_ids = []
                 for s in ord_segs[key]:
@@ -46577,51 +48480,37 @@
                                 + str(s)
                                 + " in list: "
                                 + str(ord_segs)
                             )
                     existing_ids.append(s.id)
 
         if include_cumulative_lengths or include_path_lengths:
-            import math
-
             cumulative_lengths = {}
             path_lengths_to_proximal = {}
             path_lengths_to_distal = {}
 
             for key in ord_segs.keys():
                 cumulative_lengths[key] = []
                 path_lengths_to_proximal[key] = {}
                 path_lengths_to_distal[key] = {}
 
                 tot_len = 0
                 for seg in ord_segs[key]:
-
                     length = self.get_segment_length(seg.id)
 
                     if (
                         not seg.parent
                         or not seg.parent.segments in path_lengths_to_distal[key]
                     ):
-
                         path_lengths_to_proximal[key][seg.id] = 0
                         last_seg = seg
                         par_seg_element = seg.parent
                         while par_seg_element != None:
-
                             par_seg = segments[par_seg_element.segments]
-                            d = par_seg.distal
-                            p = par_seg.proximal
-
-                            if not p:
-                                par_seg_parent_seg = segments[par_seg.parent.segments]
-                                p = par_seg_parent_seg.distal
-
-                            par_length = math.sqrt(
-                                (d.x - p.x) ** 2 + (d.y - p.y) ** 2 + (d.z - p.z) ** 2
-                            )
+                            par_length = self.get_segment_length(par_seg.id)
 
                             fract = float(last_seg.parent.fraction_along)
                             path_lengths_to_proximal[key][seg.id] += par_length * fract
 
                             last_seg = par_seg
                             par_seg_element = par_seg.parent
 
@@ -46636,23 +48525,20 @@
                         path_lengths_to_proximal[key][seg.id] + length
                     )
 
                     tot_len += length
                     cumulative_lengths[key].append(tot_len)
 
         if include_path_lengths and not include_cumulative_lengths:
-
             return ord_segs, path_lengths_to_proximal, path_lengths_to_distal
 
         if include_cumulative_lengths and not include_path_lengths:
-
             return ord_segs, cumulative_lengths
 
         if include_cumulative_lengths and include_path_lengths:
-
             return (
                 ord_segs,
                 cumulative_lengths,
                 path_lengths_to_proximal,
                 path_lengths_to_distal,
             )
 
@@ -46694,48 +48580,149 @@
                 "Segment group with id matching "
                 + str(substring)
                 + " not found in cell "
                 + str(self.id)
             )
         return sgs
 
-    def summary(self):
+    def summary(self, morph=True, biophys=True):
         """Print cell summary.
 
-        Currently prints:
+        Shows the number of segments and segment groups, and information on the
+        biophysical properties of the cell. See the `morphinfo` and
+        `biophysinfo` methods for more details.
+
+        :param morph: toggle showing/hiding morphology information
+        :type morph: bool
+        :param biophys: toggle showing/hiding biophysology information
+        :type biophys: bool
+        :returns: None
+        """
 
-        - id of cell
-        - any notes
-        - number of segments
-        - number of segment groups
+        print(f"*********** Summary ({self.id}) ************")
+        print("* Notes: " + str(self.notes))
+        print()
 
-        TODO: extend to show more information about the cell that may be useful
-        to users.
+        if morph:
+            print(f"*********** Morphology summary ({self.id}) ************")
+            self.morphinfo()
+            print("*******************************************************")
+            print("Tip: use morphinfo(True) to see more detailed information.")
+
+        if biophys:
+            print(f"*********** Biophys summary ({self.id}) ************")
+            self.biophysinfo()
+            print("*******************************************************")
+
+    def morphinfo(self, segment_detail=False):
+        """Show info on morphology of the cell.
+        By default, since cells can have large numbers of segments and segment
+        groups, it only provides metrics on the total numbers. To see details,
+        pass `segment_detail=True`.
+
+        See also: `get_segment_group_info`.
+
+        :param segment_detail: toggle whether to show detailed information on
+            segment groups and their segments
+        :type segment_detail: bool
+        :returns: None
 
         """
-
-        print("*******************************************************")
-        print("* Cell: " + str(self.id))
-        print("* Notes: " + str(self.notes))
         print("* Segments: " + str(len(self.morphology.segments)))
         print("* SegmentGroups: " + str(len(self.morphology.segment_groups)))
-        print("*******************************************************")
+
+        if segment_detail:
+            for sg in self.morphology.segment_groups:
+                self.get_segment_group_info(sg.id)
+
+    def biophysinfo(self):
+        """Get information on the biophysical properties of the cell.
+        :returns: None
+
+        """
+        bp = None
+        mp = None
+        ip = None
+        if self.__class__.__name__ == "Cell":
+            bp = self.biophysical_properties
+            mp = bp.membrane_properties
+            ip = bp.intracellular_properties
+        elif self.__class__.__name__ == "Cell2CaPools":
+            bp = self.biophysical_properties2_ca_pools
+            mp = bp.membrane_properties2_ca_pools
+            ip = bp.intracellular_properties2_ca_pools
+
+        membp = mp.info(show_contents=True, return_format="dict")
+        # check if there are any membrane properties
+        for prop, val in membp.items():
+            if len(val["members"]) > 0:
+                print(f"* Membrane properties")
+                break
+
+        for prop, val in membp.items():
+            ctype = val["type"]
+            # objects
+            ms = val["members"]
+            if len(ms) > 0:
+                print(f"	* {ctype}:")
+                for am in ms:
+                    inf = am.info(show_contents=True, return_format="dict")
+                    for p, v in inf.items():
+                        print(f"		* {p}: {v['members']}")
+
+                    print()
+
+        intp = ip.info(show_contents=True, return_format="dict")
+        for prop, val in intp.items():
+            if len(val["members"]) > 0:
+                print(f"* Intracellular properties")
+                break
+
+        for prop, val in intp.items():
+            ctype = val["type"]
+            # objects
+            ms = val["members"]
+            if len(ms) > 0:
+                print(f"	* {ctype}:")
+                for am in ms:
+                    inf = am.info(show_contents=True, return_format="dict")
+                    for p, v in inf.items():
+                        print(f"		* {p}: {v['members']}")
+
+                    print()
+
+    def get_segment_group_info(self, group_id):
+        """Get information about a segment group
+
+        :param group_id: id of segment group
+        :type group_id: int
+        :returns: None
+
+        """
+        print(f"* Segment group: {group_id}:")
+        segs = self.get_all_segments_in_group(segment_group=group_id)
+        for s in segs:
+            sinfo = self.get_segment(s)
+            print(
+                f"	 * {s} (Parent: {sinfo.parent.segments if sinfo.parent else '-'}; {self.get_actual_proximal(s)} -> {sinfo.distal})"
+            )
 
     def add_segment(
         self,
         prox,
         dist,
         seg_id=None,
         name=None,
         parent=None,
         fraction_along=1.0,
         group_id=None,
         use_convention=True,
         seg_type=None,
         reorder_segment_groups=True,
+        optimise_segment_groups=True,
     ):
         """Add a segment to the cell, to the provided segment group, creating
         it if required.
 
         :param prox: proximal segment information
         :type prox: list with 4 float entries: [x, y, z, diameter]
         :param dist: dist segment information
@@ -46760,16 +48747,16 @@
             If `use_convention` is `True`, and a `group_id` is provided, the
             segment group will also be added to the default segment groups if
             it has not been previously added. If `group_id` is `None`, the
             segment will be added to the default groups instead.
 
             If `use_convention` is `False`, this is unused.
         :type seg_type: str
-        :param parent: parent segment
-        :type parent: SegmentParent
+        :param parent: parent segment object
+        :type parent: Segment
         :param fraction_along: where the new segment is connected to the parent (0: distal point, 1: proximal point)
         :type fraction_along: float
         :param group_id: id of segment group to add the segment to
             If a segment group with this id does not exist, a new segment group
             will be created.
 
             The suggested convention is: `axon_`, `soma_`, `dend_` for axonal,
@@ -46791,14 +48778,17 @@
             included in the default groups should be declared before they are
             used in the default groups. When adding lots of segments, one may
             want to only reorder at the end of the process instead of after
             each segment is added.
 
             This is only relevant if `use_convention=True`.
         :type reorder_segment_groups: bool
+        :param optimise_segment_groups: toggle whether segment groups should be
+            optimised after operation
+        :type optimise_segment_groups: bool
         :returns: the created segment
         :rtype: Segment
         :raises ValueError: if `seg_id` is provided and a segment with this ID
             already exists
 
         """
         try:
@@ -46833,15 +48823,15 @@
 
         if seg_id:
             try:
                 seg = None
                 seg = self.get_segment(seg_id)
                 if seg:
                     raise ValueError(
-                        "A segment with provided id f{seg_id} already exists"
+                        f"A segment with provided id {seg_id} already exists"
                     )
             except ValueError:
                 # a segment with this ID does not already exist
                 pass
         else:
             seg_id = segid
 
@@ -46863,35 +48853,36 @@
                 seg_group = self.add_segment_group(group_id=group_id)
             seg_group.members.append(Member(segments=segment.id))
 
         if use_convention:
             if not seg_type:
                 raise ValueError("Please provide a seg_type")
             if seg_type == "axon":
-                seg_group_default = self.get_segment_group("axon_group")
+                [seg_group_all, seg_group_default] = self.setup_default_segment_groups(
+                    use_convention=True, default_groups=["all", "axon_group"]
+                )
             elif seg_type == "soma":
-                seg_group_default = self.get_segment_group("soma_group")
+                [seg_group_all, seg_group_default] = self.setup_default_segment_groups(
+                    use_convention=True, default_groups=["all", "soma_group"]
+                )
             elif seg_type == "dendrite":
-                seg_group_default = self.get_segment_group("dendrite_group")
+                [seg_group_all, seg_group_default] = self.setup_default_segment_groups(
+                    use_convention=True, default_groups=["all", "dendrite_group"]
+                )
             else:
                 raise ValueError(f"Invalid segment type provided: {seg_type}")
 
-            seg_group_all = self.get_segment_group("all")
-
-            # get_segment_group raises a ValueError, so won't get here if one
-            # is not found
-
             # Now add the segment group that contains this segment if it exists
             # to the global groups. If a segment group does not exist for this
             # segment, add the segment itself to the global groups
 
             # Do not use add here, we do not need it's extra features (and
             # their performance costs)
             # De-duplicate/optimise later if required
-            if seg_group:
+            if seg_group and seg_group.id != seg_group_default.id:
                 seg_group_default.includes.append(Include(segment_groups=seg_group.id))
                 seg_group_all.includes.append(Include(segment_groups=seg_group.id))
             else:
                 seg_group_default.members.append(Member(segments=segment.id))
                 seg_group_all.members.append(Member(segments=segment.id))
 
             if reorder_segment_groups:
@@ -46910,50 +48901,77 @@
             else:
                 # if it doesn't belong to a group, use the type to indicate
                 # what kind of segment this is
                 segment_name = f"Seg{seg_id}"
             segment.name = segment_name
 
         self.morphology.segments.append(segment)
+
+        if optimise_segment_groups:
+            self.optimise_segment_groups()
+
         return segment
 
-    def add_segment_group(self, group_id):
+    def add_segment_group(self, group_id, neuro_lex_id=None, notes=None):
         """Add a new general segment group.
 
         The segments included in this group do not need to be contiguous. This
-        segment group will not be marked as a section using the required
-        NeuroLex ID.
+        segment group will not be automatically marked as a section using the
+        required NeuroLex ID.
+
+        If a segment group with provided ID already exists, it will not be
+        overwritten.
 
         :param group_id: ID of segment group
         :type group_id: str
+        :param neuro_lex_id: NeuroLex ID to use for segment group
+        :type neuro_lex_id: str
+        :param notes: Notes text to add
+        :type notes: str
         :returns: new segment group
         :rtype: SegmentGroup
 
         """
-        seg_group = self.component_factory("SegmentGroup", id=group_id)
-        self.morphology.segment_groups.append(seg_group)
+        seg_group = None
+        try:
+            seg_group = self.get_segment_group(group_id)
+        except ValueError:
+            seg_group = self.morphology.add(
+                "SegmentGroup",
+                id=group_id,
+                neuro_lex_id=neuro_lex_id,
+                notes=notes,
+                validate=False,
+            )
+        else:
+            print(f"Warning: Segment group {seg_group.id} already exists.")
+
         return seg_group
 
-    def add_unbranched_segment_group(self, group_id):
+    def add_unbranched_segment_group(self, group_id, notes=None):
         """Add a new unbranched segment group.
 
         This is similar to the `add_segment_group` method, but this segment
         group will be used to store contiguous segments, which form an
-        unbranched section of a cell.
+        unbranched section of a cell. It adds the NeuroLex ID for a neuronal
+        branch to the segment group.
 
         :param group_id: ID of segment group
         :type group_id: str
+        :param notes: notes to add
+        :type notes: str
         :returns: new segment group
         :rtype: SegmentGroup
 
         """
-        seg_group = self.component_factory(
-            "SegmentGroup", id=group_id, neuro_lex_id=self.neuro_lex_ids["section"]
+        seg_group = self.add_segment_group(
+            group_id=group_id,
+            neuro_lex_id=neuroml.neuro_lex_ids.neuro_lex_ids["section"],
+            notes=notes,
         )
-        self.morphology.segment_groups.append(seg_group)
         return seg_group
 
     def reorder_segment_groups(self):
         """Move default segment groups to the end.
 
         This is required so that the segment groups included in the default
         groups are defined before they are used.
@@ -46961,19 +48979,18 @@
         :returns: None
 
         """
         seg_groups = self.morphology.segment_groups
         for group in ["soma_group", "axon_group", "dendrite_group", "all"]:
             try:
                 sg = self.get_segment_group(group)
+                seg_groups.append(seg_groups.pop(seg_groups.index(sg)))
             except ValueError:
                 pass
 
-            seg_groups.append(seg_groups.pop(seg_groups.index(sg)))
-
     def optimise_segment_groups(self):
         """Optimise all segment groups in the cell.
 
         This will:
 
         - deduplicate members and includes in segment groups
         - remove members that have already been included using a segment group
@@ -47026,87 +49043,91 @@
         """Set the spike threshold of the cell.
 
         :param v: value to set for spike threshold with units
         :type v: str
         :param group_id: id of segment group to modify
         :type group_id: str
         """
-        self.biophysical_properties.membrane_properties.add(
-            "SpikeThresh", value=v, segment_groups=group_id
-        )
+        self.add_membrane_property("SpikeThresh", value=v, segment_groups=group_id)
 
     def set_init_memb_potential(self, v, group_id="all"):
         """Set the initial membrane potential of the cell.
 
         :param v: value to set for membrane potential with units
         :type v: str
         :param group_id: id of segment group to modify
         :type group_id: str
         """
-        self.biophysical_properties.membrane_properties.add(
+        self.add_membrane_property(
             "InitMembPotential", value=v, segment_groups=group_id
         )
 
     def set_resistivity(self, resistivity, group_id="all") -> None:
         """Set the resistivity of the cell
 
         :type resistivity: str
         :param group_id: segment group to modify
         :type group_id: str
         """
-        self.biophysical_properties.intracellular_properties.add(
+        self.add_intracellular_property(
             "Resistivity", value=resistivity, segment_groups=group_id
         )
 
     def set_specific_capacitance(self, spec_cap, group_id="all"):
         """Set the specific capacitance for the cell.
 
         :param spec_cap: value of specific capacitance with units
         :type spec_cap: str
         :param group_id: segment group to modify
         :type group_id: str
         """
-        self.biophysical_properties.membrane_properties.add(
+        self.add_membrane_property(
             "SpecificCapacitance", value=spec_cap, segment_groups=group_id
         )
 
     def add_intracellular_property(self, property_name, **kwargs):
         """Generic function to add an intracellular property to the cell.
 
         For a full list of membrane properties, see:
         https://docs.neuroml.org/Userdocs/Schemas/Cells.html?#intracellularproperties
 
         :param property_name: name of intracellular property to add
         :type property_name: str
         :param kwargs: named arguments for intracellular property to be added
         :type kwargs: Any
-        :returns: None
+        :returns: added property
 
         """
-        self.biophysical_properties.intracellular_properties.add(
+        self.setup_nml_cell(use_convention=False)
+        prop = self.biophysical_properties.intracellular_properties.add(
             property_name, **kwargs
         )
+        return prop
 
     def add_membrane_property(self, property_name, **kwargs):
         """Generic function to add a membrane property to the cell.
 
         For a full list of membrane properties, see:
         https://docs.neuroml.org/Userdocs/Schemas/Cells.html?#membraneproperties
 
         Please also see specific functions in this module, which are designed to be
         easier to use than this generic function.
 
         :param property_name: name of membrane to add
         :type property_name: str
         :param kwargs: named arguments for membrane property to be added
         :type kwargs: Any
-        :returns: None
+        :returns: added property
 
         """
-        self.biophysical_properties.membrane_properties.add(property_name, **kwargs)
+        self.setup_nml_cell(use_convention=False)
+        prop = self.biophysical_properties.membrane_properties.add(
+            property_name, **kwargs
+        )
+        return prop
 
     def add_channel_density_v(
         self, channel_density_type, nml_cell_doc, ion_chan_def_file="", **kwargs
     ):
         """Generic function to add channel density components to a Cell.
 
         :param channel_density_type: type of channel density to add.
@@ -47115,26 +49136,28 @@
         :type channel_density_type: str
         :param nml_cell_doc: cell NeuroML document to which channel density is to be added
         :type nml_cell_doc: NeuroMLDocument
         :param ion_chan_def_file: path to NeuroML2 file defining the ion channel, if empty, it assumes the channel is defined in the same file
         :type ion_chan_def_file: str
         :param kwargs: named arguments for required channel density type
         :type kwargs: Any
-        :returns: None
+        :returns: added channel density
         """
 
-        self.add_membrane_property(channel_density_type, **kwargs)
+        cd = self.add_membrane_property(channel_density_type, **kwargs)
 
         if len(ion_chan_def_file) > 0:
             if (
                 self.component_factory("IncludeType", href=ion_chan_def_file)
                 not in nml_cell_doc.includes
             ):
                 nml_cell_doc.add("IncludeType", href=ion_chan_def_file)
 
+        return cd
+
     def add_channel_density(
         self,
         nml_cell_doc,
         cd_id,
         ion_channel,
         cond_density,
         erev="0.0 mV",
@@ -47156,16 +49179,18 @@
         :type erev: str
         :param group_id: segment groups to add to
         :type group_id: str
         :param ion: name of ion
         :type ion: str
         :param ion_chan_def_file: path to NeuroML2 file defining the ion channel, if empty, it assumes the channel is defined in the same file
         :type ion_chan_def_file: str
+        :returns: added channel density
+        :rtype: ChannelDensity
         """
-        cd = self.biophysical_properties.membrane_properties.add(
+        cd = self.add_membrane_property(
             "ChannelDensity",
             id=cd_id,
             segment_groups=group_id,
             ion=ion,
             ion_channel=ion_channel,
             erev=erev,
             cond_density=cond_density,
@@ -47174,44 +49199,52 @@
         if len(ion_chan_def_file) > 0:
             if (
                 self.component_factory("IncludeType", href=ion_chan_def_file)
                 not in nml_cell_doc.includes
             ):
                 nml_cell_doc.add("IncludeType", href=ion_chan_def_file)
 
-    def setup_nml_cell(self, use_convention=True, overwrite=False):
+        return cd
+
+    def setup_nml_cell(
+        self, use_convention=True, overwrite=False, default_groups=["all", "soma_group"]
+    ):
         """Correctly initialise a NeuroML cell.
 
         To be called after a new component has been created to initialise the
         cell with these properties:
 
         - Morphology: id="morphology"
         - BiophysicalProperties: id="biophys":
 
           - MembraneProperties
           - IntracellularProperties
 
-        If `use_convention` is True, it also creates some default SegmentGroups for
-        convenience:
-
-        - "all", "soma_group", "dendrite_group", "axon_group" which
-          are used by other helper functions to include all, soma, dendrite, and
-          axon segments respectively.
+        If `use_convention` is True, it also creates the provided
+        `default_groups` SegmentGroups for convenience. By default, it creates
+        the "all", and "soma_group" groups since each cell must at least have a
+        soma.
+
+        When dendritic and axonal segments are added, the `add_segment`
+        function will create `dendrite_group` and `axon_group` groups as
+        required.
 
         Note that since this cell does not currently include a segment in its
         morphology, it is *not* a valid NeuroML construct. Use the `add_segment`
         and `add_unbranched_segments` functions to add segments and branches.
         They will also populate the default segment groups.
 
         :param id: id of the cell
         :type id: str
         :param use_convention: whether helper segment groups should be created using the default convention
         :type use_convention: bool
         :param overwrite: overwrite existing components
         :type overwrite: bool
+        :param default_groups: list of default segment groups to create
+        :type default_groups: list of strings
         :returns: None
         :rtype: None
 
         """
         # do not validate yet, because segments are required
         self.add("Morphology", id="morphology", validate=False, force=overwrite)
 
@@ -47220,48 +49253,76 @@
         self.biophysical_properties.add(
             "IntracellularProperties", validate=False, force=overwrite
         )
         self.biophysical_properties.add(
             "MembraneProperties", validate=False, force=overwrite
         )
 
+        self.setup_default_segment_groups(use_convention, default_groups)
+
+    def setup_default_segment_groups(
+        self, use_convention=True, default_groups=["all", "soma_group"]
+    ):
+        """Create default segment groups for the cell.
+
+        If `use_convention` is True, it also creates the provided
+        `default_groups` SegmentGroups for convenience. By default, it creates
+        the "all", and "soma_group" groups since each cell must at least have a
+        soma. Allowed values are: "all", "soma_group", "axon_group", "dendrite_group".
+
+        :param use_convention: whether helper segment groups should be created using the default convention
+        :type use_convention: bool
+        :param default_groups: list of default segment groups to create
+        :type default_groups: list of strings
+        :returns: list of created segment groups (or empty list if none created)
+        :rtype: list
+        """
+        new_groups = []
         if use_convention:
-            seg_group_all = self.component_factory("SegmentGroup", id="all")
-            seg_group_soma = self.component_factory(
-                "SegmentGroup",
-                id="soma_group",
-                neuro_lex_id=self.neuro_lex_ids["soma"],
-                notes="Default soma segment group for the cell",
-            )
-            seg_group_axon = self.component_factory(
-                "SegmentGroup",
-                id="axon_group",
-                neuro_lex_id=self.neuro_lex_ids["axon"],
-                notes="Default axon segment group for the cell",
-            )
-            seg_group_dend = self.component_factory(
-                "SegmentGroup",
-                id="dendrite_group",
-                neuro_lex_id=self.neuro_lex_ids["dend"],
-                notes="Default dendrite segment group for the cell",
-            )
-            # skip validation: segments etc needed, cell is invalid
-            self.morphology.add(seg_group_all, validate=False, force=overwrite)
-            self.morphology.add(seg_group_soma, validate=False, force=overwrite)
-            self.morphology.add(seg_group_axon, validate=False, force=overwrite)
-            self.morphology.add(seg_group_dend, validate=False, force=overwrite)
+            for grp in default_groups:
+                neuro_lex_id = None
+                notes = None
+
+                if grp == "soma_group":
+                    neuro_lex_id = neuroml.neuro_lex_ids.neuro_lex_ids["soma"]
+                    notes = "Default soma segment group for the cell"
+                elif grp == "axon_group":
+                    neuro_lex_id = neuroml.neuro_lex_ids.neuro_lex_ids["axon"]
+                    notes = "Default axon segment group for the cell"
+                elif grp == "dendrite_group":
+                    neuro_lex_id = neuroml.neuro_lex_ids.neuro_lex_ids["dend"]
+                    notes = "Default dendrite segment group for the cell"
+                elif grp == "all":
+                    neuro_lex_id = None
+                    notes = "Default segment group for all segments in the cell"
+                else:
+                    print(
+                        f"Error: only 'all', 'soma_group', 'dendrite_group', and 'axon_group' are supported. Received {grp}"
+                    )
+                    return []
+
+                seg_group = self.add_segment_group(
+                    group_id=grp, neuro_lex_id=neuro_lex_id, notes=notes
+                )
+                new_groups.append(seg_group)
+
+            self.reorder_segment_groups()
+
+        return new_groups
 
     def add_unbranched_segments(
         self,
         points,
         parent=None,
         fraction_along=1.0,
         group_id=None,
         use_convention=True,
         seg_type=None,
+        reorder_segment_groups=True,
+        optimise_segment_groups=True,
     ):
         """Add an unbranched list of segments to the cell.
 
         The list of points will include the first proximal point where this
         should be joined to the cell, followed by a list of distal points:
 
         ::
@@ -47291,14 +49352,28 @@
         :type group_id: SegmentGroup
         :param use_convention: whether helper segment groups should be created using the default convention
             See the documentation of the `add_segment` method for more information
             on the convention
         :type use_convention: bool
         :param seg_type: type of segments ("axon", "soma", "dendrite")
         :type seg_type: str
+        :param reorder_segment_groups: whether the groups should be reordered
+            to put the default segment groups last after the segment has been
+            added.
+            This is required for a valid NeuroML file because segment groups
+            included in the default groups should be declared before they are
+            used in the default groups. When adding lots of segments, one may
+            want to only reorder at the end of the process instead of after
+            each segment is added.
+
+            This is only relevant if `use_convention=True`.
+        :type reorder_segment_groups: bool
+        :param optimise_segment_groups: toggle whether segment groups should be
+            optimised after operation
+        :type optimise_segment_groups: bool
         :returns: the segment group containing this new list of segments
         :rtype: SegmentGroup
 
         """
         prox = points[0]
         dist = points[1]
 
@@ -47330,19 +49405,28 @@
                 group_id=group_id,
                 use_convention=use_convention,
                 seg_type=seg_type,
                 reorder_segment_groups=False,
             )
             prox = dist
 
-        self.reorder_segment_groups()
+        if reorder_segment_groups:
+            self.reorder_segment_groups()
+
+        if optimise_segment_groups:
+            self.optimise_segment_groups()
+
         return self.get_segment_group(group_id)
 
     def create_unbranched_segment_group_branches(
-        self, root_segment_id: int, use_convention: bool = True
+        self,
+        root_segment_id: int,
+        use_convention: bool = True,
+        reorder_segment_groups=True,
+        optimise_segment_groups=True,
     ):
         """Organise the segments of the cell into new segment groups that each
         form a single contiguous unbranched cell branch.
 
         Note that the first segment (root segment) of a branch must have a proximal
         point that connects it to the rest of the neuronal morphology. If, when
         constructing these branches, a root segment is found that does not include
@@ -47352,29 +49436,52 @@
         segment groups.
 
         :param root_segment_id: id of segment considered the root of the tree,
             generally the first soma segment
         :type root_segment_id: int
         :param use_convention: toggle using NeuroML convention for segment groups
         :type use_convention: bool
+        :param reorder_segment_groups: whether the groups should be reordered
+            to put the default segment groups last after the segment has been
+            added.
+            This is required for a valid NeuroML file because segment groups
+            included in the default groups should be declared before they are
+            used in the default groups. When adding lots of segments, one may
+            want to only reorder at the end of the process instead of after
+            each segment is added.
+
+            This is only relevant if `use_convention=True`.
+        :type reorder_segment_groups: bool
+        :param optimise_segment_groups: toggle whether segment groups should be
+            optimised after operation
+        :type optimise_segment_groups: bool
         :returns: modified cell with new section groups
         :rtype: neuroml.Cell
 
         """
+        # don't recompute if already exists
         # get morphology tree
-        morph_tree = self.get_segment_adjacency_list()
+        morph_tree = getattr(self, "adjacency_list", None)
+        if morph_tree is None:
+            morph_tree = self.get_segment_adjacency_list()
 
         # initialise root segment and first segment group
         seg = self.get_segment(root_segment_id)
         group_name = f"seg_group_{len(self.morphology.segment_groups) - 1}_seg_{seg.id}"
         new_seg_group = self.add_unbranched_segment_group(group_name)
 
         # run recursive function
         self.__sectionise(root_segment_id, new_seg_group, morph_tree)
 
+        if reorder_segment_groups:
+            self.reorder_segment_groups()
+
+        if optimise_segment_groups:
+            self.optimise_segment_groups()
+
     def __sectionise(self, root_segment_id, seg_group, morph_tree):
         """Main recursive sectionising method.
 
         :param root_segment_id: id of root of branch
         :type root_segment_id: int
         :returns: TODO
 
@@ -47420,31 +49527,285 @@
         """Get the adjacency list of all segments in the cell morphology.
         Returns a dict where each key is a parent segment, and the value is the
         list of its children segments.
 
         Segment without children (leaf segments) are not included as parents in the
         adjacency list.
 
-        :returns: dict with parent segments as keys and their children as values
-        :rtype: dict
+        This method also stores the computed adjacency list in
+        `self.adjacency_list` for future use by other methods.
+
+        `self.adjacency_list` is populated each time this method is run, to
+        ensure that users can regenerate it after making modifications to the
+        cell morphology. If the morphology has not changed, one only needs to
+        populate it once and then re-use it as required.
+
+        :returns: dict with parent segment ids as keys and ids of their children as values
+        :rtype: dict[int, list[int]]
 
         """
         # create data structure holding list of children for each segment
         child_lists = {}
         for segment in self.morphology.segments:
             try:
                 parent = segment.parent.segments
                 if parent not in child_lists:
                     child_lists[parent] = []
                 child_lists[parent].append(segment.id)
             except AttributeError:
                 print(f"Warning: Segment: {segment} has no parent")
 
+        self.adjacency_list = child_lists
         return child_lists
 
+    def get_graph(self):
+        """Get a networkx DiGraph of the morphology of the cell with distances
+        between the proximal point of a parent and the point where a child
+        connects to it as the weights of the edges of the graph.
+
+        Please see https://networkx.org/documentation/stable/reference
+        for information on networkx routines that can be used on this graph.
+
+        This method also stores the graph in the `self.cell_graph` attribute
+        for future use.
+
+        :returns: networkx.Graph
+
+        """
+        cell_graph = nx.DiGraph()
+
+        # don't recompute if already exists
+        adlist = getattr(self, "adjacency_list", None)
+        if adlist is None:
+            adlist = self.get_segment_adjacency_list()
+
+        for parid, childrenids in adlist.items():
+            par_length = self.get_segment_length(parid)
+
+            for cid in childrenids:
+                child = self.get_segment(cid)
+
+                fract = float(child.parent.fraction_along)
+                len_to_proximal = par_length * fract
+
+                cell_graph.add_edge(parid, cid, weight=len_to_proximal)
+
+        self.cell_graph = cell_graph
+        return cell_graph
+
+    def get_distance(self, dest, source=0):
+        """Get path length between between two segments on a cell.
+
+        Uses `networkx.dijkstra_path_length` to compute the shortest
+        path between source and dest
+
+        :param from: id of segment to get distance from
+        :type from: int
+        :param to: id of segment to get distance to
+        :type to: int
+        :returns: float
+        """
+        graph = getattr(self, "cell_graph", None)
+        if graph is None:
+            graph = self.get_graph()
+        return nx.dijkstra_path_length(graph, source, dest)
+
+    def get_all_distances_from_segment(self, seg_id=0):
+        """Get distances of all segments from the segment with id seg_id.
+
+        Useful to get distances of segments from the soma.
+
+        Uses networkx.single_source_dijkstra on the cell graph, without a
+        target.
+
+        :param seg_id: id of segment to get distances from
+        :type seg_id: int
+        :returns: pair of dictionaries for distance, path
+            The return value is a tuple of two dictionaries keyed by target
+            nodes. The first dictionary stores distance to each target node.
+            The second stores the path to each target node.
+
+        """
+        graph = getattr(self, "cell_graph", None)
+        if graph is None:
+            graph = self.get_graph()
+        return nx.single_source_dijkstra(graph, source=seg_id)
+
+    def get_segments_at_distance(self, distance, src_seg=0):
+        """Get all segments at distance from the provided `src_seg`.
+
+        For each segment, it returns the fraction along the segment that the
+        provided distance is at. For example, if segment N is 500 units long,
+        and the `distance` cut-off is at 200, the fraction along is: 200/500.
+
+        :param src_seg: id of segment to get distances from
+        :type src_seg: int
+        :param distance: distance to get segments at
+        :type distance: float
+        :returns: dict with segment ids as keys, and fraction along at which
+            the cut off is as values
+
+        """
+        graph = getattr(self, "cell_graph", None)
+        if graph is None:
+            graph = self.get_graph()
+        # returns all segments that are less than `distance` away.
+        (target_dict, path_dict) = nx.single_source_dijkstra(
+            graph, source=src_seg, cutoff=distance
+        )
+
+        segs_frac_alongs = {}
+
+        for tgt, dist in target_dict.items():
+            try:
+                frac_along = (distance - dist) / self.get_segment_length(tgt)
+            except ZeroDivisionError:
+                # ignore zero length segments
+                print(f"Warning: encountered zero length segment: {tgt}")
+                continue
+
+            if frac_along > 1.0:
+                # not in this segment
+                continue
+            else:
+                segs_frac_alongs[tgt] = frac_along
+
+        return segs_frac_alongs
+
+    def get_branching_points(self):
+        """Get segments where the cell morphology branches.
+
+        That is, the out-degree of the segment is > 1
+
+        :returns: list of segment ids
+
+        """
+        graph = getattr(self, "cell_graph", None)
+        if graph is None:
+            graph = self.get_graph()
+
+        segs = [n for (n, d) in graph.out_degree if d > 1]
+        return segs
+
+    def get_extremeties(self):
+        """Get segments that are at the ends/tips of the neuronal morphology,
+        with their distances from the soma.
+
+        :returns: dict of segment ids and their distances from cell root as values
+
+        """
+        graph = getattr(self, "cell_graph", None)
+        if graph is None:
+            graph = self.get_graph()
+        segs = [n for (n, d) in graph.out_degree if d == 0]
+
+        res = {}
+        for s in segs:
+            res[s] = self.get_distance(s)
+        return res
+
+    def get_segment_location_info(self, seg_id):
+        """Get location information about a particular segment.
+
+        :param seg_id: id of segment to get information for
+        :type seg_id: int
+        :returns: a dictionary with various metrics about the segment
+
+            - length of segment
+            - distance from cell root
+            - distance from nearest branching point
+            - name of unbranched segment group segment belongs to (if any)
+            - id of root segment of the unbranched segment group
+            - distance from the segment group root segment
+
+        """
+        soma_id = self.get_morphology_root()
+        distance_from_soma = self.get_distance(seg_id, source=soma_id)
+        in_sg = None
+        sg_segs = None
+        sg_root = None
+        distance_from_sg_root = None
+        distance_from_bpt = None
+
+        # get the unbranched segment group that this segment is in
+        for sg in self.morphology.segment_groups:
+            if sg.neuro_lex_id == neuroml.neuro_lex_ids.neuro_lex_ids["section"]:
+                sg_segs = self.get_all_segments_in_group(sg)
+                if seg_id in sg_segs:
+                    in_sg = sg
+
+                    # break out of loop
+                    break
+
+        graph = getattr(self, "cell_graph", None)
+        if graph is None:
+            graph = self.get_graph()
+
+        # find first ancestral branching point
+        # (a segment with more than one child)
+        current = seg_id
+        sg_root = current
+        parent = list(graph.predecessors(current))[0]
+        children = list(graph.successors(parent))
+
+        while len(children) == 1:
+            # the root of the segment group may not be at a
+            # branching point: an unbranched cell branch can consist of
+            # multiple unbranched segment groups
+            if in_sg is not None:
+                if current in sg_segs:
+                    sg_root = current
+
+            current = parent
+            parent = list(graph.predecessors(current))[0]
+            children = list(graph.successors(parent))
+
+        distance_from_bpt = self.get_distance(seg_id, source=current)
+
+        res = {}
+        res["id"] = seg_id
+        res["length"] = self.get_segment_length(seg_id)
+        res["distance_from_cell_root"] = distance_from_soma
+        res["distance_from_nearest_branching_point"] = distance_from_bpt
+
+        # at unbranched segment root
+        if in_sg is not None:
+            res["in_unbranched_segment_group"] = in_sg.id
+            res["unbranched_segment_group_root"] = sg_root
+            distance_from_sg_root = self.get_distance(seg_id, source=sg_root)
+            res["distance_from_segment_group_root"] = distance_from_sg_root
+
+        return res
+
+    def get_morphology_root(self):
+        """Return the root of the complete cell morphology.
+
+        This is usually the first segment of the soma, and there should only be
+        one such segment.
+
+        :returns: id of the root segment
+
+        """
+        # check if convention was followed and segment id 0 is root (has no
+        # parents)
+        try:
+            root_seg = self.get_segment(0)
+            if root_seg.parent is None:
+                return 0
+        except ValueError:
+            pass
+
+        graph = getattr(self, "cell_graph", None)
+        if graph is None:
+            graph = self.get_graph()
+        segs = [n for (n, d) in graph.in_degree if d == 0]
+        # there should only be one segment with 0 indegree
+        assert len(segs) == 1
+        return segs[0]
+
     # end class Cell
 
 
 class PinskyRinzelCA3Cell(BaseCell):
     """PinskyRinzelCA3Cell -- Reduced CA3 cell model from Pinsky and Rinzel 1994. See https://github.com/OpenSourceBrain/PinskyRinzelModel
     \n
     :param iSoma:
@@ -53586,14 +55947,203 @@
         super(LEMS_Property, self)._buildChildren(child_, node, nodeName_, True)
         pass
 
 
 # end class LEMS_Property
 
 
+class DerivedParameter(NamedDimensionalType):
+    """DerivedParameter -- LEMS DerivedParamter element"""
+
+    __hash__ = GeneratedsSuper.__hash__
+    member_data_items_ = [
+        MemberSpec_("value", "xs:string", 0, 0, {"use": "required", "name": "value"}),
+    ]
+    subclass = None
+    superclass = NamedDimensionalType
+
+    def __init__(
+        self,
+        name: "a string (required)" = None,
+        dimension: "a string (required)" = None,
+        description: "a string (optional)" = None,
+        value: "a string (required)" = None,
+        gds_collector_=None,
+        **kwargs_,
+    ):
+        self.gds_collector_ = gds_collector_
+        self.gds_elementtree_node_ = None
+        self.original_tagname_ = None
+        self.parent_object_ = kwargs_.get("parent_object_")
+        self.ns_prefix_ = None
+        super(globals().get("DerivedParameter"), self).__init__(
+            name, dimension, description, **kwargs_
+        )
+        self.value = _cast(None, value)
+        self.value_nsprefix_ = None
+
+    def factory(*args_, **kwargs_):
+        if CurrentSubclassModule_ is not None:
+            subclass = getSubclassFromModule_(CurrentSubclassModule_, DerivedParameter)
+            if subclass is not None:
+                return subclass(*args_, **kwargs_)
+        if DerivedParameter.subclass:
+            return DerivedParameter.subclass(*args_, **kwargs_)
+        else:
+            return DerivedParameter(*args_, **kwargs_)
+
+    factory = staticmethod(factory)
+
+    def _hasContent(self):
+        if super(DerivedParameter, self)._hasContent():
+            return True
+        else:
+            return False
+
+    def export(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_="",
+        name_="DerivedParameter",
+        pretty_print=True,
+    ):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get("DerivedParameter")
+        if imported_ns_def_ is not None:
+            namespacedef_ = imported_ns_def_
+        if pretty_print:
+            eol_ = "\n"
+        else:
+            eol_ = ""
+        if self.original_tagname_ is not None and name_ == "DerivedParameter":
+            name_ = self.original_tagname_
+        if UseCapturedNS_ and self.ns_prefix_:
+            namespaceprefix_ = self.ns_prefix_ + ":"
+        showIndent(outfile, level, pretty_print)
+        outfile.write(
+            "<%s%s%s"
+            % (
+                namespaceprefix_,
+                name_,
+                namespacedef_ and " " + namespacedef_ or "",
+            )
+        )
+        already_processed = set()
+        self._exportAttributes(
+            outfile,
+            level,
+            already_processed,
+            namespaceprefix_,
+            name_="DerivedParameter",
+        )
+        if self._hasContent():
+            outfile.write(">%s" % (eol_,))
+            self._exportChildren(
+                outfile,
+                level + 1,
+                namespaceprefix_,
+                namespacedef_,
+                name_="DerivedParameter",
+                pretty_print=pretty_print,
+            )
+            outfile.write("</%s%s>%s" % (namespaceprefix_, name_, eol_))
+        else:
+            outfile.write("/>%s" % (eol_,))
+
+    def _exportAttributes(
+        self,
+        outfile,
+        level,
+        already_processed,
+        namespaceprefix_="",
+        name_="DerivedParameter",
+    ):
+        super(DerivedParameter, self)._exportAttributes(
+            outfile,
+            level,
+            already_processed,
+            namespaceprefix_,
+            name_="DerivedParameter",
+        )
+        if self.value is not None and "value" not in already_processed:
+            already_processed.add("value")
+            outfile.write(
+                " value=%s"
+                % (
+                    self.gds_encode(
+                        self.gds_format_string(
+                            quote_attrib(self.value), input_name="value"
+                        )
+                    ),
+                )
+            )
+
+    def _exportChildren(
+        self,
+        outfile,
+        level,
+        namespaceprefix_="",
+        namespacedef_="",
+        name_="DerivedParameter",
+        fromsubclass_=False,
+        pretty_print=True,
+    ):
+        super(DerivedParameter, self)._exportChildren(
+            outfile,
+            level,
+            namespaceprefix_,
+            namespacedef_,
+            name_,
+            True,
+            pretty_print=pretty_print,
+        )
+        pass
+
+    def validate_(self, gds_collector, recursive=False):
+        self.gds_collector_ = gds_collector
+        message_count = len(self.gds_collector_.get_messages())
+        # validate simple type attributes
+        self.gds_validate_builtin_ST_(self.gds_validate_string, self.value, "value")
+        self.gds_check_cardinality_(self.value, "value", required=True)
+        # validate simple type children
+        # validate complex type children
+        if recursive:
+            pass
+        return message_count == len(self.gds_collector_.get_messages())
+
+    def build(self, node, gds_collector_=None):
+        self.gds_collector_ = gds_collector_
+        if SaveElementTreeNode:
+            self.gds_elementtree_node_ = node
+        already_processed = set()
+        self.ns_prefix_ = node.prefix
+        self._buildAttributes(node, node.attrib, already_processed)
+        for child in node:
+            nodeName_ = Tag_pattern_.match(child.tag).groups()[-1]
+            self._buildChildren(child, node, nodeName_, gds_collector_=gds_collector_)
+        return self
+
+    def _buildAttributes(self, node, attrs, already_processed):
+        value = find_attr_value_("value", node)
+        if value is not None and "value" not in already_processed:
+            already_processed.add("value")
+            self.value = value
+        super(DerivedParameter, self)._buildAttributes(node, attrs, already_processed)
+
+    def _buildChildren(
+        self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None
+    ):
+        super(DerivedParameter, self)._buildChildren(child_, node, nodeName_, True)
+        pass
+
+
+# end class DerivedParameter
+
+
 class Parameter(NamedDimensionalType):
     __hash__ = GeneratedsSuper.__hash__
     member_data_items_ = []
     subclass = None
     superclass = NamedDimensionalType
 
     def __init__(
@@ -55521,15 +58071,14 @@
             + "%.5f" % self.get_post_fraction_along()
             + ")"
             if self.get_post_segment_id() != 0 or self.get_post_fraction_along() != 0.5
             else ""
         )
 
     def __str__(self):
-
         return (
             "Continuous Connection "
             + str(self.id)
             + ": "
             + str(self.get_pre_info())
             + " -> "
             + str(self.get_post_info())
@@ -55866,15 +58415,14 @@
             + "%.5f" % self.get_post_fraction_along()
             + ")"
             if self.get_post_segment_id() != 0 or self.get_post_fraction_along() != 0.5
             else ""
         )
 
     def __str__(self):
-
         return (
             "Electrical Connection "
             + str(self.id)
             + ": "
             + str(self.get_pre_info())
             + " -> "
             + str(self.get_post_info())
@@ -56212,26 +58760,24 @@
             + "%.5f" % self.get_post_fraction_along()
             + ")"
             if self.get_post_segment_id() != 0 or self.get_post_fraction_along() != 0.5
             else ""
         )
 
     def __str__(self):
-
         return (
             "Connection "
             + str(self.id)
             + ": "
             + str(self.get_pre_info())
             + " -> "
             + str(self.get_post_info())
         )
 
     def __str__(self):
-
         return (
             "Connection "
             + str(self.id)
             + ": "
             + str(self.get_pre_info())
             + " -> "
             + str(self.get_post_info())
@@ -56493,15 +59039,14 @@
             + "%.5f" % self.get_post_fraction_along()
             + ")"
             if self.get_post_segment_id() != 0 or self.get_post_fraction_along() != 0.5
             else ""
         )
 
     def __str__(self):
-
         return (
             "Connection "
             + str(self.id)
             + ": "
             + str(self.get_pre_info())
             + " -> "
             + str(self.get_post_info())
@@ -61109,15 +63654,14 @@
     def _get_cell_id(self, id_string):
         if "[" in id_string:
             return int(id_string.split("[")[1].split("]")[0])
         else:
             return int(id_string.split("/")[2])
 
     def __str__(self):
-
         return (
             "Continuous Connection (Instance based) "
             + str(self.id)
             + ": "
             + str(self.get_pre_info())
             + " -> "
             + str(self.get_post_info())
@@ -61338,15 +63882,14 @@
     def _get_cell_id(self, id_string):
         if "[" in id_string:
             return int(id_string.split("[")[1].split("]")[0])
         else:
             return int(id_string.split("/")[2])
 
     def __str__(self):
-
         return (
             "Electrical Connection (Instance based) "
             + str(self.id)
             + ": "
             + str(self.get_pre_info())
             + " -> "
             + str(self.get_post_info())
@@ -63454,15 +65997,14 @@
 
         If weight is not set, the default value of 1.0 is returned.
         """
 
         return float(self.weight) if self.weight != None else 1.0
 
     def __str__(self):
-
         return (
             "Continuous Connection (Instance based & weight) "
             + str(self.id)
             + ": "
             + str(self.get_pre_info())
             + " -> "
             + str(self.get_post_info())
@@ -63694,15 +66236,14 @@
         :returns: weight of connection or 1.0 if not set
         :rtype: float
         """
 
         return float(self.weight) if self.weight != None else 1.0
 
     def __str__(self):
-
         return (
             "Electrical Connection (Instance based & weight) "
             + str(self.id)
             + ": "
             + str(self.get_pre_info())
             + " -> "
             + str(self.get_post_info())
@@ -64491,14 +67032,15 @@
         ("MetaId", "NeuroML_v2.3.xsd", "ST"),
         ("NeuroLexId", "NeuroML_v2.3.xsd", "ST"),
         ("NonNegativeInteger", "NeuroML_v2.3.xsd", "ST"),
         ("PositiveInteger", "NeuroML_v2.3.xsd", "ST"),
         ("DoubleGreaterThanZero", "NeuroML_v2.3.xsd", "ST"),
         ("ZeroOrOne", "NeuroML_v2.3.xsd", "ST"),
         ("Notes", "NeuroML_v2.3.xsd", "ST"),
+        ("TrueOrFalse", "NeuroML_v2.3.xsd", "ST"),
         ("ZeroToOne", "NeuroML_v2.3.xsd", "ST"),
         ("channelTypes", "NeuroML_v2.3.xsd", "ST"),
         ("gateTypes", "NeuroML_v2.3.xsd", "ST"),
         ("BlockTypes", "NeuroML_v2.3.xsd", "ST"),
         ("PlasticityTypes", "NeuroML_v2.3.xsd", "ST"),
         ("Metric", "NeuroML_v2.3.xsd", "ST"),
         ("networkTypes", "NeuroML_v2.3.xsd", "ST"),
@@ -64508,23 +67050,32 @@
         ("Annotation", "NeuroML_v2.3.xsd", "CT"),
         ("ComponentType", "NeuroML_v2.3.xsd", "CT"),
         ("Constant", "NeuroML_v2.3.xsd", "CT"),
         ("Exposure", "NeuroML_v2.3.xsd", "CT"),
         ("NamedDimensionalType", "NeuroML_v2.3.xsd", "CT"),
         ("NamedDimensionalVariable", "NeuroML_v2.3.xsd", "CT"),
         ("Parameter", "NeuroML_v2.3.xsd", "CT"),
+        ("DerivedParameter", "NeuroML_v2.3.xsd", "CT"),
         ("LEMS_Property", "NeuroML_v2.3.xsd", "CT"),
         ("Requirement", "NeuroML_v2.3.xsd", "CT"),
         ("InstanceRequirement", "NeuroML_v2.3.xsd", "CT"),
         ("Dynamics", "NeuroML_v2.3.xsd", "CT"),
         ("DerivedVariable", "NeuroML_v2.3.xsd", "CT"),
         ("StateVariable", "NeuroML_v2.3.xsd", "CT"),
         ("ConditionalDerivedVariable", "NeuroML_v2.3.xsd", "CT"),
         ("Case", "NeuroML_v2.3.xsd", "CT"),
         ("TimeDerivative", "NeuroML_v2.3.xsd", "CT"),
+        ("OnStart", "NeuroML_v2.3.xsd", "CT"),
+        ("StateAssignment", "NeuroML_v2.3.xsd", "CT"),
+        ("OnEvent", "NeuroML_v2.3.xsd", "CT"),
+        ("EventOut", "NeuroML_v2.3.xsd", "CT"),
+        ("OnCondition", "NeuroML_v2.3.xsd", "CT"),
+        ("Transition", "NeuroML_v2.3.xsd", "CT"),
+        ("Regime", "NeuroML_v2.3.xsd", "CT"),
+        ("OnEntry", "NeuroML_v2.3.xsd", "CT"),
         ("NeuroMLDocument", "NeuroML_v2.3.xsd", "CT"),
         ("IncludeType", "NeuroML_v2.3.xsd", "CT"),
         ("IonChannelScalable", "NeuroML_v2.3.xsd", "CT"),
         ("IonChannelKS", "NeuroML_v2.3.xsd", "CT"),
         ("IonChannel", "NeuroML_v2.3.xsd", "CT"),
         ("IonChannelHH", "NeuroML_v2.3.xsd", "CT"),
         ("IonChannelVShift", "NeuroML_v2.3.xsd", "CT"),
@@ -64746,24 +67297,26 @@
     "ConnectionWD",
     "Constant",
     "ContinuousConnection",
     "ContinuousConnectionInstance",
     "ContinuousConnectionInstanceW",
     "ContinuousProjection",
     "DecayingPoolConcentrationModel",
+    "DerivedParameter",
     "DerivedVariable",
     "DistalDetails",
     "DoubleSynapse",
     "Dynamics",
     "EIF_cond_alpha_isfa_ista",
     "EIF_cond_exp_isfa_ista",
     "ElectricalConnection",
     "ElectricalConnectionInstance",
     "ElectricalConnectionInstanceW",
     "ElectricalProjection",
+    "EventOut",
     "ExpCondSynapse",
     "ExpCurrSynapse",
     "ExpOneSynapse",
     "ExpThreeSynapse",
     "ExpTwoSynapse",
     "ExplicitInput",
     "Exposure",
@@ -64825,14 +67378,18 @@
     "MembraneProperties",
     "MembraneProperties2CaPools",
     "Morphology",
     "NamedDimensionalType",
     "NamedDimensionalVariable",
     "Network",
     "NeuroMLDocument",
+    "OnCondition",
+    "OnEntry",
+    "OnEvent",
+    "OnStart",
     "OpenState",
     "Parameter",
     "Path",
     "PinskyRinzelCA3Cell",
     "PlasticityMechanism",
     "Point3DWithDiam",
     "PoissonFiringSynapse",
@@ -64844,14 +67401,15 @@
     "PulseGeneratorDL",
     "Q10ConductanceScaling",
     "Q10Settings",
     "RampGenerator",
     "RampGeneratorDL",
     "RandomLayout",
     "ReactionScheme",
+    "Regime",
     "Region",
     "Requirement",
     "Resistivity",
     "ReverseTransition",
     "Segment",
     "SegmentEndPoint",
     "SegmentGroup",
@@ -64868,21 +67426,23 @@
     "SpikeGenerator",
     "SpikeGeneratorPoisson",
     "SpikeGeneratorRandom",
     "SpikeGeneratorRefPoisson",
     "SpikeSourcePoisson",
     "SpikeThresh",
     "Standalone",
+    "StateAssignment",
     "StateVariable",
     "SubTree",
     "SynapticConnection",
     "TauInfTransition",
     "TimeDerivative",
     "TimedSynapticInput",
     "TransientPoissonFiringSynapse",
+    "Transition",
     "UnstructuredLayout",
     "VariableParameter",
     "VoltageClamp",
     "VoltageClampTriple",
     "basePyNNCell",
     "basePyNNIaFCell",
     "basePyNNIaFCondCell",
```

### Comparing `libNeuroML-0.4.1/neuroml/test/misc_tests.py` & `libNeuroML-0.5.1/neuroml/test/misc_tests.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.4.1/neuroml/test/test_arraymorph.py` & `libNeuroML-0.5.1/neuroml/test/test_arraymorph.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,14 @@
     def test_segment_instance(self):
         seg = self.test_morphology.segments[47]
         self.assertIsInstance(seg, neuroml.nml.nml.Segment)
 
 
 class TestArrayMorphology(unittest.TestCase):
     def setUp(self):
-
         num_segments = int(100)
         num_vertices = num_segments + 1
 
         x = np.linspace(0, 10, num_vertices)
         y = np.zeros(num_vertices)
         z = np.zeros(num_vertices)
         d = np.linspace(1, 0.01, num_vertices)
@@ -299,17 +298,15 @@
         # Ignore the VisibleDeprecationWarning that numpy throws.
         with warnings.catch_warnings():
             warnings.filterwarnings(
                 "ignore", "Creating an ndarray from ragged nested sequences"
             )
             vertices = [[0, 0, 0], [1, 1]]
             connectivity = [-1, 0]
-            self.assertRaises(
-                AssertionError, am.ArrayMorphology, vertices, connectivity
-            )
+            self.assertRaises(Exception, am.ArrayMorphology, vertices, connectivity)
 
         vertices = [[0, 0, 0], [1, 1, 1]]
         connectivity = [-1, 0, 0]
         self.assertRaises(AssertionError, am.ArrayMorphology, vertices, connectivity)
 
         vertices = [[0, 0, 0], [1, 1, 1]]
         connectivity = []
@@ -356,27 +353,25 @@
 
     def test_segmentlist_getter(self):
         segment = self.optimized_morphology.segments[1]
         segment_again = self.optimized_morphology.segments[1]
         self.assertEqual(segment, segment_again)
 
     def test_segmentlist_setter(self):
-
         p = neuroml.Point3DWithDiam(x=0.9, y=0.0, z=0.0, diameter=0.1)
 
         d = neuroml.Point3DWithDiam(x=0.0, y=0.0, z=0.0, diameter=0.1)
 
         new_segment = neuroml.Segment(proximal=p, distal=d)
 
         self.optimized_morphology.segments[2] = new_segment
 
         self.assertEqual(self.optimized_morphology.segments[2], new_segment)
 
     def test_segmentlist_setter_by_inference(self):
-
         p = neuroml.Point3DWithDiam(x=0.9, y=0.0, z=0.0, diameter=0.1)
 
         d = neuroml.Point3DWithDiam(x=0.0, y=0.0, z=0.0, diameter=0.1)
 
         new_segment = neuroml.Segment(proximal=p, distal=d)
 
         self.optimized_morphology.segments[2] = new_segment
```

### Comparing `libNeuroML-0.4.1/neuroml/test/test_hdf5_optimized.py` & `libNeuroML-0.5.1/neuroml/test/test_hdf5_optimized.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,23 +13,21 @@
 try:
     import unittest2 as unittest
 except ImportError:
     import unittest
 
 
 class TestNeuroMLHDF5Optimized(unittest.TestCase):
-
     base_dir = os.path.dirname(__file__)
     # base_dir = '.'
 
     def runTest(self):
         print("Running tests in TestNeuroMLHDF5Optimized")
 
     def test_write_load(self):
-
         # for f in []:
         # for f in ['complete.nml']:
         # for f in ['simplenet.nml','testh5.nml','MediumNet.net.nml','complete.nml']:
 
         for f in ["simplenet.nml", "MediumNet.net.nml"]:
             file_name = "%s/../examples/test_files/%s" % (self.base_dir, f)
 
@@ -75,10 +73,9 @@
             print("Reloaded: %s" % nml_h5_file_3)
             print("\n" + summary3)
 
             compare(summary0, summary3)
 
 
 if __name__ == "__main__":
-
     tnxp = TestNeuroMLHDF5Optimized()
     tnxp.test_write_load()
```

### Comparing `libNeuroML-0.4.1/neuroml/test/test_hdf5_parser.py` & `libNeuroML-0.5.1/neuroml/test/test_hdf5_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 try:
     import unittest2 as unittest
 except ImportError:
     import unittest
 
 
 class TestNeuroMLHDF5Parser(unittest.TestCase):
-
     base_dir = os.path.dirname(__file__)
     # base_dir = '.'
 
     def test_write_load_hdf5(self):
         # for f in []:
         # for f in ['MediumNet.net.nml']:
         for f in ["simplenet.nml", "testh5.nml", "MediumNet.net.nml", "complete.nml"]:
@@ -66,10 +65,9 @@
         compare(summary0, summary1)
 
     def runTest(self):
         print("Running tests in TestNeuroMLHDF5Parser")
 
 
 if __name__ == "__main__":
-
     tnxp = TestNeuroMLHDF5Parser()
     tnxp.test_write_load_hdf5()
```

### Comparing `libNeuroML-0.4.1/neuroml/test/test_integration.py` & `libNeuroML-0.5.1/neuroml/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.4.1/neuroml/test/test_loaders.py` & `libNeuroML-0.5.1/neuroml/test/test_loaders.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.4.1/neuroml/test/test_morphology.py` & `libNeuroML-0.5.1/neuroml/test/test_morphology.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.4.1/neuroml/test/test_nml.py` & `libNeuroML-0.5.1/neuroml/test/test_nml.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 """
 Test nml.py functions/methods.
 
 File: neuroml/test/test_nml.py
 
-Copyright 2021 NeuroML contributors
+Copyright 2023 NeuroML contributors
 """
 
 try:
     import unittest2 as unittest
 except ImportError:
     import unittest
 
@@ -234,123 +234,149 @@
         print(cm.exception)
         nml_doc._check_arg_list(id="yep")
 
     def test_add_segment(self):
         """Test adding a segment."""
         new_cell = component_factory("Cell", id="test_cell")
         segment = new_cell.add_segment(
-            (0, 0, 0, 20), (20, 0, 0, 20), name="soma", group_id="soma_group",
-            seg_type="soma"
+            (0, 0, 0, 20),
+            (20, 0, 0, 20),
+            name="soma",
+            group_id="soma_group",
+            seg_type="soma",
         )
         self.assertIsInstance(segment, neuroml.Segment)
         self.assertEqual(segment.proximal.diameter, 20.0)
         self.assertEqual(segment.proximal.x, 0.0)
         self.assertEqual(segment.distal.diameter, 20.0)
         self.assertEqual(segment.distal.x, 20.0)
 
         self.assertIsNone(new_cell.validate(True))
 
     def test_add_segment_no_group(self):
         """Test adding a segment but without a group."""
         new_cell = component_factory("Cell", id="test_cell")
         segment = new_cell.add_segment(
-            (0, 0, 0, 20), (20, 0, 0, 20), name="soma", group_id=None,
-            seg_type="soma"
+            (0, 0, 0, 20), (20, 0, 0, 20), name="soma", group_id=None, seg_type="soma"
         )
         self.assertIsInstance(segment, neuroml.Segment)
         self.assertEqual(segment.proximal.diameter, 20.0)
         self.assertEqual(segment.proximal.x, 0.0)
         self.assertEqual(segment.distal.diameter, 20.0)
         self.assertEqual(segment.distal.x, 20.0)
 
         self.assertIsNone(new_cell.validate(True))
 
     def test_setting_init_memb_potential(self):
         """Test adding initial membrane potential."""
         new_cell = component_factory("Cell", id="test_cell")
         new_cell.add_segment(
-            (0, 0, 0, 20), (20, 0, 0, 20), name="soma", group_id="soma_group",
-            seg_type="soma"
+            (0, 0, 0, 20),
+            (20, 0, 0, 20),
+            name="soma",
+            group_id="soma_group",
+            seg_type="soma",
         )
         new_cell.set_init_memb_potential("-65mV")
 
         self.assertIsNone(new_cell.validate(True))
 
     def test_setting_spike_thresh(self):
         """Test adding spike threshold."""
         new_cell = component_factory("Cell", id="test_cell")
         new_cell.add_segment(
-            (0, 0, 0, 20), (20, 0, 0, 20), name="soma", group_id="soma_group",
-            seg_type="soma"
+            (0, 0, 0, 20),
+            (20, 0, 0, 20),
+            name="soma",
+            group_id="soma_group",
+            seg_type="soma",
         )
         new_cell.set_spike_thresh("40mV")
 
         self.assertIsNone(new_cell.validate(True))
 
     @unittest.expectedFailure
     def test_setting_init_memb_potential_should_fail(self):
         """Units of membrane potential are wrong: should fail."""
         new_cell = component_factory("Cell", id="test_cell")
         new_cell.add_segment(
-            (0, 0, 0, 20), (20, 0, 0, 20), name="soma", group_id="soma_group",
-            seg_type="soma"
+            (0, 0, 0, 20),
+            (20, 0, 0, 20),
+            name="soma",
+            group_id="soma_group",
+            seg_type="soma",
         )
         # Make it invalid: wrong dimensions for membrane potential
         new_cell.set_init_memb_potential(new_cell, "-65 cm")
 
         self.assertIsNone(new_cell.validate(True))
 
     def test_setting_resistivity(self):
         """Test setting the resistivity."""
         new_cell = component_factory("Cell", id="test_cell")
         new_cell.add_segment(
-            (0, 0, 0, 20), (20, 0, 0, 20), name="soma", group_id="soma_group",
-            seg_type="soma"
+            (0, 0, 0, 20),
+            (20, 0, 0, 20),
+            name="soma",
+            group_id="soma_group",
+            seg_type="soma",
         )
         new_cell.set_resistivity("2000 ohm_cm")
         self.assertIsNone(new_cell.validate(True))
 
     @unittest.expectedFailure
     def test_setting_resistivity_should_fail(self):
         """Test setting the resistivity."""
         new_cell = component_factory("Cell", id="test_cell")
         new_cell.add_segment(
-            (0, 0, 0, 20), (20, 0, 0, 20), name="soma", group_id="soma_group",
-            seg_type="soma"
+            (0, 0, 0, 20),
+            (20, 0, 0, 20),
+            name="soma",
+            group_id="soma_group",
+            seg_type="soma",
         )
         new_cell.set_resistivity("2000 kilO")
         self.assertIsNone(new_cell.validate(True))
 
     def test_setting_specific_capacitance(self):
         """Test setting the specific_capacitance."""
         new_cell = component_factory("Cell", id="test_cell")
         new_cell.add_segment(
-            (0, 0, 0, 20), (20, 0, 0, 20), name="soma", group_id="soma_group",
-            seg_type="soma"
+            (0, 0, 0, 20),
+            (20, 0, 0, 20),
+            name="soma",
+            group_id="soma_group",
+            seg_type="soma",
         )
         new_cell.set_specific_capacitance("1.0 uF_per_cm2")
         self.assertIsNone(new_cell.validate(True))
 
     @unittest.expectedFailure
     def test_setting_specific_capacitance_should_fail(self):
         """Test setting the specific_capacitance."""
         new_cell = component_factory("Cell", id="test_cell")
         new_cell.add_segment(
-            (0, 0, 0, 20), (20, 0, 0, 20), name="soma", group_id="soma_group",
-            seg_type="soma"
+            (0, 0, 0, 20),
+            (20, 0, 0, 20),
+            name="soma",
+            group_id="soma_group",
+            seg_type="soma",
         )
         new_cell.set_specific_capacitance("kilo")
         self.assertIsNone(new_cell.validate(True))
 
     def test_setting_channel_density(self):
         """Test setting the channel_density."""
         new_cell = component_factory("Cell", id="test_cell")
         new_cell.add_segment(
-            (0, 0, 0, 20), (20, 0, 0, 20), name="soma", group_id="soma_group",
-            seg_type="soma"
+            (0, 0, 0, 20),
+            (20, 0, 0, 20),
+            name="soma",
+            group_id="soma_group",
+            seg_type="soma",
         )
         nml_doc = component_factory(
             "NeuroMLDocument", id="test_cell_with_channel_density_doc"
         )
         nml_doc.cells.append(new_cell)
 
         nml_doc.add(
@@ -382,16 +408,19 @@
         )
         self.assertIsNone(nml_doc.validate(True))
 
     def test_setting_channel_density_v(self):
         """Test setting the channel_density."""
         new_cell = component_factory("Cell", id="test_cell")
         new_cell.add_segment(
-            (0, 0, 0, 20), (20, 0, 0, 20), name="soma", group_id="soma_group",
-            seg_type="soma"
+            (0, 0, 0, 20),
+            (20, 0, 0, 20),
+            name="soma",
+            group_id="soma_group",
+            seg_type="soma",
         )
         nml_doc = component_factory(
             "NeuroMLDocument", id="test_cell_with_channel_density_doc"
         )
         nml_doc.add(new_cell)
 
         nml_doc.add(
@@ -426,16 +455,19 @@
         self.assertIsNone(nml_doc.validate(True))
 
     @unittest.expectedFailure
     def test_setting_channel_density_should_fail(self):
         """Test setting the channel_density."""
         new_cell = component_factory("Cell", id="test_cell")
         new_cell.add_segment(
-            (0, 0, 0, 20), (20, 0, 0, 20), name="soma", group_id="soma_group",
-            seg_type="soma"
+            (0, 0, 0, 20),
+            (20, 0, 0, 20),
+            name="soma",
+            group_id="soma_group",
+            seg_type="soma",
         )
         nml_doc = component_factory(
             "NeuroMLDocument", id="test_cell_with_channel_density_doc"
         )
         nml_doc.add(new_cell)
 
         ion_chan = nml_doc.add(
@@ -455,16 +487,19 @@
         self.assertIsNone(new_cell.validate(True))
         self.assertIsNone(nml_doc.validate(True))
 
     def test_setting_membrane_property(self):
         """Test adding a new membrane property"""
         new_cell = component_factory("Cell", id="test_cell")
         new_cell.add_segment(
-            (0, 0, 0, 20), (20, 0, 0, 20), name="soma", group_id="soma_group",
-            seg_type="soma"
+            (0, 0, 0, 20),
+            (20, 0, 0, 20),
+            name="soma",
+            group_id="soma_group",
+            seg_type="soma",
         )
         new_cell.add_membrane_property("InitMembPotential", value="-65mV")
 
         self.assertEqual(
             new_cell.biophysical_properties.membrane_properties.init_memb_potentials[
                 0
             ].value,
@@ -473,16 +508,19 @@
 
         self.assertIsNone(new_cell.validate(True))
 
     def test_setting_intracellular_property(self):
         """Test adding a new membrane property"""
         new_cell = component_factory("Cell", id="test_cell")
         new_cell.add_segment(
-            (0, 0, 0, 20), (20, 0, 0, 20), name="soma", group_id="soma_group",
-            seg_type="soma"
+            (0, 0, 0, 20),
+            (20, 0, 0, 20),
+            name="soma",
+            group_id="soma_group",
+            seg_type="soma",
         )
         new_cell.add_intracellular_property(
             "Resistivity",
             value="0ohm_cm",
         )
 
         self.assertEqual(
@@ -503,15 +541,15 @@
         # Add soma segment
         diam = 10.0
         soma_0 = cell.add_segment(
             prox=[0.0, 0.0, 0.0, diam],
             dist=[0.0, 10.0, 0.0, diam],
             name="Seg0_soma_0",
             group_id="soma_0",
-            seg_type="soma"
+            seg_type="soma",
         )
 
         self.assertIsInstance(soma_0, neuroml.Segment)
 
         self.assertIsNone(cell.validate(True))
 
     def test_complex_cell(self):
@@ -523,25 +561,25 @@
         # Add soma segment
         diam = 30.0
         soma_0 = cell.add_segment(
             prox=[0.0, 0.0, 0.0, diam],
             dist=[0.0, 20.0, 0.0, diam],
             name="Seg0_soma_0",
             group_id="soma_0",
-            seg_type="soma"
+            seg_type="soma",
         )
         self.assertIsInstance(soma_0, neuroml.Segment)
 
         dend_0 = cell.add_segment(
             prox=[soma_0.distal.x, soma_0.distal.y, soma_0.distal.z, 5],
             dist=[soma_0.distal.x, soma_0.distal.y + 50, soma_0.distal.z, 2],
             name="dend_0",
             group_id="dend_0",
             parent=soma_0,
-            seg_type="soma"
+            seg_type="soma",
         )
         self.assertIsInstance(dend_0, neuroml.Segment)
 
         self.assertIsNone(cell.validate(True))
 
     def test_component_factory_create_cell(self):
         """Test cell creation"""
@@ -561,67 +599,70 @@
         # Add soma segment
         diam = 10.0
         soma_0 = cell.add_segment(
             prox=[0.0, 0.0, 0.0, diam],
             dist=[0.0, 10.0, 0.0, diam],
             name="Seg0_soma_0",
             group_id="soma_0",
-            seg_type="soma"
+            seg_type="soma",
         )
 
         dend_group = cell.add_unbranched_segments(
             points=[
                 [0.0, 10.0, 0.0, diam],
                 [0.0, 20.0, 0.0, diam],
                 [0.0, 30.0, 0.0, diam],
             ],
             parent=soma_0,
             fraction_along=1.0,
             group_id="dend_group_0",
             use_convention=True,
-            seg_type="dendrite"
+            seg_type="dendrite",
         )
 
         self.assertIsInstance(dend_group, neuroml.SegmentGroup)
 
         self.assertIsNone(cell.validate(True))
         self.assertEqual(3, len(cell.morphology.segments))
 
         cell.summary()
 
     def test_optimise_segment_group(self):
-        """Test `optimise_segment_group`
-        """
+        """Test `optimise_segment_group`"""
         cell = component_factory("Cell", id="simple_cell")  # type: neuroml.Cell
         cell.notes = "NeuroML cell created by CellBuilder"
 
         # Add soma segment
         diam = 10.0
         soma_0 = cell.add_segment(
             prox=[0.0, 0.0, 0.0, diam],
             dist=[0.0, 10.0, 0.0, diam],
             name="Seg0_soma_0",
             group_id="soma_0",
-            seg_type="soma"
+            seg_type="soma",
         )
 
         # add the segment again to all group
-        cell.get_segment_group("all").members.append(cell.component_factory(neuroml.Member,
-                                                     segments=cell.get_segment_group("soma_0").members[0].segments))
+        cell.get_segment_group("all").members.append(
+            cell.component_factory(
+                neuroml.Member,
+                segments=cell.get_segment_group("soma_0").members[0].segments,
+            )
+        )
 
         # add group to all, explicitly
-        cell.get_segment_group("all").add(neuroml.Include,
-                                          segment_groups="soma_0",
-                                          force=True)
-        cell.get_segment_group("all").add(neuroml.Include,
-                                          segment_groups="soma_0",
-                                          force=True)
-        cell.get_segment_group("all").add(neuroml.Include,
-                                          segment_groups="soma_0",
-                                          force=True)
+        cell.get_segment_group("all").add(
+            neuroml.Include, segment_groups="soma_0", force=True
+        )
+        cell.get_segment_group("all").add(
+            neuroml.Include, segment_groups="soma_0", force=True
+        )
+        cell.get_segment_group("all").add(
+            neuroml.Include, segment_groups="soma_0", force=True
+        )
         self.assertEqual(4, len(cell.get_segment_group("all").includes))
         # should have only one included segment group
         # should have no segments, because the segment is included in the one
         # segment group already
         cell.optimise_segment_group("all")
         self.assertEqual(1, len(cell.get_segment_group("all").includes))
 
@@ -633,47 +674,49 @@
         # Add soma segment
         diam = 10.0
         soma_0 = cell.add_segment(
             prox=[0.0, 0.0, 0.0, diam],
             dist=[0.0, 10.0, 0.0, diam],
             name="Seg0_soma_0",
             group_id="soma_0",
-            seg_type="soma"
+            seg_type="soma",
         )
 
         # create two unbranched segment group
         dend_group = cell.add_unbranched_segments(
             points=[
                 [0.0, 10.0, 0.0, diam],
                 [0.0, 20.0, 0.0, diam],
                 [0.0, 30.0, 0.0, diam],
             ],
             parent=soma_0,
             fraction_along=1.0,
             group_id="dend_group_0",
             use_convention=True,
-            seg_type="dendrite"
+            seg_type="dendrite",
         )
         dend_group_1 = cell.add_unbranched_segments(
             points=[
                 [0.0, 10.0, 0.0, diam],
                 [0.0, 20.0, 5.0, diam],
                 [0.0, 30.0, 5.0, diam],
             ],
             parent=soma_0,
             fraction_along=1.0,
             group_id="dend_group_1",
             use_convention=True,
-            seg_type="dendrite"
+            seg_type="dendrite",
         )
         cell.optimise_segment_groups()
 
         self.assertIsNone(cell.validate(True))
         self.assertEqual(5, len(cell.morphology.segments))
-        self.assertEqual(7, len(cell.morphology.segment_groups))
+        # all, dend_group_1, dend_group_0, soma_0, and dendrite_group,
+        # soma_group
+        self.assertEqual(6, len(cell.morphology.segment_groups))
         print("initial")
         for g in cell.morphology.segment_groups:
             print(g)
             print([x.segments for x in g.members])
 
         # remove the two unbranched groups
         cell.morphology.segment_groups.remove(cell.get_segment_group("soma_0"))
@@ -686,7 +729,36 @@
 
         # create the unbranched segments
         cell.create_unbranched_segment_group_branches(soma_0.id)
         print("after re-creation")
         for g in cell.morphology.segment_groups:
             print(g)
             print([x.segments for x in g.members])
+
+    def test_morphinfo(self):
+        """Test the morphinfo method"""
+        # with component_factory
+        cell = component_factory("Cell", id="complex_cell")  # type: neuroml.Cell
+        cell.notes = "NeuroML cell created by CellBuilder"
+
+        # Add soma segment
+        diam = 30.0
+        soma_0 = cell.add_segment(
+            prox=[0.0, 0.0, 0.0, diam],
+            dist=[0.0, 20.0, 0.0, diam],
+            name="Seg0_soma_0",
+            group_id="soma_0",
+            seg_type="soma",
+        )
+        self.assertIsInstance(soma_0, neuroml.Segment)
+
+        dend_0 = cell.add_segment(
+            prox=[soma_0.distal.x, soma_0.distal.y, soma_0.distal.z, 5],
+            dist=[soma_0.distal.x, soma_0.distal.y + 50, soma_0.distal.z, 2],
+            name="dend_0",
+            group_id="dend_0",
+            parent=soma_0,
+            seg_type="soma",
+        )
+
+        cell.morphinfo(True)
+        cell.biophysinfo()
```

### Comparing `libNeuroML-0.4.1/neuroml/test/test_segment.py` & `libNeuroML-0.5.1/neuroml/test/test_segment.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,25 +97,23 @@
         p = Point3DWithDiam(x=0.5, y=2.0, z=1.8, diameter=0.9)
 
         seg = Segment(proximal=p, distal=d)
 
         self.assertAlmostEqual(seg.surface_area, 4.19011944, places=7)
 
     def test_volume0(self):
-
         diam = 1.0
         len = 1.0
         d = Point3DWithDiam(x=0, y=0, z=0, diameter=diam)
         p = Point3DWithDiam(x=0, y=len, z=0, diameter=diam)
         seg = Segment(proximal=p, distal=d)
 
         self.assertAlmostEqual(seg.volume, math.pi * (diam / 2) ** 2 * len, places=7)
 
     def test_volume1(self):
-
         diam = 1.0
         len = 1.0
         d = Point3DWithDiam(x=0, y=0, z=0, diameter=diam)
         p = Point3DWithDiam(x=0, y=len, z=0, diameter=diam * 1.01)
         seg = Segment(proximal=p, distal=d)
 
         self.assertAlmostEqual(seg.volume, 0.793278324, places=7)
@@ -124,26 +122,24 @@
         d = Point3DWithDiam(x=0.2, y=2.4, z=3.5, diameter=0.6)
         p = Point3DWithDiam(x=0.5, y=2.0, z=1.8, diameter=0.9)
         seg = Segment(proximal=p, distal=d)
 
         self.assertAlmostEqual(seg.volume, 0.7932855820702964, places=7)
 
     def test_spherical(self):
-
         diam = 1.0
         d = Point3DWithDiam(x=0, y=0, z=0, diameter=diam)
         p = Point3DWithDiam(x=0, y=0, z=0, diameter=diam)
 
         seg = Segment(id=0, proximal=p, distal=d)
 
         self.assertEqual(seg.length, 0)
         self.assertEqual(seg.surface_area, math.pi)
 
     def test_cell_with_segs(self):
-
         cell = Cell(id="cell0")
 
         diam = 1.0
         d0 = Point3DWithDiam(x=0, y=0, z=0, diameter=diam)
         p = Point3DWithDiam(x=0, y=0, z=0, diameter=diam)
 
         seg0 = Segment(id=0, proximal=p, distal=d0)
@@ -225,15 +221,14 @@
 
 
 class TestAttachedSegments(unittest.TestCase):
     pass
 
 
 if __name__ == "__main__":
-
     ta = TestHelperProperties()
 
     ta.test_length0()
     ta.test_length()
 
     ta.test_area0()
     ta.test_area1()
```

### Comparing `libNeuroML-0.4.1/neuroml/test/test_utils.py` & `libNeuroML-0.5.1/neuroml/test/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 """
 Test utilities
 
 File: neuroml/test/test_utils.py
 
-Copyright 2022 NeuroML contributors
+Copyright 2023 NeuroML contributors
 """
 
 import neuroml
 from neuroml.utils import component_factory
 import unittest
 import tempfile
```

### Comparing `libNeuroML-0.4.1/neuroml/test/test_writers.py` & `libNeuroML-0.5.1/neuroml/test/test_writers.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.4.1/neuroml/test/test_xml_parser.py` & `libNeuroML-0.5.1/neuroml/test/test_xml_parser.py`

 * *Files identical despite different names*

### Comparing `libNeuroML-0.4.1/neuroml/utils.py` & `libNeuroML-0.5.1/neuroml/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,14 @@
     """
     membs = inspect.getmembers(nml_doc_src)
 
     for memb in membs:
         if isinstance(memb[1], list) and len(memb[1]) > 0 and not memb[0].endswith("_"):
             for entry in memb[1]:
                 if memb[0] != "includes":
-
                     added = False
                     for c in getattr(nml_doc_tgt, memb[0]):
                         if hasattr(c, "id") and c.id == entry.id:
                             added = True
                     if not added:
                         # print("  Adding %s to list: %s" \
                         #    %(entry.id if hasattr(entry,'id') else entry.name, memb[0]))
```

### Comparing `libNeuroML-0.4.1/neuroml/writers.py` & `libNeuroML-0.5.1/neuroml/writers.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         if close:
             file.close()
 
 
 class NeuroMLHdf5Writer(object):
     @classmethod
     def write(cls, nml_doc, h5_file_name, embed_xml=True, compress=True):
-
         import tables
 
         FILTERS = (
             tables.Filters(complib="zlib", complevel=5)
             if compress
             else tables.Filters()
         )
@@ -53,19 +52,17 @@
         rootGroup = h5file.create_group("/", "neuroml", "Root NeuroML group")
 
         rootGroup._f_setattr("id", nml_doc.id)
         rootGroup._f_setattr("notes", nml_doc.notes)
         rootGroup._f_setattr("GENERATED_BY", "libNeuroML v%s" % (neuroml.__version__))
 
         for network in nml_doc.networks:
-
             network.exportHdf5(h5file, rootGroup)
 
         if embed_xml:
-
             networks = []
             for n in nml_doc.networks:
                 networks.append(n)
 
             nml_doc.networks = []
 
             try:
@@ -163,23 +160,21 @@
                 morphology.id = "Morphology" + str(default_id)
             if cell.id == None:
                 cell.id = "Cell" + str(default_id)
 
             cls.__write_single_cell(morphology, fileh, cell_id=cell.id)
 
         for default_id, morphology in enumerate(document.morphology):
-
             if morphology.id == None:
                 morphology.id = "Morphology" + str(default_id)
 
             cls.__write_single_cell(morphology, fileh, cell_id=cell.id)
 
     @classmethod
     def write(cls, data, filepath):
-
         import tables
 
         fileh = tables.open_file(filepath, mode="w")
 
         # Now instead we should go through a document/cell/morphology
         # hierarchy - this kind of tree traversal should be done recursively
```

### Comparing `libNeuroML-0.4.1/setup.py` & `libNeuroML-0.5.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     packages=["neuroml", "neuroml.test", "neuroml.nml", "neuroml.hdf5"],
     package_data={"neuroml.test": ["*.nml"], "neuroml.nml": ["*.xsd"]},
     author="libNeuroML authors and contributors",
     author_email="vellamike@gmail.com, p.gleeson@gmail.com",
     description="A Python library for working with NeuroML descriptions of neuronal models",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=["lxml", "six"],
+    install_requires=["lxml", "six", "networkx"],
     tests_require=["pytest"],
     extras_require={
         "full": [
             "cython",
             "numpy",
             "numexpr",
             "tables>=3.3.0",
@@ -37,11 +37,12 @@
         "Operating System :: OS Independent",
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "Topic :: Scientific/Engineering",
     ],
 )
```

