# Comparing `tmp/domino-py-0.1.9.tar.gz` & `tmp/domino-py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domino-py-0.1.9.tar", last modified: Fri Apr 28 19:15:19 2023, max compression
+gzip compressed data, was "domino-py-0.2.0.tar", last modified: Wed May 10 09:47:55 2023, max compression
```

## Comparing `domino-py-0.1.9.tar` & `domino-py-0.2.0.tar`

### file list

```diff
@@ -1,103 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.462423 domino-py-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-28 19:15:06.000000 domino-py-0.1.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-28 19:15:06.000000 domino-py-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-28 19:15:19.462423 domino-py-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-28 19:15:06.000000 domino-py-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.454423 domino-py-0.1.9/domino/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/base_piece.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.454423 domino-py-0.1.9/domino/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.454423 domino-py-0.1.9/domino/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/cli/utils/config-domino-local.toml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/cli/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17343 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/cli/utils/pieces_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    22540 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/cli/utils/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.454423 domino-py-0.1.9/domino/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/client/airflow_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/client/domino_backend_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/client/fs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/client/github_rest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/client/local_files_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/client/s3_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.454423 domino-py-0.1.9/domino/custom_operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/custom_operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/custom_operators/bash_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/custom_operators/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/custom_operators/python_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.454423 domino-py-0.1.9/domino/custom_operators/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/custom_operators/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/custom_operators/sidecar/fuse.conf
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/custom_operators/sidecar/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/custom_operators/sidecar/mount.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/custom_operators/sidecar/rclone.conf
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/custom_operators/sidecar/sidecar_lifecycle.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.454423 domino-py-0.1.9/domino/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.454423 domino-py-0.1.9/domino/helm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.454423 domino-py-0.1.9/domino/helm/domino-airflow/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-airflow/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.458423 domino-py-0.1.9/domino/helm/domino-airflow/charts/
--rw-r--r--   0 runner    (1001) docker     (123)   157053 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-airflow/charts/airflow-1.7.0.tgz
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-airflow/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.458423 domino-py-0.1.9/domino/helm/domino-base/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/.helmignore
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/Chart.lock
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.458423 domino-py-0.1.9/domino/helm/domino-base/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/templates/domino-backend-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/templates/domino-frontend-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/templates/domino-postgres-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/templates/ingress-api.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/templates/ingress-frontend.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.458423 domino-py-0.1.9/domino/helm/domino-base/templates/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/templates/jobs/domino-migrations.yml
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/templates/secrets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.458423 domino-py-0.1.9/domino/helm/domino-base/templates/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/templates/volumes/domino-rest-volume-claim-dev.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/templates/volumes/domino-rest-volume-dev.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/helm/domino-base/values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/piece_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.458423 domino-py-0.1.9/domino/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/schemas/container_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/schemas/from_upstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/schemas/piece_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/schemas/shared_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.458423 domino-py-0.1.9/domino/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/scripts/build_docker_images_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/scripts/create_docker_compose_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/scripts/docker_compose_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/scripts/docker_compose_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/scripts/generate_infrasctructure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/scripts/load_piece.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/scripts/run_piece_bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/scripts/run_piece_dry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/scripts/run_piece_k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)    11812 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.462423 domino-py-0.1.9/domino/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/utils/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/utils/enum_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/utils/metadata_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/utils/types_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/utils/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/utils/workflow_shared_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 19:15:06.000000 domino-py-0.1.9/domino/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:15:19.462423 domino-py-0.1.9/domino_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-28 19:15:19.000000 domino-py-0.1.9/domino_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-28 19:15:19.000000 domino-py-0.1.9/domino_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:15:19.000000 domino-py-0.1.9/domino_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-28 19:15:19.000000 domino-py-0.1.9/domino_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-28 19:15:19.000000 domino-py-0.1.9/domino_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 19:15:19.000000 domino-py-0.1.9/domino_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-28 19:15:06.000000 domino-py-0.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 19:15:19.462423 domino-py-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-28 19:15:06.000000 domino-py-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:55.610128 domino-py-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-10 09:47:42.000000 domino-py-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-05-10 09:47:55.610128 domino-py-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-05-10 09:47:42.000000 domino-py-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:55.606128 domino-py-0.2.0/domino/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14950 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/base_piece.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:55.606128 domino-py-0.2.0/domino/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:55.606128 domino-py-0.2.0/domino/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/cli/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17348 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/cli/utils/pieces_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/cli/utils/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:55.606128 domino-py-0.2.0/domino/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/client/airflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/client/domino_backend_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/client/fs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/client/github_rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/client/local_files_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/client/s3_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:55.606128 domino-py-0.2.0/domino/custom_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/custom_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/custom_operators/docker_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/custom_operators/external_python_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17007 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/custom_operators/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/custom_operators/python_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:55.606128 domino-py-0.2.0/domino/custom_operators/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/custom_operators/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/custom_operators/sidecar/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/custom_operators/sidecar/mount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:55.606128 domino-py-0.2.0/domino/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/exceptions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:55.606128 domino-py-0.2.0/domino/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/schemas/container_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/schemas/deploy_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/schemas/from_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/schemas/piece_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/schemas/shared_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:55.610128 domino-py-0.2.0/domino/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/scripts/build_docker_images_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/scripts/create_docker_compose_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/scripts/docker_compose_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/scripts/docker_compose_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/scripts/load_piece.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/scripts/piece_dry_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/scripts/run_piece_bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/scripts/run_piece_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/scripts/run_piece_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:55.610128 domino-py-0.2.0/domino/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/utils/metadata_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/utils/piece_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/utils/workflow_shared_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 09:47:42.000000 domino-py-0.2.0/domino/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:47:55.610128 domino-py-0.2.0/domino_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-05-10 09:47:55.000000 domino-py-0.2.0/domino_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-10 09:47:55.000000 domino-py-0.2.0/domino_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:47:55.000000 domino-py-0.2.0/domino_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 09:47:55.000000 domino-py-0.2.0/domino_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-10 09:47:55.000000 domino-py-0.2.0/domino_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 09:47:55.000000 domino-py-0.2.0/domino_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 09:47:55.610128 domino-py-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-10 09:47:42.000000 domino-py-0.2.0/setup.py
```

### Comparing `domino-py-0.1.9/LICENSE.md` & `domino-py-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.9/domino/base_piece.py` & `domino-py-0.2.0/domino/base_piece.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import abc
 import json
 import os
 import ast
 from datetime import datetime
 from pathlib import Path
 import pydantic
