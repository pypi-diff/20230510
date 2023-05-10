# Comparing `tmp/pii-extract-base-0.3.1.tar.gz` & `tmp/pii-extract-base-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pii-extract-base-0.3.1.tar", last modified: Wed Mar 22 22:02:39 2023, max compression
+gzip compressed data, was "pii-extract-base-0.4.0.tar", last modified: Wed May 10 18:09:42 2023, max compression
```

## Comparing `pii-extract-base-0.3.1.tar` & `pii-extract-base-0.4.0.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:02:39.967865 pii-extract-base-0.3.1/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)    11357 2021-11-20 15:10:50.000000 pii-extract-base-0.3.1/LICENSE
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       25 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/MANIFEST.in
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2409 2023-03-22 22:02:39.967865 pii-extract-base-0.3.1/PKG-INFO
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2087 2023-03-20 21:07:56.000000 pii-extract-base-0.3.1/README.md
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       39 2023-03-20 21:07:56.000000 pii-extract-base-0.3.1/requirements.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       38 2023-03-22 22:02:39.967865 pii-extract-base-0.3.1/setup.cfg
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2668 2023-03-20 21:07:56.000000 pii-extract-base-0.3.1/setup.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:02:39.963865 pii-extract-base-0.3.1/src/
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:02:39.963865 pii-extract-base-0.3.1/src/pii_extract/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       18 2023-03-22 21:59:33.000000 pii-extract-base-0.3.1/src/pii_extract/__init__.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:02:39.963865 pii-extract-base-0.3.1/src/pii_extract/api/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       68 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/api/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     4470 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/api/file.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     8468 2023-03-22 19:23:45.000000 pii-extract-base-0.3.1/src/pii_extract/api/processor.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:02:39.967865 pii-extract-base-0.3.1/src/pii_extract/app/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/app/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2234 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/app/detect.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     4383 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/app/task_info.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:02:39.967865 pii-extract-base-0.3.1/src/pii_extract/build/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        1 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/build/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1187 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/build/build.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:02:39.967865 pii-extract-base-0.3.1/src/pii_extract/build/collection/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       99 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/build/collection/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1305 2023-03-22 21:59:33.000000 pii-extract-base-0.3.1/src/pii_extract/build/collection/get.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     7275 2023-03-22 21:59:33.000000 pii-extract-base-0.3.1/src/pii_extract/build/collection/task_collection.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:02:39.967865 pii-extract-base-0.3.1/src/pii_extract/build/task/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      149 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/build/task/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     4528 2023-03-20 21:07:56.000000 pii-extract-base-0.3.1/src/pii_extract/build/task/base.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1711 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/build/task/callable.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     3524 2023-03-22 12:51:58.000000 pii-extract-base-0.3.1/src/pii_extract/build/task/multi.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1200 2023-03-22 21:59:33.000000 pii-extract-base-0.3.1/src/pii_extract/build/task/regex.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      238 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/defs.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:02:39.967865 pii-extract-base-0.3.1/src/pii_extract/gather/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/gather/__init__.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:02:39.967865 pii-extract-base-0.3.1/src/pii_extract/gather/collector/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      116 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/gather/collector/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     3442 2023-03-22 21:59:33.000000 pii-extract-base-0.3.1/src/pii_extract/gather/collector/base.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      111 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/gather/collector/defs.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     6822 2023-03-20 21:07:56.000000 pii-extract-base-0.3.1/src/pii_extract/gather/collector/folder.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2529 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/gather/collector/json.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     3770 2023-03-22 21:59:33.000000 pii-extract-base-0.3.1/src/pii_extract/gather/collector/plugin.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:02:39.967865 pii-extract-base-0.3.1/src/pii_extract/gather/parser/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       97 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/gather/parser/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      257 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/gather/parser/defs.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     8030 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/gather/parser/parser.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     3368 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/gather/parser/utils.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:02:39.967865 pii-extract-base-0.3.1/src/pii_extract/helper/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        1 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/helper/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     3532 2023-03-20 21:07:56.000000 pii-extract-base-0.3.1/src/pii_extract/helper/context.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      289 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/helper/exception.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       59 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/helper/json.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       80 2023-03-22 21:59:33.000000 pii-extract-base-0.3.1/src/pii_extract/helper/logger.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      592 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/helper/normalizer.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:02:39.967865 pii-extract-base-0.3.1/src/pii_extract/helper/tasks/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/helper/tasks/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       70 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/helper/types.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1059 2023-01-22 16:30:32.000000 pii-extract-base-0.3.1/src/pii_extract/helper/utils.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:02:39.967865 pii-extract-base-0.3.1/src/pii_extract_base.egg-info/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2409 2023-03-22 22:02:39.000000 pii-extract-base-0.3.1/src/pii_extract_base.egg-info/PKG-INFO
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1707 2023-03-22 22:02:39.000000 pii-extract-base-0.3.1/src/pii_extract_base.egg-info/SOURCES.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        1 2023-03-22 22:02:39.000000 pii-extract-base-0.3.1/src/pii_extract_base.egg-info/dependency_links.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      107 2023-03-22 22:02:39.000000 pii-extract-base-0.3.1/src/pii_extract_base.egg-info/entry_points.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       63 2023-03-22 22:02:39.000000 pii-extract-base-0.3.1/src/pii_extract_base.egg-info/requires.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       12 2023-03-22 22:02:39.000000 pii-extract-base-0.3.1/src/pii_extract_base.egg-info/top_level.txt
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:42.401250 pii-extract-base-0.4.0/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)    11357 2021-11-20 15:10:50.000000 pii-extract-base-0.4.0/LICENSE
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       25 2023-01-22 16:30:32.000000 pii-extract-base-0.4.0/MANIFEST.in
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2048 2023-05-10 18:09:42.401250 pii-extract-base-0.4.0/PKG-INFO
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2087 2023-03-20 21:07:56.000000 pii-extract-base-0.4.0/README.md
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       39 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/requirements.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       38 2023-05-10 18:09:42.401250 pii-extract-base-0.4.0/setup.cfg
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2668 2023-03-20 21:07:56.000000 pii-extract-base-0.4.0/setup.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:42.397250 pii-extract-base-0.4.0/src/
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:42.397250 pii-extract-base-0.4.0/src/pii_extract/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       18 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/__init__.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:42.397250 pii-extract-base-0.4.0/src/pii_extract/api/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       68 2023-01-22 16:30:32.000000 pii-extract-base-0.4.0/src/pii_extract/api/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     4470 2023-01-22 16:30:32.000000 pii-extract-base-0.4.0/src/pii_extract/api/file.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     9249 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/api/processor.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:42.397250 pii-extract-base-0.4.0/src/pii_extract/app/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-22 16:30:32.000000 pii-extract-base-0.4.0/src/pii_extract/app/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2234 2023-01-22 16:30:32.000000 pii-extract-base-0.4.0/src/pii_extract/app/detect.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     4392 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/app/task_info.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:42.397250 pii-extract-base-0.4.0/src/pii_extract/build/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       59 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/build/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1362 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/build/build.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:42.397250 pii-extract-base-0.4.0/src/pii_extract/build/task/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      244 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/build/task/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     4589 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/build/task/base.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1721 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/build/task/callable.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     3527 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/build/task/multi.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1202 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/build/task/regex.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      238 2023-01-22 16:30:32.000000 pii-extract-base-0.4.0/src/pii_extract/defs.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:42.397250 pii-extract-base-0.4.0/src/pii_extract/gather/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-22 16:30:32.000000 pii-extract-base-0.4.0/src/pii_extract/gather/__init__.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:42.397250 pii-extract-base-0.4.0/src/pii_extract/gather/collection/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      154 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/gather/collection/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1294 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/gather/collection/get.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:42.397250 pii-extract-base-0.4.0/src/pii_extract/gather/collection/sources/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      183 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/gather/collection/sources/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     3460 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/gather/collection/sources/base.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      111 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/gather/collection/sources/defs.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     6870 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/gather/collection/sources/folder.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2551 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/gather/collection/sources/json.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     3826 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/gather/collection/sources/plugin.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     3094 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/gather/collection/sources/utils.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     5785 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/gather/collection/task_collection.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2028 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/gather/collection/utils.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:42.397250 pii-extract-base-0.4.0/src/pii_extract/gather/parser/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       69 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/gather/parser/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      257 2023-01-22 16:30:32.000000 pii-extract-base-0.4.0/src/pii_extract/gather/parser/defs.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     8060 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/gather/parser/parser.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      247 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/gather/parser/utils.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:42.397250 pii-extract-base-0.4.0/src/pii_extract/helper/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        1 2023-01-22 16:30:32.000000 pii-extract-base-0.4.0/src/pii_extract/helper/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     3532 2023-03-20 21:07:56.000000 pii-extract-base-0.4.0/src/pii_extract/helper/context.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      289 2023-01-22 16:30:32.000000 pii-extract-base-0.4.0/src/pii_extract/helper/exception.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       59 2023-01-22 16:30:32.000000 pii-extract-base-0.4.0/src/pii_extract/helper/json.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       80 2023-03-22 21:59:33.000000 pii-extract-base-0.4.0/src/pii_extract/helper/logger.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      592 2023-01-22 16:30:32.000000 pii-extract-base-0.4.0/src/pii_extract/helper/normalizer.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:42.397250 pii-extract-base-0.4.0/src/pii_extract/helper/tasks/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-22 16:30:32.000000 pii-extract-base-0.4.0/src/pii_extract/helper/tasks/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       70 2023-01-22 16:30:32.000000 pii-extract-base-0.4.0/src/pii_extract/helper/types.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1116 2023-05-10 16:02:09.000000 pii-extract-base-0.4.0/src/pii_extract/helper/utils.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:42.397250 pii-extract-base-0.4.0/src/pii_extract_base.egg-info/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2048 2023-05-10 18:09:42.000000 pii-extract-base-0.4.0/src/pii_extract_base.egg-info/PKG-INFO
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1858 2023-05-10 18:09:42.000000 pii-extract-base-0.4.0/src/pii_extract_base.egg-info/SOURCES.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        1 2023-05-10 18:09:42.000000 pii-extract-base-0.4.0/src/pii_extract_base.egg-info/dependency_links.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      106 2023-05-10 18:09:42.000000 pii-extract-base-0.4.0/src/pii_extract_base.egg-info/entry_points.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       63 2023-05-10 18:09:42.000000 pii-extract-base-0.4.0/src/pii_extract_base.egg-info/requires.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       12 2023-05-10 18:09:42.000000 pii-extract-base-0.4.0/src/pii_extract_base.egg-info/top_level.txt
```

### Comparing `pii-extract-base-0.3.1/LICENSE` & `pii-extract-base-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pii-extract-base-0.3.1/PKG-INFO` & `pii-extract-base-0.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 Metadata-Version: 2.1
 Name: pii-extract-base
