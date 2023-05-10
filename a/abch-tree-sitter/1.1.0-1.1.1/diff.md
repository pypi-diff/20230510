# Comparing `tmp/abch_tree_sitter-1.1.0.tar.gz` & `tmp/abch_tree_sitter-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abch_tree_sitter-1.1.0.tar", last modified: Mon Apr 17 08:59:50 2023, max compression
+gzip compressed data, was "abch_tree_sitter-1.1.1.tar", last modified: Wed May 10 08:52:05 2023, max compression
```

## Comparing `abch_tree_sitter-1.1.0.tar` & `abch_tree_sitter-1.1.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:50.943534 abch_tree_sitter-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-17 08:59:39.000000 abch_tree_sitter-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-17 08:59:39.000000 abch_tree_sitter-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-04-17 08:59:50.943534 abch_tree_sitter-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-04-17 08:59:39.000000 abch_tree_sitter-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:50.935535 abch_tree_sitter-1.1.0/abch_tree_sitter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-04-17 08:59:50.000000 abch_tree_sitter-1.1.0/abch_tree_sitter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-17 08:59:50.000000 abch_tree_sitter-1.1.0/abch_tree_sitter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:59:50.000000 abch_tree_sitter-1.1.0/abch_tree_sitter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 08:59:50.000000 abch_tree_sitter-1.1.0/abch_tree_sitter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-17 08:59:39.000000 abch_tree_sitter-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 08:59:50.943534 abch_tree_sitter-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-17 08:59:39.000000 abch_tree_sitter-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:50.935535 abch_tree_sitter-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    35192 2023-04-17 08:59:39.000000 abch_tree_sitter-1.1.0/tests/test_tree_sitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:50.935535 abch_tree_sitter-1.1.0/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-17 08:59:39.000000 abch_tree_sitter-1.1.0/tree_sitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64088 2023-04-17 08:59:39.000000 abch_tree_sitter-1.1.0/tree_sitter/binding.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:50.935535 abch_tree_sitter-1.1.0/tree_sitter/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:50.935535 abch_tree_sitter-1.1.0/tree_sitter/core/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:50.935535 abch_tree_sitter-1.1.0/tree_sitter/core/lib/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:50.939535 abch_tree_sitter-1.1.0/tree_sitter/core/lib/include/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (123)    30214 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/include/tree_sitter/api.h
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/include/tree_sitter/parser.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:50.939535 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/alloc.c
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/alloc.h
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/array.h
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/atomic.h
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/clock.h
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/error_costs.h
--rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/get_changed_ranges.c
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/get_changed_ranges.h
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/host.h
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/language.c
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/language.h
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/length.h
--rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/lexer.c
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/lexer.h
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/lib.c
--rw-r--r--   0 runner    (1001) docker     (123)    19287 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/node.c
--rw-r--r--   0 runner    (1001) docker     (123)    69800 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/parser.c
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/point.h
--rw-r--r--   0 runner    (1001) docker     (123)   139078 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/query.c
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/reduce_action.h
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/reusable_node.h
--rw-r--r--   0 runner    (1001) docker     (123)    27418 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/stack.c
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/stack.h
--rw-r--r--   0 runner    (1001) docker     (123)    34154 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/subtree.c
--rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/subtree.h
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/tree.c
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/tree.h
--rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/tree_cursor.c
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/tree_cursor.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:59:50.943534 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/unicode/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/unicode/ICU_SHA
--rw-r--r--   0 runner    (1001) docker     (123)    21001 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/unicode/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/unicode/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/unicode/ptypes.h
--rw-r--r--   0 runner    (1001) docker     (123)    14865 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/unicode/umachine.h
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/unicode/urename.h
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/unicode/utf.h
--rw-r--r--   0 runner    (1001) docker     (123)    23878 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/unicode/utf16.h
--rw-r--r--   0 runner    (1001) docker     (123)    31698 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/unicode/utf8.h
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-17 08:59:42.000000 abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/unicode.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:05.288296 abch_tree_sitter-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-10 08:51:52.000000 abch_tree_sitter-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-10 08:51:52.000000 abch_tree_sitter-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-05-10 08:52:05.288296 abch_tree_sitter-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-10 08:51:52.000000 abch_tree_sitter-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:05.280296 abch_tree_sitter-1.1.1/abch_tree_sitter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-05-10 08:52:05.000000 abch_tree_sitter-1.1.1/abch_tree_sitter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-10 08:52:05.000000 abch_tree_sitter-1.1.1/abch_tree_sitter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 08:52:05.000000 abch_tree_sitter-1.1.1/abch_tree_sitter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 08:52:05.000000 abch_tree_sitter-1.1.1/abch_tree_sitter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-10 08:51:52.000000 abch_tree_sitter-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 08:52:05.288296 abch_tree_sitter-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-10 08:51:52.000000 abch_tree_sitter-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:05.280296 abch_tree_sitter-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    35192 2023-05-10 08:51:52.000000 abch_tree_sitter-1.1.1/tests/test_tree_sitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:05.284296 abch_tree_sitter-1.1.1/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-10 08:51:52.000000 abch_tree_sitter-1.1.1/tree_sitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64107 2023-05-10 08:51:52.000000 abch_tree_sitter-1.1.1/tree_sitter/binding.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:05.280296 abch_tree_sitter-1.1.1/tree_sitter/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:05.280296 abch_tree_sitter-1.1.1/tree_sitter/core/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:05.280296 abch_tree_sitter-1.1.1/tree_sitter/core/lib/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:05.284296 abch_tree_sitter-1.1.1/tree_sitter/core/lib/include/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (123)    30214 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/include/tree_sitter/api.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/include/tree_sitter/parser.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:05.284296 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/alloc.c
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/alloc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/atomic.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/clock.h
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/error_costs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/get_changed_ranges.c
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/get_changed_ranges.h
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/host.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/language.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/language.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/length.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/lexer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/lexer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/lib.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19287 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/node.c
+-rw-r--r--   0 runner    (1001) docker     (123)    69800 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/parser.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/point.h
+-rw-r--r--   0 runner    (1001) docker     (123)   139078 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/query.c
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/reduce_action.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/reusable_node.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27418 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/stack.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/stack.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34154 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/subtree.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/subtree.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/tree.c
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/tree_cursor.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/tree_cursor.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:52:05.288296 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/unicode/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/unicode/ICU_SHA
+-rw-r--r--   0 runner    (1001) docker     (123)    21001 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/unicode/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/unicode/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/unicode/ptypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14865 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/unicode/umachine.h
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/unicode/urename.h
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/unicode/utf.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23878 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/unicode/utf16.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31698 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/unicode/utf8.h
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-10 08:51:54.000000 abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/unicode.h
```

### Comparing `abch_tree_sitter-1.1.0/LICENSE` & `abch_tree_sitter-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/PKG-INFO` & `abch_tree_sitter-1.1.1/abch_tree_sitter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: abch_tree_sitter
-Version: 1.1.0
+Name: abch-tree-sitter
+Version: 1.1.1
 Summary: Python bindings to the Tree-sitter parsing library
 Home-page: https://github.com/Ackee-Blockchain/py-tree-sitter
 Author: Ackee Blockchain
 License: MIT
 Project-URL: Source, https://github.com/Ackee-Blockchain/py-tree-sitter
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abch_tree_sitter-1.1.0/README.md` & `abch_tree_sitter-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/abch_tree_sitter.egg-info/PKG-INFO` & `abch_tree_sitter-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: abch-tree-sitter
-Version: 1.1.0
+Name: abch_tree_sitter
+Version: 1.1.1
 Summary: Python bindings to the Tree-sitter parsing library
 Home-page: https://github.com/Ackee-Blockchain/py-tree-sitter
 Author: Ackee Blockchain
 License: MIT
 Project-URL: Source, https://github.com/Ackee-Blockchain/py-tree-sitter
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abch_tree_sitter-1.1.0/abch_tree_sitter.egg-info/SOURCES.txt` & `abch_tree_sitter-1.1.1/abch_tree_sitter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/setup.py` & `abch_tree_sitter-1.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 with open(path.join(path.dirname(__file__), "README.md")) as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="abch_tree_sitter",
-    version="1.1.0",
+    version="1.1.1",
     author="Ackee Blockchain",
     url="https://github.com/Ackee-Blockchain/py-tree-sitter",
     license="MIT",
     platforms=["any"],
     python_requires=">=3.7",
     description="Python bindings to the Tree-sitter parsing library",
     long_description=LONG_DESCRIPTION,
