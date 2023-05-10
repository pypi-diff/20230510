# Comparing `tmp/cbcflow-0.1.2a6.tar.gz` & `tmp/cbcflow-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcflow-0.1.2a6.tar", last modified: Tue Apr 18 14:12:07 2023, max compression
+gzip compressed data, was "cbcflow-0.2.1.tar", last modified: Wed May 10 10:09:15 2023, max compression
```

## Comparing `cbcflow-0.1.2a6.tar` & `cbcflow-0.2.1.tar`

### file list

```diff
@@ -1,109 +1,114 @@
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.878687 cbcflow-0.1.2a6/
--rw-r--r--   0 greg      (1000) greg      (1000)       37 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/.gitattributes
--rw-r--r--   0 greg      (1000) greg      (1000)      217 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/.gitignore
--rw-r--r--   0 greg      (1000) greg      (1000)     1533 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/.gitlab-ci.yml
--rw-r--r--   0 greg      (1000) greg      (1000)      873 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/.pre-commit-config.yaml
--rw-r--r--   0 greg      (1000) greg      (1000)      405 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/CHANGELOG.md
--rw-r--r--   0 greg      (1000) greg      (1000)     1084 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/LICENSE.md
--rw-r--r--   0 greg      (1000) greg      (1000)      123 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/MANIFEST.in
--rw-r--r--   0 greg      (1000) greg      (1000)     3039 2023-04-18 14:12:07.878687 cbcflow-0.1.2a6/PKG-INFO
--rw-r--r--   0 greg      (1000) greg      (1000)     2394 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/README.md
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.824520 cbcflow-0.1.2a6/docs/
--rw-r--r--   0 greg      (1000) greg      (1000)      613 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/Makefile
--rw-r--r--   0 greg      (1000) greg      (1000)       53 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/requirements.txt
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.846187 cbcflow-0.1.2a6/docs/source/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.846187 cbcflow-0.1.2a6/docs/source/_templates/
--rw-r--r--   0 greg      (1000) greg      (1000)      662 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/_templates/custom-class-template.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1408 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/_templates/custom-module-template.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1158 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/actionitems.rst
--rw-r--r--   0 greg      (1000) greg      (1000)      690 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/adding-to-the-schema.rst
--rw-r--r--   0 greg      (1000) greg      (1000)       39 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/asimov.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     2616 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/conf.py
--rw-r--r--   0 greg      (1000) greg      (1000)     1770 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/configuration.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1444 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/development-setup.rst
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.846187 cbcflow-0.1.2a6/docs/source/example_mini_schema/
--rw-r--r--   0 greg      (1000) greg      (1000)     2924 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/example_mini_schema/example.schema
--rw-r--r--   0 greg      (1000) greg      (1000)     6391 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/example_mini_schema/schema_doc.css
--rw-r--r--   0 greg      (1000) greg      (1000)    27212 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/example_mini_schema/schema_doc.html
--rw-r--r--   0 greg      (1000) greg      (1000)      984 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/example_mini_schema/schema_doc.min.js
--rw-r--r--   0 greg      (1000) greg      (1000)      458 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/gwosc.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1191 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/index.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     2799 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/libraries.rst
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.857020 cbcflow-0.1.2a6/docs/source/libraries_images/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.857020 cbcflow-0.1.2a6/docs/source/libraries_images/.ipynb_checkpoints/
--rw-r--r--   0 greg      (1000) greg      (1000)    72683 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png
--rw-r--r--   0 greg      (1000) greg      (1000)     8993 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/libraries_images/part_1.png
--rw-r--r--   0 greg      (1000) greg      (1000)    15966 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/libraries_images/part_2.png
--rw-r--r--   0 greg      (1000) greg      (1000)    38016 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/libraries_images/part_3.png
--rw-r--r--   0 greg      (1000) greg      (1000)    51488 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/libraries_images/part_4.png
--rw-r--r--   0 greg      (1000) greg      (1000)    41435 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/libraries_images/part_5.png
--rw-r--r--   0 greg      (1000) greg      (1000)    54941 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/libraries_images/part_6.png
--rw-r--r--   0 greg      (1000) greg      (1000)    67345 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/libraries_images/part_7.png
--rw-r--r--   0 greg      (1000) greg      (1000)    72180 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/libraries_images/part_8.png
--rw-r--r--   0 greg      (1000) greg      (1000)    10255 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/library-index-labelling.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1358 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/library-indices.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1960 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/library-setup.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1782 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/monitor-usage.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     4809 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/reading-the-schema.rst
--rw-r--r--   0 greg      (1000) greg      (1000)      106 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/docs/source/schema-visualization.rst
--rw-r--r--   0 greg      (1000) greg      (1000)    15476 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/updating-metadata-from-the-command-line.rst
--rw-r--r--   0 greg      (1000) greg      (1000)    12152 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/updating-metadata-with-the-python-api.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     4916 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/docs/source/what-is-metadata.rst
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.857020 cbcflow-0.1.2a6/examples/
--rw-r--r--   0 greg      (1000) greg      (1000)     7368 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/examples/initial_example.md
--rw-r--r--   0 greg      (1000) greg      (1000)      860 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/pyproject.toml
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.857020 cbcflow-0.1.2a6/schema/
--rw-r--r--   0 greg      (1000) greg      (1000)    40294 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/schema/cbc-meta-data-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)    88906 2023-04-18 14:11:16.000000 cbcflow-0.1.2a6/schema/cbc-meta-data-v2.schema
--rwxr-xr-x   0 greg      (1000) greg      (1000)     1768 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/schema/index-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)     1503 2023-04-18 14:12:07.878687 cbcflow-0.1.2a6/setup.cfg
--rw-r--r--   0 greg      (1000) greg      (1000)      567 2023-04-13 22:38:42.000000 cbcflow-0.1.2a6/setup.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.813687 cbcflow-0.1.2a6/src/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.867854 cbcflow-0.1.2a6/src/cbcflow/
--rw-r--r--   0 greg      (1000) greg      (1000)     1426 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/src/cbcflow/__init__.py
--rw-r--r--   0 greg      (1000) greg      (1000)      162 2023-04-18 14:12:07.000000 cbcflow-0.1.2a6/src/cbcflow/_version.py
--rw-r--r--   0 greg      (1000) greg      (1000)    12824 2023-04-18 14:11:16.000000 cbcflow-0.1.2a6/src/cbcflow/asimov.py
--rwxr-xr-x   0 greg      (1000) greg      (1000)     7347 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/src/cbcflow/cbcflow.py
--rw-r--r--   0 greg      (1000) greg      (1000)     1325 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/src/cbcflow/configuration.py
--rw-r--r--   0 greg      (1000) greg      (1000)    29553 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/src/cbcflow/database.py
--rw-r--r--   0 greg      (1000) greg      (1000)     9226 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/src/cbcflow/gracedb.py
--rw-r--r--   0 greg      (1000) greg      (1000)    13615 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/src/cbcflow/metadata.py
--rw-r--r--   0 greg      (1000) greg      (1000)     4757 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/src/cbcflow/monitor.py
--rw-r--r--   0 greg      (1000) greg      (1000)     7734 2023-04-18 03:41:18.000000 cbcflow-0.1.2a6/src/cbcflow/parser.py
--rw-r--r--   0 greg      (1000) greg      (1000)    20427 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/src/cbcflow/process.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.867854 cbcflow-0.1.2a6/src/cbcflow/schema/
--rw-r--r--   0 greg      (1000) greg      (1000)    40294 2023-04-18 14:12:07.000000 cbcflow-0.1.2a6/src/cbcflow/schema/cbc-meta-data-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)    88906 2023-04-18 14:12:07.000000 cbcflow-0.1.2a6/src/cbcflow/schema/cbc-meta-data-v2.schema
--rwxr-xr-x   0 greg      (1000) greg      (1000)     1768 2023-04-18 14:12:07.000000 cbcflow-0.1.2a6/src/cbcflow/schema/index-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)     2750 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/src/cbcflow/schema.py
--rw-r--r--   0 greg      (1000) greg      (1000)     5044 2023-04-18 14:11:05.000000 cbcflow-0.1.2a6/src/cbcflow/utils.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.867854 cbcflow-0.1.2a6/src/cbcflow.egg-info/
--rw-r--r--   0 greg      (1000) greg      (1000)     3039 2023-04-18 14:12:07.000000 cbcflow-0.1.2a6/src/cbcflow.egg-info/PKG-INFO
--rw-r--r--   0 greg      (1000) greg      (1000)     3082 2023-04-18 14:12:07.000000 cbcflow-0.1.2a6/src/cbcflow.egg-info/SOURCES.txt
--rw-r--r--   0 greg      (1000) greg      (1000)        1 2023-04-18 14:12:07.000000 cbcflow-0.1.2a6/src/cbcflow.egg-info/dependency_links.txt
--rw-r--r--   0 greg      (1000) greg      (1000)      481 2023-04-18 14:12:07.000000 cbcflow-0.1.2a6/src/cbcflow.egg-info/entry_points.txt
--rw-r--r--   0 greg      (1000) greg      (1000)      115 2023-04-18 14:12:07.000000 cbcflow-0.1.2a6/src/cbcflow.egg-info/requires.txt
--rw-r--r--   0 greg      (1000) greg      (1000)        8 2023-04-18 14:12:07.000000 cbcflow-0.1.2a6/src/cbcflow.egg-info/top_level.txt
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.867854 cbcflow-0.1.2a6/tests/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.878687 cbcflow-0.1.2a6/tests/files_for_testing/
--rw-r--r--   0 greg      (1000) greg      (1000)    26759 2023-04-04 20:38:56.000000 cbcflow-0.1.2a6/tests/files_for_testing/cbc-meta-data-example.json
--rw-r--r--   0 greg      (1000) greg      (1000)       56 2023-04-04 20:38:56.000000 cbcflow-0.1.2a6/tests/files_for_testing/test-file-for-linking-1.txt
--rw-r--r--   0 greg      (1000) greg      (1000)       86 2023-04-04 20:38:56.000000 cbcflow-0.1.2a6/tests/files_for_testing/test-file-for-linking-2.txt
--rw-r--r--   0 greg      (1000) greg      (1000)     3091 2023-04-04 20:38:56.000000 cbcflow-0.1.2a6/tests/files_for_testing/update_json_1.json
--rw-r--r--   0 greg      (1000) greg      (1000)     1221 2023-04-04 20:38:56.000000 cbcflow-0.1.2a6/tests/files_for_testing/update_json_2.json
--rw-r--r--   0 greg      (1000) greg      (1000)     1626 2023-04-04 20:38:56.000000 cbcflow-0.1.2a6/tests/files_for_testing/update_yaml_1.yaml
--rw-r--r--   0 greg      (1000) greg      (1000)      571 2023-04-04 20:38:56.000000 cbcflow-0.1.2a6/tests/files_for_testing/update_yaml_2.yaml
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 14:12:07.878687 cbcflow-0.1.2a6/tests/library_for_testing/
--rw-r--r--   0 greg      (1000) greg      (1000)     5338 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/tests/library_for_testing/S230227hp-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     4289 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/tests/library_for_testing/S230331e-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     4275 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/tests/library_for_testing/S230401h-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     2416 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/tests/library_for_testing/S230402dv-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     3353 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/tests/library_for_testing/S230403ae-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     5238 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/tests/library_for_testing/S230404hb-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     3256 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/tests/library_for_testing/S230404jc-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)      193 2023-04-04 20:38:56.000000 cbcflow-0.1.2a6/tests/library_for_testing/library.cfg
--rw-r--r--   0 greg      (1000) greg      (1000)       90 2023-04-04 20:38:56.000000 cbcflow-0.1.2a6/tests/library_for_testing/testing-library-index.json
--rw-r--r--   0 greg      (1000) greg      (1000)     1840 2023-04-13 21:35:01.000000 cbcflow-0.1.2a6/tests/test_database.py
--rw-r--r--   0 greg      (1000) greg      (1000)    23461 2023-04-04 20:38:56.000000 cbcflow-0.1.2a6/tests/test_metadata.py
--rw-r--r--   0 greg      (1000) greg      (1000)    23461 2023-04-13 22:03:31.000000 cbcflow-0.1.2a6/tests/test_parser.py
--rw-r--r--   0 greg      (1000) greg      (1000)      755 2023-04-04 15:21:01.000000 cbcflow-0.1.2a6/tests/test_schema.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.622659 cbcflow-0.2.1/
+-rw-r--r--   0 greg      (1000) greg      (1000)       37 2023-04-21 10:34:59.000000 cbcflow-0.2.1/.gitattributes
+-rw-r--r--   0 greg      (1000) greg      (1000)      217 2023-04-21 10:34:59.000000 cbcflow-0.2.1/.gitignore
+-rw-r--r--   0 greg      (1000) greg      (1000)     1533 2023-04-21 10:34:59.000000 cbcflow-0.2.1/.gitlab-ci.yml
+-rw-r--r--   0 greg      (1000) greg      (1000)      873 2023-04-21 10:34:59.000000 cbcflow-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 greg      (1000) greg      (1000)     1010 2023-05-10 10:07:05.000000 cbcflow-0.2.1/CHANGELOG.md
+-rw-r--r--   0 greg      (1000) greg      (1000)     1084 2023-04-21 10:34:59.000000 cbcflow-0.2.1/LICENSE.md
+-rw-r--r--   0 greg      (1000) greg      (1000)      123 2023-04-21 10:34:59.000000 cbcflow-0.2.1/MANIFEST.in
+-rw-r--r--   0 greg      (1000) greg      (1000)     3027 2023-05-10 10:09:15.622659 cbcflow-0.2.1/PKG-INFO
+-rw-r--r--   0 greg      (1000) greg      (1000)     2390 2023-04-21 14:02:43.000000 cbcflow-0.2.1/README.md
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.592659 cbcflow-0.2.1/docs/
+-rw-r--r--   0 greg      (1000) greg      (1000)      613 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/Makefile
+-rw-r--r--   0 greg      (1000) greg      (1000)       53 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/requirements.txt
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.602659 cbcflow-0.2.1/docs/source/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.602659 cbcflow-0.2.1/docs/source/_templates/
+-rw-r--r--   0 greg      (1000) greg      (1000)      662 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/_templates/custom-class-template.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1408 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/_templates/custom-module-template.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1158 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/actionitems.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)      690 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/adding-to-the-schema.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)       39 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/asimov.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     4404 2023-05-10 08:29:20.000000 cbcflow-0.2.1/docs/source/cbcflow-git-merging.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     2616 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/conf.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     1770 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/configuration.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1444 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/development-setup.rst
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.602659 cbcflow-0.2.1/docs/source/example_mini_schema/
+-rw-r--r--   0 greg      (1000) greg      (1000)     2924 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/example_mini_schema/example.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)     6391 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/example_mini_schema/schema_doc.css
+-rw-r--r--   0 greg      (1000) greg      (1000)    27212 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/example_mini_schema/schema_doc.html
+-rw-r--r--   0 greg      (1000) greg      (1000)      984 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/example_mini_schema/schema_doc.min.js
+-rw-r--r--   0 greg      (1000) greg      (1000)      458 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/gwosc.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1255 2023-05-10 08:29:20.000000 cbcflow-0.2.1/docs/source/index.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     2799 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/libraries.rst
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.602659 cbcflow-0.2.1/docs/source/libraries_images/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.602659 cbcflow-0.2.1/docs/source/libraries_images/.ipynb_checkpoints/
+-rw-r--r--   0 greg      (1000) greg      (1000)    72683 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png
+-rw-r--r--   0 greg      (1000) greg      (1000)     8993 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/libraries_images/part_1.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    15966 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/libraries_images/part_2.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    38016 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/libraries_images/part_3.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    51488 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/libraries_images/part_4.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    41435 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/libraries_images/part_5.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    54941 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/libraries_images/part_6.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    67345 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/libraries_images/part_7.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    72180 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/libraries_images/part_8.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    10255 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/library-index-labelling.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1352 2023-05-10 10:03:05.000000 cbcflow-0.2.1/docs/source/library-indices.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     3620 2023-05-10 08:29:20.000000 cbcflow-0.2.1/docs/source/library-setup-from-scratch.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1287 2023-05-10 08:29:20.000000 cbcflow-0.2.1/docs/source/local-library-copy-setup.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1782 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/monitor-usage.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     4809 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/reading-the-schema.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)      106 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/schema-visualization.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)    15476 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/updating-metadata-from-the-command-line.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)    12152 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/updating-metadata-with-the-python-api.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     4916 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/what-is-metadata.rst
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.602659 cbcflow-0.2.1/examples/
+-rw-r--r--   0 greg      (1000) greg      (1000)     7368 2023-04-21 10:34:59.000000 cbcflow-0.2.1/examples/initial_example.md
+-rw-r--r--   0 greg      (1000) greg      (1000)      856 2023-04-21 14:02:43.000000 cbcflow-0.2.1/pyproject.toml
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.602659 cbcflow-0.2.1/schema/
+-rw-r--r--   0 greg      (1000) greg      (1000)    40294 2023-04-21 10:34:59.000000 cbcflow-0.2.1/schema/cbc-meta-data-v1.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)    88906 2023-04-24 13:44:33.000000 cbcflow-0.2.1/schema/cbc-meta-data-v2.schema
+-rwxr-xr-x   0 greg      (1000) greg      (1000)     1766 2023-05-10 10:03:05.000000 cbcflow-0.2.1/schema/index-v1.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)     1635 2023-05-10 10:09:15.622659 cbcflow-0.2.1/setup.cfg
+-rw-r--r--   0 greg      (1000) greg      (1000)      567 2023-04-21 10:34:59.000000 cbcflow-0.2.1/setup.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.592659 cbcflow-0.2.1/src/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.612659 cbcflow-0.2.1/src/cbcflow/
+-rw-r--r--   0 greg      (1000) greg      (1000)     1462 2023-04-24 14:06:13.000000 cbcflow-0.2.1/src/cbcflow/__init__.py
+-rw-r--r--   0 greg      (1000) greg      (1000)      160 2023-05-10 10:09:15.000000 cbcflow-0.2.1/src/cbcflow/_version.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    14041 2023-05-10 08:29:20.000000 cbcflow-0.2.1/src/cbcflow/asimov.py
+-rwxr-xr-x   0 greg      (1000) greg      (1000)     9343 2023-05-10 10:03:05.000000 cbcflow-0.2.1/src/cbcflow/cbcflow.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     1330 2023-04-24 14:06:13.000000 cbcflow-0.2.1/src/cbcflow/configuration.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    37157 2023-05-10 10:03:05.000000 cbcflow-0.2.1/src/cbcflow/database.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    14125 2023-05-10 10:03:05.000000 cbcflow-0.2.1/src/cbcflow/gracedb.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    14413 2023-05-10 10:03:05.000000 cbcflow-0.2.1/src/cbcflow/metadata.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     6270 2023-05-10 08:29:20.000000 cbcflow-0.2.1/src/cbcflow/monitor.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     5096 2023-05-10 10:03:05.000000 cbcflow-0.2.1/src/cbcflow/online_pe.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     8049 2023-05-10 08:29:20.000000 cbcflow-0.2.1/src/cbcflow/parser.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    35849 2023-05-10 10:03:05.000000 cbcflow-0.2.1/src/cbcflow/process.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.612659 cbcflow-0.2.1/src/cbcflow/schema/
+-rw-r--r--   0 greg      (1000) greg      (1000)    40294 2023-05-10 10:09:15.000000 cbcflow-0.2.1/src/cbcflow/schema/cbc-meta-data-v1.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)    88906 2023-05-10 10:09:15.000000 cbcflow-0.2.1/src/cbcflow/schema/cbc-meta-data-v2.schema
+-rwxr-xr-x   0 greg      (1000) greg      (1000)     1766 2023-05-10 10:09:15.000000 cbcflow-0.2.1/src/cbcflow/schema/index-v1.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)     2779 2023-04-24 14:06:13.000000 cbcflow-0.2.1/src/cbcflow/schema.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     7294 2023-05-10 08:29:20.000000 cbcflow-0.2.1/src/cbcflow/utils.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.612659 cbcflow-0.2.1/src/cbcflow.egg-info/
+-rw-r--r--   0 greg      (1000) greg      (1000)     3027 2023-05-10 10:09:15.000000 cbcflow-0.2.1/src/cbcflow.egg-info/PKG-INFO
+-rw-r--r--   0 greg      (1000) greg      (1000)     3290 2023-05-10 10:09:15.000000 cbcflow-0.2.1/src/cbcflow.egg-info/SOURCES.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)        1 2023-05-10 10:09:15.000000 cbcflow-0.2.1/src/cbcflow.egg-info/dependency_links.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)      599 2023-05-10 10:09:15.000000 cbcflow-0.2.1/src/cbcflow.egg-info/entry_points.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)      130 2023-05-10 10:09:15.000000 cbcflow-0.2.1/src/cbcflow.egg-info/requires.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)        8 2023-05-10 10:09:15.000000 cbcflow-0.2.1/src/cbcflow.egg-info/top_level.txt
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.612659 cbcflow-0.2.1/tests/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.622659 cbcflow-0.2.1/tests/files_for_testing/
+-rw-r--r--   0 greg      (1000) greg      (1000)    26759 2023-04-21 10:34:59.000000 cbcflow-0.2.1/tests/files_for_testing/cbc-meta-data-example.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     5972 2023-05-10 08:29:20.000000 cbcflow-0.2.1/tests/files_for_testing/merge_test.json
+-rw-r--r--   0 greg      (1000) greg      (1000)       56 2023-04-21 10:34:59.000000 cbcflow-0.2.1/tests/files_for_testing/test-file-for-linking-1.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)       86 2023-04-21 10:34:59.000000 cbcflow-0.2.1/tests/files_for_testing/test-file-for-linking-2.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)       53 2023-05-10 08:29:20.000000 cbcflow-0.2.1/tests/files_for_testing/test-file-for-linking-3.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)     3091 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/files_for_testing/update_json_1.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     1221 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/files_for_testing/update_json_2.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     1626 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/files_for_testing/update_yaml_1.yaml
+-rw-r--r--   0 greg      (1000) greg      (1000)      571 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/files_for_testing/update_yaml_2.yaml
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.622659 cbcflow-0.2.1/tests/library_for_testing/
+-rw-r--r--   0 greg      (1000) greg      (1000)     5338 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/library_for_testing/S230227hp-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     4289 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/library_for_testing/S230331e-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     4275 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/library_for_testing/S230401h-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     2416 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/library_for_testing/S230402dv-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     3353 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/library_for_testing/S230403ae-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     5238 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/library_for_testing/S230404hb-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     3256 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/library_for_testing/S230404jc-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)      193 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/library_for_testing/library.cfg
+-rw-r--r--   0 greg      (1000) greg      (1000)       90 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/library_for_testing/testing-library-index.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     1838 2023-05-10 10:03:05.000000 cbcflow-0.2.1/tests/test_database.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    38496 2023-05-10 08:29:20.000000 cbcflow-0.2.1/tests/test_merging.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    23545 2023-05-10 08:29:20.000000 cbcflow-0.2.1/tests/test_metadata.py
+-rw-r--r--   0 greg      (1000) greg      (1000)      755 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/test_schema.py
```

### Comparing `cbcflow-0.1.2a6/.gitlab-ci.yml` & `cbcflow-0.2.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/.pre-commit-config.yaml` & `cbcflow-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/LICENSE.md` & `cbcflow-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/PKG-INFO` & `cbcflow-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: cbcflow
-Version: 0.1.2a6
+Version: 0.2.1
 Summary: A package for enabling CBC analyses