-Version: 0.3.1
+Version: 0.4.0
 Summary: Extraction of PII from text chunks
 Home-page: https://github.com/piisa/pii-extract-base
+Download-URL: https://github.com/piisa/pii-extract-base/tarball/v0.4.0
 Author: Paulo Villegas
 Author-email: paulo.vllgs@gmail.com
 License: Apache
-Download-URL: https://github.com/piisa/pii-extract-base/tarball/v0.3.1
-Description: # Pii Extract Base
-        
-        
-        This repository builds a Python package providing a base library for PII 
-        detection for Source Documents i.e. extraction of PII (Personally Identifiable
-        Information aka Personal Data) items existing in the document.
-        
-        The package itself does **not** implement any PII Detection tasks, it only
-        provides the base infrastructure for the process. Detection tasks must be
-        supplied externally.
-        
-        
-        ## Requirements
-        
-        The package needs
-         * at least Python 3.8
-         * the pii-data base package
-         * one or more pii-extract plugins (to actually do real detection work)
-        
-        ## Usage
-        
-        The package can be used:
-         * As an API, in two flavors: function-based API and object-based API
-         * As a command-line tool
-        
-        For details, see the usage document.
-        
-        
-        ## Building
-        
-        The provided Makefile can be used to process the package:
-         * `make pkg` will build the Python package, creating a file that can be
-           installed with `pip`
-         * `make unit` will launch all unit tests (using pytest, so pytest must be
-           available)
-         * `make install` will install the package in a Python virtualenv. The
-           virtualenv will be chosen as, in this order:
-             - the one defined in the `VENV` environment variable, if it is defined
-             - if there is a virtualenv activated in the shell, it will be used
-             - otherwise, a default is chosen as `/opt/venv/pii` (it will be
-               created if it does not exist)
-        
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
+# Pii Extract Base
+
+
+This repository builds a Python package providing a base library for PII 
+detection for Source Documents i.e. extraction of PII (Personally Identifiable
+Information aka Personal Data) items existing in the document.
+
+The package itself does **not** implement any PII Detection tasks, it only
+provides the base infrastructure for the process. Detection tasks must be
+supplied externally.
+
+
+## Requirements
+
+The package needs
+ * at least Python 3.8
+ * the pii-data base package
+ * one or more pii-extract plugins (to actually do real detection work)
+
+## Usage
+
+The package can be used:
+ * As an API, in two flavors: function-based API and object-based API
+ * As a command-line tool
+
+For details, see the usage document.
+
+
+## Building
+
+The provided Makefile can be used to process the package:
+ * `make pkg` will build the Python package, creating a file that can be
+   installed with `pip`
+ * `make unit` will launch all unit tests (using pytest, so pytest must be
+   available)
+ * `make install` will install the package in a Python virtualenv. The
+   virtualenv will be chosen as, in this order:
+     - the one defined in the `VENV` environment variable, if it is defined
+     - if there is a virtualenv activated in the shell, it will be used
+     - otherwise, a default is chosen as `/opt/venv/pii` (it will be
+       created if it does not exist)
+
+
+
```

### Comparing `pii-extract-base-0.3.1/README.md` & `pii-extract-base-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pii-extract-base-0.3.1/setup.py` & `pii-extract-base-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `pii-extract-base-0.3.1/src/pii_extract/api/file.py` & `pii-extract-base-0.4.0/src/pii_extract/api/file.py`

 * *Files identical despite different names*

