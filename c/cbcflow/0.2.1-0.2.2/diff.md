# Comparing `tmp/cbcflow-0.2.1.tar.gz` & `tmp/cbcflow-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcflow-0.2.1.tar", last modified: Wed May 10 10:09:15 2023, max compression
+gzip compressed data, was "cbcflow-0.2.2.tar", last modified: Wed May 10 10:17:23 2023, max compression
```

## Comparing `cbcflow-0.2.1.tar` & `cbcflow-0.2.2.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.622659 cbcflow-0.2.1/
--rw-r--r--   0 greg      (1000) greg      (1000)       37 2023-04-21 10:34:59.000000 cbcflow-0.2.1/.gitattributes
--rw-r--r--   0 greg      (1000) greg      (1000)      217 2023-04-21 10:34:59.000000 cbcflow-0.2.1/.gitignore
--rw-r--r--   0 greg      (1000) greg      (1000)     1533 2023-04-21 10:34:59.000000 cbcflow-0.2.1/.gitlab-ci.yml
--rw-r--r--   0 greg      (1000) greg      (1000)      873 2023-04-21 10:34:59.000000 cbcflow-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 greg      (1000) greg      (1000)     1010 2023-05-10 10:07:05.000000 cbcflow-0.2.1/CHANGELOG.md
--rw-r--r--   0 greg      (1000) greg      (1000)     1084 2023-04-21 10:34:59.000000 cbcflow-0.2.1/LICENSE.md
--rw-r--r--   0 greg      (1000) greg      (1000)      123 2023-04-21 10:34:59.000000 cbcflow-0.2.1/MANIFEST.in
--rw-r--r--   0 greg      (1000) greg      (1000)     3027 2023-05-10 10:09:15.622659 cbcflow-0.2.1/PKG-INFO
--rw-r--r--   0 greg      (1000) greg      (1000)     2390 2023-04-21 14:02:43.000000 cbcflow-0.2.1/README.md
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.592659 cbcflow-0.2.1/docs/
--rw-r--r--   0 greg      (1000) greg      (1000)      613 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/Makefile
--rw-r--r--   0 greg      (1000) greg      (1000)       53 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/requirements.txt
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.602659 cbcflow-0.2.1/docs/source/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.602659 cbcflow-0.2.1/docs/source/_templates/
--rw-r--r--   0 greg      (1000) greg      (1000)      662 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/_templates/custom-class-template.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1408 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/_templates/custom-module-template.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1158 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/actionitems.rst
--rw-r--r--   0 greg      (1000) greg      (1000)      690 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/adding-to-the-schema.rst
--rw-r--r--   0 greg      (1000) greg      (1000)       39 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/asimov.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     4404 2023-05-10 08:29:20.000000 cbcflow-0.2.1/docs/source/cbcflow-git-merging.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     2616 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/conf.py
--rw-r--r--   0 greg      (1000) greg      (1000)     1770 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/configuration.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1444 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/development-setup.rst
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.602659 cbcflow-0.2.1/docs/source/example_mini_schema/
--rw-r--r--   0 greg      (1000) greg      (1000)     2924 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/example_mini_schema/example.schema
--rw-r--r--   0 greg      (1000) greg      (1000)     6391 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/example_mini_schema/schema_doc.css
--rw-r--r--   0 greg      (1000) greg      (1000)    27212 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/example_mini_schema/schema_doc.html
--rw-r--r--   0 greg      (1000) greg      (1000)      984 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/example_mini_schema/schema_doc.min.js
--rw-r--r--   0 greg      (1000) greg      (1000)      458 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/gwosc.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1255 2023-05-10 08:29:20.000000 cbcflow-0.2.1/docs/source/index.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     2799 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/libraries.rst
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.602659 cbcflow-0.2.1/docs/source/libraries_images/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.602659 cbcflow-0.2.1/docs/source/libraries_images/.ipynb_checkpoints/
--rw-r--r--   0 greg      (1000) greg      (1000)    72683 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png
--rw-r--r--   0 greg      (1000) greg      (1000)     8993 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/libraries_images/part_1.png
--rw-r--r--   0 greg      (1000) greg      (1000)    15966 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/libraries_images/part_2.png
--rw-r--r--   0 greg      (1000) greg      (1000)    38016 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/libraries_images/part_3.png
--rw-r--r--   0 greg      (1000) greg      (1000)    51488 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/libraries_images/part_4.png
--rw-r--r--   0 greg      (1000) greg      (1000)    41435 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/libraries_images/part_5.png
--rw-r--r--   0 greg      (1000) greg      (1000)    54941 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/libraries_images/part_6.png
--rw-r--r--   0 greg      (1000) greg      (1000)    67345 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/libraries_images/part_7.png
--rw-r--r--   0 greg      (1000) greg      (1000)    72180 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/libraries_images/part_8.png
--rw-r--r--   0 greg      (1000) greg      (1000)    10255 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/library-index-labelling.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1352 2023-05-10 10:03:05.000000 cbcflow-0.2.1/docs/source/library-indices.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     3620 2023-05-10 08:29:20.000000 cbcflow-0.2.1/docs/source/library-setup-from-scratch.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1287 2023-05-10 08:29:20.000000 cbcflow-0.2.1/docs/source/local-library-copy-setup.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1782 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/monitor-usage.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     4809 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/reading-the-schema.rst
--rw-r--r--   0 greg      (1000) greg      (1000)      106 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/schema-visualization.rst
--rw-r--r--   0 greg      (1000) greg      (1000)    15476 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/updating-metadata-from-the-command-line.rst
--rw-r--r--   0 greg      (1000) greg      (1000)    12152 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/updating-metadata-with-the-python-api.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     4916 2023-04-21 10:34:59.000000 cbcflow-0.2.1/docs/source/what-is-metadata.rst
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.602659 cbcflow-0.2.1/examples/
--rw-r--r--   0 greg      (1000) greg      (1000)     7368 2023-04-21 10:34:59.000000 cbcflow-0.2.1/examples/initial_example.md
--rw-r--r--   0 greg      (1000) greg      (1000)      856 2023-04-21 14:02:43.000000 cbcflow-0.2.1/pyproject.toml
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.602659 cbcflow-0.2.1/schema/
--rw-r--r--   0 greg      (1000) greg      (1000)    40294 2023-04-21 10:34:59.000000 cbcflow-0.2.1/schema/cbc-meta-data-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)    88906 2023-04-24 13:44:33.000000 cbcflow-0.2.1/schema/cbc-meta-data-v2.schema
--rwxr-xr-x   0 greg      (1000) greg      (1000)     1766 2023-05-10 10:03:05.000000 cbcflow-0.2.1/schema/index-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)     1635 2023-05-10 10:09:15.622659 cbcflow-0.2.1/setup.cfg
--rw-r--r--   0 greg      (1000) greg      (1000)      567 2023-04-21 10:34:59.000000 cbcflow-0.2.1/setup.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.592659 cbcflow-0.2.1/src/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.612659 cbcflow-0.2.1/src/cbcflow/
--rw-r--r--   0 greg      (1000) greg      (1000)     1462 2023-04-24 14:06:13.000000 cbcflow-0.2.1/src/cbcflow/__init__.py
--rw-r--r--   0 greg      (1000) greg      (1000)      160 2023-05-10 10:09:15.000000 cbcflow-0.2.1/src/cbcflow/_version.py
--rw-r--r--   0 greg      (1000) greg      (1000)    14041 2023-05-10 08:29:20.000000 cbcflow-0.2.1/src/cbcflow/asimov.py
--rwxr-xr-x   0 greg      (1000) greg      (1000)     9343 2023-05-10 10:03:05.000000 cbcflow-0.2.1/src/cbcflow/cbcflow.py
--rw-r--r--   0 greg      (1000) greg      (1000)     1330 2023-04-24 14:06:13.000000 cbcflow-0.2.1/src/cbcflow/configuration.py
--rw-r--r--   0 greg      (1000) greg      (1000)    37157 2023-05-10 10:03:05.000000 cbcflow-0.2.1/src/cbcflow/database.py
--rw-r--r--   0 greg      (1000) greg      (1000)    14125 2023-05-10 10:03:05.000000 cbcflow-0.2.1/src/cbcflow/gracedb.py
--rw-r--r--   0 greg      (1000) greg      (1000)    14413 2023-05-10 10:03:05.000000 cbcflow-0.2.1/src/cbcflow/metadata.py
--rw-r--r--   0 greg      (1000) greg      (1000)     6270 2023-05-10 08:29:20.000000 cbcflow-0.2.1/src/cbcflow/monitor.py
--rw-r--r--   0 greg      (1000) greg      (1000)     5096 2023-05-10 10:03:05.000000 cbcflow-0.2.1/src/cbcflow/online_pe.py
--rw-r--r--   0 greg      (1000) greg      (1000)     8049 2023-05-10 08:29:20.000000 cbcflow-0.2.1/src/cbcflow/parser.py
--rw-r--r--   0 greg      (1000) greg      (1000)    35849 2023-05-10 10:03:05.000000 cbcflow-0.2.1/src/cbcflow/process.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.612659 cbcflow-0.2.1/src/cbcflow/schema/
--rw-r--r--   0 greg      (1000) greg      (1000)    40294 2023-05-10 10:09:15.000000 cbcflow-0.2.1/src/cbcflow/schema/cbc-meta-data-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)    88906 2023-05-10 10:09:15.000000 cbcflow-0.2.1/src/cbcflow/schema/cbc-meta-data-v2.schema
--rwxr-xr-x   0 greg      (1000) greg      (1000)     1766 2023-05-10 10:09:15.000000 cbcflow-0.2.1/src/cbcflow/schema/index-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)     2779 2023-04-24 14:06:13.000000 cbcflow-0.2.1/src/cbcflow/schema.py
--rw-r--r--   0 greg      (1000) greg      (1000)     7294 2023-05-10 08:29:20.000000 cbcflow-0.2.1/src/cbcflow/utils.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.612659 cbcflow-0.2.1/src/cbcflow.egg-info/
--rw-r--r--   0 greg      (1000) greg      (1000)     3027 2023-05-10 10:09:15.000000 cbcflow-0.2.1/src/cbcflow.egg-info/PKG-INFO
--rw-r--r--   0 greg      (1000) greg      (1000)     3290 2023-05-10 10:09:15.000000 cbcflow-0.2.1/src/cbcflow.egg-info/SOURCES.txt
--rw-r--r--   0 greg      (1000) greg      (1000)        1 2023-05-10 10:09:15.000000 cbcflow-0.2.1/src/cbcflow.egg-info/dependency_links.txt
--rw-r--r--   0 greg      (1000) greg      (1000)      599 2023-05-10 10:09:15.000000 cbcflow-0.2.1/src/cbcflow.egg-info/entry_points.txt
--rw-r--r--   0 greg      (1000) greg      (1000)      130 2023-05-10 10:09:15.000000 cbcflow-0.2.1/src/cbcflow.egg-info/requires.txt
--rw-r--r--   0 greg      (1000) greg      (1000)        8 2023-05-10 10:09:15.000000 cbcflow-0.2.1/src/cbcflow.egg-info/top_level.txt
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.612659 cbcflow-0.2.1/tests/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.622659 cbcflow-0.2.1/tests/files_for_testing/
--rw-r--r--   0 greg      (1000) greg      (1000)    26759 2023-04-21 10:34:59.000000 cbcflow-0.2.1/tests/files_for_testing/cbc-meta-data-example.json
--rw-r--r--   0 greg      (1000) greg      (1000)     5972 2023-05-10 08:29:20.000000 cbcflow-0.2.1/tests/files_for_testing/merge_test.json
--rw-r--r--   0 greg      (1000) greg      (1000)       56 2023-04-21 10:34:59.000000 cbcflow-0.2.1/tests/files_for_testing/test-file-for-linking-1.txt
--rw-r--r--   0 greg      (1000) greg      (1000)       86 2023-04-21 10:34:59.000000 cbcflow-0.2.1/tests/files_for_testing/test-file-for-linking-2.txt
--rw-r--r--   0 greg      (1000) greg      (1000)       53 2023-05-10 08:29:20.000000 cbcflow-0.2.1/tests/files_for_testing/test-file-for-linking-3.txt
--rw-r--r--   0 greg      (1000) greg      (1000)     3091 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/files_for_testing/update_json_1.json
--rw-r--r--   0 greg      (1000) greg      (1000)     1221 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/files_for_testing/update_json_2.json
--rw-r--r--   0 greg      (1000) greg      (1000)     1626 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/files_for_testing/update_yaml_1.yaml
--rw-r--r--   0 greg      (1000) greg      (1000)      571 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/files_for_testing/update_yaml_2.yaml
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:09:15.622659 cbcflow-0.2.1/tests/library_for_testing/
--rw-r--r--   0 greg      (1000) greg      (1000)     5338 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/library_for_testing/S230227hp-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     4289 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/library_for_testing/S230331e-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     4275 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/library_for_testing/S230401h-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     2416 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/library_for_testing/S230402dv-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     3353 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/library_for_testing/S230403ae-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     5238 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/library_for_testing/S230404hb-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     3256 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/library_for_testing/S230404jc-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)      193 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/library_for_testing/library.cfg
--rw-r--r--   0 greg      (1000) greg      (1000)       90 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/library_for_testing/testing-library-index.json
--rw-r--r--   0 greg      (1000) greg      (1000)     1838 2023-05-10 10:03:05.000000 cbcflow-0.2.1/tests/test_database.py
--rw-r--r--   0 greg      (1000) greg      (1000)    38496 2023-05-10 08:29:20.000000 cbcflow-0.2.1/tests/test_merging.py
--rw-r--r--   0 greg      (1000) greg      (1000)    23545 2023-05-10 08:29:20.000000 cbcflow-0.2.1/tests/test_metadata.py
--rw-r--r--   0 greg      (1000) greg      (1000)      755 2023-04-21 10:35:00.000000 cbcflow-0.2.1/tests/test_schema.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.972633 cbcflow-0.2.2/
+-rw-r--r--   0 greg      (1000) greg      (1000)       37 2023-04-21 10:34:59.000000 cbcflow-0.2.2/.gitattributes
+-rw-r--r--   0 greg      (1000) greg      (1000)      217 2023-04-21 10:34:59.000000 cbcflow-0.2.2/.gitignore
+-rw-r--r--   0 greg      (1000) greg      (1000)     1533 2023-04-21 10:34:59.000000 cbcflow-0.2.2/.gitlab-ci.yml
+-rw-r--r--   0 greg      (1000) greg      (1000)      873 2023-04-21 10:34:59.000000 cbcflow-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 greg      (1000) greg      (1000)     1078 2023-05-10 10:16:22.000000 cbcflow-0.2.2/CHANGELOG.md
+-rw-r--r--   0 greg      (1000) greg      (1000)     1084 2023-04-21 10:34:59.000000 cbcflow-0.2.2/LICENSE.md
+-rw-r--r--   0 greg      (1000) greg      (1000)      123 2023-04-21 10:34:59.000000 cbcflow-0.2.2/MANIFEST.in
+-rw-r--r--   0 greg      (1000) greg      (1000)     3027 2023-05-10 10:17:23.972633 cbcflow-0.2.2/PKG-INFO
+-rw-r--r--   0 greg      (1000) greg      (1000)     2390 2023-04-21 14:02:43.000000 cbcflow-0.2.2/README.md
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/docs/
+-rw-r--r--   0 greg      (1000) greg      (1000)      613 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/Makefile
+-rw-r--r--   0 greg      (1000) greg      (1000)       53 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/requirements.txt
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/docs/source/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/docs/source/_templates/
+-rw-r--r--   0 greg      (1000) greg      (1000)      662 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/_templates/custom-class-template.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1408 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/_templates/custom-module-template.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1158 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/actionitems.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)      690 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/adding-to-the-schema.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)       39 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/asimov.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     4404 2023-05-10 08:29:20.000000 cbcflow-0.2.2/docs/source/cbcflow-git-merging.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     2616 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/conf.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     1770 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/configuration.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1444 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/development-setup.rst
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/docs/source/example_mini_schema/
+-rw-r--r--   0 greg      (1000) greg      (1000)     2924 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/example_mini_schema/example.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)     6391 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/example_mini_schema/schema_doc.css
+-rw-r--r--   0 greg      (1000) greg      (1000)    27212 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/example_mini_schema/schema_doc.html
+-rw-r--r--   0 greg      (1000) greg      (1000)      984 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/example_mini_schema/schema_doc.min.js
+-rw-r--r--   0 greg      (1000) greg      (1000)      458 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/gwosc.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1255 2023-05-10 08:29:20.000000 cbcflow-0.2.2/docs/source/index.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     2799 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/libraries.rst
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/docs/source/libraries_images/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/docs/source/libraries_images/.ipynb_checkpoints/
+-rw-r--r--   0 greg      (1000) greg      (1000)    72683 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png
+-rw-r--r--   0 greg      (1000) greg      (1000)     8993 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/libraries_images/part_1.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    15966 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/libraries_images/part_2.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    38016 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/libraries_images/part_3.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    51488 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/libraries_images/part_4.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    41435 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/libraries_images/part_5.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    54941 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/libraries_images/part_6.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    67345 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/libraries_images/part_7.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    72180 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/libraries_images/part_8.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    10255 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/library-index-labelling.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1352 2023-05-10 10:03:05.000000 cbcflow-0.2.2/docs/source/library-indices.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     3620 2023-05-10 08:29:20.000000 cbcflow-0.2.2/docs/source/library-setup-from-scratch.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1287 2023-05-10 08:29:20.000000 cbcflow-0.2.2/docs/source/local-library-copy-setup.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1782 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/monitor-usage.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     4809 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/reading-the-schema.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)      106 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/schema-visualization.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)    15476 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/updating-metadata-from-the-command-line.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)    12152 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/updating-metadata-with-the-python-api.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     4916 2023-04-21 10:34:59.000000 cbcflow-0.2.2/docs/source/what-is-metadata.rst
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/examples/
+-rw-r--r--   0 greg      (1000) greg      (1000)     7368 2023-04-21 10:34:59.000000 cbcflow-0.2.2/examples/initial_example.md
+-rw-r--r--   0 greg      (1000) greg      (1000)      856 2023-04-21 14:02:43.000000 cbcflow-0.2.2/pyproject.toml
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/schema/
+-rw-r--r--   0 greg      (1000) greg      (1000)    40294 2023-04-21 10:34:59.000000 cbcflow-0.2.2/schema/cbc-meta-data-v1.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)    88906 2023-04-24 13:44:33.000000 cbcflow-0.2.2/schema/cbc-meta-data-v2.schema
+-rwxr-xr-x   0 greg      (1000) greg      (1000)     1766 2023-05-10 10:03:05.000000 cbcflow-0.2.2/schema/index-v1.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)     1635 2023-05-10 10:17:23.972633 cbcflow-0.2.2/setup.cfg
+-rw-r--r--   0 greg      (1000) greg      (1000)      567 2023-04-21 10:34:59.000000 cbcflow-0.2.2/setup.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.952633 cbcflow-0.2.2/src/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/src/cbcflow/
+-rw-r--r--   0 greg      (1000) greg      (1000)     1462 2023-04-24 14:06:13.000000 cbcflow-0.2.2/src/cbcflow/__init__.py
+-rw-r--r--   0 greg      (1000) greg      (1000)      160 2023-05-10 10:17:23.000000 cbcflow-0.2.2/src/cbcflow/_version.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    14041 2023-05-10 08:29:20.000000 cbcflow-0.2.2/src/cbcflow/asimov.py
+-rwxr-xr-x   0 greg      (1000) greg      (1000)     9343 2023-05-10 10:03:05.000000 cbcflow-0.2.2/src/cbcflow/cbcflow.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     1330 2023-04-24 14:06:13.000000 cbcflow-0.2.2/src/cbcflow/configuration.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    37155 2023-05-10 10:15:43.000000 cbcflow-0.2.2/src/cbcflow/database.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    14125 2023-05-10 10:03:05.000000 cbcflow-0.2.2/src/cbcflow/gracedb.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    14413 2023-05-10 10:03:05.000000 cbcflow-0.2.2/src/cbcflow/metadata.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     6270 2023-05-10 08:29:20.000000 cbcflow-0.2.2/src/cbcflow/monitor.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     5096 2023-05-10 10:03:05.000000 cbcflow-0.2.2/src/cbcflow/online_pe.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     8049 2023-05-10 08:29:20.000000 cbcflow-0.2.2/src/cbcflow/parser.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    35849 2023-05-10 10:03:05.000000 cbcflow-0.2.2/src/cbcflow/process.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/src/cbcflow/schema/
+-rw-r--r--   0 greg      (1000) greg      (1000)    40294 2023-05-10 10:17:23.000000 cbcflow-0.2.2/src/cbcflow/schema/cbc-meta-data-v1.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)    88906 2023-05-10 10:17:23.000000 cbcflow-0.2.2/src/cbcflow/schema/cbc-meta-data-v2.schema
+-rwxr-xr-x   0 greg      (1000) greg      (1000)     1766 2023-05-10 10:17:23.000000 cbcflow-0.2.2/src/cbcflow/schema/index-v1.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)     2779 2023-04-24 14:06:13.000000 cbcflow-0.2.2/src/cbcflow/schema.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     7294 2023-05-10 08:29:20.000000 cbcflow-0.2.2/src/cbcflow/utils.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/src/cbcflow.egg-info/
+-rw-r--r--   0 greg      (1000) greg      (1000)     3027 2023-05-10 10:17:23.000000 cbcflow-0.2.2/src/cbcflow.egg-info/PKG-INFO
+-rw-r--r--   0 greg      (1000) greg      (1000)     3290 2023-05-10 10:17:23.000000 cbcflow-0.2.2/src/cbcflow.egg-info/SOURCES.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)        1 2023-05-10 10:17:23.000000 cbcflow-0.2.2/src/cbcflow.egg-info/dependency_links.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)      599 2023-05-10 10:17:23.000000 cbcflow-0.2.2/src/cbcflow.egg-info/entry_points.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)      130 2023-05-10 10:17:23.000000 cbcflow-0.2.2/src/cbcflow.egg-info/requires.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)        8 2023-05-10 10:17:23.000000 cbcflow-0.2.2/src/cbcflow.egg-info/top_level.txt
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.962633 cbcflow-0.2.2/tests/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.972633 cbcflow-0.2.2/tests/files_for_testing/
+-rw-r--r--   0 greg      (1000) greg      (1000)    26759 2023-04-21 10:34:59.000000 cbcflow-0.2.2/tests/files_for_testing/cbc-meta-data-example.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     5972 2023-05-10 08:29:20.000000 cbcflow-0.2.2/tests/files_for_testing/merge_test.json
+-rw-r--r--   0 greg      (1000) greg      (1000)       56 2023-04-21 10:34:59.000000 cbcflow-0.2.2/tests/files_for_testing/test-file-for-linking-1.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)       86 2023-04-21 10:34:59.000000 cbcflow-0.2.2/tests/files_for_testing/test-file-for-linking-2.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)       53 2023-05-10 08:29:20.000000 cbcflow-0.2.2/tests/files_for_testing/test-file-for-linking-3.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)     3091 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/files_for_testing/update_json_1.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     1221 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/files_for_testing/update_json_2.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     1626 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/files_for_testing/update_yaml_1.yaml
+-rw-r--r--   0 greg      (1000) greg      (1000)      571 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/files_for_testing/update_yaml_2.yaml
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-05-10 10:17:23.972633 cbcflow-0.2.2/tests/library_for_testing/
+-rw-r--r--   0 greg      (1000) greg      (1000)     5338 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/library_for_testing/S230227hp-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     4289 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/library_for_testing/S230331e-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     4275 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/library_for_testing/S230401h-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     2416 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/library_for_testing/S230402dv-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     3353 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/library_for_testing/S230403ae-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     5238 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/library_for_testing/S230404hb-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     3256 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/library_for_testing/S230404jc-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)      193 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/library_for_testing/library.cfg
+-rw-r--r--   0 greg      (1000) greg      (1000)       90 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/library_for_testing/testing-library-index.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     1838 2023-05-10 10:03:05.000000 cbcflow-0.2.2/tests/test_database.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    38496 2023-05-10 08:29:20.000000 cbcflow-0.2.2/tests/test_merging.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    23545 2023-05-10 08:29:20.000000 cbcflow-0.2.2/tests/test_metadata.py
+-rw-r--r--   0 greg      (1000) greg      (1000)      755 2023-04-21 10:35:00.000000 cbcflow-0.2.2/tests/test_schema.py
```

### Comparing `cbcflow-0.2.1/.gitlab-ci.yml` & `cbcflow-0.2.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/.pre-commit-config.yaml` & `cbcflow-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/CHANGELOG.md` & `cbcflow-0.2.2/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.2.2] - 2023-05-24
+### Changed
+- Fix minor bug in the labeler
+
 ## [0.2.1] - 2023-05-24
 ### Added
 - Method to safely merge json files (!79)
 - Fallback option for GraceDB preferred entries (!80)
 - Scraping of onlinePE results (!81)
 - Function to make changes on a branch (!84)