-Home-page: https://git.ligo.org/cbc/meta-data
+Home-page: https://git.ligo.org/cbc/cbcflow
 Author: Gregory Ashton
 Author-email: Gregory Ashton <gregory.ashton@ligo.org>, Rhiannon Udall <rhiannon.udall@ligo.org>
-Project-URL: Homepage, https://git.ligo.org/cbc/projects/meta-data
-Project-URL: Bug Tracker, https://git.ligo.org/cbc/projects/meta-data/-/issues
+Project-URL: Homepage, https://git.ligo.org/cbc/projects/cbcflow
+Project-URL: Bug Tracker, https://git.ligo.org/cbc/projects/cbcflow/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # CBC Workflow
 
 This is the repository for the CBC Workflow project ("CBCFlow").
 This consists of two parts - a metadata schema which governs the structure of the json files in which data is stored,
 and a code base which provides tools to interact with those files. 
 
-## [Documentation](https://cbc.docs.ligo.org/projects/meta-data/index.html)
+## [Documentation](https://cbc.docs.ligo.org/projects/cbcflow/index.html)
 
 This should be the first point of reference for usage and API of cbcflow.
 If you would like something to be added to the documentation, please contact the developers.
 
 ## The meta-data schema
 
 CBC meta-data for O4 will be stored in structured json files, as recommended by an investigatory committee [here](https://dcc.ligo.org/LIGO-T2100502).
 The second version (v2) of this schema is nearing completion, and will be used for the first part of the fourth observing run (O4a).
-For more information on the schema, please see [the appropriate section of the documentation](https://cbc.docs.ligo.org/projects/meta-data/metadata.html). 
+For more information on the schema, please see [the appropriate section of the documentation](https://cbc.docs.ligo.org/projects/cbcflow/metadata.html). 
 
 ## CBCFlow
 
 `cbcflow` is a set of tools provided for users to interact with the metadata libraries being used. This includes:
 - Tools for creating new default metadata files, validating them against the schema and viewing their contents.
 - Monitors which pull information on events from GraceDB, according to structured queries.
 - An infrastructure for parsing libraries of these events, and configuration of those libraries which structures the aformenetioned queries.
```

### Comparing `cbcflow-0.1.2a6/README.md` & `cbcflow-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # CBC Workflow
 
 This is the repository for the CBC Workflow project ("CBCFlow").
 This consists of two parts - a metadata schema which governs the structure of the json files in which data is stored,
 and a code base which provides tools to interact with those files. 
 
-## [Documentation](https://cbc.docs.ligo.org/projects/meta-data/index.html)
+## [Documentation](https://cbc.docs.ligo.org/projects/cbcflow/index.html)
 
 This should be the first point of reference for usage and API of cbcflow.
 If you would like something to be added to the documentation, please contact the developers.
 
 ## The meta-data schema
 
 CBC meta-data for O4 will be stored in structured json files, as recommended by an investigatory committee [here](https://dcc.ligo.org/LIGO-T2100502).
 The second version (v2) of this schema is nearing completion, and will be used for the first part of the fourth observing run (O4a).
-For more information on the schema, please see [the appropriate section of the documentation](https://cbc.docs.ligo.org/projects/meta-data/metadata.html). 
+For more information on the schema, please see [the appropriate section of the documentation](https://cbc.docs.ligo.org/projects/cbcflow/metadata.html). 
 
 ## CBCFlow
 
 `cbcflow` is a set of tools provided for users to interact with the metadata libraries being used. This includes:
 - Tools for creating new default metadata files, validating them against the schema and viewing their contents.
 - Monitors which pull information on events from GraceDB, according to structured queries.
 - An infrastructure for parsing libraries of these events, and configuration of those libraries which structures the aformenetioned queries.
```

### Comparing `cbcflow-0.1.2a6/docs/Makefile` & `cbcflow-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/_templates/custom-class-template.rst` & `cbcflow-0.2.1/docs/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/_templates/custom-module-template.rst` & `cbcflow-0.2.1/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/actionitems.rst` & `cbcflow-0.2.1/docs/source/actionitems.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/adding-to-the-schema.rst` & `cbcflow-0.2.1/docs/source/adding-to-the-schema.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/conf.py` & `cbcflow-0.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/configuration.rst` & `cbcflow-0.2.1/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/development-setup.rst` & `cbcflow-0.2.1/docs/source/development-setup.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/example_mini_schema/example.schema` & `cbcflow-0.2.1/docs/source/example_mini_schema/example.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/example_mini_schema/schema_doc.css` & `cbcflow-0.2.1/docs/source/example_mini_schema/schema_doc.css`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/example_mini_schema/schema_doc.html` & `cbcflow-0.2.1/docs/source/example_mini_schema/schema_doc.html`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/example_mini_schema/schema_doc.min.js` & `cbcflow-0.2.1/docs/source/example_mini_schema/schema_doc.min.js`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/index.rst` & `cbcflow-0.2.1/docs/source/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -8,29 +8,31 @@
 Finally, we provide autobuilt API documentation. 
 
 .. toctree::
    :maxdepth: 1
    :caption: Getting Started
 
    configuration
+   local-library-copy-setup
    what-is-metadata
    reading-the-schema
    updating-metadata-from-the-command-line
    updating-metadata-with-the-python-api
    gwosc
 
 .. toctree::
    :maxdepth: 1
    :caption: Expert Usage
 
    development-setup
-   library-setup
+   library-setup-from-scratch
    monitor-usage
    library-indices
    library-index-labelling
+   cbcflow-git-merging
 
 .. toctree::
    :maxdepth: 1
    :caption: Schema Information:
 
    schema-visualization
    adding-to-the-schema
```

### Comparing `cbcflow-0.1.2a6/docs/source/libraries.rst` & `cbcflow-0.2.1/docs/source/libraries.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png` & `cbcflow-0.2.1/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/libraries_images/part_1.png` & `cbcflow-0.2.1/docs/source/libraries_images/part_1.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/libraries_images/part_2.png` & `cbcflow-0.2.1/docs/source/libraries_images/part_2.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/libraries_images/part_3.png` & `cbcflow-0.2.1/docs/source/libraries_images/part_3.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/libraries_images/part_4.png` & `cbcflow-0.2.1/docs/source/libraries_images/part_4.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/libraries_images/part_5.png` & `cbcflow-0.2.1/docs/source/libraries_images/part_5.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/libraries_images/part_6.png` & `cbcflow-0.2.1/docs/source/libraries_images/part_6.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/libraries_images/part_7.png` & `cbcflow-0.2.1/docs/source/libraries_images/part_7.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/libraries_images/part_8.png` & `cbcflow-0.2.1/docs/source/libraries_images/part_8.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/library-index-labelling.rst` & `cbcflow-0.2.1/docs/source/library-index-labelling.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/library-indices.rst` & `cbcflow-0.2.1/docs/source/library-indices.rst`

 * *Files 1% similar despite different names*

```diff
@@ -12,31 +12,31 @@
 
   {
     "LibraryStatus": {
       "LastUpdated": "2023/04/09 21:11:20"
     },
     "Superevents": [
       {
-        "Sname": "S230301f",
+        "UID": "S230301f",
         "LastUpdated": "2023/04/09 21:11:20",
         "Labels": [
           "PE::high-significance",
           "PE-status::unstarted"
         ]
       },
       {
-        "Sname": "S230301h",
+        "UID": "S230301h",
         "LastUpdated": "2023/04/09 21:11:17",
         "Labels": [
           "PE::high-significance",
           "PE-status::unstarted"
         ]
       },
       {
-        "Sname": "S230303m",
+        "UID": "S230303m",
         "LastUpdated": "2023/04/09 21:11:14",
         "Labels": [
           "PE::high-significance",
           "PE-status::unstarted"
         ]
       },
     ]
```

### Comparing `cbcflow-0.1.2a6/docs/source/monitor-usage.rst` & `cbcflow-0.2.1/docs/source/monitor-usage.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/reading-the-schema.rst` & `cbcflow-0.2.1/docs/source/reading-the-schema.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/updating-metadata-from-the-command-line.rst` & `cbcflow-0.2.1/docs/source/updating-metadata-from-the-command-line.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/updating-metadata-with-the-python-api.rst` & `cbcflow-0.2.1/docs/source/updating-metadata-with-the-python-api.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/docs/source/what-is-metadata.rst` & `cbcflow-0.2.1/docs/source/what-is-metadata.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/examples/initial_example.md` & `cbcflow-0.2.1/examples/initial_example.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/pyproject.toml` & `cbcflow-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -26,9 +26,9 @@
 ]
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = {attr = "cbcflow._version.__version__"}
 
 [project.urls]
-"Homepage" = "https://git.ligo.org/cbc/projects/meta-data"
-"Bug Tracker" = "https://git.ligo.org/cbc/projects/meta-data/-/issues"
+"Homepage" = "https://git.ligo.org/cbc/projects/cbcflow"
+"Bug Tracker" = "https://git.ligo.org/cbc/projects/cbcflow/-/issues"
```

### Comparing `cbcflow-0.1.2a6/schema/cbc-meta-data-v1.schema` & `cbcflow-0.2.1/schema/cbc-meta-data-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/schema/cbc-meta-data-v2.schema` & `cbcflow-0.2.1/schema/cbc-meta-data-v2.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/schema/index-v1.schema` & `cbcflow-0.2.1/schema/index-v1.schema`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973958333333334%*

 * *Differences: {"'$defs'": "{'Superevent': {'properties': {'UID': OrderedDict([('description', 'The GraceDB "*

 * *            "defined sname'), ('type', 'string'), ('pattern', '^S[0-9]{6}[a-z]+')]), delete: "*

 * *            "['Sname']}}}"}*

```diff
@@ -5,15 +5,15 @@
             "description": "A superevent stored in this library",
             "properties": {
                 "LastUpdate": {
                     "description": "The time and date yyyy-mm-dd hh:mm:ss of this superevent's metadata's last update",
                     "pattern": "20[0-9]{2}-[0-1][0-9]-[0-3][0-9] [0-2][0-9]:[0-6][0-9]:[0-6][0-9]*",
                     "type": "string"
                 },
-                "Sname": {
+                "UID": {
                     "description": "The GraceDB defined sname",
                     "pattern": "^S[0-9]{6}[a-z]+",
                     "type": "string"
                 }
             },
             "type": "object"
         }
```

### Comparing `cbcflow-0.1.2a6/setup.cfg` & `cbcflow-0.2.1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
 name = cbcflow
 author = Gregory Ashton
 author_email = gregory.ashton@ligo.org
 description = A tool for managing the workflow of CBC data product
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://git.ligo.org/cbc/meta-data
+url = https://git.ligo.org/cbc/cbcflow
 project_urls = 
-	Bug Tracker = https://git.ligo.org/cbc/meta-data/-/issues
+	Bug Tracker = https://git.ligo.org/cbc/cbcflow/-/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
@@ -27,31 +27,34 @@
 	GitPython
 	lscsoft-glue
 	coverage
 	python-benedict
 	jsonmerge
 	PyYAML
 	gwpy
+	python-crontab
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 asimov.hooks.postmonitor = 
 	cbcflow = cbcflow.asimov:Collector
 asimov.hooks.applicator = 
 	cbcflow = cbcflow.asimov:Applicator
 console_scripts = 
 	cbcflow_print = cbcflow:cbcflow.print_metadata
 	cbcflow_pull = cbcflow:cbcflow.pull
 	cbcflow_update_from_flags = cbcflow:cbcflow.update
 	cbcflow_update_from_file = cbcflow:cbcflow.from_file
-	cbcflow_monitor_make = cbcflow:generate_crondor
+	cbcflow_monitor_make_crondor = cbcflow:generate_crondor
+	cbcflow_monitor_make_crontab = cbcflow:generate_crontab
 	cbcflow_monitor_run = cbcflow:run_monitor
 	cbcflow_validate_library = cbcflow:cbcflow.validate_library
+	cbcflow_git_merge = cbcflow:cbcflow.cbcflow_git_merge
 
 [flake8]
 exclude = .git,docs,build,dist,test,*__init__.py,*_version.py, versioneer.py
 max-line-length = 120
 ignore = E129 W504 W503 E203 E266
 
 [tool:pytest]
```

### Comparing `cbcflow-0.1.2a6/setup.py` & `cbcflow-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/src/cbcflow/__init__.py` & `cbcflow-0.2.1/src/cbcflow/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """The core (and presently only) module for cbcflow"""
 from typing import Union
 
 from . import _version
-from .cbcflow import from_file, setup_logger, setup_args_metadata
+from .utils import setup_logger
+from .cbcflow import from_file, setup_args_metadata
 from .configuration import get_cbcflow_config
 from .metadata import MetaData
-from .monitor import generate_crondor, run_monitor
+from .monitor import generate_crondor, generate_crontab, run_monitor
 from .parser import get_parser_and_default_data
 from .schema import get_schema
 
 __version__ = _version.__version__
 
 
 def get_superevent(
```

### Comparing `cbcflow-0.1.2a6/src/cbcflow/asimov.py` & `cbcflow-0.2.1/src/cbcflow/asimov.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import cbcflow
-import logging
 import os
 import glob
 
 from asimov.event import Event
-from asimov import config
-
-logger = logging.getLogger(__name__)
+from asimov import config, logger
 
 
 class Collector:
     status_map = {
         "ready": "unstarted",
         "processing": "running",
         "running": "running",
         "stuck": "running",
         "restart": "running",
         "stopped": "cancelled",
         "finished": "running",
         "uploaded": "complete",
     }
 
+    supported_pipelines = ["bayeswave", "bilby", "rift"]
+
     def __init__(self, ledger):
         """
         Collect data from the asimov ledger and write it to a CBCFlow library.
         """
         hook_data = ledger.data["hooks"]["postmonitor"]["cbcflow"]
         self.library = hook_data["library location"]
         self.schema_section = hook_data["schema section"]
@@ -40,163 +39,176 @@
             output = {}
             output[self.schema_section] = {}
             pe = output[self.schema_section]["Results"] = []
             metadata = cbcflow.get_superevent(
                 event.meta["ligo"]["sname"], library=self.library
             )
             for analysis in event.productions:
-                analysis_output = {}
-                analysis_output["UID"] = analysis.name
-                analysis_output["InferenceSoftware"] = str(analysis.pipeline)
-                if analysis.status.lower() in self.status_map.keys():
-                    analysis_output["RunStatus"] = self.status_map[
-                        analysis.status.lower()
-                    ]
-                if "waveform" in analysis.meta:
-                    if "approximant" in analysis.meta["waveform"]:
-                        analysis_output["WaveformApproximant"] = str(
-                            analysis.meta["waveform"]["approximant"]
-                        )
-                try:
-                    ini = analysis.pipeline.production.event.repository.find_prods(
-                        analysis.pipeline.production.name, analysis.pipeline.category
-                    )[0]
-                    analysis_output["ConfigFile"] = {}
-                    analysis_output["ConfigFile"]["Path"] = ini
-                except IndexError:
-                    logger.warning("Could not find ini file for this analysis")
-                analysis_output["Notes"] = [analysis.comment]
-                if analysis.review.status:
-                    if analysis.review.status.lower() == "approved":
-                        analysis_output["ReviewStatus"] = "pass"
-                    elif analysis.review.status.lower() == "rejected":
-                        analysis_output["ReviewStatus"] = "fail"
-                    elif analysis.review.status.lower() == "deprecated":
-                        analysis_output["Deprecated"] = True
-                    messages = sorted(
-                        analysis.review.messages, key=lambda k: k.timestamp
-                    )
-                    if len(messages) > 0:
-                        analysis_output["Notes"].append(
-                            f"{messages[0].timestamp:%Y-%m-%d}: {messages[0].message}"
+                if str(analysis.pipeline).lower() in self.supported_pipelines:
+                    analysis_output = {}
+                    analysis_output["UID"] = analysis.name
+                    analysis_output["InferenceSoftware"] = str(analysis.pipeline)
+                    if analysis.status.lower() in self.status_map.keys():
+                        analysis_output["RunStatus"] = self.status_map[
+                            analysis.status.lower()
+                        ]
+                    if "waveform" in analysis.meta:
+                        if "approximant" in analysis.meta["waveform"]:
+                            analysis_output["WaveformApproximant"] = str(
+                                analysis.meta["waveform"]["approximant"]
+                            )
+                    try:
+                        ini = analysis.pipeline.production.event.repository.find_prods(
+                            analysis.pipeline.production.name,
+                            analysis.pipeline.category,
+                        )[0]
+                        analysis_output["ConfigFile"] = {}
+                        analysis_output["ConfigFile"]["Path"] = ini
+                    except IndexError:
+                        logger.warning("Could not find ini file for this analysis")
+                    analysis_output["Notes"] = [analysis.comment]
+                    if analysis.review.status:
+                        if analysis.review.status.lower() == "approved":
+                            analysis_output["ReviewStatus"] = "pass"
+                        elif analysis.review.status.lower() == "rejected":
+                            analysis_output["ReviewStatus"] = "fail"
+                        elif analysis.review.status.lower() == "deprecated":
+                            analysis_output["Deprecated"] = True
+                        messages = sorted(
+                            analysis.review.messages, key=lambda k: k.timestamp
                         )
-                if analysis.finished:
-                    # Get the results
-                    results = analysis.pipeline.collect_assets()
-                    if str(analysis.pipeline).lower() == "bayeswave":
-                        # If the pipeline is Bayeswave, we slot each psd into its designated spot
-                        analysis_output["BayeswaveResults"] = {}
-                        for ifo, psd in results["psds"].items():
-                            analysis_output["BayeswaveResults"][f"{ifo}PSD"][
-                                "Path"
-                            ] = psd
-                        if analysis_output["BayeswaveResults"] == {}:
-                            # Cleanup if we fail to write any results
-                            analysis_output.pop("BayeswaveResults")
-                    elif str(analysis.pipeline).lower() == "bilby":
-                        # If it's bilby, we need to parse out which of possibly multiple merge results we want
-                        analysis_output["ResultFile"] = {}
-                        if len(results["samples"]) == 0:
-                            logger.warning(
-                                "Could not get samples from Bilby analysis, even though run is nominally finished!"
+                        if len(messages) > 0:
+                            analysis_output["Notes"].append(
+                                f"{messages[0].timestamp:%Y-%m-%d}: {messages[0].message}"
                             )
-                        elif len(results["samples"]) == 1:
-                            # If there's only one easy enough
-                            analysis_output["ResultFile"]["Path"] = results["samples"][
-                                0
-                            ]
-                        else:
-                            # If greater than one, we will try to prefer the hdf5 results
-                            hdf_results = [
-                                x
-                                for x in results["samples"]
-                                if "hdf5" in x or "h5" in x
-                            ]
-                            if len(hdf_results) == 0:
-                                # If there aren't any, this implies we have more than one result, and they are all jsons
-                                # This is a bad situation, because it implies CBCFlow
-                                # does not have the requisite fields to handle the analysis outputs.
+                    if analysis.finished:
+                        # Get the results
+                        results = analysis.pipeline.collect_assets()
+                        if str(analysis.pipeline).lower() == "bayeswave":
+                            # If the pipeline is Bayeswave, we slot each psd into its designated spot
+                            analysis_output["BayeswaveResults"] = {}
+                            for ifo, psd in results["psds"].items():
+                                analysis_output["BayeswaveResults"][f"{ifo}PSD"][
+                                    "Path"
+                                ] = psd
+                            if analysis_output["BayeswaveResults"] == {}:
+                                # Cleanup if we fail to write any results
+                                analysis_output.pop("BayeswaveResults")
+                        elif str(analysis.pipeline).lower() == "bilby":
+                            # If it's bilby, we need to parse out which of possibly multiple merge results we want
+                            analysis_output["ResultFile"] = {}
+                            if len(results["samples"]) == 0:
                                 logger.warning(
-                                    "No hdf5 results were found, but more than one json result is present -\
-                                               skipping since we can't choose!"
+                                    "Could not get samples from Bilby analysis, even though run is nominally finished!"
                                 )
+                            elif len(results["samples"]) == 1:
+                                # If there's only one easy enough
                                 analysis_output["ResultFile"]["Path"] = results[
                                     "samples"
                                 ][0]
-                            elif len(hdf_results) == 1:
-                                # If there's only one hdf5, then we can proceed smoothly
-                                analysis_output["ResultFile"]["Path"] = hdf_results[0]
-                            elif len(hdf_results) > 1:
-                                # This is the same issue as described above, just with all hdf5s instead
+                            else:
+                                # If greater than one, we will try to prefer the hdf5 results
+                                hdf_results = [
+                                    x
+                                    for x in results["samples"]
+                                    if "hdf5" in x or "h5" in x
+                                ]
+                                if len(hdf_results) == 0:
+                                    # If there aren't any, this implies we have more than one result,
+                                    # and they are all jsons
+                                    # This is a bad situation, because it implies CBCFlow
+                                    # does not have the requisite fields to handle the analysis outputs.
+                                    logger.warning(
+                                        "No hdf5 results were found, but more than one json result is present -\
+                                                skipping since we can't choose!"
+                                    )
+                                    analysis_output["ResultFile"]["Path"] = results[
+                                        "samples"
+                                    ][0]
+                                elif len(hdf_results) == 1:
+                                    # If there's only one hdf5, then we can proceed smoothly
+                                    analysis_output["ResultFile"]["Path"] = hdf_results[
+                                        0
+                                    ]
+                                elif len(hdf_results) > 1:
+                                    # This is the same issue as described above, just with all hdf5s instead
+                                    logger.warning(
+                                        "Multiple merge_result hdf5s returned from Bilby analysis -\
+                                                skipping since we can't choose!"
+                                    )
+                                # This has treated the case of >1 json and only 1 hdf5 as being fine
+                                # Maybe it should throw a warning for this too?
+                                if analysis_output["ResultFile"] == {}:
+                                    # Cleanup if we fail to get any results
+                                    analysis_output.pop("ResultFile")
+                        elif str(analysis.pipeline).lower() == "rift":
+                            # RIFT should only ever return one result file - extrinsic_posterior_samples.dat
+                            results = analysis.pipeline.collect_assets()
+                            if len(results) == 1:
+                                analysis_output["ResultFile"] = {}
+                                analysis_output["ResultFile"]["Path"] = results[0]
+                            else:
                                 logger.warning(
-                                    "Multiple merge_result hdf5s returned from Bilby analysis -\
-                                               skipping since we can't choose!"
+                                    "Could not get results from RIFT run - to many or too few outputs"
                                 )
-                            # This has treated the case of >1 json and only 1 hdf5 as being fine
-                            # Maybe it should throw a warning for this too?
-                            if analysis_output["ResultFile"] == {}:
-                                # Cleanup if we fail to get any results
-                                analysis_output.pop("ResultFile")
-                    elif str(analysis.pipeline).lower() == "rift":
-                        # RIFT should only ever return one result file - extrinsic_posterior_samples.dat
-                        results = analysis.pipeline.collect_assets()
-                        if len(results) == 1:
-                            analysis_output["ResultFile"] = {}
-                            analysis_output["ResultFile"]["Path"] = results[0]
+
+                    if analysis.status == "uploaded":
+                        # Next, try to get PESummary information
+                        pesummary_pages_dir = os.path.join(
+                            config.get("general", "webroot"),
+                            analysis.subject.name,
+                            analysis.name,
+                            "pesummary",
+                        )
+                        sample_h5s = glob.glob(f"{pesummary_pages_dir}/samples/*.h5")
+                        if len(sample_h5s) == 1:
+                            # If there is only one samples h5, we're good!
+                            # This *should* be true, and it should normally be called "posterior_samples.h5"
+                            # But this may not be universal?
+                            analysis_output["PESummaryResultFile"] = {}
+                            analysis_output["PESummaryResultFile"]["Path"] = sample_h5s[
+                                0
+                            ]
                         else:
                             logger.warning(
-                                "Could not get results from RIFT run - to many or too few outputs"
+                                "Could not uniquely determine location of PESummary result samples"
                             )
-                    else:
-                        logger.warning(
-                            f"Method to obtain result file for pipeline {str(analysis.pipeline)} is not implemented"
-                        )
-
-                if analysis.status == "uploaded":
-                    # Next, try to get PESummary information
-                    pesummary_pages_dir = os.path.join(
-                        config.get("general", "webroot"),
-                        analysis.subject.name,
-                        analysis.name,
-                        "pesummary",
-                    )
-                    sample_h5s = glob.glob(f"{pesummary_pages_dir}/samples/*.h5")
-                    if len(sample_h5s) == 1:
-                        # If there is only one samples h5, we're good!
-                        # This *should* be true, and it should normally be called "posterior_samples.h5"
-                        # But this may not be universal?
-                        analysis_output["PESummaryResultFile"] = {}
-                        analysis_output["PESummaryResultFile"]["Path"] = sample_h5s[0]
-                    else:
-                        logger.warning(
-                            "Could not uniquely determine location of PESummary result samples"
-                        )
-                    if pesummary_pages_dir.split("/")[2] == "public_html":
-                        # Currently, we do the bit of trying to guess the URL ourselves
-                        # In the future there may be an asimov config value for this
-                        pesummary_pages_url_dir = (
-                            cbcflow.utils.get_url_from_public_html_dir(
-                                pesummary_pages_dir
+                        if "public_html" in pesummary_pages_dir.split("/"):
+                            # Currently, we do the bit of trying to guess the URL ourselves
+                            # In the future there may be an asimov config value for this
+                            pesummary_pages_url_dir = (
+                                cbcflow.utils.get_url_from_public_html_dir(
+                                    pesummary_pages_dir
+                                )
                             )
-                        )
-                        # If we've written a result file, infer its url
-                        if "PESummaryResultFile" in analysis_output.keys():
-                            # We want to get whatever the name we previously decided was
-                            # This will only run if we did make that decision before, so we can use similar logic
-                            analysis_output["PESummaryResultFile"][
-                                "PublicHTML"
-                            ] = f"{pesummary_pages_url_dir}/samples/{sample_h5s[0].split('/')[-1]}"
-                        # Infer the summary pages URL
-                        analysis_output[
-                            "PESummaryPageURL"
-                        ] = f"{pesummary_pages_url_dir}/home.html"
-
-                pe.append(analysis_output)
-                metadata.update(output)
-                metadata.write_to_library(message="Analysis run update by asimov")
+                            # If we've written a result file, infer its url
+                            if "PESummaryResultFile" in analysis_output.keys():
+                                # We want to get whatever the name we previously decided was
+                                # This will only run if we did make that decision before, so we can use similar logic
+                                analysis_output["PESummaryResultFile"][
+                                    "PublicHTML"
+                                ] = f"{pesummary_pages_url_dir}/samples/{sample_h5s[0].split('/')[-1]}"
+                            # Infer the summary pages URL
+                            analysis_output[
+                                "PESummaryPageURL"
+                            ] = f"{pesummary_pages_url_dir}/home.html"
+
+                    pe.append(analysis_output)
+                    metadata.update(output)
+                    # Note that Asimov *should* write to main, unlike most other processes
+                    metadata.write_to_library(
+                        message="Analysis run update by asimov", branch_name="main"
+                    )
+                else:
+                    logger.info(
+                        f"Pipeline {analysis.pipeline} is not supported by cbcflow"
+                    )
+                    logger.info(
+                        "If this is a mistake, please contact the cbcflow developers to add support."
+                    )
 
 
 class Applicator:
     """Apply information from CBCFlow to an asimov event"""
 
     def __init__(self, ledger):
         hook_data = ledger.data["hooks"]["applicator"]["cbcflow"]
@@ -233,18 +245,19 @@
             if "RecommendedMinimumFrequency" in ifo.keys():
                 min_f[ifo_name] = ifo["RecommendedMinimumFrequency"]
             if "RecommendedChannel" in ifo.keys():
                 channels[ifo_name] = ifo["RecommendedChannel"]
             if "FrameType" in ifo.keys():
                 frame_types[ifo_name] = ifo["FrameType"]
 
+        recommended_ifos_list = list()
         if ifo_list != []:
-            data["interferometers"] = ifo_list
+            recommended_ifos_list = ifo_list
         else:
-            data["interferometers"] = participating_detectors
+            recommended_ifos_list = participating_detectors
             logger.info(
                 "No detchar recommended IFOs provided, falling back to participating detectors"
             )
 
         # GraceDB Settings
         ligo = {}
         for event in grace["Events"]:
@@ -255,12 +268,13 @@
         ligo["sname"] = sid
 
         output = {
             "name": metadata.data["Sname"],
             "quality": quality,
             "ligo": ligo,
             "data": data,
+            "interferometers": recommended_ifos_list,
             "event time": event_time,
         }
 
         event = Event.from_dict(output)
         self.ledger.add_event(event)
```

### Comparing `cbcflow-0.1.2a6/src/cbcflow/cbcflow.py` & `cbcflow-0.2.1/src/cbcflow/cbcflow.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,33 +3,26 @@
 
 """Client level methods for cbcflow (i.e. those that use argument parsing)"""
 
 import argparse
 import copy
 import glob
 import json
-import logging
 from typing import Tuple
 
-import jsonschema
 
 from .configuration import config_defaults
 from .gracedb import fetch_gracedb_information
+from .online_pe import add_onlinepe_information
 from .metadata import MetaData
 from .database import LocalLibraryDatabase
 from .parser import get_parser_and_default_data, sname_string
 from .process import process_user_input
 from .schema import get_schema
-
-
-def setup_logger() -> "logging.Logger":
-    """Setup a logger for CBCFlow"""
-    logging.basicConfig(level=logging.INFO)
-    logger = logging.getLogger(__name__)
-    return logger
+from .utils import setup_logger
 
 
 def setup_args_metadata() -> Tuple[argparse.Namespace, "MetaData"]:
     """Take in command line arguments, and return a metadata object
 
     Returns
     =======
@@ -54,34 +47,40 @@
         no_git_library=args.no_git_library,
     )
     return args, metadata
 
 
 def pull() -> None:
     """Pull updates from GraceDB to the library"""
+    import jsonschema
+
     logger = setup_logger()
     args, metadata = setup_args_metadata()
 
     default_metadata = copy.deepcopy(metadata)
 
     # Pull information from GraceDB
     gdb_data = fetch_gracedb_information(args.sname, args.gracedb_service_url)
     metadata.data.update(gdb_data)
+
+    # Pull information from onlinePE
+    add_onlinepe_information(metadata, args.sname)
+
     try:
-        metadata.write_to_library()
+        metadata.write_to_library(branch_name=args.branch_name)
     except jsonschema.exceptions.ValidationError:
         logger.info(
-            "GraceDB data cannot be validated against current schema\n\
+            "Recorded meta-data cannot be validated against current schema\n\
             Accordingly, the local library will not be updated"
         )
         if not metadata.library_file_exists:
             logger.info(
                 "Since no local library file exists yet, it will be initialized with valid defaults"
             )
-            default_metadata.write_to_library()
+            default_metadata.write_to_library(branch_name=args.branch_name)
 
 
 def update() -> None:
     """Update the library metadata according to input arguments"""
     args, metadata = setup_args_metadata()
     if metadata.library_file_exists is False:
         raise ValueError(
@@ -90,15 +89,17 @@
         )
     else:
         process_user_input(args, metadata)
         if args.yes:
             check_changes = False
         else:
             check_changes = True
-        metadata.write_to_library(check_changes=check_changes)
+        metadata.write_to_library(
+            check_changes=check_changes, branch_name=args.branch_name
+        )
 
 
 def print_metadata() -> None:
     """Print the metadata for a given event in a given library, as passed in args"""
     # Read in command line arguments
     schema = get_schema()
     _, default_data = get_parser_and_default_data(schema)
@@ -122,16 +123,14 @@
     )
 
     metadata.pretty_print()
 
 
 def from_file() -> None:
     """Given a superevent and an update file, apply the updates"""
-    logger = setup_logger()
-
     # Read in command line arguments
     schema = get_schema()
     _, default_data = get_parser_and_default_data(schema)
 
     file_parser = argparse.ArgumentParser()
     file_parser.add_argument("sname", help="The superevent SNAME", type=sname_string)
     file_parser.add_argument(
@@ -155,14 +154,27 @@
         default=config_defaults["schema"],
     )
     file_parser.add_argument(
         "--no-git-library",
         action="store_true",
         help="If true, do not treat the library as a git repo",
     )
+    file_parser.add_argument(
+        "--branch-name",
+        help="The name of the branch to which commits should be written."
+        "If this is not provided and main is the current active branch"
+        "A new branch will be constructed with format"
+        "user-name-yyyy-mm-dd",
+        default=None,
+    )
+    file_parser.add_argument(
+        "--yes",
+        help="Do not ask for confirmation",
+        action="store_true",
+    )
     args = file_parser.parse_args()
 
     # Set the sname in the default data
     default_data["Sname"] = args.sname
 
     # Instantiate the metadata
     metadata = MetaData(
@@ -189,22 +201,21 @@
     else:
         raise ValueError(
             "Could not interpret type of file,\
             check that it is either a json or a yaml,\
             and that it's ending reflects this."
         )
 
-    logger.info("Read File Contents:")
-    logger.info(json.dumps(file_contents, indent=4))
-
-    logger.info("Updating Metadata")
     metadata.update(file_contents, is_removal=args.removal_file)
 
-    logger.info("Writing to library")
-    metadata.write_to_library()
+    if args.yes:
+        check_changes = False
+    else:
+        check_changes = True
+    metadata.write_to_library(check_changes=check_changes, branch_name=args.branch_name)
 
 
 def validate_library() -> None:
     """Go through the library, validating that all metadata files satisfy the schema"""
     # Read in command line arguments
     schema = get_schema()
     _, default_data = get_parser_and_default_data(schema)
@@ -233,7 +244,52 @@
         )
 
 
 class ValidationError(Exception):
     """An error in schema validation"""
 
     pass
+
+
+def cbcflow_git_merge() -> int:
+    """A script"""
+    logger = setup_logger()
+
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
+        "mrcafile",
+        type=str,
+        help="The version of the file from the most recent common ancestor",
+    )
+    parser.add_argument(
+        "ourfile", type=str, help="The version of the file on our current branch"
+    )
+    parser.add_argument(
+        "theirfile", type=str, help="The version of the file on the other branch"
+    )
+    parser.add_argument(
+        "--library",
+        type=str,
+        default=config_defaults["library"],
+        help="The library to operate in",
+    )
+    args = parser.parse_args()
+
+    logger.info(f"Merging file {args.ourfile}")
+
+    # Setup the library, necessary to do the merge operation
+    local_library = LocalLibraryDatabase(args.library)
+    # Do the merge and get the return status
+    return_status = local_library.git_merge_metadata_jsons(
+        args.ourfile, args.theirfile, args.mrcafile
+    )
+
+    if return_status == 1:
+        logger.warning("A merge conflict has occurred as part of this process")
+        logger.warning("Conflicted fields will now be strings bounded by <<<<<<>>>>>>")
+        logger.warning("Please fix these conflicted fields and commit the result")
+        logger.warning(
+            "Note that some fields may not pass validation, due to type or enum conflicts"
+        )
+        logger.warning("Use the schema to identify these cases and correct")
+
+    return return_status
```

### Comparing `cbcflow-0.1.2a6/src/cbcflow/configuration.py` & `cbcflow-0.2.1/src/cbcflow/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Methods for fetching cbcflow configuration information"""
 import configparser
-import logging
 import os
 
-logger = logging.getLogger(__name__)
+from .utils import setup_logger
+
+logger = setup_logger()
 
 
 def get_cbcflow_config(config_file: str = "~/.cbcflow.cfg") -> dict:
     """Get the configuration information for cbcflow
 
     Parameters
     ==========
```

### Comparing `cbcflow-0.1.2a6/src/cbcflow/database.py` & `cbcflow-0.2.1/src/cbcflow/database.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 """Class objects for databases, and for providing supplemental database behavior"""
 import configparser
 import copy
 import glob
 import json
-import logging
 import os
 from functools import cached_property
 import sys
 from pprint import pformat
 from typing import Union, Dict, Type, TypeVar
+from datetime import datetime
 
 import dateutil.parser as dp
 from jsondiff import diff
 import jsonschema
 import git
-from ligo.gracedb.rest import GraceDb
-from ligo.gracedb.exceptions import HTTPError
-from gwpy.time import to_gps
+import tqdm
 
 from .metadata import MetaData
 from .parser import get_parser_and_default_data
-from .process import get_all_schema_def_defaults, get_simple_schema_defaults
+from .process import (
+    get_all_schema_def_defaults,
+    get_simple_schema_defaults,
+    process_update_json,
+    process_merge_json,
+)
 from .schema import get_schema
 from .gracedb import fetch_gracedb_information
-from .utils import get_dumpable_json_diff
+from .online_pe import add_onlinepe_information
+from .utils import get_dumpable_json_diff, setup_logger
 
-logger = logging.getLogger(__name__)
+logger = setup_logger()
 
 
 class Labeller(object):
     """A generic parent class for labellers,
     which apply labels to the index entry
     for events based on the contents of the metadata"""
 
@@ -184,23 +188,33 @@
         Returns
         =======
         list
             The collection of superevents (represented by their sname) satisfying the query
         """
         return list()
 
-    def pull_library_updates(self) -> None:
+    def pull_library_updates(self, branch_name: Union[str, None] = None) -> None:
         """Propagates metadata in superevents_to_propagate into the library.
         Should be overwritten by the child class.
+
+        Parameters
+        ==========
+        branch_name : str | None, optional
+            The branch_name to write commits to, per `cbcflow.database.LocalLibraryDatabase.git_add_and_commit`
         """
         return None
 
-    def sync_library(self) -> None:
+    def sync_library(self, branch_name: Union[str, None] = None) -> None:
         """A method for syncing the library, using the query specified in the library config.
-        This should be overwritten by the child class."""
+        This should be overwritten by the child class.
+
+        Parameters
+        ==========
+        branch_name : str | None, optional
+            The branch_name to write commits to, per `cbcflow.database.LocalLibraryDatabase.git_add_and_commit`"""
         return None
 
 
 class GraceDbDatabase(LibraryParent):
     """The LibraryParent class to use when the parent is GraceDB"""
 
     def __init__(self, service_url: str, library: "LocalLibraryDatabase") -> None:
@@ -240,86 +254,109 @@
             see https://gracedb.ligo.org/documentation/queries.html
 
         Returns
         =======
         list
             The superevents which satisfy the query
         """
+        from ligo.gracedb.rest import GraceDb
+
         queried_superevents = []
         with GraceDb(service_url=self.source_path) as gdb:
             superevent_iterator = gdb.superevents(query)
             for superevent in superevent_iterator:
                 queried_superevents.append(superevent["superevent_id"])
         return queried_superevents
 
-    def pull_library_updates(self) -> None:
-        """Pulls updates from GraceDb and writes them to library, creates default data as required"""
+    def pull_library_updates(self, branch_name: Union[str, None] = None) -> None:
+        """Pulls updates from GraceDb and writes them to library, creates default data as required
+
+        Parameters
+        ==========
+        branch_name : str, optional
+            The name of the branch to write to, as passed to `cbcflow.database.LocalLibraryDatabase.git_add_and_commit`
+        """
+        from ligo.gracedb.exceptions import HTTPError
+
         if hasattr(self, "superevents_to_propagate"):
-            for superevent_id in self.superevents_to_propagate:
+            for superevent_id in tqdm.tqdm(self.superevents_to_propagate):
                 if superevent_id in self.library.metadata_dict.keys():
                     metadata = self.library.metadata_dict[superevent_id]
                 else:
                     metadata = MetaData(
                         superevent_id,
                         local_library=self.library,
                         schema=self.library.metadata_schema,
                         default_data=self.library.metadata_default_data,
                     )
                 try:
                     backup_data = copy.deepcopy(metadata.data)
-                    database_data = self.pull(superevent_id)
-                    metadata.update(database_data)
+
+                    # Pull information from GraceDB
+                    gdb_data = self.pull(superevent_id)
+                    metadata.data.update(gdb_data)
+
+                    # Pull information from onlinePE
+                    add_onlinepe_information(metadata, superevent_id)
+
                     changes = metadata.get_diff()
                     if "GraceDB" in changes.keys() and len(changes.keys()) == 1:
                         if len(changes["GraceDB"].keys()) == 1:
                             continue
                         # This is a hack to make it not update if the only update would be "LastUpdate"
                         # It may have to change in further schema versions
                     logger.info(f"Updates to supervent {superevent_id}")
                     string_rep_changes = get_dumpable_json_diff(changes)
-                    logger.info(json.dumps(string_rep_changes, indent=2))
-                    metadata.write_to_library()
+                    logger.debug(json.dumps(string_rep_changes, indent=2))
+                    metadata.write_to_library(branch_name=branch_name)
                 except jsonschema.exceptions.ValidationError:
                     logger.warning(
                         f"For superevent {superevent_id}, GraceDB generated metadata failed validation\
                         Writing backup data (either default or pre-loaded) to library instead\n"
                     )
                     metadata.update(backup_data)
-                    metadata.write_to_library()
+                    metadata.write_to_library(branch_name=branch_name)
                 except HTTPError:
                     logger.warning(
                         f"For superevent {superevent_id}, failed to obtain data from GraceDB\
                         Writing backup data (either default or pre-loaded) to library instead\n"
                     )
                     metadata.update(backup_data)
-                    metadata.write_to_library()
+                    metadata.write_to_library(branch_name=branch_name)
         else:
             logger.info(
                 "This GraceDbDatabase instance has not assigned any superevents to propagate yet\
                  please do so before attempting to pull them."
             )
 
-    def sync_library(self) -> None:
+    def sync_library(self, branch_name: Union[str, None] = None) -> None:
         """Attempts to sync library and GraceDb,
         pulling any new events and changes to GraceDB data.
+
+        Parameters
+        ==========
+        branch_name : str | None, optional
+            The branch_name to write commits to, per `cbcflow.database.LocalLibraryDatabase.git_add_and_commit`
         """
+        from ligo.gracedb.exceptions import HTTPError
+
         # setup defaults
         # monitor_config = local_library.library_config["Monitor"]
         event_config = self.library.library_config["Events"]
 
         # annying hack due to gracedb query bug
         import datetime
 
         if event_config["created-before"] == "now":
             now = datetime.datetime.utcnow()
             now_str = now.strftime("%Y-%m-%d %H:%M:%S")
         else:
             now_str = event_config["created-before"]
 
-        logging.info(f"Syncing with GraceDB at time UTC:{now_str}")
+        logger.info(f"Syncing with GraceDB at time UTC:{now_str}")
         # make query and defaults, query
         query = f"created: {event_config['created-since']} .. {now_str} \
         FAR <= {event_config['far-threshold']}"
         logger.info(f"Constructed query {query} from library config")
         try:
             self.superevents_to_propagate = self.query_superevents(query)
         except HTTPError:
@@ -332,20 +369,20 @@
         logger.info(
             f"Querying based on library configuration returned {len(self.superevents_to_propagate)} superevents"
         )
         # for superevents not in the query parameters, but already in the library
         for superevent_id in self.library.metadata_dict.keys():
             if superevent_id not in self.superevents_to_propagate:
                 self.superevents_to_propagate.append(superevent_id)
-                logging.info(
+                logger.info(
                     f"Also querying superevent {superevent_id} which was in the library\
                 \n but which did not meet query parameters"
                 )
 
-        self.pull_library_updates()
+        self.pull_library_updates(branch_name=branch_name)
 
 
 class LocalLibraryDatabase(object):
     """An object reflecting the contents of a local library, and offering methods to interact with it"""
 
     def __init__(
         self,
@@ -461,14 +498,16 @@
         for md in metadata_list:
             metadata_dict[md.sname] = md
         self.metadata_dict.update(metadata_dict)
 
     @property
     def downselected_metadata_dict(self) -> Dict[str, MetaData]:
         """The metadata of events that satisfy library inclusion criteria, labelled by sname"""
+        from gwpy.time import to_gps
+
         downselected_metadata_dict = dict()
         self.load_library_metadata_dict()
         for sname, metadata in self.metadata_dict.items():
             library_created_earliest = to_gps(
                 self.library_config["Events"]["created-since"]
             )
             library_created_latest = to_gps(
@@ -559,72 +598,184 @@
                 f"The library directory {self.library} is not a repository,\
                 so you can't initialize pygit information for it."
             )
 
         self.repo = git.Repo(self.library)
 
     def git_add_and_commit(
-        self, filename, message: Union[str, None] = None, sname: Union[str, None] = None
+        self,
+        filename,
+        message: Union[str, None] = None,
+        sname: Union[str, None] = None,
+        branch_name: Union[str, None] = None,
     ) -> None:
         """
         Perform the git operations add and commit
 
         Parameters
         ==========
         filename : str
             The path to the file to commit
         message : str, optional
             If passed, this message will be used in the git commit, rather than the default.
         sname : str, optional
             The sname of the metadata, if a metadata file is what is being committed.
             Used for generating a default commit message.
+        branch_name: str, optional
+            The name of the branch to which the commit will be written:
+            If not passed, then:
+                - If the current branch is main, a new branch name will be formulaically generated
+                - If the current branch is not main, then the current branch will be used
+            If passed as "main", then the main branch will be written to explicitly
+            If passed as a string other than main, then that branch will be created if necessary, and checked out.
         """
         if not hasattr(self, "repo"):
             # If necessary, initialize git information for this library
             self._initialize_library_git_repo()
 
         if message is None:
             # If no message is given, make a default
             if sname is not None:
                 # The case where the file being committed is a metadata file
                 if sname in self.metadata_dict:
                     # If we are updating an extant bit of metadata
                     metadata = self.metadata_dict[sname]
-                    message = f"Changes made to [{metadata.toplevel_diff}]\n"
+                    diff = metadata.toplevel_diff
+                    if "New file" in diff:
+                        message = f"New file created for {metadata.sname}\n"
+                    else:
+                        message = f"Changes made to {metadata.toplevel_diff} for {metadata.sname}\n"
                 else:
                     # If we are creating a new metadata file
                     message = f"Committing metadata for new superevent {sname}"
             if sys.argv is not [""]:
                 if message is None:
                     message = ""
                 message += f"cmd line: {' '.join(sys.argv)}"
             if message is None:
                 message = "No information provided about this commit, and could not infer from context"
 
+        if branch_name is None:
+            if self.repo.active_branch == self.repo.heads["main"]:
+                # If we are currently on main, we want to checkout a new branch
+                logger.info(
+                    "Branch main is currently checked out, and no new branch title was passed"
+                )
+                user_name = (
+                    self.repo.config_reader()
+                    .get_value("user", "name")
+                    .replace(" ", "-")
+                )
+                date = datetime.today().strftime("%Y-%m-%d")
+                generated_branch_name = f"{user_name}-{date}"
+                self.git_checkout_new_branch(generated_branch_name)
+            else:
+                # Otherwise, we can stay on our current branch
+                pass
+        else:
+            if branch_name == "main":
+                # The case where we are forcing the commit onto main
+                logger.info("Commit explicitly made to main")
+            self.git_checkout_new_branch(branch_name)
+
         self.repo.git.add(filename)
         self.repo.git.commit("-m", message)
+        logger.info(f"Wrote commit {self.repo.active_branch.commit}")
+
+    def git_merge_metadata_jsons(
+        self, our_file: str, their_file: str, most_recent_common_ancestor_file: str
+    ) -> None:
+        """Merge metadata jsons in a manner which preserves meaning
+
+        Parameters
+        ==========
+        our_file : str
+            The file in the base (current)
+        their_file : str
+            The file from head (changes being applied)
+        most_recent_common_ancestor_file : str
+            The file from the MRCA (last commit shared by head and base)
+        """
+        # `cbcflow.process.process_merge_json handles the logic for us`
+        # We just need to load in files here
+        with open(our_file, "r") as file:
+            head_json = json.load(file)
+        with open(their_file, "r") as file:
+            base_json = json.load(file)
+        with open(most_recent_common_ancestor_file, "r") as file:
+            mrca_json = json.load(file)
+
+        # Now get the merged json and the return status
+        merge_json, return_status = process_merge_json(
+            base_json=base_json,
+            head_json=head_json,
+            mrca_json=mrca_json,
+            schema=self.metadata_schema,
+        )
+
+        # Base is where changes should be written
+        with open(our_file, "w") as file:
+            json.dump(merge_json, file, indent=2)
+
+        # Return status tracks whether there are merge conflicts
+        # 0 is good
+        # 1 is conflicts
+        return return_status
 
     def git_push_to_remote(self) -> None:
         """Push changes made to the library to the tracking remote"""
         if not hasattr(self, "repo"):
             self._initialize_library_git_repo()
         self.repo.git.push()
 
-    def git_pull_from_remote(self) -> None:
-        """Attempt to pull from the remote"""
+    def git_pull_from_remote(self, automated=False) -> None:
+        """Pull from remote using our special logic"""
         if not hasattr(self, "repo"):
             self._initialize_library_git_repo()
         try:
             self.repo.git.pull()
         except Exception as e:
             logger.info("Pull failed:")
             logger.info(e)
-            self.remote_has_merge_conflict = True
-            logger.info("Resetting to pre-merge state")
-            self.repo.git.reset("--merge")
+            if automated:
+                logger.info("Automated mode prioritizes continued json validity")
+                self.remote_has_merge_conflict = True
+                logger.info("Resetting to pre-merge state")
+                self.repo.git.reset("--merge")
+
+    def git_checkout_new_branch(
+        self, branch_name: str, remote_to_track: str = "origin"
+    ) -> None:
+        """Checkout a branch, creating it if necessary
+
+        Parameters
+        ==========
+        branch_name : str
+            The title of the branch to create
+        remote_to_track : str
+            If a new branch is being created, such that we want to track a remote, this designates
+            the remote which the tracking branch should be pushed to
+        """
+        # If necessary initialize the repo
+        if not hasattr(self, "repo"):
+            self._initialize_library_git_repo()
+        # https://gitpython.readthedocs.io/en/stable/tutorial.html
+        if branch_name not in self.repo.heads:
+            # If necessary create a new branch with title branch_name
+            logger.info(f"Creating branch {branch_name}")
+            self.repo.create_head(branch_name)
+        if self.repo.active_branch != self.repo.heads[branch_name]:
+            # If necessary check out the branch with title branch_name
+            logger.info(f"Checking out branch {branch_name}")
+            self.repo.heads[branch_name].checkout()
+        if self.repo.active_branch.tracking_branch() is None:
+            logger.info(
+                f"Pushing to tracked remote branch {remote_to_track}/{branch_name}"
+            )
+            self.repo.git.push("-u", remote_to_track, branch_name)
 
     ############################################################################
     ############################################################################
     ####               Index Related Functions and Properties               ####
     ############################################################################
     ############################################################################
 
@@ -691,22 +842,22 @@
         superevent_default = get_all_schema_def_defaults(self.library_index_schema)[
             "Superevents"
         ]
         # Loop over all superevents included in the downselected library
         for sname, metadata in self.downselected_metadata_dict.items():
             # Fill out basic info
             superevent_meta = copy.deepcopy(superevent_default)
-            superevent_meta["Sname"] = sname
+            superevent_meta["UID"] = sname
             superevent_meta["LastUpdated"] = metadata.get_date_last_modified()
             new_index["Superevents"].append(superevent_meta)
             # Get the datetime of the most recent change
             if dp.parse(superevent_meta["LastUpdated"]) > dp.parse(current_most_recent):
                 current_most_recent = superevent_meta["LastUpdated"]
         # Sort by Sname for readability
-        new_index["Superevents"].sort(key=lambda x: x["Sname"])
+        new_index["Superevents"].sort(key=lambda x: x["UID"])
         # Set the most recent change as the time of the library's most recent change
         new_index["LibraryStatus"]["LastUpdated"] = current_most_recent
         return new_index
 
     def check_for_index_update(self) -> dict:
         """Check if the index file will see any changes
 
@@ -718,28 +869,54 @@
         """
         if self.working_index == dict():
             self.working_index = self.generate_index_from_metadata()
         index_diff = diff(self.index_from_file, self.working_index)
         if index_diff != {}:
             logger.info("Index data has changed since it was last written")
             string_rep_diff = get_dumpable_json_diff(index_diff)
-            logger.info(json.dumps(string_rep_diff, indent=2))
+            logger.debug(json.dumps(string_rep_diff, indent=2))
         return index_diff
 
-    def write_index_file(self) -> None:
-        """Writes the new index to the library"""
+    def set_working_index_with_updates_to_file_index(self) -> None:
+        """Sometimes, we want to *update* the index instead of overwrite it.
+        This sets the working index to do just that.
+        Note:
+        - This will not remove events even if they are no longer satisfy index requirements
+        - If the working index has labels already set, this will concatenate those to the
+        labels in the file index, rather than overwriting, which may be undesirable"""
+        # Generate the working index from
+        if self.working_index == dict():
+            self.working_index = self.generate_index_from_metadata()
+        # Do a copy in case of python scope shenanigans
+        working_index_copy = copy.deepcopy(self.working_index)
+        # Use update methods to apply the update
+        self.working_index = process_update_json(
+            working_index_copy,
+            self.index_from_file,
+            self.library_index_schema,
+        )
+
+    def write_index_file(self, branch_name: Union[str, None] = None) -> None:
+        """Writes the new index to the library
+
+        Parameters
+        ==========
+        branch_name: str | None, optional
+            The branch name, as passed to `cbcflow.database.LocalLibraryDatabase.git_add_and_commit`.
+        """
         index_delta = self.check_for_index_update()
         if index_delta != dict():
             with open(self.index_file_path, "w") as f:
                 json.dump(self.working_index, f, indent=2)
             if self.is_git_repository:
                 self.git_add_and_commit(
                     filename=self.index_file_name,
                     message=f"Updating index with changes:\n\
                         {pformat(get_dumpable_json_diff(index_delta))}",
+                    branch_name=branch_name,
                 )
 
     def label_index_file(
         self, labeller_class: Type[LabellerType] = StandardLabeller
     ) -> None:
         """Apply labels to the working index file"""
         if self.working_index == dict():
```

### Comparing `cbcflow-0.1.2a6/src/cbcflow/metadata.py` & `cbcflow-0.2.1/src/cbcflow/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Class object for core metadata"""
 from __future__ import annotations
 
 import copy
 import json
-import logging
 import os
 import subprocess
 import sys
 from typing import TYPE_CHECKING, Union
 
 import jsondiff
 
 from .process import process_update_json
 from .utils import get_date_last_modified
 from .parser import get_parser_and_default_data
 from .schema import get_schema
+from .utils import setup_logger
 
 if TYPE_CHECKING:
     from .database import LocalLibraryDatabase
 
-logger = logging.getLogger(__name__)
+logger = setup_logger()
 
 
 class MetaData(object):
     """The core object for superevent level metadata, connecting to stored json information"""
 
     def __init__(
         self,
@@ -240,45 +240,58 @@
         ==========
         update_dict : dict
             The dictionary containing instructions to update with
         is_removal : bool, optional
             If true, this dictionary will treat all primitive list elements (i.e. not objects)
             as something to be removed, rather than added. Use sparingly.
         """
+        import jsonschema
+
         new_metadata_data = copy.deepcopy(self.data)
         new_metadata_data = process_update_json(
             update_dict,
             new_metadata_data,
             self.library._metadata_schema,
             is_removal=is_removal,
         )
-        self.library.validate(new_metadata_data)
+        try:
+            self.library.validate(new_metadata_data)
+        except jsonschema.ValidationError as e:
+            logger.warning("Failed to validate")
+            logger.warning(f"Changes are {jsondiff.diff(new_metadata_data, self.data)}")
+            raise jsonschema.ValidationError(e.message)
         self.data = new_metadata_data
 
     def load_from_library(self) -> None:
         """Load metadata from a library"""
         with open(self.library_file, "r") as file:
             data = json.load(file)
 
         self.library.validate(data)
         self.data = data
         self._loaded_data = copy.deepcopy(data)
 
     def write_to_library(
-        self, message: Union[str, None] = None, check_changes: bool = False
+        self,
+        message: Union[str, None] = None,
+        check_changes: bool = False,
+        branch_name: Union[str, None] = None,
     ) -> None:
         """
         Write loaded metadata back to library, and stage/commit if the library is a git repository
 
         Parameters
         ==========
         message : str | None, optional
             If passed, this message will be used for the git commit instead of the default.
         check_changes : bool | True, False
             If true, ask the user to confirm the changes before changing the information on disk.
+        branch_name: str | None, optional
+            The branch name, as passed to `cbcflow.database.LocalLibraryDatabase.git_add_and_commit`.
+            See that function for documentation.
         """
         if self.is_updated is False:
             logger.info("No changes made, exiting")
             return
 
         self.library.validate(self.data)
         self.print_summary()
@@ -291,15 +304,18 @@
 
         if commit_changes:
             logger.info(f"Writing file {self.library_file}")
             with open(self.library_file, "w") as file:
                 json.dump(self.data, file, indent=2)
             if self.no_git_library is False:
                 self.library.git_add_and_commit(
-                    filename=self.filename, message=message, sname=self.sname
+                    filename=self.filename,
+                    message=message,
+                    sname=self.sname,
+                    branch_name=branch_name,
                 )
         else:
             logger.info(f"No changes made to {self.library_file}")
 
     def confirm_changes(self) -> bool:
         """Get input from the user that draft changes should be adopted
 
@@ -373,13 +389,17 @@
         if diff:
             logger.info("Changes between loaded and current data:")
             logger.info(diff)
 
     @property
     def toplevel_diff(self) -> str:
         """A clean string representation of the output of get_diff"""
-        return ",".join([str(k) for k in self.get_diff().keys()])
+        diff_keys = [k for k in self.get_diff().keys()]
+        if len(diff_keys) == 1 and list(diff_keys)[0] == jsondiff.replace:
+            return "New file"
+        else:
+            return ",".join([str(k) for k in diff_keys])
 
     def pretty_print(self) -> None:
         """Prettily print the contents of the data"""
         logger.info(f"Metadata contents for {self.sname}:")
         logger.info(json.dumps(self.data, indent=4))
```

### Comparing `cbcflow-0.1.2a6/src/cbcflow/monitor.py` & `cbcflow-0.2.1/src/cbcflow/monitor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-"""Methods for setting up and running monitors through htcondor"""
+"""Methods for setting up and running monitors"""
 import argparse
-import logging
 import os
 from shutil import which
 
 from glue import pipeline
+from crontab import CronTab
 
+from .utils import setup_logger
 from .configuration import get_cbcflow_config
 from .database import LocalLibraryDatabase
 
-logging.basicConfig(level=logging.INFO)
-logger = logging.getLogger(__name__)
+logger = setup_logger()
 
 
-def generate_crondor() -> None:
-    """Creates a periodic condor to run the monitor action."""
+def get_base_parser():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--config-file",
         default="~/.cbcflow.cfg",
         help="The cfg from which to obtain monitor configuration info",
     )
     parser.add_argument(
@@ -29,30 +28,64 @@
     )
     parser.add_argument(
         "--rundir",
         default=None,
         help="The directory in which to produce sub and output files",
     )
     parser.add_argument(
+        "--monitor-minute",
+        type=int,
+        default=0,
+        help="If passed, sets the minute to run the job, so that one can get quick feedback"
+        "Defaults to 0 for normal operation",
+    )
+    return parser
+
+
+def generate_crontab() -> None:
+    parser = get_base_parser()
+    parser.add_argument(
+        "--user-name",
+        default=os.environ.get("USER", "N/A"),
+        help="The LIGO accounting user for the job to be tagged with",
+    )
+
+    args = parser.parse_args()
+
+    if args.rundir is None:
+        rundir = os.getcwd()
+    else:
+        rundir = args.rundir
+
+    monitor_exe = which("cbcflow_monitor_run")
+    monitor_args = f" {os.path.expanduser(args.config_file)} "
+
+    log_file = f"{rundir}/monitor.log"
+
+    cron = CronTab(user=args.user_name)
+    job = cron.new(command=f"{monitor_exe} {monitor_args} >> {log_file} 2>&1")
+    job.hour.every(args.monitor_interval)
+    job.minute.on(args.monitor_minute)
+    cron.write()
+
+
+def generate_crondor() -> None:
+    """Creates a periodic condor to run the monitor action."""
+
+    parser = get_base_parser()
+    parser.add_argument(
         "--ligo-accounting",
-        default=os.environ["LIGO_ACCOUNTING"],
+        default=os.environ.get("LIGO_ACCOUNTING", "N/A"),
         help="The LIGO accounting group for the job to be tagged with",
     )
     parser.add_argument(
         "--ligo-user-name",
-        default=os.environ["LIGO_USER_NAME"],
+        default=os.environ.get("LIGO_USER_NAME", "N/A"),
         help="The LIGO accounting user for the job to be tagged with",
     )
-    parser.add_argument(
-        "--monitor-minute",
-        type=int,
-        default=0,
-        help="If passed, sets the minute to run the job, so that one can get quick feedback"
-        "Defaults to 0 for normal operation",
-    )
     args = parser.parse_args()
 
     if args.rundir is None:
         rundir = os.getcwd()
     else:
         rundir = args.rundir
 
@@ -92,31 +125,44 @@
     """
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "cbcflowconfig",
         type=str,
         help="The .cbcflow.cfg file to use for library and service URL info",
     )
+    parser.add_argument(
+        "--branch-name",
+        type=str,
+        default="main",
+        help="The branch the monitor should write to - defaults to main",
+    )
     args = parser.parse_args()
 
     config_values = get_cbcflow_config(args.cbcflowconfig)
     local_library = LocalLibraryDatabase(library_path=config_values["library"])
     logger.info("CBCFlow monitor is beginning sweep")
     logger.info("Attempting to pull from remote")
-    local_library.git_pull_from_remote()
+    # Pull before we potentially checkout a new branch
+    local_library.git_pull_from_remote(automated=True)
+    # Make sure we switch to main for monitor operations
+    local_library.git_checkout_new_branch(branch_name=args.branch_name)
+    # Pull again in case the remote already existed and we want to update it
     if local_library.remote_has_merge_conflict:
         logger.info(
             "Could not pull from remote, continuing with standard sync sequence\n\
                     Before these changes can be propagated to the remote, this merge conflict\n\
                     must be resolved manually."
         )
     logger.info(f"Config values are {config_values}")
     local_library.initialize_parent(source_path=config_values["gracedb_service_url"])
-    local_library.library_parent.sync_library()
+    # Note that we explicitly sync to main instead of any other branch
+    local_library.library_parent.sync_library(branch_name=args.branch_name)
     logger.info("Updating index file for library")
-    # In the future labelling can happen via monitor, but for now do it in gitlab
-    local_library.label_index_file()
-    local_library.write_index_file()
+    # For now we don't want to do any labelling locally, instead doing it all in gitlab
+    # set_working_index... will change LastUpdate and add events
+    # but won't touch the labels
+    local_library.set_working_index_with_updates_to_file_index()
+    local_library.write_index_file(branch_name=args.branch_name)
     if not local_library.remote_has_merge_conflict:
         logger.info("Pushing to remote")
         local_library.git_push_to_remote()
     logger.info("Sweep completed, resting")
```

### Comparing `cbcflow-0.1.2a6/src/cbcflow/parser.py` & `cbcflow-0.2.1/src/cbcflow/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Parsing tools, and tools for generating default data"""
 import argparse
-import logging
 from typing import Tuple
 import re
 
 import argcomplete
 
 from .configuration import config_defaults
+from .utils import setup_logger
 
-logger = logging.getLogger(__name__)
+logger = setup_logger()
 
 IGNORE_ARGS = ["info-sname"]
 
 group_shorthands = dict(
     parameter_estimation="parameter_estimation",
     publications="publications",
 )
@@ -205,14 +205,22 @@
         default=config_defaults["gracedb_service_url"],
     )
     parser.add_argument(
         "--yes",
         help="Do not ask for confirmation",
         action="store_true",
     )
+    parser.add_argument(
+        "--branch-name",
+        help="The name of the branch to which commits should be written."
+        "If this is not provided and main is the current active branch"
+        "A new branch will be constructed with format"
+        "user-name-yyyy-mm-dd",
+        default=None,
+    )
 
     parser, default_data = build_parser_from_schema(parser, schema)
     argcomplete.autocomplete(parser)
     return parser, default_data
 
 
 def sname_string(sname):
```

### Comparing `cbcflow-0.1.2a6/src/cbcflow/schema/cbc-meta-data-v1.schema` & `cbcflow-0.2.1/src/cbcflow/schema/cbc-meta-data-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/src/cbcflow/schema/cbc-meta-data-v2.schema` & `cbcflow-0.2.1/src/cbcflow/schema/cbc-meta-data-v2.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/src/cbcflow/schema/index-v1.schema` & `cbcflow-0.2.1/src/cbcflow/schema/index-v1.schema`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973958333333334%*

 * *Differences: {"'$defs'": "{'Superevent': {'properties': {'UID': OrderedDict([('description', 'The GraceDB "*

 * *            "defined sname'), ('type', 'string'), ('pattern', '^S[0-9]{6}[a-z]+')]), delete: "*

 * *            "['Sname']}}}"}*

```diff
@@ -5,15 +5,15 @@
             "description": "A superevent stored in this library",
             "properties": {
                 "LastUpdate": {
                     "description": "The time and date yyyy-mm-dd hh:mm:ss of this superevent's metadata's last update",
                     "pattern": "20[0-9]{2}-[0-1][0-9]-[0-3][0-9] [0-2][0-9]:[0-6][0-9]:[0-6][0-9]*",
                     "type": "string"
                 },
-                "Sname": {
+                "UID": {
                     "description": "The GraceDB defined sname",
                     "pattern": "^S[0-9]{6}[a-z]+",
                     "type": "string"
                 }
             },
             "type": "object"
         }
```

### Comparing `cbcflow-0.1.2a6/src/cbcflow/schema.py` & `cbcflow-0.2.1/src/cbcflow/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Methods for fetching schema information"""
 import importlib.resources as importlib_resources
 import json
-import logging
 import sys
 from typing import Union
 from pathlib import Path
 
 from .configuration import get_cbcflow_config
+from .utils import setup_logger
 
-logger = logging.getLogger(__name__)
+logger = setup_logger()
 
 
 def get_schema_path(version, schema_type_designator="cbc"):
     """Get the path to the schema file
 
     Parameters
     ==========
@@ -81,12 +81,12 @@
             version, schema_type_designator=schema_type_designator
         )
     else:
         schema_file = get_schema_path(
             VERSION, schema_type_designator=schema_type_designator
         )
 
-    logger.info(f"Using schema file {schema_file}")
+    logger.info(f"Using {schema_type_designator} schema file {schema_file}")
     with Path(schema_file).open("r") as file:
         schema = json.load(file)
 
     return schema
```

### Comparing `cbcflow-0.1.2a6/src/cbcflow/utils.py` & `cbcflow-0.2.1/src/cbcflow/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 """Miscellaneous functions, especially relating to OS I/O"""
 import hashlib
+from typing import Union, List, Dict
 import os
 import subprocess
 from datetime import datetime
 from jsondiff import Symbol
 import logging
 
-logger = logging.getLogger(__name__)
+
+def setup_logger() -> "logging.Logger":
+    """Setup a logger for CBCFlow"""
+    logging.basicConfig(
+        format="%(asctime)s CBCFlow %(levelname)s: %(message)s",
+        level=logging.INFO,
+        datefmt="%Y-%m-%d %H:%M:%S",
+    )
+    logger = logging.getLogger(__name__)
+    return logger
+
+
+logger = setup_logger()
 
 
 def standardize_list(inlist: list) -> list:
     """Creates a list sorted in a standard way
 
     Parameters
     ==========
@@ -99,29 +112,33 @@
     with open(path, "rb") as f:
         file_hash = hashlib.md5()
         while chunk := f.read(8192):
             file_hash.update(chunk)
     return file_hash.hexdigest()
 
 
-def fill_out_linked_file(path: str, linked_file_dict: dict = dict()) -> dict:
+def fill_out_linked_file(path: str, linked_file_dict: Union[dict, None] = None) -> dict:
     """Fill out the contents of a LinkedFile object
 
     Parameters
     ==========
     path : str
         A path - absolute or relative - to the file on the cluster.
     linked_file_dict : dict, optional
         A pre-existing object to modify, if applicable
 
     Returns
     =======
     dict
         Either the linked_file_dict updated, or a new linked_file dict
     """
+
+    if linked_file_dict is None:
+        linked_file_dict = dict()
+
     path = os.path.expanduser(path)
     if path[0] != "/":
         # presumably this means it's a relative path, so prepend cwd
         path = os.path.join(os.getcwd(), path)
     working_dict = dict()
     working_dict["Path"] = ":".join([get_cluster(), path])
     working_dict["MD5Sum"] = get_md5sum(path)
@@ -156,22 +173,89 @@
         else:
             string_rep_diff[key] = val_to_write
     return string_rep_diff
 
 
 def get_url_from_public_html_dir(dirpath):
     """Given a path to a directory in public_html, get the corresponding URL (on CIT)"""
-    if dirpath.split("/")[2] == "public_html":
-        # This is the case where files are being written directly into public html
-        # First get the stuff that comes after public_html - this structure will stay the same
-        url_extension = "/".join(dirpath.split("/")[3:])
-        # next get the user in ldas form
-        url_user = f"~{dirpath.split('/')}"
-        # Combine them
-        dir_url = f"https://ldas-jobs.ligo.caltech.edu/\
-            {url_user}/{url_extension}"
-        return dir_url
-    else:
+    # Ensure the path is well formed
+    if dirpath[0] != "/":
+        dirpath = "/" + dirpath
+
+    elements = dirpath.split("/")
+
+    # Check if it is in public_html
+    if "public_html" not in elements:
         logger.info(
-            "Given directory path was not in public HTML, so URL cannot be extrapolated from it"
+            "Given dirpath was not in public HTML, so URL cannot be extrapolated from it"
+            " returning the path"
         )
-        return None
+        return dirpath
+
+    # First get the stuff that comes after public_html - this structure will stay the same
+    public_html_index = elements.index("public_html")
+    url_extension = "/".join(elements[public_html_index + 1 :])
+
+    # next get the user in ldas form
+    url_user = elements[2]
+
+    # Combine them
+    dir_url = f"https://ldas-jobs.ligo.caltech.edu/~{url_user}/{url_extension}"
+    return dir_url
+
+
+def get_number_suffixed_key(key: str, keys_so_far: list) -> str:
+    """We want unique keys - this will suffix a number to make one if necessary
+
+    Parameters
+    ==========
+    key : str
+       The key to check and possibly modify
+    keys_so_far : list
+        The keys so far to reference for uniqueness
+
+    Returns
+    =======
+    str
+        The key, suffixed if necessary for uniqueness
+    """
+    overlapping_keys = [x for x in keys_so_far if key in x]
+    if key in overlapping_keys:
+        suffixes = [x.split("_")[-1] for x in overlapping_keys if "_" in x]
+        highest_integer_not_yet_taken = 1
+        for suffix in suffixes:
+            if suffix.isdigit():
+                if int(suffix) == highest_integer_not_yet_taken:
+                    highest_integer_not_yet_taken += 1
+        new_key = f"{key}_{highest_integer_not_yet_taken}"
+        return new_key
+    else:
+        return key
+
+
+def get_uids_from_object_array(array: List[Dict], refId: str = "UID") -> list:
+    """Get the list of unique IDs from the object array
+
+    Parameters
+    ==========
+    array : List[Dict]
+        A list of objects each with a unique ID (the refId)
+    refId : str
+        The reference ID which uniquely identifies objects, in normal operation UID
+
+    Returns
+    =======
+    list
+        The list of UIDs reflected in the object array
+    """
+    list_of_uids = []
+    for entry in array:
+        try:
+            list_of_uids.append(entry[refId])
+        except KeyError as e:
+            raise KeyError(
+                (
+                    f"Failed with key error {e}\n"
+                    f"Why is there an object without {refId} in this key-tracked array?"
+                )
+            )
+    return list_of_uids
```

### Comparing `cbcflow-0.1.2a6/src/cbcflow.egg-info/PKG-INFO` & `cbcflow-0.2.1/src/cbcflow.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: cbcflow
-Version: 0.1.2a6
+Version: 0.2.1
 Summary: A package for enabling CBC analyses
-Home-page: https://git.ligo.org/cbc/meta-data
+Home-page: https://git.ligo.org/cbc/cbcflow
 Author: Gregory Ashton
 Author-email: Gregory Ashton <gregory.ashton@ligo.org>, Rhiannon Udall <rhiannon.udall@ligo.org>
-Project-URL: Homepage, https://git.ligo.org/cbc/projects/meta-data
-Project-URL: Bug Tracker, https://git.ligo.org/cbc/projects/meta-data/-/issues
+Project-URL: Homepage, https://git.ligo.org/cbc/projects/cbcflow
+Project-URL: Bug Tracker, https://git.ligo.org/cbc/projects/cbcflow/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # CBC Workflow
 
 This is the repository for the CBC Workflow project ("CBCFlow").
 This consists of two parts - a metadata schema which governs the structure of the json files in which data is stored,
 and a code base which provides tools to interact with those files. 
 
-## [Documentation](https://cbc.docs.ligo.org/projects/meta-data/index.html)
+## [Documentation](https://cbc.docs.ligo.org/projects/cbcflow/index.html)
 
 This should be the first point of reference for usage and API of cbcflow.
 If you would like something to be added to the documentation, please contact the developers.
 
 ## The meta-data schema
 
 CBC meta-data for O4 will be stored in structured json files, as recommended by an investigatory committee [here](https://dcc.ligo.org/LIGO-T2100502).
 The second version (v2) of this schema is nearing completion, and will be used for the first part of the fourth observing run (O4a).
-For more information on the schema, please see [the appropriate section of the documentation](https://cbc.docs.ligo.org/projects/meta-data/metadata.html). 
+For more information on the schema, please see [the appropriate section of the documentation](https://cbc.docs.ligo.org/projects/cbcflow/metadata.html). 
 
 ## CBCFlow
 
 `cbcflow` is a set of tools provided for users to interact with the metadata libraries being used. This includes:
 - Tools for creating new default metadata files, validating them against the schema and viewing their contents.
 - Monitors which pull information on events from GraceDB, according to structured queries.
 - An infrastructure for parsing libraries of these events, and configuration of those libraries which structures the aformenetioned queries.
```

### Comparing `cbcflow-0.1.2a6/src/cbcflow.egg-info/SOURCES.txt` & `cbcflow-0.2.1/src/cbcflow.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,25 @@
 setup.cfg
 setup.py
 docs/Makefile
 docs/requirements.txt
 docs/source/actionitems.rst
 docs/source/adding-to-the-schema.rst
 docs/source/asimov.rst
+docs/source/cbcflow-git-merging.rst
 docs/source/conf.py
 docs/source/configuration.rst
 docs/source/development-setup.rst
 docs/source/gwosc.rst
 docs/source/index.rst
 docs/source/libraries.rst
 docs/source/library-index-labelling.rst
 docs/source/library-indices.rst
-docs/source/library-setup.rst
+docs/source/library-setup-from-scratch.rst
+docs/source/local-library-copy-setup.rst
 docs/source/monitor-usage.rst
 docs/source/reading-the-schema.rst
 docs/source/schema-visualization.rst
 docs/source/updating-metadata-from-the-command-line.rst
 docs/source/updating-metadata-with-the-python-api.rst
 docs/source/what-is-metadata.rst
 docs/source/_templates/custom-class-template.rst
@@ -53,34 +55,37 @@
 src/cbcflow/asimov.py
 src/cbcflow/cbcflow.py
 src/cbcflow/configuration.py
 src/cbcflow/database.py
 src/cbcflow/gracedb.py
 src/cbcflow/metadata.py
 src/cbcflow/monitor.py
+src/cbcflow/online_pe.py
 src/cbcflow/parser.py
 src/cbcflow/process.py
 src/cbcflow/schema.py
 src/cbcflow/utils.py
 src/cbcflow.egg-info/PKG-INFO
 src/cbcflow.egg-info/SOURCES.txt
 src/cbcflow.egg-info/dependency_links.txt
 src/cbcflow.egg-info/entry_points.txt
 src/cbcflow.egg-info/requires.txt
 src/cbcflow.egg-info/top_level.txt
 src/cbcflow/schema/cbc-meta-data-v1.schema
 src/cbcflow/schema/cbc-meta-data-v2.schema
 src/cbcflow/schema/index-v1.schema
 tests/test_database.py
+tests/test_merging.py
 tests/test_metadata.py
-tests/test_parser.py
 tests/test_schema.py
 tests/files_for_testing/cbc-meta-data-example.json
+tests/files_for_testing/merge_test.json
 tests/files_for_testing/test-file-for-linking-1.txt
 tests/files_for_testing/test-file-for-linking-2.txt
+tests/files_for_testing/test-file-for-linking-3.txt
 tests/files_for_testing/update_json_1.json
 tests/files_for_testing/update_json_2.json
 tests/files_for_testing/update_yaml_1.yaml
 tests/files_for_testing/update_yaml_2.yaml
 tests/library_for_testing/S230227hp-cbc-metadata.json
 tests/library_for_testing/S230331e-cbc-metadata.json
 tests/library_for_testing/S230401h-cbc-metadata.json
```

### Comparing `cbcflow-0.1.2a6/tests/files_for_testing/cbc-meta-data-example.json` & `cbcflow-0.2.1/tests/files_for_testing/cbc-meta-data-example.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/tests/files_for_testing/update_json_1.json` & `cbcflow-0.2.1/tests/files_for_testing/update_json_1.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/tests/files_for_testing/update_json_2.json` & `cbcflow-0.2.1/tests/files_for_testing/update_json_2.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/tests/files_for_testing/update_yaml_1.yaml` & `cbcflow-0.2.1/tests/files_for_testing/update_yaml_1.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/tests/files_for_testing/update_yaml_2.yaml` & `cbcflow-0.2.1/tests/files_for_testing/update_yaml_2.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/tests/library_for_testing/S230227hp-cbc-metadata.json` & `cbcflow-0.2.1/tests/library_for_testing/S230227hp-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/tests/library_for_testing/S230331e-cbc-metadata.json` & `cbcflow-0.2.1/tests/library_for_testing/S230331e-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/tests/library_for_testing/S230401h-cbc-metadata.json` & `cbcflow-0.2.1/tests/library_for_testing/S230401h-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/tests/library_for_testing/S230402dv-cbc-metadata.json` & `cbcflow-0.2.1/tests/library_for_testing/S230402dv-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/tests/library_for_testing/S230403ae-cbc-metadata.json` & `cbcflow-0.2.1/tests/library_for_testing/S230403ae-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/tests/library_for_testing/S230404hb-cbc-metadata.json` & `cbcflow-0.2.1/tests/library_for_testing/S230404hb-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/tests/library_for_testing/S230404jc-cbc-metadata.json` & `cbcflow-0.2.1/tests/library_for_testing/S230404jc-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a6/tests/test_database.py` & `cbcflow-0.2.1/tests/test_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,9 +45,9 @@
         Returns
         =======
         list
             The superevents located in the library json
         """
         events_in_library = []
         for superevent in json["Superevents"]:
-            events_in_library.append(superevent["Sname"])
+            events_in_library.append(superevent["UID"])
         return events_in_library
```

### Comparing `cbcflow-0.1.2a6/tests/test_metadata.py` & `cbcflow-0.2.1/tests/test_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,23 +380,25 @@
         cmd_1 = [
             "cbcflow_update_from_file",
             "S190425z",
             "tests/files_for_testing/update_json_1.json",
             "--library",
             self.test_library_directory,
             "--no-git-library",
+            "--yes",
         ]
         subprocess.check_output(cmd_1)
         cmd_2 = [
             "cbcflow_update_from_file",
             "S190425z",
             "tests/files_for_testing/update_json_2.json",
             "--library",
             self.test_library_directory,
             "--no-git-library",
+            "--yes",
         ]
         subprocess.check_output(cmd_2)
         altered_metadata = MetaData(
             self.test_sname,
             local_library_path=self.test_library_directory,
             **self.default_metadata_kwargs,
         )
@@ -417,23 +419,25 @@
         cmd_1 = [
             "cbcflow_update_from_file",
             "S190425z",
             "tests/files_for_testing/update_yaml_1.yaml",
             "--library",
             self.test_library_directory,
             "--no-git-library",
+            "--yes",
         ]
         subprocess.check_output(cmd_1)
         cmd_2 = [
             "cbcflow_update_from_file",
             "S190425z",
             "tests/files_for_testing/update_yaml_2.yaml",
             "--library",
             self.test_library_directory,
             "--no-git-library",
+            "--yes",
         ]
         subprocess.check_output(cmd_2)
         altered_metadata = MetaData(
             self.test_sname,
             local_library_path=self.test_library_directory,
             **self.default_metadata_kwargs,
         )
```

### Comparing `cbcflow-0.1.2a6/tests/test_schema.py` & `cbcflow-0.2.1/tests/test_schema.py`

 * *Files identical despite different names*