### Comparing `pii-extract-base-0.3.1/src/pii_extract/api/processor.py` & `pii-extract-base-0.4.0/src/pii_extract/api/processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Definition of the main PiiProcessor object: a class that 
+Definition of the main PiiProcessor object: a class that
  * creates a PiiTaskCollection and fills it with tasks definitions
  * uses it to build task objects
  * and applies the objects to documents
  * creating a PiiCollection with the results.
 """
 
 import logging
@@ -13,17 +13,17 @@
 from typing import Tuple, List, Dict, Iterable, Union
 
 from pii_data.types import PiiEntityInfo, PiiEntity, PiiDetector, PiiCollection
 from pii_data.types.doc import SrcDocument, DocumentChunk
 from pii_data.helper.exception import ProcException, InvArgException
 
 from ..helper.logger import PiiLogger
-from ..gather.collector import JsonTaskCollector
 from ..build.task import PiiTaskInfo
-from ..build.collection import get_task_collection, TYPE_TASKENUM
+from ..gather.collection import get_task_collection, TYPE_TASKENUM
+from ..gather.collection.sources import JsonTaskCollector
 
 
 
 TYPE_LANG = Union[str, Iterable[str]]
 
 def check_language(lang1: TYPE_LANG, lang2: TYPE_LANG) -> bool:
     """
@@ -37,31 +37,50 @@
         lang2 = [lang2]
     return bool(set(lang1) & set(lang2))
 
 
 
 class PiiCollectionBuilder(PiiCollection):
     """
-    A small varianto of the PiiCollection class, in which the add() method
-    accepts a PiiTaskInfo object instead of a PiiDetector, and builds it
+    A small variant of the PiiCollection class, with a couple of additional
+    convenience methods to add PiiEntity instances
+      - add_detector_fields(), which accepts a PiiTaskInfo object instead of a
+        PiiDetector, and builds the PiiDetector
+      - add_collection(), which adds all pii in a collection to another
     """
 
-    def add(self, pii: PiiEntity, info: Union[PiiTaskInfo, Dict], method: str):
+    def add_detector_fields(self, pii: PiiEntity,
+                            info: Union[PiiTaskInfo, Dict], method: str = None):
         """
+        Add a detector, given its fields
          :param pii: the detected Pii entity
          :param info: a PiiTaskInfo (or equivalent dict) for the task that
            did the detection
+         :param method: task detector method, if not found in `info`
         """
         if isinstance(info, PiiTaskInfo):
             info = info.asdict()
-        kwargs = {k: info.get(k) for k in ("source", "name", "version")}
-        detector = PiiDetector(**kwargs, method=method)
+        kwargs = {k: info.get(k)
+                  for k in ("source", "name", "version", "method")}
+        if method:
+            kwargs["method"] = method
+        detector = PiiDetector(**kwargs)
         super().add(pii, detector)
 
 
