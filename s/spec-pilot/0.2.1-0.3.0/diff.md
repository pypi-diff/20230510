# Comparing `tmp/spec_pilot-0.2.1.tar.gz` & `tmp/spec-pilot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spec_pilot-0.2.1.tar", last modified: Fri Apr 28 02:17:45 2023, max compression
+gzip compressed data, was "spec-pilot-0.3.0.tar", last modified: Wed May 10 03:57:34 2023, max compression
```

## Comparing `spec_pilot-0.2.1.tar` & `spec-pilot-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:17:45.889836 spec_pilot-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 02:17:32.000000 spec_pilot-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-28 02:17:45.889836 spec_pilot-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-28 02:17:32.000000 spec_pilot-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 02:17:45.889836 spec_pilot-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-28 02:17:32.000000 spec_pilot-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:17:45.889836 spec_pilot-0.2.1/spec_pilot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-28 02:17:45.000000 spec_pilot-0.2.1/spec_pilot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-28 02:17:45.000000 spec_pilot-0.2.1/spec_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 02:17:45.000000 spec_pilot-0.2.1/spec_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-28 02:17:45.000000 spec_pilot-0.2.1/spec_pilot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-28 02:17:45.000000 spec_pilot-0.2.1/spec_pilot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-28 02:17:45.000000 spec_pilot-0.2.1/spec_pilot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:17:45.889836 spec_pilot-0.2.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-28 02:17:32.000000 spec_pilot-0.2.1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-28 02:17:32.000000 spec_pilot-0.2.1/src/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-28 02:17:32.000000 spec_pilot-0.2.1/src/spec_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-28 02:17:32.000000 spec_pilot-0.2.1/src/spec_pilot.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-28 02:17:32.000000 spec_pilot-0.2.1/src/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:57:34.826766 spec-pilot-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-10 03:57:14.000000 spec-pilot-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-10 03:57:34.826766 spec-pilot-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-10 03:57:14.000000 spec-pilot-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:57:34.826766 spec-pilot-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-10 03:57:14.000000 spec-pilot-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:57:34.822765 spec-pilot-0.3.0/spec_pilot/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 03:57:14.000000 spec-pilot-0.3.0/spec_pilot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-10 03:57:14.000000 spec-pilot-0.3.0/spec_pilot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-10 03:57:14.000000 spec-pilot-0.3.0/spec_pilot/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-10 03:57:14.000000 spec-pilot-0.3.0/spec_pilot/language_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-10 03:57:14.000000 spec-pilot-0.3.0/spec_pilot/prompt_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-10 03:57:14.000000 spec-pilot-0.3.0/spec_pilot/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:57:34.822765 spec-pilot-0.3.0/spec_pilot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-10 03:57:34.000000 spec-pilot-0.3.0/spec_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-10 03:57:34.000000 spec-pilot-0.3.0/spec_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 03:57:34.000000 spec-pilot-0.3.0/spec_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 03:57:34.000000 spec-pilot-0.3.0/spec_pilot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-10 03:57:34.000000 spec-pilot-0.3.0/spec_pilot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 03:57:34.000000 spec-pilot-0.3.0/spec_pilot.egg-info/top_level.txt
```

### Comparing `spec_pilot-0.2.1/LICENSE` & `spec-pilot-0.3.0/LICENSE`

 * *Files identical despite different names*