-
+import pickle
 from domino.logger import get_configured_logger
-from domino.utils.enum_types import DeployModeType
+from domino.schemas.deploy_mode import DeployModeType
 from domino.exceptions.exceptions import InvalidPieceOutputError
 import time
 import subprocess
 
 
 class BasePiece(metaclass=abc.ABCMeta):
 
@@ -113,35 +113,40 @@
                 self.upstream_tasks_data[tid]["results"] = self.workflow_shared_storage + f"/{tid}/results"
                 with open(f"{self.workflow_shared_storage}/{tid}/xcom/return.json") as f:
                     self.upstream_tasks_data[tid]["xcom"] = json.load(f)
         else:
             raise NotImplementedError(f"Get upstream XCOM not implemented for deploy_mode=={self.deploy_mode}")
 
     
-    def validate_and_get_env_secrets(self, piece_secrets_model: pydantic.BaseModel = None):
+    def validate_and_get_env_secrets(self, piece_secrets_model: pydantic.BaseModel = None, secrets_values=None):
         """
         Get secret variables for this Piece from ENV. The necessary secret variables to run the Piece should be defined in the Piece's SecretsModel.
         The secrets can then be retrieved and used in the Piece's `piece_function` method as such:
         ```
         my_secret = self.secrets.my_secret
         ```
 
         Args:
             piece_secrets_model (pydantic.BaseModel): _description_
         """
         self.secrets = None
-        if piece_secrets_model:
+        if piece_secrets_model and self.deploy_mode in ['local-k8s', 'local-k8s-dev', 'prod']:
             secrets_names = list(piece_secrets_model.schema()["properties"].keys())
             secrets = dict()
-            secrets_values = ast.literal_eval(os.environ.get('DOMINO_K8S_PIECE_SECRETS'))
+            secrets_values = ast.literal_eval(os.environ.get('DOMINO_K8S_PIECE_SECRETS', '{}'))
             if not secrets_values:
                 secrets_values = {}
             for s in secrets_names:
                 secrets[s] = secrets_values.get(s, None)
             self.secrets = piece_secrets_model(**secrets)
+        elif piece_secrets_model and self.deploy_mode == 'local-compose':
+            secrets_names = list(piece_secrets_model.schema()["properties"].keys())
+            secrets = dict()
+            secrets_values = ast.literal_eval(os.environ.get('DOMINO_DOCKER_PIECE_SECRETS', '{}'))
+            self.secrets = piece_secrets_model(**secrets_values)
 
 
     def format_xcom(self, output_obj: pydantic.BaseModel) -> dict:
         """
         Formats and adds extra metadata to XCOM dictionary content.
 
         Args:
@@ -187,16 +192,22 @@
 
         Args:
             xcom_obj (dict): Formatted XCOM object as a dictionary
 
         Raises:
             NotImplementedError: _description_
         """
-        if self.deploy_mode == "local-python":
+        if self.deploy_mode in ["local-python"]:
             self.airflow_context['ti'].xcom_push(key=self.task_id, value=xcom_obj)
+        elif self.deploy_mode == "local-compose":
+            file_path = Path('/airflow/xcom/return.out')
+            file_path.parent.mkdir(parents=True, exist_ok=True)
+            with open(str(file_path), 'wb') as fp:
+                pickle.dump(xcom_obj, fp)
+
         elif self.deploy_mode == "local-bash":
             # For our extended BashOperator, return XCom must be stored in /opt/mnt/fs/tmp/xcom_output.json
             file_path = Path("/opt/mnt/fs/tmp/xcom_output.json")
             file_path.parent.mkdir(parents=True, exist_ok=True)
             with open(str(file_path), 'w') as fp:
                 json.dump(xcom_obj, fp, indent=4)
         elif self.deploy_mode in ["k8s", "local-k8s", "local-k8s-dev"]:
@@ -207,25 +218,27 @@
             with open(str(file_path), 'w') as fp:
                 json.dump(xcom_obj, fp)
 
             # Also store it at /home/workflow_shared_data/{self.task_id}/xcom/return.json for convenience
             file_path = self.xcom_path + "/return.json"
             with open(file_path, 'w') as fp:
                 json.dump(xcom_obj, fp)