+    def add_collection(self, piic: PiiCollection) -> int:
+        """
+        Add all PiiEntity instances in a collection to another.
+        If needed, add also the detectors
+        """
+        num = 0
+        for num, pii in enumerate(piic, start=1):
+            self.add(pii, piic.get_detector(pii.fields["detector"]))
+        return num
+
 
 # --------------------------------------------------------------------------
 
 
 class PiiProcessor:
 
     def __init__(self, config: Dict = None, skip_plugins: bool = False,
@@ -165,15 +184,15 @@
 
         # Select the list of tasks to apply, based on the chunk language
         lang = (chunk.context or {}).get("lang") or default_lang
         if lang:
             tasks = self._tasks.get(lang, [])
         else:
             if len(self._tasks) > 1:
-                raise InvArgException("no language chosen for tasks")
+                raise InvArgException("must select a language for tasks")
             tasks = next(iter(self._tasks.values()))
 
         piilist = []
         processed = set()
         for task in tasks:
 
             # See if we have already applied this task to the chunk
@@ -187,15 +206,15 @@
                     pii.fields["process"] = {"stage": "detection"}
                 piilist.append((pii, task.task_info, task.get_method(pii.info)))
                 self._stats["num"]["entities"] += 1
                 self._stats["entities"][pii.info.pii.name] += 1
 
         # Add all entities to the collection, sorted by position in chunk
         for pii in sorted(piilist, key=lambda p: p[0].pos):
-            piic.add(*pii)
+            piic.add_detector_fields(*pii)
 
         return len(piilist)
 
 
     def detect(self, doc: SrcDocument,
                chunk_context: bool = False) -> PiiCollection:
         """
```

### Comparing `pii-extract-base-0.3.1/src/pii_extract/app/detect.py` & `pii-extract-base-0.4.0/src/pii_extract/app/detect.py`

 * *Files identical despite different names*

### Comparing `pii-extract-base-0.3.1/src/pii_extract/app/task_info.py` & `pii-extract-base-0.4.0/src/pii_extract/app/task_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from textwrap import TextWrapper
 
 from typing import List, TextIO
 
 from pii_data.helper.config import load_config
 
 from .. import VERSION
-from ..gather.collector import PluginTaskCollector
+from ..gather.collection.sources import PluginTaskCollector
 from ..api import PiiProcessor
 from ..api.file import print_tasks
 
 
 def print_plugins(args: argparse.Namespace, out: TextIO, debug: bool = False):
     """
     List the plugins
```

### Comparing `pii-extract-base-0.3.1/src/pii_extract/build/build.py` & `pii-extract-base-0.4.0/src/pii_extract/build/build.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 """
 Build task objects
 """
 
-from typing import Dict
+from typing import Dict, Any
 
 from pii_data.helper.exception import InvArgException
 
 from .task import BasePiiTask, CallablePiiTask, RegexPiiTask
 
 
+def is_pii_class(obj: Any) -> bool:
+    """
+    Return if an object is a PiiTask class object
+    """
+    return isinstance(obj, type) and issubclass(obj, BasePiiTask)
+
+
 def build_task(taskd: Dict) -> BasePiiTask:
     """
     Build a task object from its task definition
     """
     # Prepare standard arguments
     try:
         odef = taskd["obj"]
```

### Comparing `pii-extract-base-0.3.1/src/pii_extract/build/collection/get.py` & `pii-extract-base-0.4.0/src/pii_extract/gather/collection/get.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from typing import Dict
 
 from pii_data.helper.logger import PiiLogger
 
 from ...defs import FMT_CONFIG_TASKS
-from ...gather.collector import PluginTaskCollector, JsonTaskCollector
+from .sources import PluginTaskCollector, JsonTaskCollector
 from .task_collection import PiiTaskCollection
 
 
 LOGGER = None
 
 def get_task_collection(config: Dict = None, load_plugins: bool = True,
                         debug: bool = False) -> PiiTaskCollection:
```

### Comparing `pii-extract-base-0.3.1/src/pii_extract/build/collection/task_collection.py` & `pii-extract-base-0.4.0/src/pii_extract/gather/collection/task_collection.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,155 +1,94 @@
 """
-Build collections of tasks
+Build collections of task definitions
 """
-from typing import Dict, List, Iterable, Union, Set
 
-from pii_data.helper.exception import InvArgException
+from typing import Dict, List, Iterable
+
 from pii_data.helper.logger import PiiLogger
-from pii_data.types import PiiEnum
 
 from ...defs import LANG_ANY, COUNTRY_ANY
-from ...gather.collector.base import BaseTaskCollector
-from ...gather.parser import parse_task_descriptor
 from ...helper.utils import field_set, taskd_field, union_sets
-from ..task import BasePiiTask
-from ..build import build_task
-
-
-TYPE_TASKENUM = Union[PiiEnum, List[PiiEnum], str, List[str]]
-TYPE_PIID = Union[Dict, List[Dict]]
-
-# --------------------------------------------------------------------------
-
-
-def ensure_enum(pii: Union[str, PiiEnum]) -> PiiEnum:
-    """
-    Ensure a task specification is a PiiEnum
-    """
-    try:
-        return pii if isinstance(pii, PiiEnum) else PiiEnum[str(pii).upper()]
-    except KeyError:
-        raise InvArgException("unknown pii type: {}", pii)
-
-
-def ensure_enum_list(pii: TYPE_TASKENUM) -> List[PiiEnum]:
-    """
-    Ensure a task specification is a list of PiiEnum
-    """
-    if isinstance(pii, (list, tuple)):
-        return [ensure_enum(t) for t in pii]
-    else:
-        return [ensure_enum(pii)]
-
+from ...build.task import BasePiiTask
+from ...build import build_task
+from ..parser import parse_task_descriptor
+from .sources.base import BaseTaskCollector
+from .utils import ensure_enum_list, filter_piid, TYPE_TASKENUM
 
-def piid_ok(piid: Dict, lang: Set[str], country: Set[str],
-            pii: Set[PiiEnum]) -> bool:
-    """
-    Decide if a PII descriptor agrees with a language/country filter
-    """
-    if pii and not pii & taskd_field(piid, "pii"):
-        return False
-
-    if lang and not lang & taskd_field(piid, "lang"):
-        return False
-
-    # Country is different: the task descriptor may not have it
-    if country:
-        task_country = taskd_field(piid, "country")
-        if task_country and not country & task_country:
-            return False
-
-    return True
-
-
-def filter_piid(piid: TYPE_PIID, lang: Set[str], country: Set[str] = None,
-                pii: Set[PiiEnum] = None) -> TYPE_PIID:
-    """
-    Select from a (possibly multiple) PII descriptor the items that agree with
-    a PiiEnum/language/country filter
-    """
-    if not lang and not country and not pii:
-        return piid
-
-    if isinstance(piid, dict):
-        return piid if piid_ok(piid, lang, country, pii) else None
-    else:
-        return [p for p in piid if piid_ok(p, lang, country, pii)]
-
-
-# --------------------------------------------------------------------------
 
 
 class PiiTaskCollection:
     """
-    The object holding the set of task descriptors, which can then be
+    An object holding a set of task definitions, which can then be
     instantiated into task objects
     """
 
     def __init__(self, debug: bool = False):
         """
         """
-        self._task_dsc = []
+        self.task_def = []
         self._lang = None
         self._countries = None
         self._log = PiiLogger(__name__, debug)
         self._num = 0
 
 
     def __repr__(self) -> str:
         return f"<PiiTaskCollection #{len(self)}>"
 
 
     def __len__(self) -> int:
         """
-        Return the number of gathered tasks descriptors
+        Return the number of gathered tasks definitions
         """
-        return len(self._task_dsc)
+        return len(self.task_def)
 
 
     def num(self, built: bool = False) -> int:
         """
-        Return the number of tasks, either gathered or built
+        Return the number of tasks, either
+          - the number available task definitions
+          - the number of built task objects
         """
-        return self._num if built else len(self._task_dsc)
+        return self._num if built else len(self.task_def)
 
 
     def add_collector(self, tc: BaseTaskCollector) -> int:
         """
         Fetch all raw tasks descriptors gathered by a task collector,
-        convert them to task definitions and add them to the list
+        convert them to task definitions and add them to the object list
         """
         # Reset list of languages/countries so that they will be computed again
         self._lang = self._countries = None
 
         # Append all tasks gathered by the collector
         self._log(". gather-tasks from: %s", tc)
         num = 0
         for num, taskd in enumerate(tc.gather_tasks(), start=1):
-            self._task_dsc.append(parse_task_descriptor(taskd))
+            self.task_def.append(parse_task_descriptor(taskd))
         return num
 
 
     def language_list(self) -> List[str]:
         """
-        Return all languages that have task descriptors
+        Return all languages that have task definitions
         """
         if self._lang is None:
             self._lang = union_sets(taskd_field(t["piid"], "lang")
-                                    for t in self._task_dsc)
+                                    for t in self.task_def)
         return self._lang
 
 
     def country_list(self) -> List[str]:
         """
         Return all countries that have task descriptors
         """
         if self._countries is None:
             self._countries = union_sets(taskd_field(t["piid"], "country")
-                                         for t in self._task_dsc)
+                                         for t in self.task_def)
         return self._countries
 
 
     def taskdef_list(self, lang: Iterable[str] = None,
                      country: Iterable[str] = None, pii: TYPE_TASKENUM = None,
                      add_any: bool = True) -> Iterable[Dict]:
         """
@@ -174,16 +113,16 @@
                 lang.add(LANG_ANY)
         if country:
             country = field_set(country)
             if add_any:
                 country.add(COUNTRY_ANY)
         pii = set(ensure_enum_list(pii)) if pii is not None else None
 
-        # Traverse the list of task descriptors and apply the filters
-        for taskd in self._task_dsc:
+        # Traverse the list of task definitions and apply the filters
+        for taskd in self.task_def:
 
             # If no lang/country filter, we're done
             if not lang and not country and not pii:
                 yield taskd
                 continue
 
             # Filter by language and/or country and/or PII
@@ -197,15 +136,21 @@
 
 
     def build_tasks(self, lang: str = None, country: Iterable[str] = None,
                     pii: TYPE_TASKENUM = None,
                     add_any: bool = True) -> Iterable[BasePiiTask]:
         """
         Build a list of tasks from their definitions stored in the collection.
