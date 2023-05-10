# Comparing `tmp/domino-py-0.2.1.tar.gz` & `tmp/domino-py-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domino-py-0.2.1.tar", last modified: Wed May 10 10:12:44 2023, max compression
+gzip compressed data, was "domino-py-0.2.2.tar", last modified: Wed May 10 14:01:36 2023, max compression
```

## Comparing `domino-py-0.2.1.tar` & `domino-py-0.2.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:12:44.789014 domino-py-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-10 10:12:29.000000 domino-py-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-05-10 10:12:44.789014 domino-py-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-05-10 10:12:29.000000 domino-py-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:12:44.781014 domino-py-0.2.1/domino/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14950 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/base_piece.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:12:44.781014 domino-py-0.2.1/domino/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:12:44.781014 domino-py-0.2.1/domino/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/cli/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17348 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/cli/utils/pieces_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/cli/utils/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:12:44.781014 domino-py-0.2.1/domino/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/client/airflow_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/client/domino_backend_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/client/fs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/client/github_rest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/client/local_files_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/client/s3_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:12:44.781014 domino-py-0.2.1/domino/custom_operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/custom_operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/custom_operators/docker_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/custom_operators/external_python_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17007 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/custom_operators/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/custom_operators/python_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:12:44.781014 domino-py-0.2.1/domino/custom_operators/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/custom_operators/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/custom_operators/sidecar/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/custom_operators/sidecar/mount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:12:44.781014 domino-py-0.2.1/domino/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/exceptions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:12:44.785014 domino-py-0.2.1/domino/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/schemas/container_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/schemas/deploy_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/schemas/from_upstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/schemas/piece_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/schemas/shared_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:12:44.785014 domino-py-0.2.1/domino/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/scripts/build_docker_images_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/scripts/create_docker_compose_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/scripts/docker_compose_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/scripts/docker_compose_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/scripts/load_piece.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/scripts/piece_dry_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/scripts/run_piece_bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/scripts/run_piece_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/scripts/run_piece_k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:12:44.785014 domino-py-0.2.1/domino/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/utils/metadata_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/utils/piece_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/utils/workflow_shared_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 10:12:29.000000 domino-py-0.2.1/domino/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:12:44.789014 domino-py-0.2.1/domino_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-05-10 10:12:44.000000 domino-py-0.2.1/domino_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-10 10:12:44.000000 domino-py-0.2.1/domino_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 10:12:44.000000 domino-py-0.2.1/domino_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 10:12:44.000000 domino-py-0.2.1/domino_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-10 10:12:44.000000 domino-py-0.2.1/domino_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 10:12:44.000000 domino-py-0.2.1/domino_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 10:12:44.789014 domino-py-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-10 10:12:29.000000 domino-py-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:01:36.203539 domino-py-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-10 14:01:21.000000 domino-py-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-05-10 14:01:36.203539 domino-py-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-10 14:01:21.000000 domino-py-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:01:36.199539 domino-py-0.2.2/domino/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14950 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/base_piece.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:01:36.199539 domino-py-0.2.2/domino/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:01:36.199539 domino-py-0.2.2/domino/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/cli/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17348 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/cli/utils/pieces_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/cli/utils/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:01:36.199539 domino-py-0.2.2/domino/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/client/airflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/client/domino_backend_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/client/fs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/client/github_rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/client/local_files_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/client/s3_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:01:36.199539 domino-py-0.2.2/domino/custom_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/custom_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/custom_operators/docker_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/custom_operators/external_python_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17007 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/custom_operators/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/custom_operators/python_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:01:36.199539 domino-py-0.2.2/domino/custom_operators/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/custom_operators/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/custom_operators/sidecar/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/custom_operators/sidecar/mount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:01:36.199539 domino-py-0.2.2/domino/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/exceptions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:01:36.203539 domino-py-0.2.2/domino/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/schemas/container_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/schemas/deploy_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/schemas/from_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/schemas/piece_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/schemas/shared_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:01:36.203539 domino-py-0.2.2/domino/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/scripts/build_docker_images_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/scripts/create_docker_compose_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/scripts/docker_compose_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/scripts/docker_compose_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/scripts/load_piece.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/scripts/piece_dry_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/scripts/run_piece_bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/scripts/run_piece_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/scripts/run_piece_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:01:36.203539 domino-py-0.2.2/domino/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/utils/metadata_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/utils/piece_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/utils/workflow_shared_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 14:01:21.000000 domino-py-0.2.2/domino/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:01:36.203539 domino-py-0.2.2/domino_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-05-10 14:01:35.000000 domino-py-0.2.2/domino_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-10 14:01:36.000000 domino-py-0.2.2/domino_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:01:35.000000 domino-py-0.2.2/domino_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 14:01:35.000000 domino-py-0.2.2/domino_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-10 14:01:35.000000 domino-py-0.2.2/domino_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 14:01:35.000000 domino-py-0.2.2/domino_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 14:01:36.203539 domino-py-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-10 14:01:22.000000 domino-py-0.2.2/setup.py
```

### Comparing `domino-py-0.2.1/LICENSE` & `domino-py-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/PKG-INFO` & `domino-py-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: domino-py
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python package for the Domino platform
 Home-page: UNKNOWN
 Author: Luiz Tauffer and Vinicius Vaz
 Author-email: luiz@taufferconsulting.com
 License: UNKNOWN
 Description: 
         
         <p align="center">