+            #time.sleep(120)
         else:
             raise NotImplementedError("deploy mode not accepted for xcom push")
     
 
     def run_piece_function(
         self, 
         airflow_context: dict,
         op_kwargs: dict,
         piece_input_model: pydantic.BaseModel,
         piece_output_model: pydantic.BaseModel, 
-        piece_secrets_model: pydantic.BaseModel = None
+        piece_secrets_model: pydantic.BaseModel = None,
+        secrets_values: dict = None
     ):
         """
         _summary_
 
         Args:
             airflow_context (dict): Dictionary containing Airflow context information
             op_kwargs (dict): Dictionary containing Piece's kwargs
@@ -245,27 +258,30 @@
 
         # Airflow context dictionary: https://composed.blog/airflow/execute-context
         # For local-bash and kubernetes deploy modes, we assemble this ourselves and the context data is more limited
         self.airflow_context = airflow_context
         self.dag_run_id = airflow_context.get("dag_run_id")
 
         # Check if Piece's necessary secrets are present in ENV
-        self.validate_and_get_env_secrets(piece_secrets_model=piece_secrets_model)
+        self.validate_and_get_env_secrets(piece_secrets_model=piece_secrets_model, secrets_values=secrets_values)
 
         # Generate paths
-        self.workflow_shared_storage = "/home/shared_storage"
+        workflow_run_subpath = os.environ.get('DOMINO_WORKFLOW_RUN_SUBPATH', '')
+        self.workflow_shared_storage = Path("/home/shared_storage") 
+        if self.deploy_mode == 'local-compose':
+            self.workflow_shared_storage = str(self.workflow_shared_storage / workflow_run_subpath)
         self.results_path = f"{self.workflow_shared_storage}/{self.task_id}/results"
         self.xcom_path = f"{self.workflow_shared_storage}/{self.task_id}/xcom"
         self.report_path = f"{self.workflow_shared_storage}/{self.task_id}/report"
         shared_storage_source = os.environ.get('DOMINO_WORKFLOW_SHARED_STORAGE', None)
-        if not shared_storage_source or shared_storage_source == "none":
+        if not shared_storage_source or shared_storage_source == "none" or self.deploy_mode == "local-compose":
             self.generate_paths()
         else:
             self._wait_for_sidecar_paths()
-
+            
         # Using pydantic to validate input data
         input_model_obj = piece_input_model(**op_kwargs)
 
         # Run piece function
         output_obj = self.piece_function(input_model=input_model_obj)
 
         # Validate output data
```

### Comparing `domino-py-0.1.9/domino/cli/cli.py` & `domino-py-0.2.0/domino/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     return cluster_name
 
 
 def get_github_workflows_ssh_private_key_from_env():
     return os.environ.get("DOMINO_GITHUB_WORKFLOWS_SSH_PRIVATE_KEY", "")
 
 def get_github_token_pieces_from_env():
-    return os.environ.get("DOMINO_GITHUB_ACCESS_TOKEN_PIECES", None)
+    return os.environ.get("DOMINO_DEFAULT_PIECES_REPOSITORY_TOKEN", None)
 
 def get_github_token_workflows_from_env():
     return os.environ.get("DOMINO_GITHUB_ACCESS_TOKEN_WORKFLOWS", None)
 
 def get_workflows_repository_from_env():
     return os.environ.get("DOMINO_GITHUB_WORKFLOWS_REPOSITORY", None)
 
@@ -79,29 +79,29 @@
 @click.option(
     '--github-workflows-ssh-private-key', 
     prompt='Github ssh private for Workflows repository. If none, it will create a ssh key pair to be used.',
     default=get_github_workflows_ssh_private_key_from_env,
     help='Github ssh key for GitSync read/write operations on Workflows repository. The private key will be used in the Domino cluster and the public key should be added to the Github repository deploy keys.'
 )
 @click.option(
-    '--github-pieces-token', 
+    '--github-default-pieces-repository-token',
     prompt='Github token for Pieces repository',
     default=get_github_token_pieces_from_env,
     help='Github token for read operations on Pieces repositories.'
 )
 @click.option(
     '--github-workflows-token', 
     prompt='Github token for Workflows Repository',
     default=get_github_token_workflows_from_env,
     help='Github token for read/write operations on Workflows Repository.'
 )
 @click.option(
-    '--dev-mode',
+    '--deploy-mode',
     prompt='Development mode',
-    default="local",
+    default="local-k8s",
     help='Development mode - either "local" or "remote". If local it will allow you to use hot reloading for local operators repositories'
 )
 @click.option(
     '--local-pieces-repository-path',
     prompt='Local pieces repository path. Example: ["/path/to/repo1", "/path/to/"repo2"]',
     default=[],
     help='List of local pieces repository paths. It is used only if dev-mode is set to "local" and it will allow you to use hot reloading for local operators repositories. Example: ["path/to/repo1", "path/to/"repo2"]',
@@ -112,26 +112,26 @@
     default="",
     help="Local Domino path. It is used only if dev-mode is set to 'local' and it will allow you to use hot reloading for local Domino.",
 )
 def cli_prepare_platform(
     cluster_name,
     workflows_repository,
     github_workflows_ssh_private_key,
-    github_pieces_token,
+    github_default_pieces_repository_token,
     github_workflows_token,
     deploy_mode,
     local_pieces_repository_path,
     local_domino_path
 ):
     """Prepare local folder for running a Domino platform."""
     platform.prepare_platform(
         cluster_name=cluster_name, 
         workflows_repository=workflows_repository,
         github_workflows_ssh_private_key=github_workflows_ssh_private_key, 
-        github_pieces_token=github_pieces_token,
+        github_default_pieces_repository_token=github_default_pieces_repository_token,
         github_workflows_token=github_workflows_token,
         deploy_mode=deploy_mode,
         local_pieces_repository_path=ast.literal_eval(local_pieces_repository_path),
         local_domino_path=local_domino_path
     )
 
 
@@ -159,26 +159,39 @@
     default=False
 )
 def cli_create_platform(domino_frontend_image, domino_rest_image, run_airflow, use_gpu):
     """Create cluster, install services and run Domino platform."""
     platform.create_platform(domino_frontend_image, domino_rest_image, run_airflow, use_gpu)
 
 
+@click.command()
+@click.option(
+    "--d",
+    is_flag=True,
+    help="Run in detached mode.",
+    default=False
+)
+def cli_run_platform_compose(d):
+    """Run Domino platform locally with docker compose. Do NOT use this in production."""
+    platform.run_platform_compose(detached=d)
+
+
 @click.group()
 @click.pass_context
 def cli_platform(ctx):
     """Domino platform actions"""
     if ctx.invoked_subcommand == "prepare":
         console.print("Let's get you started configuring a local Domino platform:")
     elif ctx.invoked_subcommand == "create":
         console.print("Your local Domino platform is being created. This might take a while...")    
 
 
 cli_platform.add_command(cli_prepare_platform, name="prepare")
 cli_platform.add_command(cli_create_platform, name="create")
+cli_platform.add_command(cli_run_platform_compose, name="run-compose")
 
 ###############################################################################
 # OPERATORS REPOSITORY 
 ###############################################################################
 
 def generate_random_repo_name():
     return f"new_repository_{str(uuid.uuid4())[0:8]}"
@@ -270,14 +283,21 @@
     from domino.scripts.run_piece_k8s import run_piece as run_piece_in_k8s
     
     console.print("Running Piece inside K8s pod...")
     run_piece_in_k8s()
 
 
 @click.command()
+def cli_run_piece_docker():
+    from domino.scripts.run_piece_docker import run_piece as run_piece_in_docker
+    console.print('Running Piece inside Docker container...')
+    run_piece_in_docker()
+
+
+@click.command()
 def cli_run_piece_bash():
     """Run Piece on bash"""
     from domino.scripts.run_piece_bash import run_piece as run_piece_in_bash
 
     console.print("Running bash Piece...")
     run_piece_in_bash()
 
@@ -294,11 +314,11 @@
     console.print("")
 
 
 cli.add_command(cli_platform, name="platform")
 cli.add_command(cli_piece, name="piece")
 cli.add_command(cli_run_piece_k8s, name="run-piece-k8s")
 cli.add_command(cli_run_piece_bash, name="run-piece-bash")
-
+cli.add_command(cli_run_piece_docker, name='run-piece-docker')
 
 if __name__ == '__main__':
     cli()
```

### Comparing `domino-py-0.1.9/domino/cli/utils/pieces_repository.py` & `domino-py-0.2.0/domino/cli/utils/pieces_repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     pattern = re.compile(regex)
     if pattern.match(token):
         return True
     return False
 
 
 REQUIRED_ENV_VARS_VALIDATORS = {
-    "DOMINO_GITHUB_ACCESS_TOKEN_PIECES": {
+    "DOMINO_DEFAULT_PIECES_REPOSITORY_TOKEN": {
         "depends": lambda arg: arg.get('OPERATORS_REPOSITORY_SOURCE') == 'github',
         "validator_func": validate_github_token
     },
     "DOMINO_GITHUB_ACCESS_TOKEN_WORKFLOWS": {
         "depends": lambda arg: arg.get('OPERATORS_REPOSITORY_SOURCE') == 'github',
         "validator_func": validate_github_token
     }
```

### Comparing `domino-py-0.1.9/domino/cli/utils/platform.py` & `domino-py-0.2.0/domino/cli/utils/platform.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import os
 import tomli
 import tomli_w
 import yaml
 import subprocess
+import base64
 from pathlib import Path
 from rich.console import Console
-
-from domino.cli.utils.constants import COLOR_PALETTE #,DOMINO_HELM_PATH
 from yaml.resolver import BaseResolver
-
 from cryptography.hazmat.primitives import serialization as crypto_serialization
 from cryptography.hazmat.primitives.asymmetric import rsa
 from cryptography.hazmat.backends import default_backend as crypto_default_backend
-import base64
-import domino.helm as domino_helm
-from tempfile import NamedTemporaryFile
+from tempfile import NamedTemporaryFile, TemporaryDirectory
 from kubernetes import client, config
 
+from domino.cli.utils.constants import COLOR_PALETTE, DOMINO_HELM_PATH, DOMINO_HELM_VERSION, DOMINO_HELM_REPOSITORY
+
 
 class AsLiteral(str):
   pass
 
 def represent_literal(dumper, data):
   return dumper.represent_scalar(BaseResolver.DEFAULT_SCALAR_TAG, data, style="|")
 
@@ -50,15 +48,15 @@
     return private_key, public_key
     
 
 def prepare_platform(
     cluster_name: str, 
     workflows_repository: str, 
     github_workflows_ssh_private_key: str, 
-    github_pieces_token: str, 
+    github_default_pieces_repository_token: str,
     github_workflows_token: str,
     deploy_mode: str,
     local_pieces_repository_path: list,
     local_domino_path: str
 ) -> None:
     # Create local configuration file updated with user-provided arguments
     config_file_path = Path(__file__).resolve().parent / "config-domino-local.toml"
@@ -88,16 +86,16 @@
     if not github_workflows_ssh_private_key:
         private_key, public_key = create_ssh_pair_key()
         config_dict["github"]["DOMINO_GITHUB_WORKFLOWS_SSH_PRIVATE_KEY"] = base64.b64encode(private_key).decode('utf-8')
         config_dict["github"]["DOMINO_GITHUB_WORKFLOWS_SSH_PUBLIC_KEY"] = public_key.decode("utf-8")
     else:
         config_dict["github"]["DOMINO_GITHUB_WORKFLOWS_SSH_PRIVATE_KEY"] = github_workflows_ssh_private_key
 
-    config_dict["github"]["DOMINO_GITHUB_ACCESS_TOKEN_PIECES"] = github_pieces_token
     config_dict['github']['DOMINO_GITHUB_ACCESS_TOKEN_WORKFLOWS'] = github_workflows_token
+    config_dict['github']['DOMINO_DEFAULT_PIECES_REPOSITORY_TOKEN'] = github_default_pieces_repository_token
     
     with open("config-domino-local.toml", "wb") as f:
         tomli_w.dump(config_dict, f)
 
     console.print("")
     console.print(f"Domino is prepared to run at: {running_path}")
     console.print(f"You can check and modify the configuration file at: {running_path}/config-domino-local.toml")
@@ -180,92 +178,67 @@
         ]
     )
     with open("kind-cluster-config.yaml", "w") as f:
         yaml.dump(kind_config, f)
 
     cluster_name = platform_config["kind"]["DOMINO_KIND_CLUSTER_NAME"]
     
-    # Open helm values file and update with user-provided arguments
-    domino_helms_path = Path(os.path.dirname(domino_helm.__file__))
-    domino_base_helm_path = domino_helms_path / 'domino-base'
-    domino_airlflow_helm_path = domino_helms_path / 'domino-airflow'
-
+    # Create Kind cluster
     console.print(f"Removing previous Kind cluster - {cluster_name}...")
     subprocess.run(["kind", "delete", "cluster", "--name", cluster_name])
     console.print(f"Creating new Kind cluster - {cluster_name}...")
     subprocess.run(["kind", "create", "cluster", "--name", cluster_name, "--config", "kind-cluster-config.yaml"])
     console.print("")
     console.print("Kind cluster created successfully!", style=f"bold {COLOR_PALETTE.get('success')}")
 
-    # TODO - Install services with helm upgrade
+    # Install Ingress NGINX controller
     console.print("")
     console.print("Installing NGINX controller...")
     subprocess.run(["kubectl", "apply", "-f", "https://raw.githubusercontent.com/kubernetes/ingress-nginx/main/deploy/static/provider/kind/deploy.yaml"], stdout=subprocess.DEVNULL)
     subprocess.run(["kubectl", "wait", "--namespace", "ingress-nginx", "--for", "condition=ready", "pod", "--selector=app.kubernetes.io/component=controller", "--timeout=180s"])
 
+    # Load images to Kind cluster
     if domino_frontend_image:
         console.print(f"Loading local frontend image {domino_frontend_image} to Kind cluster...")
         subprocess.run(["kind", "load", "docker-image", domino_frontend_image , "--name", cluster_name, "--nodes", f"{cluster_name}-worker"])
+        domino_frontend_image = f"docker.io/library/{domino_frontend_image}"
     else:
-        domino_frontend_image = "ghcr.io/tauffer-consulting/domino-frontend:latest"
+        domino_frontend_image = "ghcr.io/tauffer-consulting/domino-frontend:k8s"
     
     if domino_rest_image:
         console.print(f"Loading local REST image {domino_rest_image} to Kind cluster...")
         subprocess.run(["kind", "load", "docker-image", domino_rest_image , "--name", cluster_name, "--nodes", f"{cluster_name}-worker"])
+        domino_rest_image = f'docker.io/library/{domino_rest_image}'
     else:  
         domino_rest_image = "ghcr.io/tauffer-consulting/domino-rest:latest" 
 
-    """
-    In order to use nvidia gpu in our cluster we need nvidia plugins to be installed.
-    We can use nvidia operator to install nvidia plugins.
-
-    References: 
-        https://catalog.ngc.nvidia.com/orgs/nvidia/containers/gpu-operator
-        https://jacobtomlinson.dev/posts/2022/quick-hack-adding-gpu-support-to-kind/
-    """
+    # In order to use nvidia gpu in our cluster we need nvidia plugins to be installed.
+    # We can use nvidia operator to install nvidia plugins.
+    # References: 
+    #     https://catalog.ngc.nvidia.com/orgs/nvidia/containers/gpu-operator
+    #     https://jacobtomlinson.dev/posts/2022/quick-hack-adding-gpu-support-to-kind/
     if use_gpu:
         console.print("Installing NVIDIA GPU Operator...")
         nvidia_gpu_operator_add_repo_command = [
             "helm", "repo", "add", "nvidia", "https://nvidia.github.io/gpu-operator",
         ]
         subprocess.run(nvidia_gpu_operator_add_repo_command)
         helm_update_command = ["helm", "repo", "update"]
         subprocess.run(helm_update_command)
 
         # We don't need driver as we are using kind and our host machine already has nvidia driver that is why we are disabling it.
         nvidia_plugis_install_command = "helm install --wait --generate-name -n gpu-operator --create-namespace nvidia/gpu-operator --set driver.enabled=false"
         subprocess.run(nvidia_plugis_install_command, shell=True)
 
-    token_pieces = platform_config["github"]["DOMINO_GITHUB_ACCESS_TOKEN_PIECES"]
-    token_workflows = platform_config["github"]["DOMINO_GITHUB_ACCESS_TOKEN_WORKFLOWS"]
-    console.print("\nInstalling Domino services...\n")
+
     # Install Domino Services
-    # TODO use remote helm chart
-    subprocess.run([
-        "helm", "install", 
-        "--set", f"github_access_token_pieces={token_pieces}",
-        "--set", f"github_access_token_workflows={token_workflows}",
-        "--set", f"frontend.image={domino_frontend_image}",
-        "--set", f"backend.image={domino_rest_image}",
-        "--set", f"backend.workflowsRepository={platform_config['github']['DOMINO_GITHUB_WORKFLOWS_REPOSITORY']}",
-        "domino",
-        domino_base_helm_path
-    ])
-
-    if not run_airflow:
-        console.print("")
-        console.print("K8s resources created successfully!", style=f"bold {COLOR_PALETTE.get('success')}")
-
-        console.print("You can now access the Domino frontend at: http://localhost/")
-        console.print("and the Backend API at: http://localhost/api/")
-        return
-        
-    console.print("\nInstalling Domino Airflow services...\n")
+    console.print("\nInstalling Domino Services...\n")
+    token_pieces = platform_config["github"]["DOMINO_DEFAULT_PIECES_REPOSITORY_TOKEN"]
+    token_workflows = platform_config["github"]["DOMINO_GITHUB_ACCESS_TOKEN_WORKFLOWS"]
 
-    console.print("\nInstalling Domino Airflow services...\n")
     # Create temporary airflow values with user provided arguments
     airflow_ssh_config = dict(
         gitSshKey=f"{platform_config['github']['DOMINO_GITHUB_WORKFLOWS_SSH_PRIVATE_KEY']}",
     )
     airflow_ssh_config_parsed = AsLiteral(yaml.dump(airflow_ssh_config))
 
     workers_extra_volumes = []
@@ -296,29 +269,42 @@
         scheduler = {
             "scheduler": {
                 "extraVolumes": workers_extra_volumes,
                 "extraVolumeMounts": workers_extra_volumes_mounts,
             }
         }
 
-    
+    domino_values_override_config = {
+        "github_access_token_pieces": token_pieces,
+        "github_access_token_workflows": token_workflows,
+        "frontend": {
+            "enabled": True,
+            "image": domino_frontend_image,
+        },
+        "rest": {
+            "enabled": True,
+            "image": domino_rest_image,
+            "workflowsRepository": platform_config['github']['DOMINO_GITHUB_WORKFLOWS_REPOSITORY'],
+        },
+    }
 
     airflow_values_override_config = {
+        **domino_values_override_config,
         "airflow": {
             "enabled": True,
             "env": [
                 {
                     "name": "DOMINO_DEPLOY_MODE",
                     "value": platform_config['kind']["DOMINO_DEPLOY_MODE"]
                 },
             ],
             "images": {
                 "useDefaultImageForMigration": False,
                 "airflow": {
-                    "repository": "ghcr.io/tauffer-consulting/domino-airflow-base", # TODO change to prod # TODO change to domino image name when we have it
+                    "repository": "ghcr.io/tauffer-consulting/domino-airflow-base",
                     "tag": "latest",
                     "pullPolicy": "IfNotPresent"
                 }
             },
             "extraSecrets": {
                 "airflow-ssh-secret": {
                     "data": airflow_ssh_config_parsed
@@ -335,29 +321,41 @@
                 }
             },
             **workers,
             **scheduler,
         }
     }
 
-    # Add airflow helm repository
-    # TODO check why is not working with remote helm chart
-    # subprocess.run([
-    #     "helm", "repo", "add", "apache-airflow", "https://airflow.apache.org"
-    # ])
     # Write yaml to temp file and install domino airflow
-    with NamedTemporaryFile(suffix='.yaml', mode="w") as fp:
-        yaml.dump(airflow_values_override_config, fp)
-        # Install airflow
+    subprocess.run(["helm", "repo", "add", "domino", DOMINO_HELM_REPOSITORY])
+    subprocess.run(["helm", "repo", "add", "apache-airflow", "https://airflow.apache.org/"])  # ref: https://github.com/helm/helm/issues/8036
+    subprocess.run(["helm", "repo", "update"])
+    with TemporaryDirectory() as tmp_dir:
+        console.print("Downloading Domino Helm chart...")
         subprocess.run([
-            "helm", "upgrade",
-            "-i", "-f", str(fp.name),
-            "domino-airflow",
-            domino_airlflow_helm_path,
+            "helm",
+            "pull",
+            DOMINO_HELM_PATH,
+            "--version",
+            DOMINO_HELM_VERSION,
+            "--untar",
+            "-d",
+            tmp_dir
         ])
+        console.print("Installing dependencies...")
+        subprocess.run(["helm", "dependency", "build"], cwd=f"{tmp_dir}/domino")
+        with NamedTemporaryFile(suffix='.yaml', mode="w") as fp:
+            yaml.dump(airflow_values_override_config, fp)
+            console.print('Installing Domino...')
+            subprocess.run([
+                "helm", "install",
+                "-f", str(fp.name),
+                "domino",
+                f"{tmp_dir}/domino"
+            ])
 
     # For each path create a pv and pvc
     if platform_config['kind']['DOMINO_DEPLOY_MODE'] == 'local-k8s-dev':
         config.load_kube_config()
         k8s_client = client.CoreV1Api()
         v1 = client.RbacAuthorizationV1Api()
 
@@ -515,8 +513,38 @@
             )
             k8s_client.create_persistent_volume(body=pv)
 
     console.print("")
     console.print("K8s resources created successfully!", style=f"bold {COLOR_PALETTE.get('success')}")
 
     console.print("You can now access the Domino frontend at: http://localhost/")
-    console.print("and the Backend API at: http://localhost/api/")
+    console.print("and the Backend API at: http://localhost/api/")
+
+
+def run_platform_compose(detached: bool = False):
+    # Create local directories
+    local_path = Path(".").resolve()
+    domino_dir = local_path / "domino_data"
+    domino_dir.mkdir(parents=True, exist_ok=True)
+    subprocess.run(["chmod", "-R", "777", "domino_data"])
+    airflow_logs_dir = local_path / "airflow/logs"
+    airflow_logs_dir.mkdir(parents=True, exist_ok=True)
+    airflow_dags_dir = local_path / "airflow/dags"
+    airflow_dags_dir.mkdir(parents=True, exist_ok=True)
+    airflow_plugins_dir = local_path / "airflow/plugins"
+    airflow_plugins_dir.mkdir(parents=True, exist_ok=True)
+    subprocess.run(["chmod", "-R", "777", "airflow"])    
+
+    # Copy docker-compose.yaml file from package to local path
+    docker_compose_path = Path(__file__).resolve().parent / "docker-compose.yaml"
+    subprocess.run(["cp", str(docker_compose_path), "."])
+
+    # Run docker-compose up
+    cmd = [
+        "docker", 
+        "compose", 
+        "up"
+    ]
+    if detached:
+        cmd.append("-d")
+    environment = os.environ.copy()
+    subprocess.Popen(cmd, env=environment)
```

### Comparing `domino-py-0.1.9/domino/client/airflow_client.py` & `domino-py-0.2.0/domino/client/airflow_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.9/domino/client/domino_backend_client.py` & `domino-py-0.2.0/domino/client/domino_backend_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.9/domino/client/fs_client.py` & `domino-py-0.2.0/domino/client/fs_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.9/domino/client/github_rest_client.py` & `domino-py-0.2.0/domino/client/github_rest_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.9/domino/client/local_files_client.py` & `domino-py-0.2.0/domino/client/local_files_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.9/domino/client/s3_client.py` & `domino-py-0.2.0/domino/client/s3_client.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.9/domino/custom_operators/k8s_operator.py` & `domino-py-0.2.0/domino/custom_operators/k8s_operator.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,16 @@
         self.repository_id = repository_id
         self.workflow_shared_storage = workflow_shared_storage
         self.task_id_replaced = self.task_id.replace("_", "-").lower() # doing this because airflow doesn't allow underscores and upper case in mount names
         self.task_env_vars = kwargs.get('env_vars', [])
         # Shared Storage variables
         self.shared_storage_base_mount_path = '/home/shared_storage'
         self.shared_storage_upstream_ids_list = list()
-        # TODO change url to constants file
-        self.backend_client = DominoBackendRestClient(base_url="http://domino-backend-service:8000/")
+        # TODO change url based on DOMINO_DEPLOY_MODE
+        self.backend_client = DominoBackendRestClient(base_url="http://domino-rest-service:8000/")
     
 
     def build_pod_request_obj(self, context: Optional['Context'] = None) -> k8s.V1Pod:
         """
         We override this method to add the shared storage to the pod.
         This function runs after our own self.execute, by super().execute()
         """
@@ -166,15 +166,15 @@
             'AIRFLOW_UPSTREAM_TASKS_IDS_SHARED_STORAGE': str(self.shared_storage_upstream_ids_list),
         }
 
         self.shared_storage_sidecar_container_name = f"domino-shared-storage-sidecar-{self.task_id_replaced}"
         sidecar_container = k8s.V1Container(
             name=self.shared_storage_sidecar_container_name,
             command=['bash', '-c', './sidecar_lifecycle.sh'],
-            image='ghcr.io/tauffer-consulting/domino_shared_storage_sidecar:latest',
+            image='ghcr.io/tauffer-consulting/domino-shared-storage-sidecar:latest',
             volume_mounts=volume_mounts_sidecar_container,
             security_context=k8s.V1SecurityContext(privileged=True),
             env=[k8s.V1EnvVar(name=k, value=v) for k, v in env_vars.items()],
             resources=k8s.V1ResourceRequirements(
                 requests={
                     "cpu": "1m",
                     "memory": "128Mi",
```

### Comparing `domino-py-0.1.9/domino/custom_operators/python_operator.py` & `domino-py-0.2.0/domino/custom_operators/python_operator.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.9/domino/custom_operators/sidecar/logger.py` & `domino-py-0.2.0/domino/custom_operators/sidecar/logger.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.9/domino/custom_operators/sidecar/mount.py` & `domino-py-0.2.0/domino/custom_operators/sidecar/mount.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.9/domino/exceptions/exceptions.py` & `domino-py-0.2.0/domino/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.9/domino/logger.py` & `domino-py-0.2.0/domino/logger.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.9/domino/schemas/piece_metadata.py` & `domino-py-0.2.0/domino/schemas/piece_metadata.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.9/domino/schemas/shared_storage.py` & `domino-py-0.2.0/domino/schemas/shared_storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pydantic import BaseModel, Field
 from enum import Enum
+from typing import Optional
 
 
 class StorageSource(str, Enum):
     none = "None"
     local = 'Local'
     aws_s3 = "AWS S3"
 
@@ -16,41 +17,41 @@
 
 
 class WorkflowSharedStorage(BaseModel):
     source: StorageSource = Field(
         description="The service to be used as the source of storage.", 
         default="none",
     )
-    base_folder: str = Field(
-        description="The base folder to be used as the root of the storage source.",
-        default="",
-    )
     mode: StorageMode = Field(
         description="The access mode to the storage source.", 
         default="none"
     )
-    storage_repository_id: int = Field(
-        description="The id of the storage repository to be used as the root of the storage source.",
-    )
     default_piece_name: str = Field(
         description="The name of the default piece to be used for the storage source.",
     )
 
 
 class LocalSharedStorage(WorkflowSharedStorage):
     source = StorageSource.local
-    # default_piece_name: str = "LocalDefaultOperator" # TODO to be implemented
+    default_piece_name: str = "LocalDefaultOperator" # TODO to be implemented
 
 
 class AwsS3SharedStorage(WorkflowSharedStorage):
     source = StorageSource.aws_s3
     bucket: str = Field(
         description="The name of the bucket to be used as the root of the storage source."
     )
     default_piece_name: str = "AWSS3DefaultPiece"
+    base_folder: str = Field(
+        description="The base folder to be used as the root of the storage source.",
+        default="",
+    )
+    storage_repository_id: int = Field(
+        description="The id of the storage repository to be used as the root of the storage source.",
+    )
 
 
 shared_storage_map = {
     "none": None,
     "local": LocalSharedStorage,
     "aws_s3": AwsS3SharedStorage,
 }
```

### Comparing `domino-py-0.1.9/domino/scripts/build_docker_images_pieces.py` & `domino-py-0.2.0/domino/scripts/build_docker_images_pieces.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.9/domino/scripts/create_docker_compose_file.py` & `domino-py-0.2.0/domino/scripts/create_docker_compose_file.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.9/domino/scripts/docker_compose_constants.py` & `domino-py-0.2.0/domino/scripts/docker_compose_constants.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.9/domino/scripts/docker_compose_scripts.py` & `domino-py-0.2.0/domino/scripts/docker_compose_scripts.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.9/domino/scripts/load_piece.py` & `domino-py-0.2.0/domino/scripts/load_piece.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.9/domino/scripts/run_piece_bash.py` & `domino-py-0.2.0/domino/scripts/run_piece_bash.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.9/domino/scripts/run_piece_dry.py` & `domino-py-0.2.0/domino/scripts/piece_dry_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Example usage of dry run:
 
-from domino.scripts.run_piece_dry import run_piece_dry
+from domino.scripts.piece_dry_run import piece_dry_run
 
-run_piece_dry(
+piece_dry_run(
     repository_folder_path=".", 
     piece_name="DownloadPicsumImageOperator", 
     piece_input={
         "width_pixels": 200,
         "height_pixels": 200,
         "save_as_file": False
     }
@@ -17,15 +17,15 @@
 import importlib
 import json
 import sys
 
 
 
 
-def run_piece_dry(
+def piece_dry_run(
     repository_folder_path: str, 
     piece_name: str, 
     piece_input: dict,
     secrets_input: dict = None,
     results_path: str = None
 ):
     if not results_path:
```

### Comparing `domino-py-0.1.9/domino/scripts/run_piece_k8s.py` & `domino-py-0.2.0/domino/scripts/run_piece_k8s.py`

 * *Files identical despite different names*

### Comparing `domino-py-0.1.9/domino/task.py` & `domino-py-0.2.0/domino/task.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from airflow import DAG
 from kubernetes.client import models as k8s
 from datetime import datetime
 from typing import Callable
 
-from domino.client.domino_backend_client import DominoBackendRestClient
+from domino.custom_operators.docker_operator import DominoDockerOperator
 from domino.custom_operators.python_operator import PythonOperator
-from domino.custom_operators.bash_operator import BashOperator
 from domino.custom_operators.k8s_operator import DominoKubernetesPodOperator
 from domino.schemas.shared_storage import shared_storage_map
 from domino.utils import dict_deep_update
 from domino.logger import get_configured_logger
 from domino.schemas.shared_storage import StorageSource
 from domino.schemas.container_resources import ContainerResourcesModel
 from kubernetes import client, config
@@ -48,21 +47,20 @@
         self.workflow_shared_storage = shared_storage_map[workflow_shared_storage_source](**workflow_shared_storage, **provider_options) if shared_storage_map[workflow_shared_storage_source] else shared_storage_map[workflow_shared_storage_source]
         # Container resources
         self.container_resources = container_resources if container_resources else {}
         self.provide_gpu = self.container_resources.pop("use_gpu", False)
         
         self.deploy_mode = os.environ.get('DOMINO_DEPLOY_MODE')
 
-        config.load_incluster_config()
-        self.k8s_client = client.CoreV1Api()
 
-        # Clients
-        self.backend_client = DominoBackendRestClient(base_url="http://domino-backend-service:8000/")
+        if self.deploy_mode in ['local-k8s', 'local-k8s-dev', 'prod']:
+            config.load_incluster_config()
+            self.k8s_client = client.CoreV1Api()
 
-        # Set up Airflow piece using custom function
+        # Set up piece logic
         self._task_piece = self._set_piece(piece_input_kwargs)
 
     def _set_piece(self, piece_input_kwargs) -> None:
         """
         Set airflow piece based on task configuration
         """
 
@@ -77,34 +75,14 @@
                 make_python_callable_kwargs=dict(
                     piece_name=self.piece_name,
                     deploy_mode=self.deploy_mode,
                     task_id=self.task_id,
                     dag_id=self.dag_id,
                 )
             )
-        
-        elif self.deploy_mode == "local-bash":
-            cmds = 'source /opt/airflow/domino_env/bin/activate && pip install -e /opt/domino && domino run-piece-bash'
-            queue_name = self.piece.get("repository") + '-' + self.piece.get("dependency")
-            return BashOperator(
-                dag=self.dag,
-                task_id=self.task_id,
-                queue=queue_name,
-                bash_command=cmds,
-                env={
-                    "DOMINO_BASHOPERATOR_PIECE": str(self.piece),
-                    "DOMINO_BASHOPERATOR_INSTANTIATE_PIECE_KWARGS": str({
-                        "deploy_mode": self.deploy_mode,
-                        "task_id": self.task_id,
-                        "dag_id": self.dag_id,
-                    }),
-                    "DOMINO_BASHOPERATOR_RUN_PIECE_KWARGS": str(piece_input_kwargs),
-                },
-                append_env=True
-            )
 
         # References: 
         # - https://airflow.apache.org/docs/apache-airflow/1.10.14/_api/airflow/contrib/operators/kubernetes_pod_operator/index.html
         # - https://airflow.apache.org/docs/apache-airflow/stable/templates-ref.html
         # - https://www.astronomer.io/guides/templating/
         # - good example: https://github.com/apache/airflow/blob/main/tests/system/providers/cncf/kubernetes/example_kubernetes.py
         # - commands HAVE to go in a list object: https://stackoverflow.com/a/55149915/11483674
@@ -151,15 +129,14 @@
                 persistent_volume_claim_name = 'pvc-{}'.format(str(repository_raw_project_name.lower().replace('_', '-')))
 
                 persistent_volume_name = 'pv-{}'.format(str(repository_raw_project_name.lower().replace('_', '-')))
                 persistent_volume_claim_name = 'pvc-{}'.format(str(repository_raw_project_name.lower().replace('_', '-')))
 
                 pvc_exists = False
                 try:
-                    print('Checking for PVC')
                     self.k8s_client.read_namespaced_persistent_volume_claim(name=persistent_volume_claim_name, namespace='default')
                     pvc_exists = True
                 except client.rest.ApiException as e:
                     if e.status != 404:
                         raise e
 
                 pv_exists = False
@@ -228,21 +205,31 @@
                 arguments=["run-piece-k8s"],
                 env_vars=container_env_vars,
                 do_xcom_push=True,
                 in_cluster=True,
                 volumes=all_volumes,
                 volume_mounts=all_volume_mounts,
                 container_resources=container_resources_obj,
-                # labels={"foo": "bar"},
-                # secrets=[secret_file, secret_env, secret_all_keys],
-                # ports=[port],
-                # env_from=configmaps,
-                # affinity=affinity,
-                # is_delete_piece_pod=True,
-                # hostnetwork=False,
-                # tolerations=tolerations,
-                # init_containers=[init_container],
-                # priority_class_name="medium",
             )
+        
+        elif self.deploy_mode == 'local-compose':
+            return DominoDockerOperator(
+                task_id=self.task_id,
+                piece_name=self.piece.get('name'),
+                repository_id=self.repository_id,
+                piece_kwargs=piece_input_kwargs,
+                dag_id=self.dag_id,
+                deploy_mode=self.deploy_mode,
+                image=self.piece["source_image"],
+                workflow_shared_storage=self.workflow_shared_storage,
+                do_xcom_push=True,
+                mount_tmp_dir=False,
+                tty=True,
+                xcom_all=False,
+                retrieve_output=True,
+                retrieve_output_path='/airflow/xcom/return.out',
+                entrypoint=["domino", "run-piece-docker"],
+            )
+
 
     def __call__(self) -> Callable:
         return self._task_piece
```

### Comparing `domino-py-0.1.9/setup.py` & `domino-py-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,32 +25,25 @@
 with open(os.path.join(path, "requirements-airflow.txt")) as f:
     install_extra_requires = f.read().strip().split("\n")
 
 
 setup(
     name=f"{package_name}-py",
     version=version_dict['__version__'],
-    description="Domino project",
+    description="Python package for the Domino platform",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Luiz Tauffer and Vinicius Vaz",
     author_email="luiz@taufferconsulting.com",
-    keywords=["airflow", "UI"],
+    keywords=["domino", "airflow", "gui"],
     packages=find_packages(),
     package_data={
         'domino': [
             'cli/utils/config-domino-local.toml',
-            'helm/domino-airflow/kind-cluster-config',
-            'helm/domino-airflow/**/*',
-            'helm/domino-base/**/*',
-            'helm/domino-airflow/charts/**',
-            'domino/helm/domino-base/**',
-            'domino/helm/domino-base/templates/**',
-            'domino/helm/domino-base/templates/jobs/**',
-            'domino/helm/domino-base/templates/volumes/**',
+            'cli/utils/docker-compose.yaml',
             'custom_operators/sidecar/sidecar_lifecycle.sh',
             'custom_operators/sidecar/rclone.conf',
             'custom_operators/sidecar/fuse.conf',
         ]
     },
     include_package_data=True,
     python_requires=">=3.7",
```