-        Return the list of built task objects.
+          :param lang: select tasks to build for these languages
+          :param country: select tasks to build for these countries
+          :param country: select tasks to build for these PII types
+          :param add_any: when restricting language/country, add also language-
+             and country-independent tasks
+          :return: an iterable yielding the built task objects.
+
         """
         # Get the list of tasks to build
         tasklist = self.taskdef_list(lang, country, pii=pii, add_any=add_any)
 
         # Build and return them
         built = set()
         for td in tasklist:
```

### Comparing `pii-extract-base-0.3.1/src/pii_extract/build/task/base.py` & `pii-extract-base-0.4.0/src/pii_extract/build/task/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,27 +52,29 @@
           :param task: a task info dictionary
           :param pii: a PII descriptor dictionary
         """
         #print("INIT", task, pii)
 
         if not isinstance(pii, dict):
             raise InvArgException("invalid pii argument to PiiTask")
+        if task is None:
+            task = {}
 
         # Add context & method
-        self.method = pii.get("method")
+        self.method = pii.get("method") or task.get("method")
         context = pii.get("context")
         self.context = context_spec(context) if context else None
 
         # Fetch the options to be stored in the info subobject
         pii_info = {k: v for k, v in pii.items()
                     if k not in ("method", "extra", "context")}
 
         # Store options
         self.pii_info = PiiEntityInfo(**pii_info)
-        self.task_info = PiiTaskInfo(**(task or {}))
+        self.task_info = PiiTaskInfo(**task)
         self.debug = debug
 
 
     def get_method(self, pii: Any, **kwargs):
         """
         Return the 'method' metadata field
         """
```

### Comparing `pii-extract-base-0.3.1/src/pii_extract/build/task/callable.py` & `pii-extract-base-0.4.0/src/pii_extract/build/task/callable.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pii_data.types.doc import DocumentChunk
 
 from .base import BasePiiTask
 
 
 class CallablePiiTask(BasePiiTask):
     """
-    A wrapper for a PII implemented as a function
+    A wrapper for a PII detector implemented as a function.
     Since it inherits from BasePiiTask, it will automatically apply context
     validation to the function results, if a suitable context argument is added
     """
 
     def __init__(self, call: Callable, extra_kwargs=None, **kwargs):
         """
          :param call: callable to execute
```

### Comparing `pii-extract-base-0.3.1/src/pii_extract/build/task/multi.py` & `pii-extract-base-0.4.0/src/pii_extract/build/task/multi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Define the BaseMultiPiiTask base class
+Define the BaseMultiPiiTask base subclass
 """
 
 from typing import Union, Dict, List, Iterable
 
 from pii_data.types import PiiEnum, PiiEntityInfo, PiiEntity
 
 from ...helper.exception import InvArgException