```

### Comparing `cbcflow-0.2.1/LICENSE.md` & `cbcflow-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/PKG-INFO` & `cbcflow-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcflow
-Version: 0.2.1
+Version: 0.2.2
 Summary: A package for enabling CBC analyses
 Home-page: https://git.ligo.org/cbc/cbcflow
 Author: Gregory Ashton
 Author-email: Gregory Ashton <gregory.ashton@ligo.org>, Rhiannon Udall <rhiannon.udall@ligo.org>
 Project-URL: Homepage, https://git.ligo.org/cbc/projects/cbcflow
 Project-URL: Bug Tracker, https://git.ligo.org/cbc/projects/cbcflow/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cbcflow-0.2.1/README.md` & `cbcflow-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/Makefile` & `cbcflow-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/_templates/custom-class-template.rst` & `cbcflow-0.2.2/docs/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/_templates/custom-module-template.rst` & `cbcflow-0.2.2/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/actionitems.rst` & `cbcflow-0.2.2/docs/source/actionitems.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/adding-to-the-schema.rst` & `cbcflow-0.2.2/docs/source/adding-to-the-schema.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/cbcflow-git-merging.rst` & `cbcflow-0.2.2/docs/source/cbcflow-git-merging.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/conf.py` & `cbcflow-0.2.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/configuration.rst` & `cbcflow-0.2.2/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/development-setup.rst` & `cbcflow-0.2.2/docs/source/development-setup.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/example_mini_schema/example.schema` & `cbcflow-0.2.2/docs/source/example_mini_schema/example.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/example_mini_schema/schema_doc.css` & `cbcflow-0.2.2/docs/source/example_mini_schema/schema_doc.css`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/example_mini_schema/schema_doc.html` & `cbcflow-0.2.2/docs/source/example_mini_schema/schema_doc.html`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/example_mini_schema/schema_doc.min.js` & `cbcflow-0.2.2/docs/source/example_mini_schema/schema_doc.min.js`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/index.rst` & `cbcflow-0.2.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/libraries.rst` & `cbcflow-0.2.2/docs/source/libraries.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png` & `cbcflow-0.2.2/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/libraries_images/part_1.png` & `cbcflow-0.2.2/docs/source/libraries_images/part_1.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/libraries_images/part_2.png` & `cbcflow-0.2.2/docs/source/libraries_images/part_2.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/libraries_images/part_3.png` & `cbcflow-0.2.2/docs/source/libraries_images/part_3.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/libraries_images/part_4.png` & `cbcflow-0.2.2/docs/source/libraries_images/part_4.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/libraries_images/part_5.png` & `cbcflow-0.2.2/docs/source/libraries_images/part_5.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/libraries_images/part_6.png` & `cbcflow-0.2.2/docs/source/libraries_images/part_6.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/libraries_images/part_7.png` & `cbcflow-0.2.2/docs/source/libraries_images/part_7.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/libraries_images/part_8.png` & `cbcflow-0.2.2/docs/source/libraries_images/part_8.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/library-index-labelling.rst` & `cbcflow-0.2.2/docs/source/library-index-labelling.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/library-indices.rst` & `cbcflow-0.2.2/docs/source/library-indices.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/library-setup-from-scratch.rst` & `cbcflow-0.2.2/docs/source/library-setup-from-scratch.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/local-library-copy-setup.rst` & `cbcflow-0.2.2/docs/source/local-library-copy-setup.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/monitor-usage.rst` & `cbcflow-0.2.2/docs/source/monitor-usage.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/reading-the-schema.rst` & `cbcflow-0.2.2/docs/source/reading-the-schema.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/updating-metadata-from-the-command-line.rst` & `cbcflow-0.2.2/docs/source/updating-metadata-from-the-command-line.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/updating-metadata-with-the-python-api.rst` & `cbcflow-0.2.2/docs/source/updating-metadata-with-the-python-api.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/docs/source/what-is-metadata.rst` & `cbcflow-0.2.2/docs/source/what-is-metadata.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/examples/initial_example.md` & `cbcflow-0.2.2/examples/initial_example.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/pyproject.toml` & `cbcflow-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/schema/cbc-meta-data-v1.schema` & `cbcflow-0.2.2/schema/cbc-meta-data-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/schema/cbc-meta-data-v2.schema` & `cbcflow-0.2.2/schema/cbc-meta-data-v2.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/schema/index-v1.schema` & `cbcflow-0.2.2/schema/index-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/setup.cfg` & `cbcflow-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/setup.py` & `cbcflow-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/src/cbcflow/__init__.py` & `cbcflow-0.2.2/src/cbcflow/__init__.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/src/cbcflow/asimov.py` & `cbcflow-0.2.2/src/cbcflow/asimov.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/src/cbcflow/cbcflow.py` & `cbcflow-0.2.2/src/cbcflow/cbcflow.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/src/cbcflow/configuration.py` & `cbcflow-0.2.2/src/cbcflow/configuration.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/src/cbcflow/database.py` & `cbcflow-0.2.2/src/cbcflow/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             The list of labels from the event metadata
         """
         return list()
 
     def populate_working_index_with_labels(self) -> None:
         """Loop over all events in the index, and apply labels to them based on their metadata"""
         for superevent in self.library.working_index["Superevents"]:
-            sname = superevent["Sname"]
+            sname = superevent["UID"]
             labels = self.label_event(self.library.metadata_dict[sname])
             superevent["Labels"] = labels
 
 
 LabellerType = TypeVar("LabellerType", bound=Labeller)
```

### Comparing `cbcflow-0.2.1/src/cbcflow/gracedb.py` & `cbcflow-0.2.2/src/cbcflow/gracedb.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/src/cbcflow/metadata.py` & `cbcflow-0.2.2/src/cbcflow/metadata.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/src/cbcflow/monitor.py` & `cbcflow-0.2.2/src/cbcflow/monitor.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/src/cbcflow/online_pe.py` & `cbcflow-0.2.2/src/cbcflow/online_pe.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/src/cbcflow/parser.py` & `cbcflow-0.2.2/src/cbcflow/parser.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/src/cbcflow/process.py` & `cbcflow-0.2.2/src/cbcflow/process.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/src/cbcflow/schema/cbc-meta-data-v1.schema` & `cbcflow-0.2.2/src/cbcflow/schema/cbc-meta-data-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/src/cbcflow/schema/cbc-meta-data-v2.schema` & `cbcflow-0.2.2/src/cbcflow/schema/cbc-meta-data-v2.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/src/cbcflow/schema/index-v1.schema` & `cbcflow-0.2.2/src/cbcflow/schema/index-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/src/cbcflow/schema.py` & `cbcflow-0.2.2/src/cbcflow/schema.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/src/cbcflow/utils.py` & `cbcflow-0.2.2/src/cbcflow/utils.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/src/cbcflow.egg-info/PKG-INFO` & `cbcflow-0.2.2/src/cbcflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcflow
-Version: 0.2.1
+Version: 0.2.2
 Summary: A package for enabling CBC analyses
 Home-page: https://git.ligo.org/cbc/cbcflow
 Author: Gregory Ashton
 Author-email: Gregory Ashton <gregory.ashton@ligo.org>, Rhiannon Udall <rhiannon.udall@ligo.org>
 Project-URL: Homepage, https://git.ligo.org/cbc/projects/cbcflow
 Project-URL: Bug Tracker, https://git.ligo.org/cbc/projects/cbcflow/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cbcflow-0.2.1/src/cbcflow.egg-info/SOURCES.txt` & `cbcflow-0.2.2/src/cbcflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/src/cbcflow.egg-info/entry_points.txt` & `cbcflow-0.2.2/src/cbcflow.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/tests/files_for_testing/cbc-meta-data-example.json` & `cbcflow-0.2.2/tests/files_for_testing/cbc-meta-data-example.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/tests/files_for_testing/merge_test.json` & `cbcflow-0.2.2/tests/files_for_testing/merge_test.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/tests/files_for_testing/update_json_1.json` & `cbcflow-0.2.2/tests/files_for_testing/update_json_1.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/tests/files_for_testing/update_json_2.json` & `cbcflow-0.2.2/tests/files_for_testing/update_json_2.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/tests/files_for_testing/update_yaml_1.yaml` & `cbcflow-0.2.2/tests/files_for_testing/update_yaml_1.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/tests/files_for_testing/update_yaml_2.yaml` & `cbcflow-0.2.2/tests/files_for_testing/update_yaml_2.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/tests/library_for_testing/S230227hp-cbc-metadata.json` & `cbcflow-0.2.2/tests/library_for_testing/S230227hp-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/tests/library_for_testing/S230331e-cbc-metadata.json` & `cbcflow-0.2.2/tests/library_for_testing/S230331e-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/tests/library_for_testing/S230401h-cbc-metadata.json` & `cbcflow-0.2.2/tests/library_for_testing/S230401h-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/tests/library_for_testing/S230402dv-cbc-metadata.json` & `cbcflow-0.2.2/tests/library_for_testing/S230402dv-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/tests/library_for_testing/S230403ae-cbc-metadata.json` & `cbcflow-0.2.2/tests/library_for_testing/S230403ae-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/tests/library_for_testing/S230404hb-cbc-metadata.json` & `cbcflow-0.2.2/tests/library_for_testing/S230404hb-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/tests/library_for_testing/S230404jc-cbc-metadata.json` & `cbcflow-0.2.2/tests/library_for_testing/S230404jc-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/tests/test_database.py` & `cbcflow-0.2.2/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/tests/test_merging.py` & `cbcflow-0.2.2/tests/test_merging.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/tests/test_metadata.py` & `cbcflow-0.2.2/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.2.1/tests/test_schema.py` & `cbcflow-0.2.2/tests/test_schema.py`

 * *Files identical despite different names*

