# Comparing `tmp/pii-data-0.3.2.tar.gz` & `tmp/pii-data-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pii-data-0.3.2.tar", last modified: Wed Mar 22 21:45:23 2023, max compression
+gzip compressed data, was "pii-data-0.4.0.tar", last modified: Wed May 10 15:32:27 2023, max compression
```

## Comparing `pii-data-0.3.2.tar` & `pii-data-0.4.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 21:45:23.738941 pii-data-0.3.2/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)    11357 2021-11-20 15:10:50.000000 pii-data-0.3.2/LICENSE
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       25 2021-11-20 15:10:50.000000 pii-data-0.3.2/MANIFEST.in
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     3069 2023-03-22 21:45:23.738941 pii-data-0.3.2/PKG-INFO
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2652 2023-03-17 19:11:37.000000 pii-data-0.3.2/README.md
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       20 2022-06-04 14:02:21.000000 pii-data-0.3.2/requirements.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       38 2023-03-22 21:45:23.738941 pii-data-0.3.2/setup.cfg
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2553 2023-03-20 20:52:16.000000 pii-data-0.3.2/setup.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 21:45:23.734941 pii-data-0.3.2/src/
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 21:45:23.734941 pii-data-0.3.2/src/pii_data/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       36 2023-03-22 21:45:10.000000 pii-data-0.3.2/src/pii_data/__init__.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 21:45:23.734941 pii-data-0.3.2/src/pii_data/app/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2022-06-05 21:56:14.000000 pii-data-0.3.2/src/pii_data/app/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1109 2023-01-21 17:42:47.000000 pii-data-0.3.2/src/pii_data/app/rawdoc.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      452 2023-01-21 17:42:47.000000 pii-data-0.3.2/src/pii_data/defs.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 21:45:23.738941 pii-data-0.3.2/src/pii_data/dump/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       84 2023-01-21 17:42:47.000000 pii-data-0.3.2/src/pii_data/dump/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     3471 2023-03-17 19:11:37.000000 pii-data-0.3.2/src/pii_data/dump/json.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      900 2023-03-17 19:11:37.000000 pii-data-0.3.2/src/pii_data/dump/text.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      520 2023-01-21 17:42:47.000000 pii-data-0.3.2/src/pii_data/dump/utils.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     3351 2023-01-21 17:42:47.000000 pii-data-0.3.2/src/pii_data/dump/yaml.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 21:45:23.738941 pii-data-0.3.2/src/pii_data/helper/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       26 2022-06-04 17:18:19.000000 pii-data-0.3.2/src/pii_data/helper/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     6297 2023-03-17 19:11:37.000000 pii-data-0.3.2/src/pii_data/helper/config.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1110 2023-03-17 19:11:37.000000 pii-data-0.3.2/src/pii_data/helper/exception.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     4784 2023-03-17 19:11:37.000000 pii-data-0.3.2/src/pii_data/helper/io.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2093 2023-01-21 17:42:47.000000 pii-data-0.3.2/src/pii_data/helper/json_encoder.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1865 2023-03-22 21:45:10.000000 pii-data-0.3.2/src/pii_data/helper/logger.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      730 2023-01-21 17:42:47.000000 pii-data-0.3.2/src/pii_data/helper/misc.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1004 2023-01-21 17:42:47.000000 pii-data-0.3.2/src/pii_data/helper/peeker.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 21:45:23.738941 pii-data-0.3.2/src/pii_data/types/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      152 2023-01-21 17:42:47.000000 pii-data-0.3.2/src/pii_data/types/__init__.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 21:45:23.738941 pii-data-0.3.2/src/pii_data/types/doc/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      192 2023-01-21 17:42:47.000000 pii-data-0.3.2/src/pii_data/types/doc/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     3767 2023-01-21 17:42:47.000000 pii-data-0.3.2/src/pii_data/types/doc/chunker.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      412 2023-01-21 17:42:47.000000 pii-data-0.3.2/src/pii_data/types/doc/defs.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     8394 2023-03-20 20:52:16.000000 pii-data-0.3.2/src/pii_data/types/doc/document.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1092 2022-10-28 12:38:28.000000 pii-data-0.3.2/src/pii_data/types/doc/idxlocaldoc.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     9796 2023-03-17 19:11:37.000000 pii-data-0.3.2/src/pii_data/types/doc/localdoc.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 21:45:23.738941 pii-data-0.3.2/src/pii_data/types/piicollection/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      127 2023-01-21 17:42:47.000000 pii-data-0.3.2/src/pii_data/types/piicollection/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1317 2023-03-20 20:52:16.000000 pii-data-0.3.2/src/pii_data/types/piicollection/chunk.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     7307 2023-03-20 20:52:16.000000 pii-data-0.3.2/src/pii_data/types/piicollection/collection.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2832 2023-03-20 20:52:16.000000 pii-data-0.3.2/src/pii_data/types/piicollection/loader.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     4935 2023-03-20 20:52:16.000000 pii-data-0.3.2/src/pii_data/types/piientity.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      982 2023-01-21 17:42:47.000000 pii-data-0.3.2/src/pii_data/types/piienum.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 21:45:23.734941 pii-data-0.3.2/src/pii_data.egg-info/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     3069 2023-03-22 21:45:23.000000 pii-data-0.3.2/src/pii_data.egg-info/PKG-INFO
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1233 2023-03-22 21:45:23.000000 pii-data-0.3.2/src/pii_data.egg-info/SOURCES.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        1 2023-03-22 21:45:23.000000 pii-data-0.3.2/src/pii_data.egg-info/dependency_links.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       59 2023-03-22 21:45:23.000000 pii-data-0.3.2/src/pii_data.egg-info/entry_points.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       46 2023-03-22 21:45:23.000000 pii-data-0.3.2/src/pii_data.egg-info/requires.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        9 2023-03-22 21:45:23.000000 pii-data-0.3.2/src/pii_data.egg-info/top_level.txt
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 15:32:27.912637 pii-data-0.4.0/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)    11357 2021-11-20 15:10:50.000000 pii-data-0.4.0/LICENSE
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       25 2021-11-20 15:10:50.000000 pii-data-0.4.0/MANIFEST.in
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2628 2023-05-10 15:32:27.912637 pii-data-0.4.0/PKG-INFO
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2652 2023-03-17 19:11:37.000000 pii-data-0.4.0/README.md
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       20 2022-06-04 14:02:21.000000 pii-data-0.4.0/requirements.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       38 2023-05-10 15:32:27.912637 pii-data-0.4.0/setup.cfg
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2553 2023-03-20 20:52:16.000000 pii-data-0.4.0/setup.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 15:32:27.908636 pii-data-0.4.0/src/
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 15:32:27.912637 pii-data-0.4.0/src/pii_data/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       36 2023-05-10 15:01:06.000000 pii-data-0.4.0/src/pii_data/__init__.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 15:32:27.912637 pii-data-0.4.0/src/pii_data/app/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2022-06-05 21:56:14.000000 pii-data-0.4.0/src/pii_data/app/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1109 2023-01-21 17:42:47.000000 pii-data-0.4.0/src/pii_data/app/rawdoc.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      452 2023-01-21 17:42:47.000000 pii-data-0.4.0/src/pii_data/defs.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 15:32:27.912637 pii-data-0.4.0/src/pii_data/dump/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       84 2023-01-21 17:42:47.000000 pii-data-0.4.0/src/pii_data/dump/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     3471 2023-03-17 19:11:37.000000 pii-data-0.4.0/src/pii_data/dump/json.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      900 2023-03-17 19:11:37.000000 pii-data-0.4.0/src/pii_data/dump/text.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      520 2023-01-21 17:42:47.000000 pii-data-0.4.0/src/pii_data/dump/utils.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     3351 2023-01-21 17:42:47.000000 pii-data-0.4.0/src/pii_data/dump/yaml.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 15:32:27.912637 pii-data-0.4.0/src/pii_data/helper/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       26 2022-06-04 17:18:19.000000 pii-data-0.4.0/src/pii_data/helper/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     6297 2023-03-17 19:11:37.000000 pii-data-0.4.0/src/pii_data/helper/config.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1110 2023-03-17 19:11:37.000000 pii-data-0.4.0/src/pii_data/helper/exception.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     4784 2023-03-17 19:11:37.000000 pii-data-0.4.0/src/pii_data/helper/io.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2092 2023-05-10 15:01:06.000000 pii-data-0.4.0/src/pii_data/helper/json_encoder.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1865 2023-03-22 21:45:10.000000 pii-data-0.4.0/src/pii_data/helper/logger.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      730 2023-01-21 17:42:47.000000 pii-data-0.4.0/src/pii_data/helper/misc.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1004 2023-01-21 17:42:47.000000 pii-data-0.4.0/src/pii_data/helper/peeker.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 15:32:27.912637 pii-data-0.4.0/src/pii_data/types/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      152 2023-01-21 17:42:47.000000 pii-data-0.4.0/src/pii_data/types/__init__.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 15:32:27.912637 pii-data-0.4.0/src/pii_data/types/doc/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      192 2023-01-21 17:42:47.000000 pii-data-0.4.0/src/pii_data/types/doc/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     3767 2023-01-21 17:42:47.000000 pii-data-0.4.0/src/pii_data/types/doc/chunker.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      412 2023-01-21 17:42:47.000000 pii-data-0.4.0/src/pii_data/types/doc/defs.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     8394 2023-03-20 20:52:16.000000 pii-data-0.4.0/src/pii_data/types/doc/document.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1092 2022-10-28 12:38:28.000000 pii-data-0.4.0/src/pii_data/types/doc/idxlocaldoc.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     9796 2023-03-17 19:11:37.000000 pii-data-0.4.0/src/pii_data/types/doc/localdoc.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 15:32:27.912637 pii-data-0.4.0/src/pii_data/types/piicollection/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      127 2023-01-21 17:42:47.000000 pii-data-0.4.0/src/pii_data/types/piicollection/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1317 2023-03-20 20:52:16.000000 pii-data-0.4.0/src/pii_data/types/piicollection/chunk.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     8070 2023-05-10 15:01:06.000000 pii-data-0.4.0/src/pii_data/types/piicollection/collection.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2832 2023-03-20 20:52:16.000000 pii-data-0.4.0/src/pii_data/types/piicollection/loader.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     4935 2023-03-20 20:52:16.000000 pii-data-0.4.0/src/pii_data/types/piientity.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1080 2023-05-10 15:01:06.000000 pii-data-0.4.0/src/pii_data/types/piienum.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 15:32:27.912637 pii-data-0.4.0/src/pii_data.egg-info/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2628 2023-05-10 15:32:27.000000 pii-data-0.4.0/src/pii_data.egg-info/PKG-INFO
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1233 2023-05-10 15:32:27.000000 pii-data-0.4.0/src/pii_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        1 2023-05-10 15:32:27.000000 pii-data-0.4.0/src/pii_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       58 2023-05-10 15:32:27.000000 pii-data-0.4.0/src/pii_data.egg-info/entry_points.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       46 2023-05-10 15:32:27.000000 pii-data-0.4.0/src/pii_data.egg-info/requires.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        9 2023-05-10 15:32:27.000000 pii-data-0.4.0/src/pii_data.egg-info/top_level.txt
```

### Comparing `pii-data-0.3.2/LICENSE` & `pii-data-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pii-data-0.3.2/PKG-INFO` & `pii-data-0.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,65 @@
-Metadata-Version: 2.1
-Name: pii-data
-Version: 0.3.2
-Summary: Base data structures for PII Processing
-Home-page: https://github.com/piisa/pii-data
-Author: Paulo Villegas
-Author-email: paulo.vllgs@gmail.com
-License: Apache
-Download-URL: https://github.com/piisa/pii-data/tarball/v0.3.2
-Description: # pii-data
-        
-        
-        This package provides base data structures for the management of PII i.e.
-        Personally Identifiable Information (it does *not* contain code for processing
-        documents, or extracting PII from documents).
-        
-        For the full specification embodied by these base data structures, check the
-        PIISA Data Specification.
-        
-        ## Data structures
-        
-        Two main data types are defined to hold PII information: PII Entities and PII
-        Collections. There is also a Source Document data type.
-        
-        
-        ### PII Source Document
-        
-        A PII Source Document defines the raw data from which PII is detected. This
-        document is modeled as a number of chunks, each one having an identifier and a 
-        data contents (a raw text excerpt, or other types of content). This is managed
-        in this package by the SrcDocument class and subclasses.
-        
-        The package contains the capability to dump a Source Document to a local file,
-        following a standardized schema, and to read it back from the file. This schema
-        uses YAML as support file format, and is the _only_ document read capability
-        natively provided by the package (to read other formats into Source Document
-        objects there is an auxiliary pii-preprocess package, or you can implement
-        yout own).
-        
-        The package can also export documents as raw text files.
-        
-        
-        ### PII Collection
-        
-        A PII Collection contains a list of detected/extracted PII Entities. Each
-        entity contains all the information needed to correctly identify one PII
-        instance and locate it in the document it belongs to.
-        
-        These are the PII data classes defined:
-         * PiiEntity: a PII instance (which in turn contains a `PiiEntityInfo` 
-           object)
-         * PiiCollection: the full collection of PII (the additional
-           `PiiCollectionLoader` subclass can load a collection from a JSON file)
-         * `PiiDetector`: an object to describe the module used to generate a given
-           `PiiEntity` object
-        
-        
-        ## Online behaviour
-        
-        There is partial support to use these data classes in an streaming fashion,
-        providing a way to feed data incrementally.
-        
-        
-        
-Keywords: PIISA, PII
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Development Status :: 4 - Beta
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
+# pii-data
+
+[![version](https://img.shields.io/pypi/v/pii-data)](https://pypi.org/project/pii-data)
+[![changelog](https://img.shields.io/badge/change-log-blue)](CHANGES.md)
+[![license](https://img.shields.io/pypi/l/pii-data)](LICENSE)
+[![build status](https://github.com/piisa/pii-data/actions/workflows/pii-data-pr.yml/badge.svg)](https://github.com/piisa/pii-data/actions)
+
+This package provides base data structures for the management of PII i.e.
+Personally Identifiable Information (it does *not* contain code for processing
+documents, or extracting PII from documents).
+
+For the full specification embodied by these base data structures, check the
+[PIISA Data Specification].
+
+## Data structures
+
+Two main data types are defined to hold PII information: PII Entities and PII
+Collections. There is also a Source Document data type.
+
+
+### PII Source Document
+
+A PII Source Document defines the raw data from which PII is detected. This
+document is modeled as a number of chunks, each one having an identifier and a 
+data contents (a raw text excerpt, or other types of content). This is managed
+in this package by the [SrcDocument] class and subclasses.
+
+The package contains the capability to dump a Source Document to a local file,
+following a standardized schema, and to read it back from the file. This schema
+uses YAML as support file format, and is the _only_ document read capability
+natively provided by the package (to read other formats into Source Document
+objects there is an auxiliary [pii-preprocess] package, or you can [implement
+yout own]).
+
+The package can also export documents as raw text files.
+
+
+### PII Collection
+
+A PII Collection contains a list of detected/extracted PII Entities. Each
+entity contains all the information needed to correctly identify one PII
+instance and locate it in the document it belongs to.
+
+These are the PII data classes defined:
+ * [PiiEntity]: a PII instance (which in turn contains a `PiiEntityInfo` 
+   object)
+ * [PiiCollection]: the full collection of PII (the additional
+   `PiiCollectionLoader` subclass can load a collection from a JSON file)
+ * `PiiDetector`: an object to describe the module used to generate a given
+   `PiiEntity` object
+
+
+## Online behaviour
+
+There is partial support to use these data classes in an [streaming] fashion,
+providing a way to feed data incrementally.
+
+
+[implement your own]: doc/implementing-srcdocument.md
+[streaming]: doc/stream.md
+[SrcDocument]: doc/srcdocument.md
+[PiiEntity]: doc/piientity.md
+[PiiCollection]: doc/piicollection.md
+[PIISA Data Specification]: https://github.com/piisa/piisa/
+[pii-preprocess]: https://github.com/piisa/pii-preprocess/
```

### Comparing `pii-data-0.3.2/setup.py` & `pii-data-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `pii-data-0.3.2/src/pii_data/app/rawdoc.py` & `pii-data-0.4.0/src/pii_data/app/rawdoc.py`

 * *Files identical despite different names*

### Comparing `pii-data-0.3.2/src/pii_data/dump/json.py` & `pii-data-0.4.0/src/pii_data/dump/json.py`

 * *Files identical despite different names*

### Comparing `pii-data-0.3.2/src/pii_data/dump/text.py` & `pii-data-0.4.0/src/pii_data/dump/text.py`

 * *Files identical despite different names*

### Comparing `pii-data-0.3.2/src/pii_data/dump/utils.py` & `pii-data-0.4.0/src/pii_data/dump/utils.py`

 * *Files identical despite different names*

### Comparing `pii-data-0.3.2/src/pii_data/dump/yaml.py` & `pii-data-0.4.0/src/pii_data/dump/yaml.py`

 * *Files identical despite different names*

### Comparing `pii-data-0.3.2/src/pii_data/helper/config.py` & `pii-data-0.4.0/src/pii_data/helper/config.py`

 * *Files identical despite different names*

### Comparing `pii-data-0.3.2/src/pii_data/helper/exception.py` & `pii-data-0.4.0/src/pii_data/helper/exception.py`

 * *Files identical despite different names*

### Comparing `pii-data-0.3.2/src/pii_data/helper/io.py` & `pii-data-0.4.0/src/pii_data/helper/io.py`

 * *Files identical despite different names*

### Comparing `pii-data-0.3.2/src/pii_data/helper/json_encoder.py` & `pii-data-0.4.0/src/pii_data/helper/json_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class CustomJSONEncoder(json.JSONEncoder):
     """
     A custom JSON encoder that can serialize additional objects:
       - datetime objects (into ISO 8601 strings)
       - sets (as sorted lists)
       - iterators (as lists)
       - binary data as Base64 strings (or optionally skipped)
-      - any object having a to_json() or as_dict() method
+      - any object having a to_json() or asdict() method
 
     Any other non-serializable object is converted to its string representation
     """
 
     def __init__(self, *args, binary: Union[bool, int] = True, **kwargs):
         """
           :param binary: if False, do not serialize binary data, but turn into
```

### Comparing `pii-data-0.3.2/src/pii_data/helper/logger.py` & `pii-data-0.4.0/src/pii_data/helper/logger.py`

 * *Files identical despite different names*

### Comparing `pii-data-0.3.2/src/pii_data/helper/misc.py` & `pii-data-0.4.0/src/pii_data/helper/misc.py`

 * *Files identical despite different names*

### Comparing `pii-data-0.3.2/src/pii_data/helper/peeker.py` & `pii-data-0.4.0/src/pii_data/helper/peeker.py`

 * *Files identical despite different names*

### Comparing `pii-data-0.3.2/src/pii_data/types/doc/chunker.py` & `pii-data-0.4.0/src/pii_data/types/doc/chunker.py`

 * *Files identical despite different names*

### Comparing `pii-data-0.3.2/src/pii_data/types/doc/document.py` & `pii-data-0.4.0/src/pii_data/types/doc/document.py`

 * *Files identical despite different names*

### Comparing `pii-data-0.3.2/src/pii_data/types/doc/idxlocaldoc.py` & `pii-data-0.4.0/src/pii_data/types/doc/idxlocaldoc.py`

 * *Files identical despite different names*

### Comparing `pii-data-0.3.2/src/pii_data/types/doc/localdoc.py` & `pii-data-0.4.0/src/pii_data/types/doc/localdoc.py`

 * *Files identical despite different names*

### Comparing `pii-data-0.3.2/src/pii_data/types/piicollection/chunk.py` & `pii-data-0.4.0/src/pii_data/types/piicollection/chunk.py`

 * *Files identical despite different names*

### Comparing `pii-data-0.3.2/src/pii_data/types/piicollection/collection.py` & `pii-data-0.4.0/src/pii_data/types/piicollection/collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 A class to describe a list of detected PII entities
 """
 
 from datetime import datetime, timezone
 import json
 
-from typing import TextIO, Dict, Iterator, TypeVar, Union
+from typing import TextIO, Dict, Iterator, TypeVar, Union, Iterable
 
 from ...defs import FMT_PIICOLLECTION
 from ...helper.json_encoder import CustomJSONEncoder
 from ...helper.exception import InvArgException
 from ..piientity import PiiEntity
 
 
@@ -73,41 +73,42 @@
     def clone(cls, piic: T_PIIC) -> T_PIIC:
         """
         Clone a PiiCollection into an object with the same generic information
         (header & detectors) but no stored PiiEntity objects
         """
         df = piic.defaults
         new_piic = cls(df.get("lang"), df.get("docid"))
-        new_piic._header = piic.get_header(False)
         new_piic.detectors = {k: PiiDetector(**v)
                               for k, v in piic.get_detectors().items()}
+        new_piic._detector_map = {d._id: d for d in new_piic.detectors.values()}
+        new_piic._header = piic.get_header(False)
         return new_piic
 
 
     def __init__(self, lang: str = None, docid: str = None):
         """
          :param lang: default language (ISO 639-1 code) for all entities
            in the collection
          :param docid: default document that entities in the collection will
            refer to
         """
-        # Default values
+        # Define default values
         self.defaults = {}
         if lang:
             self.defaults['lang'] = lang
         if docid:
             self.defaults['docid'] = docid
 
-        # An encoder for generating NDJSON output
-        self._encoder = CustomJSONEncoder(ensure_ascii=False)
-
-        # Data contained in the object
-        self._detector_map = {}
-        self.detectors = {}
+        # Initialize the data container for the object
         self.pii = []
+        self.detectors = {}
+        self._detector_map = {}
+
+        # Prepare a possible encoder object for generating NDJSON output
+        self._encoder = None
 
         # Initialize the collection header
         hdr = {
             "date": datetime.utcnow().replace(tzinfo=timezone.utc),
             "format": FMT_PIICOLLECTION
         }
         if 'lang' in self.defaults:
@@ -115,45 +116,69 @@
         self._set_header(hdr)
 
 
     def _set_header(self, header: Dict):
         self._header = header
 
 
+    def get_header(self, detectors: bool = True) -> Dict:
+        """
+        Return the header of the collection object, including the detectors
+        """
+        hdr = self._header.copy()
+        if detectors:
+            hdr["detectors"] = self.get_detectors()
+        return hdr
+
+    # Old name
+    header = get_header
+
+
+    def get_detector(self, idx: int) -> PiiDetector:
+        """
+        Return a detector from this collection, given its detector index
+        """
+        return self.detectors[idx]
+
+
     def get_detectors(self, asdict: bool = True) -> TYPE_DET_ALL:
         """
         Return the detectors from this collection, as a dictionary indexed
         by detector index
-         :param asdict: return detectors as dictionaries (else as PiiDetector
-            objects)
+         :param asdict: return detectors as dictionaries (else they will be
+            returned as PiiDetector objects)
         """
         if not asdict:
             return self.detectors
         else:
             return {k: v.asdict() for k, v in self.detectors.items()}
 
 
-    def get_detector(self, idx: int) -> PiiDetector:
+    def add_detector(self, detector: PiiDetector) -> str:
         """
-        Return a detector from this collection, given its detector index
+        Add a new detector to the object (if not there yet).
+         :return: the detector index
         """
-        return self.detectors[idx]
+        if detector._id not in self._detector_map:
+            num = len(self.detectors) + 1
+            self.detectors[num] = detector
+            self._detector_map[detector._id] = num
+        self.stage('detection')
+        return self._detector_map[detector._id]
 
 
-    def get_header(self, detectors: bool = True) -> Dict:
+    def add_detectors(self, detectors: Iterable[PiiDetector]) -> int:
         """
-        Return the header of the collection object, including the detectors
+        Add all a number of detectors to the object (if not there yet).
+         :return: the number of added detectors
         """
-        hdr = self._header.copy()
-        if detectors:
-            hdr["detectors"] = self.get_detectors()
-        return hdr
-
-    # Old name
-    header = get_header
+        num = len(self.detectors)
+        for det in detectors:
+            self.add_detector(det)
+        return len(self.detectors) - num
 
 
     def stage(self, value: str = None) -> str:
         """
         Return the processing stage for the collection status, and optionally
         set it
         """
@@ -172,27 +197,14 @@
     def __iter__(self) -> Iterator[PiiEntity]:
         """
         Return an iterator over the PII instances in the object
         """
         return iter(self.pii)
 
 
-    def add_detector(self, detector: PiiDetector) -> str:
-        """
-        Add a new detector to the header (if not there yet).
-        Returns the detector index
-        """
-        if detector._id not in self._detector_map:
-            num = len(self.detectors) + 1
-            self.detectors[num] = detector
-            self._detector_map[detector._id] = num
-        self.stage('detection')
-        return self._detector_map[detector._id]
-
-
     def add(self, entity: PiiEntity, detector: PiiDetector = None):
         """
         Add a PII entity to the collection
          :param entity: the entity to add
          :param detector: the PII Detector used to create this entity
         """
         # Add detector
@@ -213,33 +225,42 @@
         Set the decision information for the collection, and change the stage
           :param info: decision information to add to the collection header
         """
         self._header["decision"] = info
         self.stage("decision")
 
 
+    def to_json(self) -> Dict:
+        """
+        Return a dictionary that is JSON-serializable (when using the
+        CustomJSONEncoder class)
+        """
+        return {"metadata": self.get_header(), "pii_list": self.pii}
+
+
     def dump(self, out: TextIO, format: str = 'ndjson', **kwargs):
         """
         Dump the collection to an output destination
           :param out: destination to write to
           :param format: output format, either `ndjson` or `json`
         For `json` format, all passed additional arguments will be added to
         the JSON serializer
         """
-        header = self.get_header()
 
         if format in ("ndjson", "jsonl"):
 
+            if self._encoder is None:
+                self._encoder = CustomJSONEncoder(ensure_ascii=False)
+            header = self.get_header()
             print(self._encoder.encode(header), file=out)
             for pii in self.pii:
                 print(self._encoder.encode(pii), file=out)
 
         elif format == "json":
 
-            data = {"metadata": header, "pii_list": self.pii}
             if "indent" not in kwargs:
                 kwargs["indent"] = 2
-            json.dump(data, out, cls=CustomJSONEncoder, ensure_ascii=False,
+            json.dump(self, out, cls=CustomJSONEncoder, ensure_ascii=False,
                       **kwargs)
 
         else:
             raise InvArgException("unknown output format: {}", format)
```

### Comparing `pii-data-0.3.2/src/pii_data/types/piicollection/loader.py` & `pii-data-0.4.0/src/pii_data/types/piicollection/loader.py`

 * *Files identical despite different names*

### Comparing `pii-data-0.3.2/src/pii_data/types/piientity.py` & `pii-data-0.4.0/src/pii_data/types/piientity.py`

 * *Files identical despite different names*

### Comparing `pii-data-0.3.2/src/pii_data.egg-info/PKG-INFO` & `pii-data-0.4.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 Metadata-Version: 2.1
 Name: pii-data
-Version: 0.3.2
+Version: 0.4.0
 Summary: Base data structures for PII Processing
 Home-page: https://github.com/piisa/pii-data
+Download-URL: https://github.com/piisa/pii-data/tarball/v0.4.0
 Author: Paulo Villegas
 Author-email: paulo.vllgs@gmail.com
 License: Apache
-Download-URL: https://github.com/piisa/pii-data/tarball/v0.3.2
-Description: # pii-data
-        
-        
-        This package provides base data structures for the management of PII i.e.
-        Personally Identifiable Information (it does *not* contain code for processing
-        documents, or extracting PII from documents).
-        
-        For the full specification embodied by these base data structures, check the
-        PIISA Data Specification.
-        
-        ## Data structures
-        
-        Two main data types are defined to hold PII information: PII Entities and PII
-        Collections. There is also a Source Document data type.
-        
-        
-        ### PII Source Document
-        
-        A PII Source Document defines the raw data from which PII is detected. This
-        document is modeled as a number of chunks, each one having an identifier and a 
-        data contents (a raw text excerpt, or other types of content). This is managed
-        in this package by the SrcDocument class and subclasses.
-        
-        The package contains the capability to dump a Source Document to a local file,
-        following a standardized schema, and to read it back from the file. This schema
-        uses YAML as support file format, and is the _only_ document read capability
-        natively provided by the package (to read other formats into Source Document
-        objects there is an auxiliary pii-preprocess package, or you can implement
-        yout own).
-        
-        The package can also export documents as raw text files.
-        
-        
-        ### PII Collection
-        
-        A PII Collection contains a list of detected/extracted PII Entities. Each
-        entity contains all the information needed to correctly identify one PII
-        instance and locate it in the document it belongs to.
-        
-        These are the PII data classes defined:
-         * PiiEntity: a PII instance (which in turn contains a `PiiEntityInfo` 
-           object)
-         * PiiCollection: the full collection of PII (the additional
-           `PiiCollectionLoader` subclass can load a collection from a JSON file)
-         * `PiiDetector`: an object to describe the module used to generate a given
-           `PiiEntity` object
-        
-        
-        ## Online behaviour
-        
-        There is partial support to use these data classes in an streaming fashion,
-        providing a way to feed data incrementally.
-        
-        
-        
 Keywords: PIISA, PII
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+# pii-data
+
+
+This package provides base data structures for the management of PII i.e.
+Personally Identifiable Information (it does *not* contain code for processing
+documents, or extracting PII from documents).
+
+For the full specification embodied by these base data structures, check the
+PIISA Data Specification.
+
+## Data structures
+
+Two main data types are defined to hold PII information: PII Entities and PII
+Collections. There is also a Source Document data type.
+
+
+### PII Source Document
+
+A PII Source Document defines the raw data from which PII is detected. This
+document is modeled as a number of chunks, each one having an identifier and a 
+data contents (a raw text excerpt, or other types of content). This is managed
+in this package by the SrcDocument class and subclasses.
+
+The package contains the capability to dump a Source Document to a local file,
+following a standardized schema, and to read it back from the file. This schema
+uses YAML as support file format, and is the _only_ document read capability
+natively provided by the package (to read other formats into Source Document
+objects there is an auxiliary pii-preprocess package, or you can implement
+yout own).
+
+The package can also export documents as raw text files.
+
+
+### PII Collection
+
+A PII Collection contains a list of detected/extracted PII Entities. Each
+entity contains all the information needed to correctly identify one PII
+instance and locate it in the document it belongs to.
+
+These are the PII data classes defined:
+ * PiiEntity: a PII instance (which in turn contains a `PiiEntityInfo` 
+   object)
+ * PiiCollection: the full collection of PII (the additional
+   `PiiCollectionLoader` subclass can load a collection from a JSON file)
+ * `PiiDetector`: an object to describe the module used to generate a given
+   `PiiEntity` object
+
+
+## Online behaviour
+
+There is partial support to use these data classes in an streaming fashion,
+providing a way to feed data incrementally.
+
+
```

### Comparing `pii-data-0.3.2/src/pii_data.egg-info/SOURCES.txt` & `pii-data-0.4.0/src/pii_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