```

### Comparing `pii-extract-base-0.3.1/src/pii_extract/build/task/regex.py` & `pii-extract-base-0.4.0/src/pii_extract/build/task/regex.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 Define the RegexPiiTask subclass
 """
+
 import regex
 
 from typing import Iterable
 
 from pii_data.types import PiiEntity
 from pii_data.types.doc import DocumentChunk
 
 from .base import BasePiiTask
 
 
 class RegexPiiTask(BasePiiTask):
     """
-    A wrapper for a PII implemented as a regex pattern
+    A wrapper for a PII implemented as a regex pattern.
     Instead of the standard "re" package it uses the "regex" package (in
     backwards-compatible mode).
     Since it inherits from BasePiiTask, it will automatically apply context
     validation after regex matching, if a suitable context argument is added
     """
 
     def __init__(self, pattern: str, **kwargs):
```

### Comparing `pii-extract-base-0.3.1/src/pii_extract/gather/collector/base.py` & `pii-extract-base-0.4.0/src/pii_extract/gather/collection/sources/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 """
 
 from typing import Dict, List, Iterable
 
 from pii_data.helper.exception import UnimplementedException
 from pii_data.helper.logger import PiiLogger
 
-from ...helper.types import TYPE_STR_LIST
-from ...helper.utils import union_sets, taskd_field
+from pii_extract.helper.types import TYPE_STR_LIST
+from pii_extract.helper.utils import union_sets, taskd_field
 
 
 
 # --------------------------------------------------------------------------
 
 class BaseTaskCollector:
     """
```

### Comparing `pii-extract-base-0.3.1/src/pii_extract/gather/collector/folder.py` & `pii-extract-base-0.4.0/src/pii_extract/gather/collection/sources/folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
-Build lists of PiiTask specifications by traversing folders
+Build lists of PiiTask descriptors by traversing folders
 """
 
 import importlib
 from pathlib import Path
 from itertools import chain
 
 from typing import Dict, List, Iterable
 
 from pii_data.types import PiiEnum
 from pii_data.helper.exception import ConfigException
-from ...defs import LANG_ANY, COUNTRY_ANY
-from ...helper.utils import union_sets
-from ..parser import RawTaskDefaults
-from ..parser.defs import FIELD_CLASS
-from ..parser.parser import piienum
+
+from pii_extract.defs import LANG_ANY, COUNTRY_ANY
+from pii_extract.helper.utils import union_sets
+from pii_extract.gather.parser.defs import FIELD_CLASS
+from pii_extract.gather.parser.parser import piienum
 from .base import BaseTaskCollector
+from .utils import RawTaskDefaults
 
 # For folder defs: name of the Python list holding pii tasks inside a module
 _LISTNAME = "PII_TASKS"
 
 
 # --------------------------------------------------------------------------
```

### Comparing `pii-extract-base-0.3.1/src/pii_extract/gather/collector/json.py` & `pii-extract-base-0.4.0/src/pii_extract/gather/collection/sources/json.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
-Build lists of PiiTask specifications by reading a JSON definition
+Build lists of PiiTask descriptors by reading a JSON definition
 """
 
 from typing import Dict, Iterable, Union
 
 from pii_data.helper.exception import InvArgException, ConfigException
 from pii_data.helper.config import load_config, TYPE_CONFIG
 from pii_data.defs import FMT_CONFIG_PREFIX
 
-from ...defs import FMT_CONFIG_TASKS
-from ...helper.types import TYPE_STR_LIST
-from ...helper.utils import taskd_field, field_set
-from ..parser import RawTaskDefaults
+from pii_extract.defs import FMT_CONFIG_TASKS
+from pii_extract.helper.types import TYPE_STR_LIST
+from pii_extract.helper.utils import taskd_field, field_set
+from .utils import RawTaskDefaults
 from .base import BaseTaskCollector
 
 
 # --------------------------------------------------------------------------
 
 
 class JsonTaskCollector(BaseTaskCollector):
```

### Comparing `pii-extract-base-0.3.1/src/pii_extract/gather/collector/plugin.py` & `pii-extract-base-0.4.0/src/pii_extract/gather/collection/sources/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 A task collector that searches for Python entry points that correspond to
-pii-extract plugins
+pii-extract plugins, providing lists of PiiTask descriptors
 
 A plugin must have 
   * an entry point of group PII_EXTRACT_PLUGIN_ID
   * the entry point must be a class with:
      - a constructor with a `config` argument, an optional "debug" keyword
        argument, and possibly additional arguments
      - a `get_plugin_tasks()` method delivering an iterable of *raw* task
@@ -15,17 +15,17 @@
 
 from importlib.metadata import entry_points
 
 from typing import Dict, List, Iterable
 
 from pii_data.helper.exception import ProcException
 
-from ...defs import FMT_CONFIG_PLUGIN
-from ..parser import RawTaskDefaults
-from ...helper.types import TYPE_STR_LIST
+from pii_extract.defs import FMT_CONFIG_PLUGIN
+from pii_extract.helper.types import TYPE_STR_LIST
+from .utils import RawTaskDefaults
 from .base import BaseTaskCollector
 from .defs import PII_EXTRACT_PLUGIN_ID
 
 
 # --------------------------------------------------------------------------
```

### Comparing `pii-extract-base-0.3.1/src/pii_extract/gather/parser/parser.py` & `pii-extract-base-0.4.0/src/pii_extract/gather/parser/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
-Build full task descriptors from raw ones
+Build full task definitions from raw task descriptors.
 """
 
 import re
 import importlib
 from inspect import cleandoc
 from dataclasses import fields as dataclass_fields
 
 from typing import Dict, Tuple, Callable, Type, Union, Iterable, List
 
 from pii_data.types import PiiEnum
 from pii_data.helper.exception import InvArgException
 