```

### Comparing `abch_tree_sitter-1.1.0/tests/test_tree_sitter.py` & `abch_tree_sitter-1.1.1/tests/test_tree_sitter.py`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/__init__.py` & `abch_tree_sitter-1.1.1/tree_sitter/__init__.py`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/binding.c` & `abch_tree_sitter-1.1.1/tree_sitter/binding.c`

 * *Files 1% similar despite different names*

```diff
@@ -1034,15 +1034,15 @@
 }
 
 static PyMethodDef parser_methods[] = {
     {
         .ml_name = "parse",
         .ml_meth = (PyCFunction)parser_parse,
         .ml_flags = METH_VARARGS | METH_KEYWORDS,
-        .ml_doc = "parse(bytes, old_tree=None, keep_text=True)\n--\n\n\
+        .ml_doc = "parse(bytes, old_tree=None, keep_text=True, encoding=\"utf8\")\n--\n\n\
                Parse source code, creating a syntax tree.",
     },
     {
         .ml_name = "set_language",
         .ml_meth = (PyCFunction)parser_set_language,
         .ml_flags = METH_O,
         .ml_doc = "set_language(language)\n--\n\n\
```

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/include/tree_sitter/api.h` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/include/tree_sitter/api.h`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/include/tree_sitter/parser.h` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/include/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/alloc.c` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/alloc.c`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/alloc.h` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/alloc.h`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/array.h` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/array.h`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/atomic.h` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/atomic.h`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/clock.h` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/clock.h`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/get_changed_ranges.c` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/get_changed_ranges.c`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/get_changed_ranges.h` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/get_changed_ranges.h`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/host.h` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/host.h`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/language.c` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/language.c`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/language.h` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/language.h`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/length.h` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/length.h`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/lexer.c` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/lexer.c`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/lexer.h` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/lexer.h`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/node.c` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/node.c`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/parser.c` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/parser.c`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/point.h` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/point.h`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/query.c` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/query.c`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/reduce_action.h` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/reduce_action.h`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/reusable_node.h` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/reusable_node.h`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/stack.c` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/stack.c`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/stack.h` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/stack.h`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/subtree.c` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/subtree.c`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/subtree.h` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/subtree.h`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/tree.c` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/tree.c`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/tree.h` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/tree.h`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/tree_cursor.c` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/tree_cursor.c`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/tree_cursor.h` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/tree_cursor.h`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/unicode/LICENSE` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/unicode/LICENSE`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/unicode/README.md` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/unicode/README.md`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/unicode/umachine.h` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/unicode/umachine.h`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/unicode/utf16.h` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/unicode/utf16.h`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/unicode/utf8.h` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/unicode/utf8.h`

 * *Files identical despite different names*

### Comparing `abch_tree_sitter-1.1.0/tree_sitter/core/lib/src/unicode.h` & `abch_tree_sitter-1.1.1/tree_sitter/core/lib/src/unicode.h`

 * *Files identical despite different names*