-          <img src="./media/logo.png" width="450" title="Domino">
+          <img src="https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/media/logo.png" width="450" title="Domino">
         </p>
         <p align="center">
           <a href="https://pypi.org/project/domino-py">
             <img src="https://img.shields.io/pypi/v/domino-py?color=%231BA331&label=PyPI&logo=python&logoColor=%23F7F991%20">
           </a>
           <a href="https://artifacthub.io/packages/helm/domino/domino">
             <img src="https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/domino">
@@ -81,54 +81,54 @@
         
         <details>
           <summary>
             <strong>Install Pieces repositories</strong>
           </summary>
           Install bundles of Pieces to your Domino Workspaces direclty from Github repositories, and use them in your Workflows. <br></br>
         
-          ![add gif]()
+          ![install pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/3_install_pieces.gif)
         
         </details>
         
         <details>
           <summary>
             <strong>Create Workflows</strong>
           </summary>
           Create Workflows by dragging and dropping Pieces to the canvas, and connecting them. <br></br>
         
-          ![add gif]()
+          ![create workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/4_create_workflow.gif)
         
         </details>
         
         <details>
           <summary>
             <strong>Edit Pieces</strong>
           </summary>
           Edit Pieces by changing their input. Outputs from upstream Pieces are automatically available as inputs for downstream Pieces. Pieces can pass forward any type of data, from simple strings to heavy files, all automatically handled by Domino shared storage system. <br></br>
         
-          ![add gif]()
+          ![edit pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/5_edit_pieces.gif)
         
         </details>
         
         <details>
           <summary>
             <strong>Schedule Workflows</strong>
           </summary>
           Schedule Workflows to run periodically, at a specific date/time, or trigger them manually. <br></br>
         
-          ![add gif]()
+          ![schedule workflows](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/6_edit_workflow.gif)
         </details>
         
         <details>
           <summary>
             <strong>Monitor Workflows</strong>
           </summary>
           Monitor Workflows in real time, including the status of each Piece, the logs and results of each run. <br></br>
         
-          ![add gif]()
+          ![monitor workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/7_monitor_workflow.gif)
         
         </details>
         
         <br>
         
         # REST
         The Backend service is a REST API that controls a running Apache Airflow instance. It is responsible for:
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
-Metadata-Version: 2.1 Name: domino-py Version: 0.2.1 Summary: Python package
+Metadata-Version: 2.1 Name: domino-py Version: 0.2.2 Summary: Python package
 for the Domino platform Home-page: UNKNOWN Author: Luiz Tauffer and Vinicius
 Vaz Author-email: luiz@taufferconsulting.com License: UNKNOWN Description:
-                              [./media/logo.png]
+   [https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/media/
+                                   logo.png]
                     [https://img.shields.io/pypi/v/domino-
   py?color=%231BA331&label=PyPI&logo=python&logoColor=%23F7F991%20] [https://
  img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/domino]
                                 [Read_the_Docs]
 # Table of contents - [About](#about) - [Quick start](#quick-start) - [GUI]
 (#gui) - [REST](#rest) - [Pieces](#pieces)
 # About Domino is an open source workflow management platform, with: - an
@@ -43,25 +44,34 @@
 Domino in a [remote Kubernetes cluster](https://domino-py.readthedocs.io/en/
 latest/pages/deployment_cloud.html)
 # GUI The Domino frontend service is a React application that provides the GUI
 for easily creating, editing and monitoring Workflows. Here are some of its
 features:   Install Pieces repositories  Install bundles of Pieces to your
 Domino Workspaces direclty from Github repositories, and use them in your
 Workflows.
-![add gif]()    Create Workflows  Create Workflows by dragging and dropping
-Pieces to the canvas, and connecting them.
-![add gif]()    Edit Pieces  Edit Pieces by changing their input. Outputs from
-upstream Pieces are automatically available as inputs for downstream Pieces.
-Pieces can pass forward any type of data, from simple strings to heavy files,
-all automatically handled by Domino shared storage system.
-![add gif]()    Schedule Workflows  Schedule Workflows to run periodically, at
-a specific date/time, or trigger them manually.
-![add gif]()    Monitor Workflows  Monitor Workflows in real time, including
-the status of each Piece, the logs and results of each run.
-![add gif]()
+![install pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/
+main/docs/source/_static/media/3_install_pieces.gif)    Create Workflows
+Create Workflows by dragging and dropping Pieces to the canvas, and connecting
+them.
+![create workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/
+main/docs/source/_static/media/4_create_workflow.gif)    Edit Pieces  Edit
+Pieces by changing their input. Outputs from upstream Pieces are automatically
+available as inputs for downstream Pieces. Pieces can pass forward any type of
+data, from simple strings to heavy files, all automatically handled by Domino
+shared storage system.
+![edit pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/
+main/docs/source/_static/media/5_edit_pieces.gif)    Schedule Workflows
+Schedule Workflows to run periodically, at a specific date/time, or trigger
+them manually.
+![schedule workflows](https://raw.githubusercontent.com/Tauffer-Consulting/
+domino/main/docs/source/_static/media/6_edit_workflow.gif)    Monitor Workflows
+Monitor Workflows in real time, including the status of each Piece, the logs
+and results of each run.
+![monitor workflow](https://raw.githubusercontent.com/Tauffer-Consulting/
+domino/main/docs/source/_static/media/7_monitor_workflow.gif)
 # REST The Backend service is a REST API that controls a running Apache Airflow
 instance. It is responsible for: - executing operations requested by the
 frontend service - interacting with the Airflow instance, including triggering,
 creating, editing and deleting Workflows (DAGs) - interacting with the Domino
 Database The REST service is written in Python, using the FastAPI framework.
 Read more about it in the [REST documentation](https://domino-
 py.readthedocs.io/en/latest/pages/rest.html).
```

### Comparing `domino-py-0.2.1/README.md` & `domino-py-0.2.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 
 <p align="center">
-  <img src="./media/logo.png" width="450" title="Domino">
+  <img src="https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/media/logo.png" width="450" title="Domino">
 </p>
 <p align="center">
   <a href="https://pypi.org/project/domino-py">
     <img src="https://img.shields.io/pypi/v/domino-py?color=%231BA331&label=PyPI&logo=python&logoColor=%23F7F991%20">
   </a>
   <a href="https://artifacthub.io/packages/helm/domino/domino">
     <img src="https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/domino">
@@ -73,54 +73,54 @@
 
 <details>
   <summary>
     <strong>Install Pieces repositories</strong>
   </summary>
   Install bundles of Pieces to your Domino Workspaces direclty from Github repositories, and use them in your Workflows. <br></br>
 
-  ![add gif]()
+  ![install pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/3_install_pieces.gif)
 
 </details>
 
 <details>
   <summary>
     <strong>Create Workflows</strong>
   </summary>
   Create Workflows by dragging and dropping Pieces to the canvas, and connecting them. <br></br>
 
-  ![add gif]()
+  ![create workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/4_create_workflow.gif)
 
 </details>
 
 <details>
   <summary>
     <strong>Edit Pieces</strong>
   </summary>
   Edit Pieces by changing their input. Outputs from upstream Pieces are automatically available as inputs for downstream Pieces. Pieces can pass forward any type of data, from simple strings to heavy files, all automatically handled by Domino shared storage system. <br></br>
 
-  ![add gif]()
+  ![edit pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/5_edit_pieces.gif)
 
 </details>
 
 <details>
   <summary>
     <strong>Schedule Workflows</strong>
   </summary>
   Schedule Workflows to run periodically, at a specific date/time, or trigger them manually. <br></br>
 
-  ![add gif]()
+  ![schedule workflows](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/6_edit_workflow.gif)
 </details>
 
 <details>
   <summary>
     <strong>Monitor Workflows</strong>
   </summary>
   Monitor Workflows in real time, including the status of each Piece, the logs and results of each run. <br></br>
 
-  ![add gif]()
+  ![monitor workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/7_monitor_workflow.gif)
 
 </details>
 
 <br>
 
 # REST
 The Backend service is a REST API that controls a running Apache Airflow instance. It is responsible for:
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
-                              [./media/logo.png]
+   [https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/media/
+                                   logo.png]
                     [https://img.shields.io/pypi/v/domino-
   py?color=%231BA331&label=PyPI&logo=python&logoColor=%23F7F991%20] [https://
  img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/domino]
                                 [Read_the_Docs]
 # Table of contents - [About](#about) - [Quick start](#quick-start) - [GUI]
 (#gui) - [REST](#rest) - [Pieces](#pieces)
 # About Domino is an open source workflow management platform, with: - an
@@ -40,25 +41,34 @@
 Domino in a [remote Kubernetes cluster](https://domino-py.readthedocs.io/en/
 latest/pages/deployment_cloud.html)
 # GUI The Domino frontend service is a React application that provides the GUI
 for easily creating, editing and monitoring Workflows. Here are some of its
 features:   Install Pieces repositories  Install bundles of Pieces to your
 Domino Workspaces direclty from Github repositories, and use them in your
 Workflows.
-![add gif]()    Create Workflows  Create Workflows by dragging and dropping
-Pieces to the canvas, and connecting them.
-![add gif]()    Edit Pieces  Edit Pieces by changing their input. Outputs from
-upstream Pieces are automatically available as inputs for downstream Pieces.
-Pieces can pass forward any type of data, from simple strings to heavy files,
-all automatically handled by Domino shared storage system.
-![add gif]()    Schedule Workflows  Schedule Workflows to run periodically, at
-a specific date/time, or trigger them manually.
-![add gif]()    Monitor Workflows  Monitor Workflows in real time, including
-the status of each Piece, the logs and results of each run.
-![add gif]()
+![install pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/
+main/docs/source/_static/media/3_install_pieces.gif)    Create Workflows
+Create Workflows by dragging and dropping Pieces to the canvas, and connecting
+them.
+![create workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/
+main/docs/source/_static/media/4_create_workflow.gif)    Edit Pieces  Edit
+Pieces by changing their input. Outputs from upstream Pieces are automatically
+available as inputs for downstream Pieces. Pieces can pass forward any type of
+data, from simple strings to heavy files, all automatically handled by Domino
+shared storage system.
+![edit pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/
+main/docs/source/_static/media/5_edit_pieces.gif)    Schedule Workflows
+Schedule Workflows to run periodically, at a specific date/time, or trigger
+them manually.
+![schedule workflows](https://raw.githubusercontent.com/Tauffer-Consulting/
+domino/main/docs/source/_static/media/6_edit_workflow.gif)    Monitor Workflows
+Monitor Workflows in real time, including the status of each Piece, the logs
+and results of each run.
+![monitor workflow](https://raw.githubusercontent.com/Tauffer-Consulting/
+domino/main/docs/source/_static/media/7_monitor_workflow.gif)
 # REST The Backend service is a REST API that controls a running Apache Airflow
 instance. It is responsible for: - executing operations requested by the
 frontend service - interacting with the Airflow instance, including triggering,
 creating, editing and deleting Workflows (DAGs) - interacting with the Domino
 Database The REST service is written in Python, using the FastAPI framework.
 Read more about it in the [REST documentation](https://domino-
 py.readthedocs.io/en/latest/pages/rest.html).
```

### Comparing `domino-py-0.2.1/domino/base_piece.py` & `domino-py-0.2.2/domino/base_piece.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/cli/cli.py` & `domino-py-0.2.2/domino/cli/cli.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/cli/utils/pieces_repository.py` & `domino-py-0.2.2/domino/cli/utils/pieces_repository.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/cli/utils/platform.py` & `domino-py-0.2.2/domino/cli/utils/platform.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/client/airflow_client.py` & `domino-py-0.2.2/domino/client/airflow_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/client/domino_backend_client.py` & `domino-py-0.2.2/domino/client/domino_backend_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/client/fs_client.py` & `domino-py-0.2.2/domino/client/fs_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/client/github_rest_client.py` & `domino-py-0.2.2/domino/client/github_rest_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/client/local_files_client.py` & `domino-py-0.2.2/domino/client/local_files_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/client/s3_client.py` & `domino-py-0.2.2/domino/client/s3_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/custom_operators/docker_operator.py` & `domino-py-0.2.2/domino/custom_operators/docker_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/custom_operators/external_python_operator.py` & `domino-py-0.2.2/domino/custom_operators/external_python_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/custom_operators/k8s_operator.py` & `domino-py-0.2.2/domino/custom_operators/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/custom_operators/python_operator.py` & `domino-py-0.2.2/domino/custom_operators/python_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/custom_operators/sidecar/logger.py` & `domino-py-0.2.2/domino/custom_operators/sidecar/logger.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/custom_operators/sidecar/mount.py` & `domino-py-0.2.2/domino/custom_operators/sidecar/mount.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/exceptions/exceptions.py` & `domino-py-0.2.2/domino/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/logger.py` & `domino-py-0.2.2/domino/logger.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/schemas/piece_metadata.py` & `domino-py-0.2.2/domino/schemas/piece_metadata.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/schemas/shared_storage.py` & `domino-py-0.2.2/domino/schemas/shared_storage.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/scripts/build_docker_images_pieces.py` & `domino-py-0.2.2/domino/scripts/build_docker_images_pieces.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/scripts/create_docker_compose_file.py` & `domino-py-0.2.2/domino/scripts/create_docker_compose_file.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/scripts/docker_compose_constants.py` & `domino-py-0.2.2/domino/scripts/docker_compose_constants.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/scripts/docker_compose_scripts.py` & `domino-py-0.2.2/domino/scripts/docker_compose_scripts.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/scripts/load_piece.py` & `domino-py-0.2.2/domino/scripts/load_piece.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/scripts/piece_dry_run.py` & `domino-py-0.2.2/domino/scripts/piece_dry_run.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/scripts/run_piece_bash.py` & `domino-py-0.2.2/domino/scripts/run_piece_bash.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/scripts/run_piece_docker.py` & `domino-py-0.2.2/domino/scripts/run_piece_docker.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/scripts/run_piece_k8s.py` & `domino-py-0.2.2/domino/scripts/run_piece_k8s.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/task.py` & `domino-py-0.2.2/domino/task.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino/utils/piece_generator.py` & `domino-py-0.2.2/domino/utils/piece_generator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/domino_py.egg-info/PKG-INFO` & `domino-py-0.2.2/domino_py.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: domino-py
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python package for the Domino platform
 Home-page: UNKNOWN
 Author: Luiz Tauffer and Vinicius Vaz
 Author-email: luiz@taufferconsulting.com
 License: UNKNOWN
 Description: 
         
         <p align="center">
-          <img src="./media/logo.png" width="450" title="Domino">
+          <img src="https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/media/logo.png" width="450" title="Domino">
         </p>
         <p align="center">
           <a href="https://pypi.org/project/domino-py">
             <img src="https://img.shields.io/pypi/v/domino-py?color=%231BA331&label=PyPI&logo=python&logoColor=%23F7F991%20">
           </a>
           <a href="https://artifacthub.io/packages/helm/domino/domino">
             <img src="https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/domino">
@@ -81,54 +81,54 @@
         
         <details>
           <summary>
             <strong>Install Pieces repositories</strong>
           </summary>
           Install bundles of Pieces to your Domino Workspaces direclty from Github repositories, and use them in your Workflows. <br></br>
         
-          ![add gif]()
+          ![install pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/3_install_pieces.gif)
         
         </details>
         
         <details>
           <summary>
             <strong>Create Workflows</strong>
           </summary>
           Create Workflows by dragging and dropping Pieces to the canvas, and connecting them. <br></br>
         
-          ![add gif]()
+          ![create workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/4_create_workflow.gif)
         
         </details>
         
         <details>
           <summary>
             <strong>Edit Pieces</strong>
           </summary>
           Edit Pieces by changing their input. Outputs from upstream Pieces are automatically available as inputs for downstream Pieces. Pieces can pass forward any type of data, from simple strings to heavy files, all automatically handled by Domino shared storage system. <br></br>
         
-          ![add gif]()
+          ![edit pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/5_edit_pieces.gif)
         
         </details>
         
         <details>
           <summary>
             <strong>Schedule Workflows</strong>
           </summary>
           Schedule Workflows to run periodically, at a specific date/time, or trigger them manually. <br></br>
         
-          ![add gif]()
+          ![schedule workflows](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/6_edit_workflow.gif)
         </details>
         
         <details>
           <summary>
             <strong>Monitor Workflows</strong>
           </summary>
           Monitor Workflows in real time, including the status of each Piece, the logs and results of each run. <br></br>
         
-          ![add gif]()
+          ![monitor workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/docs/source/_static/media/7_monitor_workflow.gif)
         
         </details>
         
         <br>
         
         # REST
         The Backend service is a REST API that controls a running Apache Airflow instance. It is responsible for:
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
-Metadata-Version: 2.1 Name: domino-py Version: 0.2.1 Summary: Python package
+Metadata-Version: 2.1 Name: domino-py Version: 0.2.2 Summary: Python package
 for the Domino platform Home-page: UNKNOWN Author: Luiz Tauffer and Vinicius
 Vaz Author-email: luiz@taufferconsulting.com License: UNKNOWN Description:
-                              [./media/logo.png]
+   [https://raw.githubusercontent.com/Tauffer-Consulting/domino/main/media/
+                                   logo.png]
                     [https://img.shields.io/pypi/v/domino-
   py?color=%231BA331&label=PyPI&logo=python&logoColor=%23F7F991%20] [https://
  img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/domino]
                                 [Read_the_Docs]
 # Table of contents - [About](#about) - [Quick start](#quick-start) - [GUI]
 (#gui) - [REST](#rest) - [Pieces](#pieces)
 # About Domino is an open source workflow management platform, with: - an
@@ -43,25 +44,34 @@
 Domino in a [remote Kubernetes cluster](https://domino-py.readthedocs.io/en/
 latest/pages/deployment_cloud.html)
 # GUI The Domino frontend service is a React application that provides the GUI
 for easily creating, editing and monitoring Workflows. Here are some of its
 features:   Install Pieces repositories  Install bundles of Pieces to your
 Domino Workspaces direclty from Github repositories, and use them in your
 Workflows.
-![add gif]()    Create Workflows  Create Workflows by dragging and dropping
-Pieces to the canvas, and connecting them.
-![add gif]()    Edit Pieces  Edit Pieces by changing their input. Outputs from
-upstream Pieces are automatically available as inputs for downstream Pieces.
-Pieces can pass forward any type of data, from simple strings to heavy files,
-all automatically handled by Domino shared storage system.
-![add gif]()    Schedule Workflows  Schedule Workflows to run periodically, at
-a specific date/time, or trigger them manually.
-![add gif]()    Monitor Workflows  Monitor Workflows in real time, including
-the status of each Piece, the logs and results of each run.
-![add gif]()
+![install pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/
+main/docs/source/_static/media/3_install_pieces.gif)    Create Workflows
+Create Workflows by dragging and dropping Pieces to the canvas, and connecting
+them.
+![create workflow](https://raw.githubusercontent.com/Tauffer-Consulting/domino/
+main/docs/source/_static/media/4_create_workflow.gif)    Edit Pieces  Edit
+Pieces by changing their input. Outputs from upstream Pieces are automatically
+available as inputs for downstream Pieces. Pieces can pass forward any type of
+data, from simple strings to heavy files, all automatically handled by Domino
+shared storage system.
+![edit pieces](https://raw.githubusercontent.com/Tauffer-Consulting/domino/
+main/docs/source/_static/media/5_edit_pieces.gif)    Schedule Workflows
+Schedule Workflows to run periodically, at a specific date/time, or trigger
+them manually.
+![schedule workflows](https://raw.githubusercontent.com/Tauffer-Consulting/
+domino/main/docs/source/_static/media/6_edit_workflow.gif)    Monitor Workflows
+Monitor Workflows in real time, including the status of each Piece, the logs
+and results of each run.
+![monitor workflow](https://raw.githubusercontent.com/Tauffer-Consulting/
+domino/main/docs/source/_static/media/7_monitor_workflow.gif)
 # REST The Backend service is a REST API that controls a running Apache Airflow
 instance. It is responsible for: - executing operations requested by the
 frontend service - interacting with the Airflow instance, including triggering,
 creating, editing and deleting Workflows (DAGs) - interacting with the Domino
 Database The REST service is written in Python, using the FastAPI framework.
 Read more about it in the [REST documentation](https://domino-
 py.readthedocs.io/en/latest/pages/rest.html).
```

### Comparing `domino-py-0.2.1/domino_py.egg-info/SOURCES.txt` & `domino-py-0.2.2/domino_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domino-py-0.2.1/setup.py` & `domino-py-0.2.2/setup.py`

 * *Files identical despite different names*