+from ...build import is_pii_class
 from ...build.task import BasePiiTask, PiiTaskInfo
 from .defs import FIELD_CLASS, FIELD_IMP
-from .utils import _is_pii_class, InvPiiTask
+from .utils import InvPiiTask
 
 
 TYPE_TASKD_LIST = Iterable[Dict]
 
 
 # --------------------------------------------------------------------------
 
@@ -58,15 +59,15 @@
     info = {f: raw_taskd[f]
             for f in map(lambda df: df.name, dataclass_fields(PiiTaskInfo))
             if f in raw_taskd}
 
     # Check task class
     task_type = raw_taskd.get(FIELD_CLASS)
     if task_type is None:
-        if _is_pii_class(raw_taskd.get(FIELD_IMP)):
+        if is_pii_class(raw_taskd.get(FIELD_IMP)):
             task_type = "piitask"
         else:
             raise InvPiiTask("missing field: {}", FIELD_CLASS)
     task_type = str(task_type).lower()
     if task_type not in ("piitask", "callable", "re", "regex", "regex-external"):
         raise InvPiiTask("unsupported task class: {}", task_type)
     task = {FIELD_CLASS: task_type}
@@ -84,15 +85,15 @@
     if task_type == "regex-external":
         task[FIELD_CLASS] = "regex"
 
     if task[FIELD_CLASS] == "regex" and not isinstance(task[FIELD_IMP], str):
         raise InvPiiTask("regex spec should be a string")
     elif task[FIELD_CLASS] == "callable" and not isinstance(task[FIELD_IMP], Callable):
         raise InvPiiTask("callable spec should be a callable")
-    elif task[FIELD_CLASS] == "piitask" and not _is_pii_class(task[FIELD_IMP]):
+    elif task[FIELD_CLASS] == "piitask" and not is_pii_class(task[FIELD_IMP]):
         raise InvPiiTask("class spec should be a PiiTask object")
 
     if "kwargs" in raw_taskd:
         task["kwargs"] = raw_taskd["kwargs"]
 
     # Add source, version from defaults, if not there yet
     if defaults:
```

### Comparing `pii-extract-base-0.3.1/src/pii_extract/gather/parser/utils.py` & `pii-extract-base-0.4.0/src/pii_extract/gather/collection/sources/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,20 @@
-"""
-Some utility functions/classes to reshape raw task descriptors
-"""
-
 from collections.abc import Iterable as AbcIterable
-from typing import Dict, Iterable, Any
-
-from pii_data.types import PiiEnum
-from pii_data.helper.exception import InvArgException
 
-from ...build.task import BasePiiTask
-from . import defs
+from typing import Dict, Iterable
 
+from pii_data.types import PiiEnum
 
-class InvPiiTask(InvArgException):
-    """
-    An exception signaling an invalid Pii Task descriptor
-    """
-    pass
-
+from pii_extract.build import is_pii_class
+from pii_extract.gather.parser import defs
+from pii_extract.gather.parser.utils import InvPiiTask
 
 # ------------------------------------------------------------------------
 
 
-def _is_pii_class(obj: Any) -> bool:
-    return isinstance(obj, type) and issubclass(obj, BasePiiTask)
-
-
 def normalize_rawtaskd(raw: defs.TYPE_TASKD) -> Dict:
     """
     Ensure a raw task descriptor is a dictionary with a "pii" field
     """
     # A full descriptor
     if isinstance(raw, dict):
 
@@ -47,15 +32,15 @@
         return raw
 
     # A simplified descriptor. First check it
     if len(raw) != 2 and (len(raw) != 3 or not isinstance(raw[2], str)):
         raise defs.InvPiiTask("invalid simplified task spec")
 
     # Task class
