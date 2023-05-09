# Comparing `tmp/petals-1.1.4.tar.gz` & `tmp/petals-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petals-1.1.4.tar", last modified: Fri Apr 21 01:40:09 2023, max compression
+gzip compressed data, was "petals-1.1.5.tar", last modified: Tue May  9 23:05:48 2023, max compression
```

## Comparing `petals-1.1.4.tar` & `petals-1.1.5.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:40:09.579757 petals-1.1.4/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1089 2023-04-21 01:39:52.000000 petals-1.1.4/LICENSE
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    11712 2023-04-21 01:40:09.579757 petals-1.1.4/PKG-INFO
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    10540 2023-04-21 01:39:52.000000 petals-1.1.4/README.md
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      333 2023-04-21 01:39:52.000000 petals-1.1.4/pyproject.toml
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1586 2023-04-21 01:40:09.579757 petals-1.1.4/setup.cfg
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:40:09.571757 petals-1.1.4/src/
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:40:09.575757 petals-1.1.4/src/petals/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      140 2023-04-21 01:39:57.000000 petals-1.1.4/src/petals/__init__.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:40:09.575757 petals-1.1.4/src/petals/bloom/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/bloom/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2672 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/bloom/block.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5146 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/bloom/from_pretrained.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3877 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/bloom/modeling_utils.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:40:09.575757 petals-1.1.4/src/petals/cli/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/cli/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4718 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/cli/convert_model.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2121 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/cli/inference_one_block.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3798 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/cli/run_dht.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    13616 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/cli/run_server.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:40:09.575757 petals-1.1.4/src/petals/client/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      484 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/client/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    14981 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/client/inference_session.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7128 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/client/remote_forward_backward.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    15928 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/client/remote_generation.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    12364 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/client/remote_model.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4340 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/client/remote_sequential.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:40:09.575757 petals-1.1.4/src/petals/client/routing/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)       71 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/client/routing/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4464 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/client/routing/sequence_info.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    16884 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/client/routing/sequence_manager.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      649 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/client/routing/spending_policy.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    12394 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/client/sequential_autograd.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      537 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/constants.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1116 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/data_structures.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7030 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/dht_utils.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:40:09.575757 petals-1.1.4/src/petals/server/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/server/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     9337 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/server/backend.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4499 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/server/block_selection.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1704 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/server/block_utils.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    24633 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/server/handler.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8655 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/server/memory_cache.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7808 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/server/reachability.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    26298 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/server/server.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8412 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/server/task_pool.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      842 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/server/task_prioritizer.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     6627 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/server/throughput.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:40:09.579757 petals-1.1.4/src/petals/utils/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/utils/__init__.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      525 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/utils/asyncio.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     6171 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/utils/convert_block.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3091 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/utils/disk_cache.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5591 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/utils/generation_algorithms.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1853 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/utils/generation_constraints.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1242 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/utils/logging.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      171 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/utils/misc.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      914 2023-04-21 01:39:52.000000 petals-1.1.4/src/petals/utils/version.py
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:40:09.575757 petals-1.1.4/src/petals.egg-info/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    11712 2023-04-21 01:40:09.000000 petals-1.1.4/src/petals.egg-info/PKG-INFO
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1953 2023-04-21 01:40:09.000000 petals-1.1.4/src/petals.egg-info/SOURCES.txt
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        1 2023-04-21 01:40:09.000000 petals-1.1.4/src/petals.egg-info/dependency_links.txt
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      347 2023-04-21 01:40:09.000000 petals-1.1.4/src/petals.egg-info/requires.txt
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        7 2023-04-21 01:40:09.000000 petals-1.1.4/src/petals.egg-info/top_level.txt
-drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-04-21 01:40:09.579757 petals-1.1.4/tests/
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      731 2023-04-21 01:39:52.000000 petals-1.1.4/tests/test_aux_functions.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3654 2023-04-21 01:39:52.000000 petals-1.1.4/tests/test_block_exact_match.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3151 2023-04-21 01:39:52.000000 petals-1.1.4/tests/test_chained_calls.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7789 2023-04-21 01:39:52.000000 petals-1.1.4/tests/test_full_model.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2848 2023-04-21 01:39:52.000000 petals-1.1.4/tests/test_priority_pool.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5773 2023-04-21 01:39:52.000000 petals-1.1.4/tests/test_remote_sequential.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1911 2023-04-21 01:39:52.000000 petals-1.1.4/tests/test_sequence_manager.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1797 2023-04-21 01:39:52.000000 petals-1.1.4/tests/test_server_stats.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1910 2023-04-21 01:39:52.000000 petals-1.1.4/tests/test_tensor_parallel.py
--rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      419 2023-04-21 01:39:52.000000 petals-1.1.4/tests/test_utils.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-05-09 23:05:48.681306 petals-1.1.5/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1089 2023-05-09 23:04:53.000000 petals-1.1.5/LICENSE
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    11754 2023-05-09 23:05:48.681306 petals-1.1.5/PKG-INFO
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    10582 2023-05-09 23:04:53.000000 petals-1.1.5/README.md
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      333 2023-05-09 23:04:53.000000 petals-1.1.5/pyproject.toml
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1586 2023-05-09 23:05:48.681306 petals-1.1.5/setup.cfg
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-05-09 23:05:48.657305 petals-1.1.5/src/
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-05-09 23:05:48.669306 petals-1.1.5/src/petals/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      355 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/__init__.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-05-09 23:05:48.673306 petals-1.1.5/src/petals/bloom/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/bloom/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2672 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/bloom/block.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5165 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/bloom/from_pretrained.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3877 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/bloom/modeling_utils.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-05-09 23:05:48.673306 petals-1.1.5/src/petals/cli/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/cli/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4718 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/cli/convert_model.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2121 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/cli/inference_one_block.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3798 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/cli/run_dht.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    13616 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/cli/run_server.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-05-09 23:05:48.673306 petals-1.1.5/src/petals/client/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      460 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/client/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    14964 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/client/inference_session.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7128 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/client/remote_forward_backward.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    14964 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/client/remote_generation.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    11521 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/client/remote_model.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2722 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/client/remote_sequential.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-05-09 23:05:48.677306 petals-1.1.5/src/petals/client/routing/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)       71 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/client/routing/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4539 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/client/routing/sequence_info.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    15148 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/client/routing/sequence_manager.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      649 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/client/routing/spending_policy.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    12420 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/client/sequential_autograd.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      537 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/constants.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1212 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/data_structures.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4637 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/dht_utils.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-05-09 23:05:48.677306 petals-1.1.5/src/petals/server/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/server/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     9337 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/server/backend.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     4499 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/server/block_selection.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1704 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/server/block_utils.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    24633 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/server/handler.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8655 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/server/memory_cache.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7808 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/server/reachability.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    26341 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/server/server.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     8412 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/server/task_pool.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      842 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/server/task_prioritizer.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7787 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/server/throughput.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-05-09 23:05:48.677306 petals-1.1.5/src/petals/utils/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        0 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/utils/__init__.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      525 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/utils/asyncio.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     6171 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/utils/convert_block.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3091 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/utils/disk_cache.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5591 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/utils/generation_algorithms.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1853 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/utils/generation_constraints.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      762 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/utils/logging.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      171 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/utils/misc.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      914 2023-05-09 23:04:53.000000 petals-1.1.5/src/petals/utils/version.py
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-05-09 23:05:48.673306 petals-1.1.5/src/petals.egg-info/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)    11754 2023-05-09 23:05:48.000000 petals-1.1.5/src/petals.egg-info/PKG-INFO
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1953 2023-05-09 23:05:48.000000 petals-1.1.5/src/petals.egg-info/SOURCES.txt
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        1 2023-05-09 23:05:48.000000 petals-1.1.5/src/petals.egg-info/dependency_links.txt
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      347 2023-05-09 23:05:48.000000 petals-1.1.5/src/petals.egg-info/requires.txt
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)        7 2023-05-09 23:05:48.000000 petals-1.1.5/src/petals.egg-info/top_level.txt
+drwxrwxr-x   0 jheuristic  (1000) jheuristic  (1000)        0 2023-05-09 23:05:48.681306 petals-1.1.5/tests/
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      731 2023-05-09 23:04:53.000000 petals-1.1.5/tests/test_aux_functions.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     3428 2023-05-09 23:04:53.000000 petals-1.1.5/tests/test_block_exact_match.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2953 2023-05-09 23:04:53.000000 petals-1.1.5/tests/test_chained_calls.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     7789 2023-05-09 23:04:53.000000 petals-1.1.5/tests/test_full_model.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     2848 2023-05-09 23:04:53.000000 petals-1.1.5/tests/test_priority_pool.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     5683 2023-05-09 23:04:53.000000 petals-1.1.5/tests/test_remote_sequential.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1910 2023-05-09 23:04:53.000000 petals-1.1.5/tests/test_sequence_manager.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1763 2023-05-09 23:04:53.000000 petals-1.1.5/tests/test_server_stats.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)     1910 2023-05-09 23:04:53.000000 petals-1.1.5/tests/test_tensor_parallel.py
+-rw-rw-r--   0 jheuristic  (1000) jheuristic  (1000)      419 2023-05-09 23:04:53.000000 petals-1.1.5/tests/test_utils.py
```

### Comparing `petals-1.1.4/LICENSE` & `petals-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/PKG-INFO` & `petals-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petals
-Version: 1.1.4
+Version: 1.1.5
 Summary: Easy way to efficiently run 100B+ language models without high-end GPUs
 Home-page: https://github.com/bigscience-workshop/petals
 Author: Petals Developers
 Author-email: petals-devs@googlegroups.com
 Project-URL: Bug Tracker, https://github.com/bigscience-workshop/petals/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -134,14 +134,16 @@
 
 If you don't use Anaconda, you can install PyTorch in [any other way](https://pytorch.org/get-started/locally/). If you want to run models with 8-bit weights, please install PyTorch with CUDA 11.x or newer for compatility with [bitsandbytes](https://github.com/timDettmers/bitsandbytes).
 
 See the instructions for macOS and Windows, the full requirements, and troubleshooting advice in our [FAQ](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions#running-a-client).
 
 ## Benchmarks
 
+The benchmarks below are for BLOOM-176B:
+
 <table align="center">
   <tr>
     <th colspan="2">Network</th>
     <th colspan="2">Single-batch inference<br>(steps/s)</th>
     <th colspan="2">Parallel forward<br>(tokens/s)</th>
   </tr>
   <tr>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: petals Version: 1.1.4 Summary: Easy way to
+Metadata-Version: 2.1 Name: petals Version: 1.1.5 Summary: Easy way to
 efficiently run 100B+ language models without high-end GPUs Home-page: https://
 github.com/bigscience-workshop/petals Author: Petals Developers Author-email:
 petals-devs@googlegroups.com Project-URL: Bug Tracker, https://github.com/
 bigscience-workshop/petals/issues Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
@@ -92,15 +92,16 @@
 pytorch-cuda=11.7 -c pytorch -c nvidia pip install -U petals ``` If you don't
 use Anaconda, you can install PyTorch in [any other way](https://pytorch.org/
 get-started/locally/). If you want to run models with 8-bit weights, please
 install PyTorch with CUDA 11.x or newer for compatility with [bitsandbytes]
 (https://github.com/timDettmers/bitsandbytes). See the instructions for macOS
 and Windows, the full requirements, and troubleshooting advice in our [FAQ]
 (https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-
-questions#running-a-client). ## Benchmarks
+questions#running-a-client). ## Benchmarks The benchmarks below are for BLOOM-
+176B:
      Network               Single-batch inference Parallel forward
                            (steps/s)              (tokens/s)
      Bandwidth  Round-trip Sequence length        Batch size
                 latency    128           2048       1              64
      Offloading, max. possible speed on 1x A100 1
      256 Gbit/s            0.18          0.18     2.7           170.3
      128 Gbit/s            0.09          0.09     2.4           152.8
```

### Comparing `petals-1.1.4/README.md` & `petals-1.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -107,14 +107,16 @@
 
 If you don't use Anaconda, you can install PyTorch in [any other way](https://pytorch.org/get-started/locally/). If you want to run models with 8-bit weights, please install PyTorch with CUDA 11.x or newer for compatility with [bitsandbytes](https://github.com/timDettmers/bitsandbytes).
 
 See the instructions for macOS and Windows, the full requirements, and troubleshooting advice in our [FAQ](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions#running-a-client).
 
 ## Benchmarks
 
+The benchmarks below are for BLOOM-176B:
+
 <table align="center">
   <tr>
     <th colspan="2">Network</th>
     <th colspan="2">Single-batch inference<br>(steps/s)</th>
     <th colspan="2">Parallel forward<br>(tokens/s)</th>
   </tr>
   <tr>
```

#### html2text {}

```diff
@@ -76,15 +76,16 @@
 pytorch-cuda=11.7 -c pytorch -c nvidia pip install -U petals ``` If you don't
 use Anaconda, you can install PyTorch in [any other way](https://pytorch.org/
 get-started/locally/). If you want to run models with 8-bit weights, please
 install PyTorch with CUDA 11.x or newer for compatility with [bitsandbytes]
 (https://github.com/timDettmers/bitsandbytes). See the instructions for macOS
 and Windows, the full requirements, and troubleshooting advice in our [FAQ]
 (https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-
-questions#running-a-client). ## Benchmarks
+questions#running-a-client). ## Benchmarks The benchmarks below are for BLOOM-
+176B:
      Network               Single-batch inference Parallel forward
                            (steps/s)              (tokens/s)
      Bandwidth  Round-trip Sequence length        Batch size
                 latency    128           2048       1              64
      Offloading, max. possible speed on 1x A100 1
      256 Gbit/s            0.18          0.18     2.7           170.3
      128 Gbit/s            0.09          0.09     2.4           152.8
```

### Comparing `petals-1.1.4/setup.cfg` & `petals-1.1.5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	torch>=1.12
 	bitsandbytes==0.38.0.post2
-	accelerate>=0.15.0,<1.0.0
+	accelerate>=0.16.0,<1.0.0
 	huggingface-hub>=0.11.1,<1.0.0
 	transformers>=4.25.1,<5.0.0
 	speedtest-cli==2.1.3
-	hivemind==1.1.7
+	hivemind==1.1.8
 	tensor_parallel==1.0.23
 	humanfriendly
 	async-timeout>=4.0.2
 	cpufeature>=0.2.0
 	packaging>=20.9
 
 [options.extras_require]
```

### Comparing `petals-1.1.4/src/petals/bloom/block.py` & `petals-1.1.5/src/petals/bloom/block.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/src/petals/bloom/from_pretrained.py` & `petals-1.1.5/src/petals/bloom/from_pretrained.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     assert not report.missing_keys, f"Some block weights are missing: {report.missing_keys}"
 
     for param_name, _ in block.named_parameters():
         assert param_name in state_dict, f"{param_name} not in state dict"
         param = state_dict[param_name]
         if torch_dtype != "auto" and not str(param.dtype).startswith(("torch.uint", "torch.int", "torch.bool")):
             param = param.to(torch_dtype)
-        set_module_tensor_to_device(block, param_name, "cpu", value=param)
+        set_module_tensor_to_device(block, param_name, "cpu", value=param, dtype=param.dtype)
 
     logger.info(f"Loaded {converted_model_name_or_path} block {block_index}, {report}")
     return block
 
 
 def _load_state_dict(
     pretrained_model_name_or_path: str,
```

### Comparing `petals-1.1.4/src/petals/bloom/modeling_utils.py` & `petals-1.1.5/src/petals/bloom/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/src/petals/cli/convert_model.py` & `petals-1.1.5/src/petals/cli/convert_model.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/src/petals/cli/inference_one_block.py` & `petals-1.1.5/src/petals/cli/inference_one_block.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/src/petals/cli/run_dht.py` & `petals-1.1.5/src/petals/cli/run_dht.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/src/petals/cli/run_server.py` & `petals-1.1.5/src/petals/cli/run_server.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/src/petals/client/inference_session.py` & `petals-1.1.5/src/petals/client/inference_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import itertools
 import logging
 import time
 from typing import AsyncIterator, List, Optional
 
 import torch
 from hivemind import (
-    P2P,
     MSGPackSerializer,
     anext,
     deserialize_torch_tensor,
     get_logger,
     nested_flatten,
     serialize_torch_tensor,
 )
@@ -158,17 +157,16 @@
 
 
 class InferenceSession:
     """
     An interface to a multi-step *inference* session for a sequence of remote transformer blocks
     """
 
-    def __init__(self, sequence_manager: RemoteSequenceManager, p2p: P2P, max_length: int):
+    def __init__(self, sequence_manager: RemoteSequenceManager, max_length: int):
         self._sequence_manager = sequence_manager
-        self._p2p = p2p
         self._closed = False
         self._chosen_spans = []
         self._server_sessions = []
         self._server_inputs = []  # Used in case of server failures to regenerate attention caches on new servers
         self._position = 0
         self._max_length = max_length
         self.last_token_id = None
@@ -177,23 +175,23 @@
     def position(self) -> int:
         return self._position
 
     def _enter_server_sessions(self, chosen_spans: List[RemoteSpanInfo]) -> List[_ServerInferenceSession]:
         server_sessions = []
         try:
             for span in chosen_spans:
-                stub = TransformerConnectionHandler.get_stub(self._p2p, span.peer_id)
+                stub = TransformerConnectionHandler.get_stub(self._sequence_manager.state.p2p, span.peer_id)
                 span_uids = CHAIN_DELIMITER.join(self._sequence_manager.block_uids[span.start : span.end])
                 metadata = self._sequence_manager.get_request_metadata("rpc_inference", span_uids, peer_id=span.peer_id)
                 session = RemoteExpertWorker.run_coroutine(
                     _ServerInferenceSession.create(
                         stub,
                         span_uids,
                         rpc_info=self._sequence_manager.rpc_info,
-                        timeout=self._sequence_manager.request_timeout,
+                        timeout=self._sequence_manager.config.request_timeout,
                         max_length=self._max_length,
                         **metadata,
                     )
                 )
                 server_sessions.append(session)
                 session.__enter__()
             return server_sessions
@@ -251,15 +249,15 @@
                         if attempt_no >= 1 and update_end > recovery_until:
                             logger.info(
                                 f"Due to a server failure, remote attention caches "
                                 f"from block {block_idx} to {update_end} will be regenerated"
                             )
                         recovery_until = max(recovery_until, update_end)
 
-                        updated_spans = self._sequence_manager.make_sequence(block_idx, update_end, mode="fastest")
+                        updated_spans = self._sequence_manager.make_sequence(block_idx, update_end, mode="min_latency")
                         # make_sequence() could return a longer sequence
                         updated_spans[-1].end = min(updated_spans[-1].end, update_end)
                         updated_sessions = self._enter_server_sessions(updated_spans)
                         logger.debug(
                             f"Found path from block {block_idx} to {update_end} via {len(updated_spans)} servers"
                         )
 
@@ -301,17 +299,16 @@
 
                     inputs = outputs
                     server_idx += 1
                     block_idx = span.end
                     self._sequence_manager.on_request_success(span.peer_id)
                     break
                 except Exception as e:
-                    if span is not None:
-                        self._sequence_manager.on_request_failure(span.peer_id)
-                    if attempt_no + 1 == self._sequence_manager.max_retries:
+                    self._sequence_manager.on_request_failure(span.peer_id if span is not None else None)
+                    if attempt_no + 1 == self._sequence_manager.config.max_retries:
                         raise
                     delay = self._sequence_manager.get_retry_delay(attempt_no)
                     logger.warning(
                         f"Caught exception when running inference via {span} (retry in {delay:.0f} sec): {repr(e)}"
                     )
                     maybe_log_traceback(e)
                     time.sleep(delay)
```

### Comparing `petals-1.1.4/src/petals/client/remote_forward_backward.py` & `petals-1.1.5/src/petals/client/remote_forward_backward.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/src/petals/client/remote_generation.py` & `petals-1.1.5/src/petals/client/remote_generation.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,30 +40,29 @@
 
         return self.transformer.h.inference_session(**kwargs)
 
     @torch.inference_mode()
     def generate(
         self,
         inputs: Optional[torch.Tensor] = None,
+        *,
         do_sample: Optional[bool] = None,
         temperature: float = 1.0,
         top_k: Optional[int] = None,
         top_p: Optional[float] = None,
         num_beams: Optional[int] = 1,
         bos_token_id: Optional[int] = None,
         eos_token_id: Optional[int] = None,
         pad_token_id: Optional[int] = None,
         max_length: Optional[int] = None,
         max_new_tokens: Optional[int] = None,
         decoding_algorithm: Optional[DecodingAlgorithm] = None,
         provided_constraints: List[ABCBloomConstraint] = [],
         num_return_sequences: Optional[int] = None,
-        *,
         session: Optional[InferenceSession] = None,
-        **model_kwargs,
     ) -> torch.LongTensor:
         """
         Generates sequences of token ids for models with a language modeling head.
 
         :param inputs: The input tokens to the model.
         :param do_sample: Whether to sample from the model predictions or take the argmax.
         :param temperature: The temperature to use for sampling.
@@ -73,27 +72,17 @@
         :param bos_token_id: The id of the beginning of sentence token.
         :param eos_token_id: The id of the end of sentence token.
         :param pad_token_id: The id of the padding token.
         :param max_length: The maximum number of tokens in the output (including input tokens).
         :param max_new_tokens: The maximum number of tokens to generate.
         :param decoding_algorithm: The decoding algorithm to use.
         :param provided_constraints: A list of constraints to use.
-        :param model_kwargs: Additional arguments to pass to the model.
         :param num_return_sequences: How many hypothesis from the beam will be in output.
         """
 
-        assert (
-            model_kwargs.get("logits_processor", None) is None
-        ), "For RemoteGenerationMixin models use BloomConstraints instead of logits_processor"
-        assert (
-            model_kwargs.get("logits_wrapper", None) is None
-        ), "For RemoveGenerationMixin models use DecodingAlgorithm instead of logits_wrapper"
-        assert (
-            model_kwargs.get("stopping_criteria", None) is None
-        ), "For RemoteGenerationMixin models use BloomConstraints instead of stopping_criteria"
         prefix_length = 0 if inputs is None else inputs.size(1)
         prefix_length += self.config.pre_seq_len
 
         bos_token_id = bos_token_id if bos_token_id is not None else self.config.bos_token_id
         pad_token_id = pad_token_id if pad_token_id is not None else self.config.pad_token_id
         eos_token_id = eos_token_id if eos_token_id is not None else self.config.eos_token_id
 
@@ -222,15 +211,14 @@
     def greedy_search(
         self,
         input_ids: torch.LongTensor,
         max_length: Optional[int] = None,
         pad_token_id: Optional[int] = None,
         eos_token_id: Optional[int] = None,
         provided_constraints: List[ABCBloomConstraint] = [],
-        **model_kwargs,
     ) -> torch.LongTensor:
         """
         Generates sequences of token ids for models with a language modeling head. Uses greedy search.
 
         :param input_ids: The input tokens to the model.
         :param max_length: The maximum length of the sequence to generate.
         :param pad_token_id: The id of the padding token.
@@ -240,109 +228,100 @@
         return self.generate(
             inputs=input_ids,
             max_new_tokens=max_length,
             pad_token_id=pad_token_id,
             eos_token_id=eos_token_id,
             decoding_algorithm=GreedyAlgorithm(),
             provided_constraints=provided_constraints,
-            **model_kwargs,
         )
 
     def sample(
         self,
         input_ids: torch.LongTensor,
         temperature: float = 1.0,
         top_k: Optional[int] = None,
         top_p: Optional[float] = None,
         max_length: Optional[int] = None,
         pad_token_id: Optional[int] = None,
         eos_token_id: Optional[int] = None,
         provided_constraints: List[ABCBloomConstraint] = [],
-        **model_kwargs,
     ) -> torch.LongTensor:
         """
         Generates sequences of token ids for models with a language modeling head. Uses multinomial sampling.
         If top_k is provided, uses top_k sampling. If top_p is provided, uses nucleus sampling.
 
         :param: input_ids: The input tokens to the model.
         :param: temperature: The temperature to use for sampling.
         :param: top_k: The number of samples to use for top_k sampling.
         :param: top_p: The probability of using top_p sampling.
         :param: max_length: The maximum length of the sequence to generate.
         :param: pad_token_id: The id of the padding token.
         :param: eos_token_id: The id of the end of sentence token.
         :param: provided_constraints: A list of constraints to use.
-        :param: model_kwargs: Additional kwargs to pass to the model.
         """
 
         return self.generate(
             inputs=input_ids,
             max_new_tokens=max_length,
             pad_token_id=pad_token_id,
             eos_token_id=eos_token_id,
             decoding_algorithm=self._choose_sample_algorithm(temperature, top_k, top_p),
             provided_constraints=provided_constraints,
-            **model_kwargs,
         )
 
     def beam_search(
         self,
         input_ids: torch.LongTensor,
         num_beams: int = 1,
         max_length: Optional[int] = None,
         pad_token_id: Optional[int] = None,
         eos_token_id: Optional[int] = None,
         provided_constraints: List[ABCBloomConstraint] = [],
-        **model_kwargs,
     ) -> torch.LongTensor:
         """
         Generates sequences of token ids for models with a language modeling head. Uses beam search.
 
         :param input_ids: The input tokens to the model.
         :param num_beams: The number of beams to use.
         :param max_length: The maximum length of the sequence to generate.
         :param pad_token_id: The id of the padding token.
         :param eos_token_id: The id of the end of sentence token.
         :param provided_constraints: A list of constraints to use.
-        :param: model_kwargs: Additional kwargs to pass to the model.
         """
         decoding_algorithm = BeamSearchAlgorithm(
             num_beams=num_beams,
             batch_size=input_ids.size(0),
         )
         return self.generate(
             inputs=input_ids,
             num_beams=num_beams,
             max_new_tokens=max_length,
             pad_token_id=pad_token_id,
             eos_token_id=eos_token_id,
             decoding_algorithm=decoding_algorithm,
             provided_constraints=provided_constraints,
-            **model_kwargs,
         )
 
     def beam_sample(
         self,
         input_ids: torch.LongTensor,
         max_length: Optional[int] = None,
         pad_token_id: Optional[int] = None,
         eos_token_id: Optional[int] = None,
         provided_constraints: List[ABCBloomConstraint] = [],
-        **model_kwargs,
     ) -> torch.LongTensor:
         raise NotImplementedError
 
     def group_beam_search(
         self,
         input_ids: torch.LongTensor,
         max_length: Optional[int] = None,
         pad_token_id: Optional[int] = None,
         eos_token_id: Optional[int] = None,
         provided_constraints: List[ABCBloomConstraint] = [],
-        **model_kwargs,
     ) -> torch.LongTensor:
         raise NotImplementedError
 
     def _choose_sample_algorithm(
         self,
         temperature: float = 1.0,
         top_k: Optional[int] = None,
```

### Comparing `petals-1.1.4/src/petals/client/remote_model.py` & `petals-1.1.5/src/petals/client/remote_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,38 +14,33 @@
     BloomModel,
     BloomPreTrainedModel,
 )
 
 from petals.bloom.modeling_utils import LMHead
 from petals.client.remote_generation import RemoteGenerationMixin
 from petals.client.remote_sequential import RemoteSequential
+from petals.client.routing.sequence_manager import SequenceManagerConfig
 from petals.constants import PUBLIC_INITIAL_PEERS
 from petals.utils.misc import DUMMY
 
 logger = get_logger(__name__)
 
 
-class DistributedBloomConfig(BloomConfig):
+class DistributedBloomConfig(BloomConfig, SequenceManagerConfig):
     """
     A bloom config that contains information about DHT peers.
     To create a distributed model, one must provide dht_prefix and either initial_peers or dht.
     """
 
     initial_peers: List[str] = PUBLIC_INITIAL_PEERS  # a list of initial peers for hivemind DHT
     dht_prefix: str  # a prefix for all dht keys that correspond to this model (usually equal to model name)
     daemon_startup_timeout: int = 60  # timeout for the libp2p daemon connecting to initial peers
-    dht: Optional[hivemind.DHT] = None  # a running DHT instance, e.g. when using the same DHT for multiple models
-    request_timeout: int = 3 * 60  # a number of seconds for waiting result from each node
-    max_retries: Optional[int] = None  # max number retries before the client raises an exception (default: inf)
-    allowed_servers: Optional[
-        Collection[Union[str, hivemind.PeerID]]
-    ] = None  # if defined, send requests only to these servers
 
     pre_seq_len: int = 0  # a number of tokens for prompt tuning.
-    tuning_mode: Optional[str] = None  # One of the finetune options: [None, 'shallow_ptune', 'deep_ptune', 'adapters']
+    tuning_mode: Optional[str] = None  # fine-tuning regime, one of [None, "ptune", "deep_ptune"]
 
     # This settings matter for running the client with dtype bfloat16 on CPU.
     # If the CPU doesn't support AVX512, chunked_forward() significantly speeds up computations.
     use_chunked_forward: Union[str, bool] = "auto"
     chunked_forward_step: int = 16384
 
 
@@ -102,38 +97,24 @@
 
     _keys_to_ignore_on_load_missing = BloomModel._keys_to_ignore_on_load_missing + [
         r"^(intermediate_)?prompt_embeddings\.weight$",
     ]
 
     config_class = DistributedBloomConfig
 
-    def __init__(self, config: DistributedBloomConfig):
+    def __init__(self, config: DistributedBloomConfig, *, dht: Optional[hivemind.DHT] = None):
         assert config.dht_prefix, "Could not find dht_prefix in config, please create model with dht_prefix=..."
-        assert config.initial_peers or config.dht, "Please specify initial_peers=list(...) or dht=hivemind.DHT(...)"
+        assert config.initial_peers or dht is not None, "Please specify `config.initial_peers` or `dht`"
 
         n_layer, config.n_layer = config.n_layer, 0  # temporarily set n_layer to 0 to prevent layer initialization
         super().__init__(config)
         assert len(self.h) == 0
         config.n_layer = n_layer
 
-        dht = config.dht
-        if dht is None:
-            dht = hivemind.DHT(
-                initial_peers=config.initial_peers,
-                client_mode=True,
-                num_workers=n_layer,
-                startup_timeout=config.daemon_startup_timeout,
-                start=True,
-            )
-        assert isinstance(dht, hivemind.DHT) and dht.is_alive(), "dht must be a running hivemind.DHT instance"
-        self.h = RemoteSequential(
-            config,
-            dht,
-            config.dht_prefix,
-        )
+        self.h = RemoteSequential(config, dht=dht)
 
         # Forbid accumulate grads for embeddings and layernorm
         self.set_requires_grad(False)
 
         if config.tuning_mode and "ptune" in config.tuning_mode:
             assert config.pre_seq_len > 0, "The number of prefix tokens must be > 0"
             self.pre_seq_len = config.pre_seq_len
```

### Comparing `petals-1.1.4/src/petals/client/routing/sequence_info.py` & `petals-1.1.5/src/petals/client/routing/sequence_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,22 +23,22 @@
      is used by most routing strategies should be moved from said strategies to this class.
     """
 
     block_uids: Tuple[ModuleUID, ...]
     block_infos: Tuple[RemoteModuleInfo, ...]  # note: the contents of RemoteModuleInfo can and will be updated
     spans_by_priority: List[RemoteSpanInfo]
     spans_containing_block: Tuple[List[RemoteSpanInfo], ...]
-    last_updated_time: float
+    last_updated_time: Optional[float]
 
     @classmethod
     def make_empty(cls: Type[T], block_uids: Iterable[ModuleUID]) -> T:
         block_uids = tuple(block_uids)
         empty_block_infos = tuple(RemoteModuleInfo(uid, {}) for uid in block_uids)
         empty_spans = tuple([] for _ in range(len(block_uids)))
-        return cls(block_uids, empty_block_infos, [], empty_spans, last_updated_time=-float("inf"))
+        return cls(block_uids, empty_block_infos, [], empty_spans, last_updated_time=None)
 
     def __getitem__(self, ix: slice):
         assert isinstance(ix, slice)
         block_uids, block_infos = self.block_uids[ix], self.block_infos[ix]
         spans_by_priority, spans_containing_block = self.compute_spans(block_infos)
         return RemoteSequenceInfo(
             block_uids, block_infos, spans_by_priority, spans_containing_block, self.last_updated_time
@@ -73,29 +73,31 @@
         active_spans = {}
         for block_index, info in enumerate(block_infos):
             if info is not None:
                 for peer_id, server in info.servers.items():
                     if server.state != ServerState.ONLINE:
                         continue
                     if peer_id not in active_spans:
-                        active_spans[peer_id] = RemoteSpanInfo(start=block_index, end=block_index + 1, peer_id=peer_id)
+                        active_spans[peer_id] = RemoteSpanInfo(
+                            peer_id=peer_id, start=block_index, end=block_index + 1, throughput=server.throughput
+                        )
                     else:  # peer_id in active_spans
                         active_spans[peer_id].end = block_index + 1
 
             for peer_id in list(active_spans.keys()):
                 if (
                     info is None
                     or peer_id not in info.servers
                     or info.servers[peer_id].state != ServerState.ONLINE
                     or block_index == len(block_infos) - 1
                 ):
                     closed_spans.append(active_spans.pop(peer_id))
         assert not active_spans, f"spans: {active_spans}"
 
-        closed_spans.sort(key=lambda span: span.end - span.start, reverse=True)
+        closed_spans.sort(key=lambda span: span.length, reverse=True)
 
         spans_containing_block = tuple(list() for _ in range(len(block_infos)))
         for span in closed_spans:
             for block_index in range(span.start, span.end):
                 spans_containing_block[block_index].append(span)
 
         return closed_spans, spans_containing_block
```

### Comparing `petals-1.1.4/src/petals/client/routing/sequence_manager.py` & `petals-1.1.5/src/petals/client/routing/sequence_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,307 +1,300 @@
 from __future__ import annotations
 
 import asyncio
+import dataclasses
 import itertools
 import logging
 import random
 import threading
 import time
 from typing import Any, Collection, Dict, List, Optional, Sequence, Union
 from weakref import WeakMethod
 
 import numpy as np
 from hivemind import DHT, P2P, MSGPackSerializer, PeerID, get_dht_time
 from hivemind.dht.node import Blacklist
 from hivemind.moe.client.remote_expert_worker import RemoteExpertWorker
-from hivemind.p2p import P2PHandlerError
 from hivemind.proto import runtime_pb2
 from hivemind.utils.logging import get_logger
 
 import petals.dht_utils
 from petals.client.routing.sequence_info import RemoteSequenceInfo
 from petals.client.routing.spending_policy import NoSpendingPolicy
 from petals.data_structures import ModuleUID, RemoteSpanInfo, ServerState
 from petals.server.handler import TransformerConnectionHandler
 
 logger = get_logger(__name__)
 
 
+@dataclasses.dataclass
+class SequenceManagerConfig:
+    allowed_servers: Optional[Collection[Union[PeerID, str]]] = None  # if defined, send requests only to these servers
+
+    request_timeout: float = 3 * 60  # timeout for forward/backward/inference requests
+    update_period: float = 60  # refresh DHT information once in this many seconds
+
+    max_retries: Optional[int] = None  # max number retries before the client raises an exception (default: inf)
+    min_backoff: float = 1  # after a repeated failure, sleep for this many seconds times 2 ** (num_failures - 1)
+    max_backoff: float = 60  # limit maximal sleep time between retries to this value
+    ban_timeout: float = 15  # when a remote peer fails to respond, prevent routing to that peer for this many seconds
+
+
+@dataclasses.dataclass
+class SequenceManagerState:
+    p2p: P2P = None
+    sequence_info: Optional[RemoteSequenceInfo] = None
+    rpc_info: Optional[dict] = None
+    banned_peers: Optional[Blacklist] = None
+
+    def __getitem__(self, ix: Union[int, slice]) -> SequenceManagerState:
+        return dataclasses.replace(self, sequence_info=self.sequence_info[ix])
+
+    def __len__(self) -> int:
+        return len(self.sequence_info)
+
+
 class RemoteSequenceManager:
     """
     Sequence manager is a thread that keeps track of remote servers that hold the specified sequence of blocks.
     TL;DR it tells you, which peers you should ask to get a specific layer. It is used in RemoteSequential.
     When created, RemoteSequenceManager looks up which servers serve necessary layers by reading from DHT.
     Using this information, sequence manager can form sequences of servers that collectively have the full sequence.
     To form such a sequence, call .make_sequence with the appropriate optimization policy (see make_sequence docstr).
 
-    :param dht: a running hivemind.DHT instance, connected to peers that serve the corresponding blocks
-    :param block_uids: a sequence of DHT keys (strings) corresponding to remote layers
-    :param p2p: an optional P2P replica (if not specified, create one via dht.replicate_p2p())
-    :param update_period: by default, refresh DHT information once in this many seconds
-    :param request_timeout: float, in seconds, default timeout for RPC forward/backward/inference requests
-    :param min_backoff: after a repeated failure, sleep for this many seconds times 2 ^ (num_failures - 1)
-    :param max_backoff: limit maximal sleep time between retries to this value
-    :param ban_timeout: when a remote peer fails to respond, prevent routing to that peer for this many seconds
-    :param sequence_info: optionally, specify pre-generated sequence info. by default, create a new one using dht
-    :param rpc_info: optionally, specify rpc info (communicated tensor shapes and compression) to save time
-    :param allowed_servers: if defined, send requests only to these servers
-    :param start: start the background thread (see the note below). If false, you will need to start it manually.
     :note: RemoteSequenceManager takes up some CPU and network I/O to operate in background. It is recommended to avoid
       running redundant sequence managers for the same set of layers.
-
     """
 
     def __init__(
         self,
-        dht: DHT,
+        config: SequenceManagerConfig,
         block_uids: Sequence[ModuleUID],
-        p2p: P2P,
-        update_period: float = 30,
-        request_timeout: float = 30,
-        max_retries: Optional[int] = None,
-        min_backoff: float = 1,
-        max_backoff: float = 15 * 60,
-        ban_timeout: float = 15,
-        sequence_info: Optional[RemoteSequenceInfo] = None,
-        rpc_info: Optional[dict] = None,
-        allowed_servers: Optional[Collection[Union[str, hivemind.PeerID]]] = None,
-        banned_peers: Optional[Blacklist] = None,
-        # dear dev, if you add more parameters to this class, please make sure to handle them in __getitem__ (below)
+        *,
+        dht: Optional[DHT] = None,
+        state: Optional[SequenceManagerState] = None,
     ):
         assert len(block_uids) > 0, "Sequences must contain at least one block"
-        self.dht, self.p2p = dht, p2p
-        self.request_timeout, self.max_retries = request_timeout, max_retries
-        self.ban_timeout, self.min_backoff, self.max_backoff = ban_timeout, min_backoff, max_backoff
+
+        self.config = config
+        if state is None:
+            state = SequenceManagerState()
+        self.state = state
+
+        if dht is None:
+            dht = DHT(
+                initial_peers=config.initial_peers,
+                client_mode=True,
+                num_workers=config.n_layer,
+                startup_timeout=config.daemon_startup_timeout,
+                start=True,
+            )
+        assert isinstance(dht, DHT) and dht.is_alive(), "`dht` must be a running hivemind.DHT instance"
+        self.dht = dht
+
+        if state.p2p is None:
+            state.p2p = RemoteExpertWorker.run_coroutine(dht.replicate_p2p())
+
         self.lock_changes = threading.Lock()
-        self._thread = _SequenceManagerUpdateThread(update_period, WeakMethod(self._update))
+        self._thread = _SequenceManagerUpdateThread(config.update_period, WeakMethod(self._update))
         self._thread_start_lock = threading.Lock()
         self.policy = NoSpendingPolicy()
-        self._rpc_info = rpc_info
 
-        if allowed_servers is not None:
-            allowed_servers = {
-                PeerID.from_base58(peer_id) if isinstance(peer_id, str) else peer_id for peer_id in allowed_servers
-            }
-        self.allowed_servers = allowed_servers
-        self.banned_peers = Blacklist(base_time=ban_timeout, backoff_rate=2.0) if banned_peers is None else banned_peers
-
-        if sequence_info is None:
-            self.sequence_info = RemoteSequenceInfo.make_empty(block_uids)
+        if state.banned_peers is None:
+            state.banned_peers = Blacklist(base_time=config.ban_timeout, backoff_rate=2.0)
+        if state.sequence_info is None:
+            state.sequence_info = RemoteSequenceInfo.make_empty(block_uids)
 
+        if state.sequence_info.last_updated_time is None:
             # Pre-fetch module infos in DHT in parallel with .from_pretrained(), then use cached records
             # in the first _update() instead of the latest ones. This makes the first .update() faster.
             petals.dht_utils.get_remote_module_infos(self.dht, self.block_uids, latest=True, return_future=True)
             self._need_latest_infos = False
         else:
-            self.sequence_info = sequence_info
-            assert block_uids == sequence_info.block_uids
+            assert block_uids == state.sequence_info.block_uids
             self._thread.ready.set()  # no need to await the first dht fetch
             self._need_latest_infos = True
 
     def make_sequence(
-        self, start_index: int = 0, end_index: Optional[int] = None, mode: str = "random"
+        self, start_index: int = 0, end_index: Optional[int] = None, *, mode: str
     ) -> List[RemoteSpanInfo]:
         """
         Form a sequence of remote servers that collectively serve all consecutive layers
 
         :param start_index: optional index of the first module in a sequence, default = the first of block_uids
         :param end_index: optional index of the last module (non-inclusive), default = after last of block uids
-        :param mode: either random or fastest
+        :param mode: one of ["max_throughput", "min_latency"]
         """
         with self._thread_start_lock:
             if not self.is_alive():
                 self._thread.start()
         if not self.ready.is_set():
             self.update(wait=True)  # this will await an existing update or trigger a new one (if not updating)
 
         end_index = end_index if end_index is not None else len(self)
         span_sequence = []
         current_index = start_index
         while current_index < end_index:
-            candidate_spans = self.sequence_info.spans_containing_block[current_index]
+            candidate_spans = self.state.sequence_info.spans_containing_block[current_index]
             if not candidate_spans:
                 raise MissingBlocksError(current_index)
-            if mode == "random":
-                chosen_span = random.choice(candidate_spans)  # TODO this should be replaced with proper load balancing
-            elif mode == "fastest":
-                # note: this too is a heuristic that will be replaced once we integrate fastest wall time routing
+
+            if mode == "max_throughput":
+                span_weights = np.array([span.throughput for span in candidate_spans], dtype=np.float64)
+            elif mode == "min_latency":
                 span_weights = np.array([span.end - current_index for span in candidate_spans], dtype=np.float64)
-                chosen_span = np.random.choice(candidate_spans, p=span_weights / span_weights.sum())
             else:
                 raise RuntimeError(f"Unexpected mode {mode}")
+            chosen_span = np.random.choice(candidate_spans, p=span_weights / span_weights.sum())
 
             assert chosen_span.start <= current_index < chosen_span.end
-            span_sequence.append(RemoteSpanInfo(start=current_index, end=chosen_span.end, peer_id=chosen_span.peer_id))
+            span_sequence.append(dataclasses.replace(chosen_span, start=current_index))
             current_index = chosen_span.end
 
         route_repr = " => ".join([f"{span.start}:{span.end} via …{str(span.peer_id)[-6:]}" for span in span_sequence])
         logger.debug(f"Route found: {route_repr}")
         return span_sequence
 
     def __getitem__(self, ix: Union[int, slice]) -> RemoteSequenceManager:
         """Get a RemoteSequenceManager for a sub-sequence of blocks"""
         assert isinstance(ix, (int, slice))
         if not isinstance(ix, slice):
             ix = slice(int(ix), int(ix) + 1, 1)
-        return type(self)(
-            self.dht,
-            self.block_uids[ix],
-            self.p2p,
-            update_period=self._thread.update_period,
-            request_timeout=self.request_timeout,
-            ban_timeout=self.ban_timeout,
-            min_backoff=self.min_backoff,
-            max_backoff=self.max_backoff,
-            sequence_info=self.sequence_info[ix],
-            rpc_info=self._rpc_info,
-            allowed_servers=self.allowed_servers,
-            banned_peers=self.banned_peers,
-        )
+        return type(self)(self.config, self.block_uids[ix], dht=self.dht, state=self.state[ix])
 
     def update(self, *, wait: bool):
         """Run an asynchronous update in background as soon as possible"""
-        self.ready.clear()  # TODO this should be a separate event
+        self.ready.clear()
         self._thread.trigger.set()
         if wait:
             self.ready.wait()
 
     def _update(self):
         """Perform an immediate and synchronous refresh, may take time"""
-        for attempt_no in itertools.count():
-            try:
-                new_block_infos = petals.dht_utils.get_remote_module_infos(
-                    self.dht, self.block_uids, latest=self._need_latest_infos
-                )
-                self._need_latest_infos = True  # All future _update() should use latest infos
+        new_block_infos = petals.dht_utils.get_remote_module_infos(
+            self.dht, self.block_uids, latest=self._need_latest_infos
+        )
+        self._need_latest_infos = True  # All future _update() should use latest infos
 
-                for block_info in new_block_infos:
-                    if not block_info:
-                        continue
-
-                    # Apply whitelist, if defined
-                    if self.allowed_servers is not None:
-                        block_info.servers = {
-                            peer_id: server_info
-                            for peer_id, server_info in block_info.servers.items()
-                            if peer_id in self.allowed_servers
-                        }
-
-                    # Remove temporarily banned peers, unless there are no peers left
-                    valid_servers = {
-                        peer_id: server_info
-                        for peer_id, server_info in block_info.servers.items()
-                        if peer_id not in self.banned_peers
-                    }
-                    if len(valid_servers) < len(block_info.servers):
-                        if valid_servers:
-                            logger.debug(
-                                f"Kept {len(valid_servers)} out of {len(block_info.servers)} servers holding {block_info.uid}"
-                            )
-                            block_info.servers = valid_servers
-                        else:
-                            # If we blacklisted all servers, the error may actually be client-caused
-                            logger.debug(f"All servers holding {block_info.uid} are blacklisted, ignoring blacklist")
-
-                with self.lock_changes:
-                    self.sequence_info.update_(new_block_infos)
-                missing_blocks = [i for i in range(len(self)) if not self.sequence_info.spans_containing_block[i]]
-                if missing_blocks:
-                    raise MissingBlocksError(missing_blocks)
-                self.ready.set()  # if there is an active server for every block, we may begin running
-                break
+        for block_info in new_block_infos:
+            if not block_info:
+                continue
+
+            # Apply whitelist, if defined
+            if self.config.allowed_servers is not None:
+                block_info.servers = {
+                    peer_id: server_info
+                    for peer_id, server_info in block_info.servers.items()
+                    if peer_id in self.config.allowed_servers or str(peer_id) in self.config.allowed_servers
+                }
+
+            # Remove temporarily banned peers, unless there are no peers left
+            valid_servers = {
+                peer_id: server_info
+                for peer_id, server_info in block_info.servers.items()
+                if peer_id not in self.state.banned_peers
+            }
+            if len(valid_servers) < len(block_info.servers):
+                if valid_servers:
+                    logger.debug(
+                        f"Kept {len(valid_servers)} out of {len(block_info.servers)} servers holding {block_info.uid}"
+                    )
+                    block_info.servers = valid_servers
+                else:
+                    # If we blacklisted all servers, the error may actually be client-caused
+                    logger.debug(f"All servers holding {block_info.uid} are blacklisted, ignoring blacklist")
 
-            except Exception as e:
-                delay = self.get_retry_delay(attempt_no)
-                logger.warning(f"Could not find route through the model: {repr(e)} (retry in {delay:.0f} sec)")
-                maybe_log_traceback(e)
-                time.sleep(delay)
+        with self.lock_changes:
+            self.state.sequence_info.update_(new_block_infos)
+        self.ready.set()
 
-    def on_request_failure(self, peer_id: PeerID):
+    def on_request_failure(self, peer_id: Optional[PeerID]):
         """remove a given peer from the routing table. If the routing is no longer possible, trigger an update"""
-        logger.info(f"Peer {peer_id} did not respond, banning it temporarily")
-        self.banned_peers.register_failure(peer_id)
+        if peer_id is not None:
+            logger.debug(f"Peer {peer_id} did not respond, banning it temporarily")
+            self.state.banned_peers.register_failure(peer_id)
         with self.lock_changes:
             should_update = False
-            for info in self.sequence_info.block_infos:
+            for info in self.state.sequence_info.block_infos:
                 info.servers.pop(peer_id, None)
                 if not info.servers:
                     should_update = True
             if should_update:
                 self.ready.clear()
                 self.update(wait=False)
 
     def on_request_success(self, peer_id: PeerID):
         """if peer has a failure streak, clear that streak"""
-        self.banned_peers.register_success(peer_id)
+        self.state.banned_peers.register_success(peer_id)
 
     def __len__(self):
         return len(self.block_uids)
 
     @property
     def is_alive(self):
         return self._thread.is_alive
 
     @property
     def ready(self) -> threading.Event:
         return self._thread.ready
 
     @property
     def block_uids(self):
-        return self.sequence_info.block_uids
+        return self.state.sequence_info.block_uids
 
     @property
     def rpc_info(self):
         """Return the rpc_info queried from one of the servers that hold the first block"""
-        if self._rpc_info is None:
-            with self._thread_start_lock:
-                if not self.is_alive():
-                    self._thread.start()
-
-            for attempt_no in itertools.count():
-                peer_id = None
-                try:
-                    if not self.ready.is_set():
-                        self.update(wait=True)
-
-                    active_servers = [
-                        peer_id
-                        for peer_id, server in self.sequence_info.block_infos[0].servers.items()
-                        if server.state == ServerState.ONLINE
-                    ]
-                    if not active_servers:
-                        raise MissingBlocksError(0)
-                    peer_id = random.choice(active_servers)
-
-                    stub = TransformerConnectionHandler.get_stub(self.p2p, peer_id)
-                    outputs = RemoteExpertWorker.run_coroutine(
-                        stub.rpc_info(runtime_pb2.ExpertUID(uid=self.block_uids[0]))
-                    )
-                    self._rpc_info = MSGPackSerializer.loads(outputs.serialized_info)
-                    self.on_request_success(peer_id)
-                    break
-                except Exception as e:
-                    if peer_id is not None and not isinstance(e, P2PHandlerError):
-                        self.on_request_failure(peer_id)
-                    if attempt_no + 1 == self.max_retries:
-                        raise
-                    delay = self.get_retry_delay(attempt_no)
-                    logger.warning(
-                        f"Caught exception when gathering information from peer {peer_id} "
-                        f"(retry in {delay:.0f} sec): {repr(e)}"
-                    )
-                    maybe_log_traceback(e)
-                    time.sleep(delay)
+        if self.state.rpc_info is not None:
+            return self.state.rpc_info
+
+        with self._thread_start_lock:
+            if not self.is_alive():
+                self._thread.start()
+
+        for attempt_no in itertools.count():
+            peer_id = None
+            try:
+                if not self.ready.is_set():
+                    self.update(wait=True)
+
+                active_servers = [
+                    peer_id
+                    for peer_id, server in self.state.sequence_info.block_infos[0].servers.items()
+                    if server.state == ServerState.ONLINE
+                ]
+                if not active_servers:
+                    raise MissingBlocksError(0)
+                peer_id = random.choice(active_servers)
+
+                stub = TransformerConnectionHandler.get_stub(self.state.p2p, peer_id)
+                outputs = RemoteExpertWorker.run_coroutine(
+                    stub.rpc_info(runtime_pb2.ExpertUID(uid=self.block_uids[0]), timeout=self.config.request_timeout)
+                )
+                self.state.rpc_info = MSGPackSerializer.loads(outputs.serialized_info)
+                self.on_request_success(peer_id)
+                break
+            except Exception as e:
+                self.on_request_failure(peer_id)
+                if attempt_no + 1 == self.config.max_retries:
+                    raise
+                delay = self.get_retry_delay(attempt_no)
+                logger.warning(
+                    f"Caught exception when gathering information from peer {peer_id} "
+                    f"(retry in {delay:.0f} sec): {repr(e)}"
+                )
+                maybe_log_traceback(e)
+                time.sleep(delay)
 
-        return self._rpc_info
+        return self.state.rpc_info
 
     def get_retry_delay(self, attempt_no: int) -> float:
         if attempt_no == 0:
             return 0
-        return min(self.min_backoff * 2 ** (attempt_no - 1), self.max_backoff)
+        return min(self.config.min_backoff * 2 ** (attempt_no - 1), self.config.max_backoff)
 
     def get_request_metadata(self, protocol: str, *args, **kwargs) -> Optional[Dict[str, Any]]:
         """
         :param protocol: one of "rpc_forward", "rpc_backward" or "rpc_inference"
         :param args: request-specific inputs, typically block uids and input tensors
         :param kwargs: additional request context, such as remote peer ID
         :returns: msgpack-serialized metadata dict that will be passed alongside a given request
```

### Comparing `petals-1.1.4/src/petals/client/routing/spending_policy.py` & `petals-1.1.5/src/petals/client/routing/spending_policy.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/src/petals/client/sequential_autograd.py` & `petals-1.1.5/src/petals/client/sequential_autograd.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,32 +56,32 @@
     block_idx = start_index
     while block_idx < end_index:
         for attempt_no in itertools.count():
             logger.debug(f"Forward: block {block_idx}, attempt {attempt_no}")
             span = None
             try:
                 if not sequences or attempt_no >= 1:
-                    sequences = deque(sequence_manager.make_sequence(block_idx, end_index, mode="random"))
+                    sequences = deque(sequence_manager.make_sequence(block_idx, end_index, mode="max_throughput"))
                     # make_sequence() could return a longer sequence
                     sequences[-1].end = min(sequences[-1].end, end_index)
                     logger.debug(f"Found path from block {block_idx} to {end_index} via {len(sequences)} servers")
 
                 span = sequences.popleft()
 
-                stub = TransformerConnectionHandler.get_stub(sequence_manager.p2p, span.peer_id)
+                stub = TransformerConnectionHandler.get_stub(sequence_manager.state.p2p, span.peer_id)
                 inputs_and_prompts = [inputs, prompts[span.start : span.end]]
 
                 span_uids = CHAIN_DELIMITER.join(sequence_manager.block_uids[span.start : span.end])
                 metadata = sequence_manager.get_request_metadata("rpc_forward", span_uids, *inputs_and_prompts)
                 (outputs,) = await run_remote_forward(
                     span_uids,
                     stub,
                     sequence_manager.rpc_info,
                     *inputs_and_prompts,
-                    timeout=sequence_manager.request_timeout,
+                    timeout=sequence_manager.config.request_timeout,
                     metadata=MSGPackSerializer.dumps(metadata),
                 )
 
                 assert isinstance(outputs, torch.Tensor)
                 assert outputs.shape == inputs.shape, f"Expected output {inputs.shape}, got {outputs.shape}"
 
                 # Save intermediate inputs and subsequences if the forward is already done for them
@@ -89,17 +89,16 @@
                 done_sequences.append(span)
 
                 inputs = outputs
                 block_idx = span.end
                 sequence_manager.on_request_success(span.peer_id)
                 break
             except Exception as e:
-                if span is not None:
-                    sequence_manager.on_request_failure(span.peer_id)
-                if attempt_no + 1 == sequence_manager.max_retries:
+                sequence_manager.on_request_failure(span.peer_id if span is not None else None)
+                if attempt_no + 1 == sequence_manager.config.max_retries:
                     raise
                 delay = sequence_manager.get_retry_delay(attempt_no)
                 logger.warning(
                     f"Caught exception when running forward via {span} (retry in {delay:.0f} sec): {repr(e)}"
                 )
                 maybe_log_traceback(e)
                 await asyncio.sleep(delay)
@@ -148,36 +147,35 @@
 
                     intermediate_inputs.extend(backup_inputs)
                     forward_sequences.extend(backup_sequences)
                     inputs = intermediate_inputs.pop()
                     span = forward_sequences.pop()
 
                 span_uids = CHAIN_DELIMITER.join(sequence_manager.block_uids[span.start : span.end])
-                stub = TransformerConnectionHandler.get_stub(sequence_manager.p2p, span.peer_id)
+                stub = TransformerConnectionHandler.get_stub(sequence_manager.state.p2p, span.peer_id)
                 metadata = sequence_manager.get_request_metadata(
                     "rpc_backward", span_uids, *inputs, *grad_outputs, peer_id=span.peer_id
                 )
                 grad_outputs, *span_grad_prompts = await run_remote_backward(
                     span_uids,
                     stub,
                     sequence_manager.rpc_info,
                     inputs,
                     grad_outputs,
                     prompts[span.start : span.end],
-                    timeout=sequence_manager.request_timeout,
+                    timeout=sequence_manager.config.request_timeout,
                     metadata=MSGPackSerializer.dumps(metadata),
                 )
                 grad_outputs = [grad_outputs]
                 grad_prompts_reversed.extend(span_grad_prompts)
                 sequence_manager.on_request_success(span.peer_id)
                 break
             except Exception as e:
-                if span is not None:
-                    sequence_manager.on_request_failure(span.peer_id)
-                if attempt_no + 1 == sequence_manager.max_retries:
+                sequence_manager.on_request_failure(span.peer_id if span is not None else None)
+                if attempt_no + 1 == sequence_manager.config.max_retries:
                     raise
                 delay = sequence_manager.get_retry_delay(attempt_no)
                 logger.warning(
                     f"Caught exception when running backward via {span} (retry in {delay:.0f} sec): {repr(e)}"
                 )
                 maybe_log_traceback(e)
                 await asyncio.sleep(delay)
```

### Comparing `petals-1.1.4/src/petals/constants.py` & `petals-1.1.5/src/petals/constants.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/src/petals/data_structures.py` & `petals-1.1.5/src/petals/data_structures.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,17 +35,22 @@
     servers: Dict[PeerID, ServerInfo]
 
 
 @dataclass
 class RemoteSpanInfo:
     """A chain of remote blocks served by one specific remote peer"""
 
+    peer_id: PeerID
     start: int
     end: int
-    peer_id: PeerID
+    throughput: float
+
+    @property
+    def length(self):
+        return self.end - self.start
 
 
 RPCInfo = Dict[str, Any]
 
 
 @dataclasses.dataclass(frozen=True)
 class InferenceMetadata:
```

### Comparing `petals-1.1.4/src/petals/server/backend.py` & `petals-1.1.5/src/petals/server/backend.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/src/petals/server/block_selection.py` & `petals-1.1.5/src/petals/server/block_selection.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/src/petals/server/block_utils.py` & `petals-1.1.5/src/petals/server/block_utils.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/src/petals/server/handler.py` & `petals-1.1.5/src/petals/server/handler.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/src/petals/server/memory_cache.py` & `petals-1.1.5/src/petals/server/memory_cache.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/src/petals/server/reachability.py` & `petals-1.1.5/src/petals/server/reachability.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/src/petals/server/server.py` & `petals-1.1.5/src/petals/server/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from petals.dht_utils import declare_active_modules, get_remote_module_infos
 from petals.server import block_selection
 from petals.server.backend import TransformerBackend, merge_inference_pools_inplace
 from petals.server.block_utils import get_block_size
 from petals.server.handler import TransformerConnectionHandler
 from petals.server.memory_cache import MemoryCache
 from petals.server.reachability import ReachabilityProtocol, check_direct_reachability, validate_reachability
-from petals.server.throughput import get_dtype_name, get_host_throughput
+from petals.server.throughput import get_dtype_name, get_server_throughput
 from petals.utils.convert_block import check_device_balance, convert_block
 from petals.utils.disk_cache import DEFAULT_CACHE_DIR
 
 logger = get_logger(__name__)
 
 
 class Server:
@@ -189,18 +189,19 @@
         if cache_dir is None:
             cache_dir = DEFAULT_CACHE_DIR
         self.cache_dir = cache_dir
         self.max_disk_space = max_disk_space
 
         assert isinstance(throughput, float) or throughput in ["auto", "eval"]
         if throughput in ["auto", "eval"]:
-            throughput = get_host_throughput(
+            throughput = get_server_throughput(
                 self.block_config,
                 device,
                 torch_dtype,
+                num_blocks=num_blocks,
                 load_in_8bit=load_in_8bit,
                 tensor_parallel_devices=self.tensor_parallel_devices,
                 force_eval=(throughput == "eval"),
                 cache_dir=cache_dir,
             )
         self.throughput = throughput
```

### Comparing `petals-1.1.4/src/petals/server/task_pool.py` & `petals-1.1.5/src/petals/server/task_pool.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/src/petals/server/task_prioritizer.py` & `petals-1.1.5/src/petals/server/task_prioritizer.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/src/petals/server/throughput.py` & `petals-1.1.5/src/petals/utils/convert_block.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,181 +1,135 @@
-import fcntl
-import json
+"""
+Tools for converting transformer blocks, applying quantization and/or tensor parallelism
+"""
 import os
-import time
-from collections import Counter
-from hashlib import sha256
-from pathlib import Path
-from typing import Optional, Sequence, Union
+import re
+from typing import Sequence
 
+import tensor_parallel as tp
 import torch
-from hivemind.utils.logging import get_logger
+import torch.nn as nn
+from hivemind.utils.logging import get_logger, use_hivemind_log_handler
+from tensor_parallel.slicing_configs import get_bloom_config
 from transformers import BloomConfig
+from transformers.models.bloom.modeling_bloom import BloomAttention
 
 from petals.bloom.block import WrappedBloomBlock
-from petals.server.block_utils import resolve_block_dtype
-from petals.utils.convert_block import convert_block
-from petals.utils.disk_cache import DEFAULT_CACHE_DIR
 
+use_hivemind_log_handler("in_root_logger")
 logger = get_logger(__name__)
 
-try:
-    import speedtest
-except ImportError:
-    raise ImportError("Please `pip install speedtest-cli==2.1.3`")
-
-if not hasattr(speedtest, "Speedtest"):
-    raise ImportError(
-        "You are using the wrong speedtest module. Please replace speedtest with speedtest-cli.\n"
-        "To do that, run `pip uninstall -y speedtest`. Depending on your python environment, "
-        "you may need to run uninstall speedtest two or more times, until it says 'not installed'.\n"
-        "After that, please `pip install speedtest-cli==2.1.3` to install the correct version."
-    )
 
-
-def get_host_throughput(
-    config: BloomConfig,
-    device: torch.device,
-    dtype: Union[str, torch.dtype],
-    *,
-    load_in_8bit: bool,
-    tensor_parallel_devices: Sequence[torch.device],
-    force_eval: bool = False,
-    cache_dir: Optional[str] = None,
-) -> float:
-    dtype = resolve_block_dtype(config, dtype)
-
-    if cache_dir is None:
-        cache_dir = DEFAULT_CACHE_DIR
-    lock_path = Path(cache_dir, "throughput.lock")
-    cache_path = Path(cache_dir, "throughput_v2.json")
-
-    # We use the system-wide lock since only one process at a time can measure the host throughput
-    os.makedirs(lock_path.parent, exist_ok=True)
-    with open(lock_path, "wb") as lock_fd:
-        logger.info("Loading throughput info")
-        fcntl.flock(lock_fd.fileno(), fcntl.LOCK_EX)
-        # The OS will release the lock when lock_fd is closed or the process is killed
-
-        cache_key = f"config_{sha256(str(config).encode()).hexdigest()[-16:]}"
-        cache_key += f"_device_{get_device_name(device).replace(' ', '_')}"
-        cache_key += f"_dtype_{get_dtype_name(dtype, load_in_8bit)}"
-        if len(tensor_parallel_devices) > 1:
-            for i, device_i in enumerate(tensor_parallel_devices):
-                cache_key += f"_tp{i}_{get_device_name(device_i).replace(' ', '_')}"
-
-        cache = {}
-        try:
-            if not force_eval and os.path.exists(cache_path):
-                with open(cache_path) as cache_fd:
-                    cache = json.load(cache_fd)
-                assert isinstance(cache, dict)
-        except Exception:
-            logger.exception(f"Failed to read throughput info from {cache_path}")
-            cache = {}
-
-        if cache_key not in cache:
-            cache[cache_key] = measure_throughput_info(
-                config, device, dtype, load_in_8bit=load_in_8bit, tensor_parallel_devices=tensor_parallel_devices
-            )
-
-            try:
-                os.makedirs(cache_path.parent, exist_ok=True)
-                with open(cache_path, "w") as cache_fd:
-                    json.dump(cache, cache_fd)
-            except Exception:
-                logger.exception(f"Failed to save throughput info in {cache_path}")
-
-    return cache[cache_key]
-
-
-def measure_throughput_info(
+def convert_block(
+    block: WrappedBloomBlock,
     config: BloomConfig,
-    device: torch.device,
-    dtype: torch.dtype,
-    *,
-    load_in_8bit: bool,
     tensor_parallel_devices: Sequence[torch.device],
-) -> float:
-    """Measure network and compute throughput in forward pass tokens per second"""
-
-    logger.info(
-        "Measuring network and compute throughput. This takes about a minute and will be cached for future runs"
-    )
-
-    result = measure_compute_rps(
-        config, device, dtype, load_in_8bit=load_in_8bit, tensor_parallel_devices=tensor_parallel_devices
-    )
-    try:
-        result = min(result, measure_network_rps(config))
-    except Exception:
-        logger.warning("Failed to measure network throughput:", exc_info=True)
-        logger.warning("Proceeding with the compute throughput only")
-    return result
-
-
-def measure_network_rps(config: BloomConfig) -> Optional[float]:
-    s = speedtest.Speedtest()
-    s.get_servers()
-    s.get_best_server()
-    s.download()
-    s.upload()
-    network_info = s.results.dict()
-
-    bits_per_request = config.hidden_size * 16  # Clients usually send 16-bit tensors for forward/backward
-    network_rps = min(network_info["download"], network_info["upload"]) / bits_per_request
-    if network_rps == 0:
-        raise ValueError("speedtest has returned network_rps == 0")
-
-    logger.info(
-        f"Network throughput: "
-        f"{network_info['download'] / 1e6:.2f} Mbit/s on download, "
-        f"{network_info['upload'] / 1e6:.2f} Mbit/s on upload, "
-        f"{network_rps:.1f} RPS"
-    )
-    return network_rps
-
-
-def measure_compute_rps(
-    config: BloomConfig,
-    device: torch.device,
-    dtype: torch.dtype,
-    *,
+    output_device: torch.device,
     load_in_8bit: bool,
-    tensor_parallel_devices: Sequence[torch.device],
-    n_tokens: int = 16,
-    n_steps: int = 500,
-) -> float:
-    if not tensor_parallel_devices:
-        tensor_parallel_devices = (device,)
-    with torch.inference_mode():
-        block = WrappedBloomBlock(config).to(dtype)
-        block = convert_block(block, config, tensor_parallel_devices, device, load_in_8bit=load_in_8bit, freeze=True)
-
-        cache = None
-        elapsed = 0
-        for step in range(n_steps + 1):
-            dummy_input = torch.randn(n_tokens, 1, config.hidden_size, device=device, dtype=dtype)
-
-            start_time = time.perf_counter()
-            _, cache = block.forward(dummy_input, use_cache=True, layer_past=cache)
-            if step >= 1:  # Skip the 1st step to exclude the initialization time
-                elapsed += time.perf_counter() - start_time
-        device_rps = n_steps * n_tokens / elapsed
-
-    devices_repr = get_device_name(device)
-    if len(tensor_parallel_devices) > 1:
-        device_names = tuple(map(get_device_name, map(torch.device, tensor_parallel_devices)))
-        devices_repr = ", ".join(f"{count}x {name}" for name, count in Counter(device_names).most_common())
-
-    logger.info(
-        f"Forward pass throughput ({devices_repr}, {get_dtype_name(dtype, load_in_8bit)}): " f"{device_rps:.1f} RPS"
-    )
-    return device_rps
-
-
-def get_device_name(device: torch.device) -> str:
-    return f"{torch.cuda.get_device_name(device)} GPU" if device.type == "cuda" else "CPU"
-
-
-def get_dtype_name(dtype: torch.dtype, load_in_8bit: bool) -> str:
-    return "8-bit" if load_in_8bit else str(dtype)
+    threshold: float = 6.0,
+    freeze: bool = True,
+) -> tp.TensorParallel:
+    """
+    Optimize a transformer block for use in a Petals server, apply tensor parallelism and/or LLM.8bit quantization
+
+    :note: some optimizations will modify the input block in-place!
+    :param block: a single transformer block, either pre-trained or newly initialized
+    :param config: HF transformers config for the full model
+    :param tensor_parallel_devices: if specified, use tensor parallelism to split the model between these devices
+    :note: if there is only a single device, model wil still be wrapped with TensorParallel (for uniformity)
+    :param output_device: if tensor_parallel_devices is True, output
+    :param load_in_8bit: if True, use LLM.int8() quantization to reduce the model memory footprint
+    :param threshold: a quantization threshold from LLM.int8() paper ( https://arxiv.org/abs/2208.07339 )
+    :param freeze: if True (default), make all module parameters non-trainable
+    :return: a module that acts like the original block, but runs with all specified optimizations
+
+    """
+    if freeze:
+        for param in block.parameters():
+            param.requires_grad = False
+
+    block = make_tensor_parallel(block, config, tensor_parallel_devices, output_device=output_device)
+
+    if load_in_8bit:
+        block = replace_8bit_linear(block, threshold=threshold)
+
+    for shard, device in zip(block.module_shards, block.devices):
+        shard.to(device)
+
+    return block
+
+
+def replace_8bit_linear(model: nn.Module, threshold=6.0):
+    """
+    A helper function to convert all `torch.nn.Linear` modules to `bnb.nn.Linear8bit` modules from the `bitsandbytes`
+    library. This will enable running your models using mixed int8 precision as described by the paper `GPT3.int8():
+    8-bit Matrix Multiplication for Transformers at Scale`. Make sure `bitsandbytes` compiled with the correct CUDA
+    version of your hardware is installed before running this function. `pip install -i https://test.pypi.org/simple/
+    bitsandbytes-cudaXXX` with `XXX` is your CUDA version (e.g., 11.6 = 116)
+    The function will be run recursively and replace all `torch.nn.Linear` modules except for the `lm_head` and 'score' that should
+    be kept as a `torch.nn.Linear` module.
+    Parameters:
+        model (`torch.nn.Module`):
+            Input model or `torch.nn.Module` as the function is run recursively.
+        threshold (`float`, *optional*):
+            `int8_threshold` for outlier detection as described in the formentioned paper. This parameters is set to
+            `6.0` as described by the paper.
+    """
+
+    # Import bitsandbytes only when necessary, so Petals runs on platforms not supported by bitsandbytes
+    os.environ["BITSANDBYTES_NOWELCOME"] = "1"
+    import bitsandbytes as bnb
+
+    for n, module in model.named_children():
+        if len(list(module.children())) > 0:
+            replace_8bit_linear(module, threshold)
+
+        if isinstance(module, torch.nn.Linear) and n not in ["lm_head", "score"]:
+            assert module.weight.device.type == "cpu", f"expected linear layers on CPU, got {module.weight.device}"
+            model._modules[n] = bnb.nn.Linear8bitLt(
+                module.in_features,
+                module.out_features,
+                module.bias is not None,
+                has_fp16_weights=False,
+                threshold=threshold,
+            )
+            model._modules[n].weight = bnb.nn.Int8Params(
+                module.weight.data, requires_grad=False, has_fp16_weights=False
+            ).to(module.weight.dtype)
+            model._modules[n].bias = module.bias
+    return model
+
+
+def make_tensor_parallel(
+    block: WrappedBloomBlock, model_config: BloomConfig, devices: Sequence[torch.device], output_device: torch.device
+):
+    tp_config = get_bloom_config(model_config, devices)
+    del tp_config.state_rules[re.compile(".*word_embeddings.weight$")]
+    tp_block = tp.TensorParallel(block, devices, config=tp_config, output_device=output_device, delay_init=True)
+    total_heads = 0
+    for tp_shard in tp_block.module_shards:
+        for submodule in tp_shard.modules():
+            if isinstance(submodule, BloomAttention):
+                total_heads += submodule.num_heads
+    assert total_heads == model_config.n_head
+    return tp_block
+
+
+def check_device_balance(devices: Sequence[torch.device]):
+    if not all(device.type == "cuda" for device in devices):
+        logger.warning("Running tensor parallelism on non-GPU devices; proceed at your own risk")
+        return
+    unique_device_capabilities = set(map(torch.cuda.get_device_capability, devices))
+    if len(unique_device_capabilities) > 1:
+        logger.warning(
+            f"Found GPUs with uneven capabilities: {unique_device_capabilities}. "
+            f"Using GPUs with different performance will cause the server to wait for the slowest GPU."
+        )
+
+    memory_per_device = tuple(torch.cuda.get_device_properties(device).total_memory for device in devices)
+    used_memory = min(memory_per_device) * len(memory_per_device)
+    wasted_memory_rate = (sum(memory_per_device) - used_memory) / sum(memory_per_device)
+    if wasted_memory_rate > 0.05:
+        logger.warning(
+            f"GPU devices have highly uneven memory, {wasted_memory_rate * 100:.2f}% memory is wasted. "
+            f"Consider running high-memory GPUs in a separate server."
+        )
```

### Comparing `petals-1.1.4/src/petals/utils/asyncio.py` & `petals-1.1.5/src/petals/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/src/petals/utils/disk_cache.py` & `petals-1.1.5/src/petals/utils/disk_cache.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/src/petals/utils/generation_algorithms.py` & `petals-1.1.5/src/petals/utils/generation_algorithms.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/src/petals/utils/generation_constraints.py` & `petals-1.1.5/src/petals/utils/generation_constraints.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/src/petals/utils/logging.py` & `petals-1.1.5/src/petals/utils/logging.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,19 @@
 import importlib
 import os
 
 from hivemind.utils import logging as hm_logging
 
 
-def in_jupyter() -> bool:
-    """Check if the code is run in Jupyter or Colab"""
-
-    try:
-        __IPYTHON__
-        return True
-    except NameError:
-        return False
-
-
 def initialize_logs():
     """Initialize Petals logging tweaks. This function is called when you import the `petals` module."""
 
     # Env var PETALS_LOGGING=False prohibits Petals do anything with logs
     if os.getenv("PETALS_LOGGING", "True").lower() in ("false", "0"):
         return
 
-    if in_jupyter():
-        os.environ["HIVEMIND_COLORS"] = "True"
-    importlib.reload(hm_logging)
-
-    # Remove log handlers from previous import of hivemind.utils.logging and extra handlers on Colab
-    hm_logging.get_logger().handlers.clear()
-    hm_logging.get_logger("hivemind").handlers.clear()
-
     hm_logging.use_hivemind_log_handler("in_root_logger")
 
     # We suppress asyncio error logs by default since they are mostly not relevant for the end user,
     # unless there is env var PETALS_ASYNCIO_LOGLEVEL
     asyncio_loglevel = os.getenv("PETALS_ASYNCIO_LOGLEVEL", "FATAL" if hm_logging.loglevel != "DEBUG" else "DEBUG")
     hm_logging.get_logger("asyncio").setLevel(asyncio_loglevel)
```

### Comparing `petals-1.1.4/src/petals/utils/version.py` & `petals-1.1.5/src/petals/utils/version.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/src/petals.egg-info/PKG-INFO` & `petals-1.1.5/src/petals.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petals
-Version: 1.1.4
+Version: 1.1.5
 Summary: Easy way to efficiently run 100B+ language models without high-end GPUs
 Home-page: https://github.com/bigscience-workshop/petals
 Author: Petals Developers
 Author-email: petals-devs@googlegroups.com
 Project-URL: Bug Tracker, https://github.com/bigscience-workshop/petals/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -134,14 +134,16 @@
 
 If you don't use Anaconda, you can install PyTorch in [any other way](https://pytorch.org/get-started/locally/). If you want to run models with 8-bit weights, please install PyTorch with CUDA 11.x or newer for compatility with [bitsandbytes](https://github.com/timDettmers/bitsandbytes).
 
 See the instructions for macOS and Windows, the full requirements, and troubleshooting advice in our [FAQ](https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-questions#running-a-client).
 
 ## Benchmarks
 
+The benchmarks below are for BLOOM-176B:
+
 <table align="center">
   <tr>
     <th colspan="2">Network</th>
     <th colspan="2">Single-batch inference<br>(steps/s)</th>
     <th colspan="2">Parallel forward<br>(tokens/s)</th>
   </tr>
   <tr>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: petals Version: 1.1.4 Summary: Easy way to
+Metadata-Version: 2.1 Name: petals Version: 1.1.5 Summary: Easy way to
 efficiently run 100B+ language models without high-end GPUs Home-page: https://
 github.com/bigscience-workshop/petals Author: Petals Developers Author-email:
 petals-devs@googlegroups.com Project-URL: Bug Tracker, https://github.com/
 bigscience-workshop/petals/issues Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
@@ -92,15 +92,16 @@
 pytorch-cuda=11.7 -c pytorch -c nvidia pip install -U petals ``` If you don't
 use Anaconda, you can install PyTorch in [any other way](https://pytorch.org/
 get-started/locally/). If you want to run models with 8-bit weights, please
 install PyTorch with CUDA 11.x or newer for compatility with [bitsandbytes]
 (https://github.com/timDettmers/bitsandbytes). See the instructions for macOS
 and Windows, the full requirements, and troubleshooting advice in our [FAQ]
 (https://github.com/bigscience-workshop/petals/wiki/FAQ:-Frequently-asked-
-questions#running-a-client). ## Benchmarks
+questions#running-a-client). ## Benchmarks The benchmarks below are for BLOOM-
+176B:
      Network               Single-batch inference Parallel forward
                            (steps/s)              (tokens/s)
      Bandwidth  Round-trip Sequence length        Batch size
                 latency    128           2048       1              64
      Offloading, max. possible speed on 1x A100 1
      256 Gbit/s            0.18          0.18     2.7           170.3
      128 Gbit/s            0.09          0.09     2.4           152.8
```

### Comparing `petals-1.1.4/src/petals.egg-info/SOURCES.txt` & `petals-1.1.5/src/petals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/tests/test_aux_functions.py` & `petals-1.1.5/tests/test_aux_functions.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/tests/test_block_exact_match.py` & `petals-1.1.5/tests/test_block_exact_match.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 import random
 from typing import Union
 
-import hivemind
 import pytest
 import torch
 from transformers.models.bloom.configuration_bloom import BloomConfig
 
 from petals.bloom.block import WrappedBloomBlock
 from petals.bloom.from_pretrained import DTYPE_MAP, _load_state_dict, load_pretrained_block
-from petals.client import DistributedBloomConfig
-from petals.client.remote_sequential import RemoteTransformerBlock
+from petals.client import DistributedBloomConfig, RemoteSequential
 from petals.data_structures import UID_DELIMITER
-from petals.dht_utils import get_remote_module
 from test_utils import *
 
 
 @pytest.mark.forked
 def test_remote_block_exact_match(atol_forward=1e-4, atol_inference=1e-3):
-    dht = hivemind.DHT(initial_peers=INITIAL_PEERS, client_mode=True, start=True)
-    config = DistributedBloomConfig.from_pretrained(MODEL_NAME)
+    config = DistributedBloomConfig.from_pretrained(MODEL_NAME, initial_peers=INITIAL_PEERS)
+    remote_sequential = RemoteSequential(config)
 
     for block_index in random.sample(range(config.n_layer), 3):
-        remote_block = get_remote_module(dht, f"{MODEL_NAME}{UID_DELIMITER}{block_index}", config)
-        assert isinstance(remote_block, RemoteTransformerBlock)
+        remote_block = remote_sequential[block_index]
 
         inputs = torch.randn(1, 8, config.hidden_size)
         outputs_forward = remote_block(inputs)
 
         outputs_inference = []
         with remote_block.inference_session(max_length=inputs.shape[1]) as sess:
             for i in range(inputs.shape[1]):
                 outputs_inference.append(sess.step(inputs[:, i : i + 1, :]))
 
             # test that max length is respected
             with pytest.raises(ValueError, match=r"Maximum length exceeded") as exc_info:
                 sess.step(inputs[:, -1:, :])
             assert "Maximum length exceeded" in repr(exc_info.value)
-
         outputs_inference = torch.cat(outputs_inference, dim=1)
 
         ref_block = load_pretrained_block(MODEL_NAME, block_index, torch_dtype=torch.float32)
         (outputs_local,) = ref_block(inputs)
 
         assert torch.allclose(outputs_local, outputs_forward, rtol=0, atol=atol_forward)
         assert torch.allclose(outputs_local, outputs_inference, rtol=0, atol=atol_inference)
```

### Comparing `petals-1.1.4/tests/test_chained_calls.py` & `petals-1.1.5/tests/test_chained_calls.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 ######
 # Warning:torch this test is a work in progress. It will be modified soon.
 # - if you want more stable tests, see test_block_exact_match
 # - if you want to figure out chained inference, ask yozh
 
 
-import hivemind
 import pytest
 import torch
 
 from petals.bloom.from_pretrained import load_pretrained_block
 from petals.client import DistributedBloomConfig
 from petals.client.remote_sequential import RemoteSequential
-from petals.dht_utils import get_remote_sequence
 from test_utils import *
 
 
 @pytest.mark.forked
 def test_forward_backward_exact_match(atol_forward=1e-4, atol_backward=1e-4, seq_length=1):
-    dht = hivemind.DHT(initial_peers=INITIAL_PEERS, client_mode=True, start=True)
-    config = DistributedBloomConfig.from_pretrained(MODEL_NAME)
-    remote_blocks = get_remote_sequence(dht, 3, 6, config)
+    config = DistributedBloomConfig.from_pretrained(MODEL_NAME, initial_peers=INITIAL_PEERS)
+    remote_blocks = RemoteSequential(config, start_block=3, end_block=6)
     assert isinstance(remote_blocks, RemoteSequential)
 
     ref_blocks = [
         load_pretrained_block(MODEL_NAME, 3, torch_dtype=torch.float32),
         load_pretrained_block(MODEL_NAME, 4, torch_dtype=torch.float32),
         load_pretrained_block(MODEL_NAME, 5, torch_dtype=torch.float32),
     ]
@@ -42,18 +39,16 @@
 
     assert torch.allclose(outputs_ref, outputs_rpc, rtol=0, atol=atol_forward)
     assert torch.allclose(grads_ref, grads_rpc, rtol=0, atol=atol_backward)
 
 
 @pytest.mark.forked
 def test_chained_inference_exact_match(atol_inference=1e-4):
-    dht = hivemind.DHT(initial_peers=INITIAL_PEERS, client_mode=True, start=True)
-    config = DistributedBloomConfig.from_pretrained(MODEL_NAME)
-    remote_blocks = get_remote_sequence(dht, 3, 5, config)
-    assert isinstance(remote_blocks, RemoteSequential)
+    config = DistributedBloomConfig.from_pretrained(MODEL_NAME, initial_peers=INITIAL_PEERS)
+    remote_blocks = RemoteSequential(config, start_block=3, end_block=5)
 
     inputs = torch.randn(1, 8, config.hidden_size)
 
     outputs_inference = []
     with remote_blocks.inference_session(max_length=inputs.shape[1]) as sess:
         for i in range(inputs.shape[1]):
             outputs_inference.append(sess.step(inputs[:, i : i + 1, :]))
```

### Comparing `petals-1.1.4/tests/test_full_model.py` & `petals-1.1.5/tests/test_full_model.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/tests/test_priority_pool.py` & `petals-1.1.5/tests/test_priority_pool.py`

 * *Files identical despite different names*

### Comparing `petals-1.1.4/tests/test_remote_sequential.py` & `petals-1.1.5/tests/test_remote_sequential.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 @pytest.mark.forked
 def test_remote_sequential():
     config = DistributedBloomConfig.from_pretrained(MODEL_NAME, initial_peers=INITIAL_PEERS)
     dht = DHT(initial_peers=config.initial_peers, client_mode=True, start=True)
     test_inputs = torch.randn(1, 5, config.hidden_size, requires_grad=True)
     grad_proj = torch.randn(1, 5, config.hidden_size)
 
-    sequential = RemoteSequential(config, dht)
+    sequential = RemoteSequential(config, dht=dht)
 
     full_outputs = sequential(test_inputs)
     (full_outputs * grad_proj).sum().backward()
     assert test_inputs.grad is not None
     full_grad = test_inputs.grad.clone()
     test_inputs.grad.data.zero_()
 
@@ -44,15 +44,15 @@
 
     (second_half_outputs * grad_proj).sum().backward()
     assert torch.allclose(test_inputs.grad, full_grad, atol=1e-3)
 
     # test RemoteSequential with lossy compression
     block_uids = [f"{config.dht_prefix}{UID_DELIMITER}{i}" for i in range(config.n_layer)]
     lossy_sequential = RemoteSequential(
-        config, dht, sequence_manager=DummyCustomSequenceManager(dht, block_uids, sequential.p2p)
+        config, sequence_manager=DummyCustomSequenceManager(config, block_uids, dht=dht)
     )
 
     test_inputs.grad = None
     approx_outputs = lossy_sequential(test_inputs)
     (approx_outputs * grad_proj).sum().backward()
 
     assert not torch.allclose(approx_outputs, full_outputs, rtol=0, atol=1e-4), "compression was not used"
@@ -81,16 +81,15 @@
             metadata["output_compression"] = (runtime_pb2.CompressionType.BLOCKWISE_8BIT,)
         return metadata
 
 
 @pytest.mark.forked
 def test_remote_sequential_prompts(batch_size=2, seq_len=5, pre_seq_len=3):
     config = DistributedBloomConfig.from_pretrained(MODEL_NAME, initial_peers=INITIAL_PEERS)
-    dht = DHT(initial_peers=config.initial_peers, client_mode=True, start=True)
-    remote_sequential = RemoteSequential(config, dht)
+    remote_sequential = RemoteSequential(config)
 
     inputs = F.normalize(torch.randn(batch_size, seq_len, config.hidden_size), dim=-1)
     output_proj = F.normalize(torch.randn(batch_size, seq_len + pre_seq_len, config.hidden_size), dim=-1)
     input_prompts = F.normalize(torch.randn(batch_size, pre_seq_len, config.hidden_size, requires_grad=True), dim=-1)
     intermediate_prompts = torch.randn(config.n_layer, batch_size, pre_seq_len, config.hidden_size, requires_grad=True)
 
     input_prompts = input_prompts.detach().requires_grad_(True)
```

### Comparing `petals-1.1.4/tests/test_sequence_manager.py` & `petals-1.1.5/tests/test_sequence_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,27 +10,26 @@
 from petals.data_structures import UID_DELIMITER
 from test_utils import *
 
 logger = get_logger(__name__)
 
 
 @pytest.mark.forked
-@pytest.mark.parametrize("mode", ["fastest", "random"])
+@pytest.mark.parametrize("mode", ["max_throughput", "min_latency"])
 def test_sequence_manager_basics(mode: str):
     config = DistributedBloomConfig.from_pretrained(MODEL_NAME, initial_peers=INITIAL_PEERS)
     dht = DHT(initial_peers=config.initial_peers, client_mode=True, start=True)
-    sequential = RemoteSequential(config, dht)
+    sequential = RemoteSequential(config, dht=dht)
     shutdown_evt = threading.Event()
 
     # test RemoteSequential with lossy compression
     block_uids = [f"{config.dht_prefix}{UID_DELIMITER}{i}" for i in range(config.n_layer)]
     sequential = RemoteSequential(
         config,
-        dht,
-        sequence_manager=TestSequenceManager(dht, block_uids, sequential.p2p, _was_shut_down=shutdown_evt),
+        sequence_manager=TestSequenceManager(config, block_uids, dht=dht, _was_shut_down=shutdown_evt),
     )
 
     sequence = sequential.sequence_manager.make_sequence(mode=mode)
     assert all(sequence[i].peer_id != sequence[i + 1].peer_id for i in range(len(sequence) - 1))
 
     assert sequential.sequence_manager.is_alive()
     assert sequential.sequence_manager._thread.ready.is_set()
```

### Comparing `petals-1.1.4/tests/test_server_stats.py` & `petals-1.1.5/tests/test_server_stats.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 import time
 
 import hivemind
 import pytest
 import torch
 
-from petals.client import DistributedBloomConfig
+from petals.client import DistributedBloomConfig, RemoteSequential
 from petals.data_structures import UID_DELIMITER
-from petals.dht_utils import get_remote_sequence
 from petals.server.handler import CACHE_TOKENS_AVAILABLE
 from test_utils import *
 
 
 @pytest.mark.forked
 def test_server_info(block_from: int = 22, block_to: int = 24, max_length: int = 100, max_length2: int = 50):
-    dht = hivemind.DHT(initial_peers=INITIAL_PEERS, client_mode=True, start=True)
     config = DistributedBloomConfig.from_pretrained(MODEL_NAME)
+    dht = hivemind.DHT(initial_peers=INITIAL_PEERS, client_mode=True, start=True)
+    blocks1 = RemoteSequential(config, dht=dht, start_block=block_from, end_block=block_to)
+    blocks2 = RemoteSequential(config, dht=dht, start_block=block_to - 1, end_block=block_to)
 
-    blocks1 = get_remote_sequence(dht, block_from, block_to, config, f"{MODEL_NAME}{UID_DELIMITER}")
-    blocks2 = get_remote_sequence(dht, block_to - 1, block_to, config, f"{MODEL_NAME}{UID_DELIMITER}")
     info_before = blocks1.sequence_manager.rpc_info
 
     with blocks1.inference_session(max_length=max_length) as sess:
         sess.step(torch.randn(1, 1, config.hidden_size))
-        blocks1.sequence_manager._rpc_info = None  # invalidate cache
+        blocks1.sequence_manager.state.rpc_info = None  # invalidate cache
         info_inside = blocks1.sequence_manager.rpc_info
 
         with blocks2.inference_session(max_length=max_length2) as sess2:
             sess2.step(torch.randn(1, 1, config.hidden_size))
-            blocks2.sequence_manager._rpc_info = None  # invalidate cache
+            blocks2.sequence_manager.state.rpc_info = None  # invalidate cache
             info_inside2 = blocks2.sequence_manager.rpc_info
 
     time.sleep(0.1)
-    blocks1.sequence_manager._rpc_info = None  # invalidate cache
+    blocks1.sequence_manager.state.rpc_info = None  # invalidate cache
     info_after = blocks1.sequence_manager.rpc_info
 
     assert info_before[CACHE_TOKENS_AVAILABLE] == info_after[CACHE_TOKENS_AVAILABLE]
     assert info_before[CACHE_TOKENS_AVAILABLE] - info_inside[CACHE_TOKENS_AVAILABLE] == max_length * len(blocks1)
     assert info_inside[CACHE_TOKENS_AVAILABLE] - info_inside2[CACHE_TOKENS_AVAILABLE] == max_length2 * len(blocks2)
```

### Comparing `petals-1.1.4/tests/test_tensor_parallel.py` & `petals-1.1.5/tests/test_tensor_parallel.py`

 * *Files identical despite different names*