-    task_class = ("PiiTask" if _is_pii_class(raw[1])
+    task_class = ("PiiTask" if is_pii_class(raw[1])
                   else "callable" if callable(raw[1])
                   else "regex" if isinstance(raw[1], str)
                   else None)
     # Build the dict
     td = {
         defs.FIELD_CLASS: task_class,
         defs.FIELD_IMP: raw[1],
@@ -64,15 +49,14 @@
     if len(raw) > 2:
         td["pii"][0]["subtype"] = raw[2]
     return td
 
 
 # ------------------------------------------------------------------------
 
-
 def _add_defaults(orig: Dict, defaults: Dict) -> Dict:
     return {**defaults, **orig}
 
 
 class RawTaskDefaults:
     """
     A class to add defaults to missing fields in a raw task descriptor
```

### Comparing `pii-extract-base-0.3.1/src/pii_extract/helper/context.py` & `pii-extract-base-0.4.0/src/pii_extract/helper/context.py`

 * *Files identical despite different names*

### Comparing `pii-extract-base-0.3.1/src/pii_extract/helper/normalizer.py` & `pii-extract-base-0.4.0/src/pii_extract/helper/normalizer.py`

 * *Files identical despite different names*

### Comparing `pii-extract-base-0.3.1/src/pii_extract/helper/utils.py` & `pii-extract-base-0.4.0/src/pii_extract/helper/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,23 +14,24 @@
     return sorted(all_values)
 
 
 def field_set(value: Union[str, Iterable[str], None]) -> Set[str]:
     """
     Return a (possibly multiple) field as a set of values
     """
-    return set([value] if isinstance(value, str) else value) if value else set()
+    return set([value] if isinstance(value, (int, str))
+               else value) if value else set()
 
 
-def taskd_field(taskd: Dict, field: str = "lang") -> Set[str]:
+def taskd_field(taskd: Union[Dict, Iterable[Dict]],
+                field: str = "lang") -> Set[str]:
     """
-    Get the a field from a descriptor dictionary
-     :param taskd: the task descriptor dictionary
+    Get the a field from a descriptor dictionary as a set of values
+     :param taskd: the task descriptor dictionary (or list of dictionaries)
      :param field: the field to fetch
-     :param as_set: return it as a set of values
      :return: a set of field values
     """
     if isinstance(taskd, dict):
         lang = taskd.get(field)
         return field_set(lang)
     else:
         allsets = (taskd_field(s, field) for s in taskd)
```

### Comparing `pii-extract-base-0.3.1/src/pii_extract_base.egg-info/PKG-INFO` & `pii-extract-base-0.4.0/src/pii_extract_base.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 Metadata-Version: 2.1
 Name: pii-extract-base
-Version: 0.3.1
+Version: 0.4.0
 Summary: Extraction of PII from text chunks
 Home-page: https://github.com/piisa/pii-extract-base
+Download-URL: https://github.com/piisa/pii-extract-base/tarball/v0.4.0
 Author: Paulo Villegas
 Author-email: paulo.vllgs@gmail.com
 License: Apache
-Download-URL: https://github.com/piisa/pii-extract-base/tarball/v0.3.1
-Description: # Pii Extract Base
-        
-        
-        This repository builds a Python package providing a base library for PII 
-        detection for Source Documents i.e. extraction of PII (Personally Identifiable
-        Information aka Personal Data) items existing in the document.
-        
-        The package itself does **not** implement any PII Detection tasks, it only
-        provides the base infrastructure for the process. Detection tasks must be
-        supplied externally.
-        
-        
-        ## Requirements
-        
-        The package needs
-         * at least Python 3.8
-         * the pii-data base package
-         * one or more pii-extract plugins (to actually do real detection work)
-        
-        ## Usage
-        
-        The package can be used:
-         * As an API, in two flavors: function-based API and object-based API
-         * As a command-line tool
-        
-        For details, see the usage document.
-        
-        
-        ## Building
-        
-        The provided Makefile can be used to process the package:
-         * `make pkg` will build the Python package, creating a file that can be
-           installed with `pip`
-         * `make unit` will launch all unit tests (using pytest, so pytest must be
-           available)
-         * `make install` will install the package in a Python virtualenv. The
-           virtualenv will be chosen as, in this order:
-             - the one defined in the `VENV` environment variable, if it is defined
-             - if there is a virtualenv activated in the shell, it will be used
-             - otherwise, a default is chosen as `/opt/venv/pii` (it will be
-               created if it does not exist)
-        
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
+# Pii Extract Base
+
+
+This repository builds a Python package providing a base library for PII 
+detection for Source Documents i.e. extraction of PII (Personally Identifiable
+Information aka Personal Data) items existing in the document.
+
+The package itself does **not** implement any PII Detection tasks, it only
+provides the base infrastructure for the process. Detection tasks must be
+supplied externally.
+
+
+## Requirements
+
+The package needs
+ * at least Python 3.8
+ * the pii-data base package
+ * one or more pii-extract plugins (to actually do real detection work)
+
+## Usage
+
+The package can be used:
+ * As an API, in two flavors: function-based API and object-based API
+ * As a command-line tool
+
+For details, see the usage document.
+
+
+## Building
+
+The provided Makefile can be used to process the package:
+ * `make pkg` will build the Python package, creating a file that can be
+   installed with `pip`
+ * `make unit` will launch all unit tests (using pytest, so pytest must be
+   available)
+ * `make install` will install the package in a Python virtualenv. The
+   virtualenv will be chosen as, in this order:
+     - the one defined in the `VENV` environment variable, if it is defined
+     - if there is a virtualenv activated in the shell, it will be used
+     - otherwise, a default is chosen as `/opt/venv/pii` (it will be
+       created if it does not exist)
+
+
+
```

### Comparing `pii-extract-base-0.3.1/src/pii_extract_base.egg-info/SOURCES.txt` & `pii-extract-base-0.4.0/src/pii_extract_base.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -9,29 +9,31 @@
 src/pii_extract/api/file.py
 src/pii_extract/api/processor.py
 src/pii_extract/app/__init__.py
 src/pii_extract/app/detect.py
 src/pii_extract/app/task_info.py
 src/pii_extract/build/__init__.py
 src/pii_extract/build/build.py
-src/pii_extract/build/collection/__init__.py
-src/pii_extract/build/collection/get.py
-src/pii_extract/build/collection/task_collection.py
 src/pii_extract/build/task/__init__.py
 src/pii_extract/build/task/base.py
 src/pii_extract/build/task/callable.py
 src/pii_extract/build/task/multi.py
 src/pii_extract/build/task/regex.py
 src/pii_extract/gather/__init__.py
-src/pii_extract/gather/collector/__init__.py
-src/pii_extract/gather/collector/base.py
-src/pii_extract/gather/collector/defs.py
-src/pii_extract/gather/collector/folder.py
-src/pii_extract/gather/collector/json.py
-src/pii_extract/gather/collector/plugin.py
+src/pii_extract/gather/collection/__init__.py
+src/pii_extract/gather/collection/get.py
+src/pii_extract/gather/collection/task_collection.py
+src/pii_extract/gather/collection/utils.py
+src/pii_extract/gather/collection/sources/__init__.py
+src/pii_extract/gather/collection/sources/base.py
+src/pii_extract/gather/collection/sources/defs.py
+src/pii_extract/gather/collection/sources/folder.py
+src/pii_extract/gather/collection/sources/json.py
+src/pii_extract/gather/collection/sources/plugin.py
+src/pii_extract/gather/collection/sources/utils.py
 src/pii_extract/gather/parser/__init__.py
 src/pii_extract/gather/parser/defs.py
 src/pii_extract/gather/parser/parser.py
 src/pii_extract/gather/parser/utils.py
 src/pii_extract/helper/__init__.py
 src/pii_extract/helper/context.py
 src/pii_extract/helper/exception.py
```

