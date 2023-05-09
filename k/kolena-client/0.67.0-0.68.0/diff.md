# Comparing `tmp/kolena_client-0.67.0.tar.gz` & `tmp/kolena_client-0.68.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolena_client-0.67.0.tar", max compression
+gzip compressed data, was "kolena_client-0.68.0.tar", max compression
```

## Comparing `kolena_client-0.67.0.tar` & `kolena_client-0.68.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0    11346 2023-05-02 18:26:43.464893 kolena_client-0.67.0/LICENSE
--rw-r--r--   0        0        0      556 2023-05-02 18:26:43.464893 kolena_client-0.67.0/LICENSE_HEADER
--rw-r--r--   0        0        0     1405 2023-05-02 18:26:43.464893 kolena_client-0.67.0/README.md
--rw-r--r--   0        0        0     1356 2023-05-02 18:26:43.464893 kolena_client-0.67.0/kolena/__init__.py
--rw-r--r--   0        0        0      579 2023-05-02 18:26:43.464893 kolena_client-0.67.0/kolena/_api/__init__.py
--rw-r--r--   0        0        0      579 2023-05-02 18:26:43.464893 kolena_client-0.67.0/kolena/_api/v1/__init__.py
--rw-r--r--   0        0        0     1725 2023-05-02 18:26:43.464893 kolena_client-0.67.0/kolena/_api/v1/batched_load.py
--rw-r--r--   0        0        0      878 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_api/v1/client_log.py
--rw-r--r--   0        0        0     7578 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_api/v1/core.py
--rw-r--r--   0        0        0     5320 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_api/v1/detection.py
--rw-r--r--   0        0        0     7480 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_api/v1/fr.py
--rw-r--r--   0        0        0     5507 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_api/v1/generic.py
--rw-r--r--   0        0        0      778 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_api/v1/repository.py
--rw-r--r--   0        0        0      690 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_api/v1/samples.py
--rw-r--r--   0        0        0      833 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_api/v1/token.py
--rw-r--r--   0        0        0      738 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_api/v1/workflow.py
--rw-r--r--   0        0        0      579 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/__init__.py
--rw-r--r--   0        0        0      784 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/_consts.py
--rw-r--r--   0        0        0     1604 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/asset_path_mapper.py
--rw-r--r--   0        0        0     7031 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/batched_load.py
--rw-r--r--   0        0        0     5608 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/cli.py
--rw-r--r--   0        0        0      579 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/dataframes/__init__.py
--rw-r--r--   0        0        0     2826 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/dataframes/validators.py
--rw-r--r--   0        0        0     1952 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/datatypes.py
--rw-r--r--   0        0        0     3403 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/endpoints.py
--rw-r--r--   0        0        0     1690 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/frozen.py
--rw-r--r--   0        0        0     1260 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/futures.py
--rw-r--r--   0        0        0     1183 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/geometry.py
--rw-r--r--   0        0        0     1087 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/inference_validators.py
--rw-r--r--   0        0        0     2646 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/instrumentation.py
--rw-r--r--   0        0        0     4866 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/krequests.py
--rw-r--r--   0        0        0     3507 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/log.py
--rw-r--r--   0        0        0      997 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/repository.py
--rw-r--r--   0        0        0     2494 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/serde.py
--rw-r--r--   0        0        0      889 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/serializable.py
--rw-r--r--   0        0        0     4768 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/state.py
--rw-r--r--   0        0        0     6672 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/stratification.py
--rw-r--r--   0        0        0     1942 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/uninstantiable.py
--rw-r--r--   0        0        0      852 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/_utils/validators.py
--rw-r--r--   0        0        0     1134 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/__init__.py
--rw-r--r--   0        0        0     1339 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/metadata.py
--rw-r--r--   0        0        0     3357 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/model.py
--rw-r--r--   0        0        0     1213 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/multiclass/__init__.py
--rw-r--r--   0        0        0     3005 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/multiclass/_utils.py
--rw-r--r--   0        0        0    14006 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/multiclass/evaluator.py
--rw-r--r--   0        0        0     3578 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/multiclass/test_run.py
--rw-r--r--   0        0        0     2541 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/multiclass/workflow.py
--rw-r--r--   0        0        0     2547 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/test_case.py
--rw-r--r--   0        0        0     2184 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/test_config.py
--rw-r--r--   0        0        0     4138 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/test_image.py
--rw-r--r--   0        0        0     6069 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/test_run.py
--rw-r--r--   0        0        0     2813 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/classification/test_suite.py
--rw-r--r--   0        0        0     1351 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/__init__.py
--rw-r--r--   0        0        0     6819 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_datatypes.py
--rw-r--r--   0        0        0     1042 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_internal/__init__.py
--rw-r--r--   0        0        0     1922 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_internal/datatypes.py
--rw-r--r--   0        0        0      765 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_internal/ground_truth.py
--rw-r--r--   0        0        0     1321 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_internal/inference.py
--rw-r--r--   0        0        0     5454 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_internal/metadata.py
--rw-r--r--   0        0        0     8540 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_internal/model.py
--rw-r--r--   0        0        0    13501 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_internal/test_case.py
--rw-r--r--   0        0        0     1405 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_internal/test_config.py
--rw-r--r--   0        0        0     2049 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_internal/test_image.py
--rw-r--r--   0        0        0    12390 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_internal/test_run.py
--rw-r--r--   0        0        0    12954 2023-05-02 18:26:43.468893 kolena_client-0.67.0/kolena/detection/_internal/test_suite.py
--rw-r--r--   0        0        0     6309 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/detection/ground_truth.py
--rw-r--r--   0        0        0     5232 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/detection/inference.py
--rw-r--r--   0        0        0     1334 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/detection/metadata.py
--rw-r--r--   0        0        0     2970 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/detection/model.py
--rw-r--r--   0        0        0     2264 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/detection/test_case.py
--rw-r--r--   0        0        0     3018 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/detection/test_config.py
--rw-r--r--   0        0        0     4707 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/detection/test_image.py
--rw-r--r--   0        0        0     5564 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/detection/test_run.py
--rw-r--r--   0        0        0     2506 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/detection/test_suite.py
--rw-r--r--   0        0        0     2536 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/errors.py
--rw-r--r--   0        0        0     1400 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/fr/__init__.py
--rw-r--r--   0        0        0      689 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/fr/_consts.py
--rw-r--r--   0        0        0    20512 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/fr/datatypes.py
--rw-r--r--   0        0        0     9301 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/fr/model.py
--rw-r--r--   0        0        0    14447 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/fr/test_case.py
--rw-r--r--   0        0        0    12177 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/fr/test_images.py
--rw-r--r--   0        0        0    17008 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/fr/test_run.py
--rw-r--r--   0        0        0    15282 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/fr/test_suite.py
--rw-r--r--   0        0        0     4134 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/initialize.py
--rw-r--r--   0        0        0     4550 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/__init__.py
--rw-r--r--   0        0        0    13815 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/_datatypes.py
--rw-r--r--   0        0        0     2559 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/_helpers.py
--rw-r--r--   0        0        0     6052 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/_validators.py
--rw-r--r--   0        0        0     6423 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/annotation.py
--rw-r--r--   0        0        0     3842 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/asset.py
--rw-r--r--   0        0        0    15849 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/evaluator.py
--rw-r--r--   0        0        0     9312 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/evaluator_function.py
--rw-r--r--   0        0        0     3359 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/ground_truth.py
--rw-r--r--   0        0        0     3433 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/inference.py
--rw-r--r--   0        0        0      625 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/metrics/__init__.py
--rw-r--r--   0        0        0     2738 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/metrics/_geometry.py
--rw-r--r--   0        0        0     7571 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/model.py
--rw-r--r--   0        0        0    13233 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/test_case.py
--rw-r--r--   0        0        0    22814 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/test_run.py
--rw-r--r--   0        0        0     9155 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/test_sample.py
--rw-r--r--   0        0        0    11542 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/test_suite.py
--rw-r--r--   0        0        0     9293 2023-05-02 18:26:43.472893 kolena_client-0.67.0/kolena/workflow/workflow.py
--rw-r--r--   0        0        0     1927 2023-05-02 18:26:59.568960 kolena_client-0.67.0/pyproject.toml
--rw-r--r--   0        0        0     2974 1970-01-01 00:00:00.000000 kolena_client-0.67.0/setup.py
--rw-r--r--   0        0        0     3276 1970-01-01 00:00:00.000000 kolena_client-0.67.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-05-09 21:48:51.859365 kolena_client-0.68.0/LICENSE
+-rw-r--r--   0        0        0      556 2023-05-09 21:48:51.859365 kolena_client-0.68.0/LICENSE_HEADER
+-rw-r--r--   0        0        0     1405 2023-05-09 21:48:51.859365 kolena_client-0.68.0/README.md
+-rw-r--r--   0        0        0     1356 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/__init__.py
+-rw-r--r--   0        0        0      579 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/__init__.py
+-rw-r--r--   0        0        0      579 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/v1/__init__.py
+-rw-r--r--   0        0        0     1725 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/v1/batched_load.py
+-rw-r--r--   0        0        0      878 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/v1/client_log.py
+-rw-r--r--   0        0        0     7594 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/v1/core.py
+-rw-r--r--   0        0        0     5320 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/v1/detection.py
+-rw-r--r--   0        0        0     7480 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/v1/fr.py
+-rw-r--r--   0        0        0     5507 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/v1/generic.py
+-rw-r--r--   0        0        0      778 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/v1/repository.py
+-rw-r--r--   0        0        0      690 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/v1/samples.py
+-rw-r--r--   0        0        0      833 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/v1/token.py
+-rw-r--r--   0        0        0      738 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_api/v1/workflow.py
+-rw-r--r--   0        0        0      579 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/__init__.py
+-rw-r--r--   0        0        0      784 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/_consts.py
+-rw-r--r--   0        0        0     1604 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/asset_path_mapper.py
+-rw-r--r--   0        0        0     7115 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/batched_load.py
+-rw-r--r--   0        0        0     5608 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/cli.py
+-rw-r--r--   0        0        0      579 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/dataframes/__init__.py
+-rw-r--r--   0        0        0     2826 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/dataframes/validators.py
+-rw-r--r--   0        0        0     1952 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/datatypes.py
+-rw-r--r--   0        0        0     3403 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/endpoints.py
+-rw-r--r--   0        0        0     1690 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/frozen.py
+-rw-r--r--   0        0        0     1260 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/futures.py
+-rw-r--r--   0        0        0     1183 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/geometry.py
+-rw-r--r--   0        0        0     1087 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/inference_validators.py
+-rw-r--r--   0        0        0     2646 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/instrumentation.py
+-rw-r--r--   0        0        0     4866 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/krequests.py
+-rw-r--r--   0        0        0     3507 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/log.py
+-rw-r--r--   0        0        0      997 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/repository.py
+-rw-r--r--   0        0        0     2494 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/serde.py
+-rw-r--r--   0        0        0      889 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/serializable.py
+-rw-r--r--   0        0        0     4768 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/state.py
+-rw-r--r--   0        0        0     6672 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/stratification.py
+-rw-r--r--   0        0        0     1942 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/uninstantiable.py
+-rw-r--r--   0        0        0      852 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/_utils/validators.py
+-rw-r--r--   0        0        0     1134 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/__init__.py
+-rw-r--r--   0        0        0     1339 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/metadata.py
+-rw-r--r--   0        0        0     3357 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/model.py
+-rw-r--r--   0        0        0     1213 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/multiclass/__init__.py
+-rw-r--r--   0        0        0     3005 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/multiclass/_utils.py
+-rw-r--r--   0        0        0    14914 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/multiclass/evaluator.py
+-rw-r--r--   0        0        0     3578 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/multiclass/test_run.py
+-rw-r--r--   0        0        0     2645 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/multiclass/workflow.py
+-rw-r--r--   0        0        0     2547 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/test_case.py
+-rw-r--r--   0        0        0     2184 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/test_config.py
+-rw-r--r--   0        0        0     4138 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/test_image.py
+-rw-r--r--   0        0        0     6069 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/test_run.py
+-rw-r--r--   0        0        0     2813 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/classification/test_suite.py
+-rw-r--r--   0        0        0     1351 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/detection/__init__.py
+-rw-r--r--   0        0        0     6819 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/detection/_datatypes.py
+-rw-r--r--   0        0        0     1042 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/detection/_internal/__init__.py
+-rw-r--r--   0        0        0     1922 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/detection/_internal/datatypes.py
+-rw-r--r--   0        0        0      765 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/detection/_internal/ground_truth.py
+-rw-r--r--   0        0        0     1321 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/detection/_internal/inference.py
+-rw-r--r--   0        0        0     5454 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/detection/_internal/metadata.py
+-rw-r--r--   0        0        0     8540 2023-05-09 21:48:51.863365 kolena_client-0.68.0/kolena/detection/_internal/model.py
+-rw-r--r--   0        0        0    13501 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/_internal/test_case.py
+-rw-r--r--   0        0        0     1405 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/_internal/test_config.py
+-rw-r--r--   0        0        0     2049 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/_internal/test_image.py
+-rw-r--r--   0        0        0    12390 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/_internal/test_run.py
+-rw-r--r--   0        0        0    12954 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/_internal/test_suite.py
+-rw-r--r--   0        0        0     6309 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/ground_truth.py
+-rw-r--r--   0        0        0     5232 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/inference.py
+-rw-r--r--   0        0        0     1334 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/metadata.py
+-rw-r--r--   0        0        0     2970 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/model.py
+-rw-r--r--   0        0        0     2264 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/test_case.py
+-rw-r--r--   0        0        0     3018 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/test_config.py
+-rw-r--r--   0        0        0     4707 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/test_image.py
+-rw-r--r--   0        0        0     5564 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/test_run.py
+-rw-r--r--   0        0        0     2506 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/detection/test_suite.py
+-rw-r--r--   0        0        0     2536 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/errors.py
+-rw-r--r--   0        0        0     1400 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/fr/__init__.py
+-rw-r--r--   0        0        0      689 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/fr/_consts.py
+-rw-r--r--   0        0        0    20512 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/fr/datatypes.py
+-rw-r--r--   0        0        0     9301 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/fr/model.py
+-rw-r--r--   0        0        0    14447 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/fr/test_case.py
+-rw-r--r--   0        0        0    12177 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/fr/test_images.py
+-rw-r--r--   0        0        0    17008 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/fr/test_run.py
+-rw-r--r--   0        0        0    15282 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/fr/test_suite.py
+-rw-r--r--   0        0        0     4134 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/initialize.py
+-rw-r--r--   0        0        0     4550 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/__init__.py
+-rw-r--r--   0        0        0    13815 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/_datatypes.py
+-rw-r--r--   0        0        0     2559 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/_helpers.py
+-rw-r--r--   0        0        0     6052 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/_validators.py
+-rw-r--r--   0        0        0     7794 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/annotation.py
+-rw-r--r--   0        0        0     3842 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/asset.py
+-rw-r--r--   0        0        0    15849 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/evaluator.py
+-rw-r--r--   0        0        0     9312 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/evaluator_function.py
+-rw-r--r--   0        0        0     3359 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/ground_truth.py
+-rw-r--r--   0        0        0     3433 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/inference.py
+-rw-r--r--   0        0        0      760 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/metrics/__init__.py
+-rw-r--r--   0        0        0     7762 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/metrics/_geometry.py
+-rw-r--r--   0        0        0     7571 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/model.py
+-rw-r--r--   0        0        0    13233 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/test_case.py
+-rw-r--r--   0        0        0    22814 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/test_run.py
+-rw-r--r--   0        0        0     9155 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/test_sample.py
+-rw-r--r--   0        0        0    11542 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/test_suite.py
+-rw-r--r--   0        0        0     9293 2023-05-09 21:48:51.867365 kolena_client-0.68.0/kolena/workflow/workflow.py
+-rw-r--r--   0        0        0     1925 2023-05-09 21:49:11.668943 kolena_client-0.68.0/pyproject.toml
+-rw-r--r--   0        0        0     2973 1970-01-01 00:00:00.000000 kolena_client-0.68.0/setup.py
+-rw-r--r--   0        0        0     3275 1970-01-01 00:00:00.000000 kolena_client-0.68.0/PKG-INFO
```

### Comparing `kolena_client-0.67.0/LICENSE` & `kolena_client-0.68.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/LICENSE_HEADER` & `kolena_client-0.68.0/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/README.md` & `kolena_client-0.68.0/README.md`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/__init__.py` & `kolena_client-0.68.0/kolena/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_api/__init__.py` & `kolena_client-0.68.0/kolena/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_api/v1/__init__.py` & `kolena_client-0.68.0/kolena/_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_api/v1/batched_load.py` & `kolena_client-0.68.0/kolena/_api/v1/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_api/v1/client_log.py` & `kolena_client-0.68.0/kolena/_api/v1/client_log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_api/v1/core.py` & `kolena_client-0.68.0/kolena/_api/v1/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
 
 CATEGORICAL = "categorical"
 NUMERIC = "numeric"
 
 
 @dataclass(frozen=True)
 class Dimension:
-    column: Literal["test_sample", "test_sample_metadata"]
+    column: Literal["test_sample", "test_sample_metadata", "ground_truth"]
     field: str
     datatype: Literal["categorical", "numeric"]
 
     def is_categorical(self):
         return self.datatype == CATEGORICAL
 
     def is_numeric(self):
```

### Comparing `kolena_client-0.67.0/kolena/_api/v1/detection.py` & `kolena_client-0.68.0/kolena/_api/v1/detection.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_api/v1/fr.py` & `kolena_client-0.68.0/kolena/_api/v1/fr.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_api/v1/generic.py` & `kolena_client-0.68.0/kolena/_api/v1/generic.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_api/v1/repository.py` & `kolena_client-0.68.0/kolena/_api/v1/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_api/v1/samples.py` & `kolena_client-0.68.0/kolena/_api/v1/samples.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_api/v1/token.py` & `kolena_client-0.68.0/kolena/_api/v1/token.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_api/v1/workflow.py` & `kolena_client-0.68.0/kolena/_api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_utils/__init__.py` & `kolena_client-0.68.0/kolena/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_utils/_consts.py` & `kolena_client-0.68.0/kolena/_utils/_consts.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_utils/asset_path_mapper.py` & `kolena_client-0.68.0/kolena/_utils/asset_path_mapper.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_utils/batched_load.py` & `kolena_client-0.68.0/kolena/_utils/batched_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from kolena._utils.asset_path_mapper import AssetPathMapper
 from kolena._utils.datatypes import LoadableDataFrame
 from kolena._utils.serde import from_dict
 from kolena.fr._consts import _BatchSize
 from kolena.fr.datatypes import _ImageChipsDataFrame
 
 VALIDATION_COUNT_LIMIT = 100
+MAX_FILE_UPLOAD_SIZE = 1_000
 STAGE_STATUS__LOADED = "LOADED"
 
 
 def init_upload() -> API.InitiateUploadResponse:
     init_res = krequests.put(endpoint_path=API.Path.INIT_UPLOAD)
     krequests.raise_for_status(init_res)
     init_response = from_dict(data_class=API.InitiateUploadResponse, data=init_res.json())
@@ -111,14 +112,15 @@
         upload_response = krequests.put(
             endpoint_path=AssetAPI.Path.BULK_UPLOAD,
             data=data,
             headers={"Content-Type": data.content_type},
         )
         krequests.raise_for_status(upload_response)
 
+    batch_size = min(batch_size, MAX_FILE_UPLOAD_SIZE)
     num_chunks = math.ceil(len(df) / batch_size)
     chunk_iter = np.array_split(df, num_chunks) if len(df) > 0 else []
     for df_chunk in chunk_iter:
         upload_batch(df_chunk)
 
 
 def sanitize_uuid(load_uuid: str) -> str:
```

### Comparing `kolena_client-0.67.0/kolena/_utils/cli.py` & `kolena_client-0.68.0/kolena/_utils/cli.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_utils/dataframes/__init__.py` & `kolena_client-0.68.0/kolena/_utils/dataframes/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_utils/dataframes/validators.py` & `kolena_client-0.68.0/kolena/_utils/dataframes/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_utils/datatypes.py` & `kolena_client-0.68.0/kolena/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_utils/endpoints.py` & `kolena_client-0.68.0/kolena/_utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_utils/frozen.py` & `kolena_client-0.68.0/kolena/_utils/frozen.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_utils/futures.py` & `kolena_client-0.68.0/kolena/_utils/futures.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_utils/geometry.py` & `kolena_client-0.68.0/kolena/_utils/geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_utils/inference_validators.py` & `kolena_client-0.68.0/kolena/_utils/inference_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_utils/instrumentation.py` & `kolena_client-0.68.0/kolena/_utils/instrumentation.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_utils/krequests.py` & `kolena_client-0.68.0/kolena/_utils/krequests.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_utils/log.py` & `kolena_client-0.68.0/kolena/_utils/log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_utils/repository.py` & `kolena_client-0.68.0/kolena/_utils/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_utils/serde.py` & `kolena_client-0.68.0/kolena/_utils/serde.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_utils/serializable.py` & `kolena_client-0.68.0/kolena/_utils/serializable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_utils/state.py` & `kolena_client-0.68.0/kolena/_utils/state.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_utils/stratification.py` & `kolena_client-0.68.0/kolena/_utils/stratification.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_utils/uninstantiable.py` & `kolena_client-0.68.0/kolena/_utils/uninstantiable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/_utils/validators.py` & `kolena_client-0.68.0/kolena/_utils/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/classification/__init__.py` & `kolena_client-0.68.0/kolena/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/classification/metadata.py` & `kolena_client-0.68.0/kolena/classification/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/classification/model.py` & `kolena_client-0.68.0/kolena/classification/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/classification/multiclass/__init__.py` & `kolena_client-0.68.0/kolena/classification/multiclass/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/classification/multiclass/_utils.py` & `kolena_client-0.68.0/kolena/classification/multiclass/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/classification/multiclass/evaluator.py` & `kolena_client-0.68.0/kolena/classification/multiclass/evaluator.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import dataclasses
-import re
 from collections import defaultdict
 from dataclasses import make_dataclass
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Set
@@ -35,29 +34,26 @@
 from kolena.classification.multiclass.workflow import InferenceLabel
 from kolena.classification.multiclass.workflow import TestCase
 from kolena.classification.multiclass.workflow import TestCaseMetrics
 from kolena.classification.multiclass.workflow import TestSample
 from kolena.classification.multiclass.workflow import TestSampleMetrics
 from kolena.classification.multiclass.workflow import TestSuiteMetrics
 from kolena.classification.multiclass.workflow import ThresholdConfiguration
+from kolena.workflow import BarPlot
 from kolena.workflow import ConfusionMatrix
 from kolena.workflow import Curve
 from kolena.workflow import CurvePlot
 from kolena.workflow import EvaluationResults
 from kolena.workflow import Histogram
 from kolena.workflow import Plot
 from kolena.workflow import TestCases
 
 Result = Tuple[TestSample, GroundTruth, Inference]
 
 
-def _clean_variable_name(name: str) -> str:
-    return re.sub(r"\W+", "_", name)
-
-
 def _compute_test_sample_metric(
     threshold_configuration: ThresholdConfiguration,
     ground_truth: GroundTruth,
     inference: Inference,
 ) -> TestSampleMetrics:
     empty_metrics = TestSampleMetrics(
         classification=None,
@@ -82,14 +78,33 @@
     return TestSampleMetrics(
         classification=match,
         margin=margin,
         is_correct=is_correct,
     )
 
 
+def _as_class_metric_plot(
+    metric_name: str,
+    metrics_by_label: Dict[str, AggregatedMetrics],
+    labels: List[str],
+) -> BarPlot:
+    if metric_name == "Recall":
+        title = f"{metric_name} (TPR) vs. Class"
+    else:
+        title = f"{metric_name} vs. Class"
+
+    return BarPlot(
+        title=title,
+        x_label="Class",
+        y_label=metric_name,
+        labels=labels,
+        values=[getattr(metrics_by_label[label], metric_name) for label in labels],
+    )
+
+
 def _as_confidence_histogram(
     title: str,
     confidence_scores: List[float],
     confidence_range: Tuple[float, float, int] = (0, 1, 25),
 ) -> Histogram:
     min_range, max_range, bins = confidence_range
     hist, bins = np.histogram(
@@ -108,29 +123,40 @@
 
 def _compute_test_case_plots(
     test_case_name: str,
     labels: List[str],
     ground_truths: List[GroundTruth],
     inferences: List[Inference],
     metrics: List[TestSampleMetrics],
+    metrics_by_label: Dict[str, AggregatedMetrics],
     confidence_range: Tuple[float, float, int],
 ) -> List[Plot]:
     confidence_all = [mts.classification.confidence for mts in metrics if mts.classification is not None]
     confidence_correct = [
         mts.classification.confidence for mts in metrics if mts.classification is not None and mts.is_correct
     ]
     confidence_incorrect = [
         mts.classification.confidence for mts in metrics if mts.classification is not None and not mts.is_correct
     ]
 
+    gt_labels = {gt.classification.label for gt in ground_truths}
+    class_metric_plots = [
+        _as_class_metric_plot(field.name, metrics_by_label, labels)
+        for field in dataclasses.fields(AggregatedMetrics)
+        if len(gt_labels) > 2
+        or field.name not in ["Precision", "Recall"]  # Omit single-class TC from precision and recall plots
+    ]
+
     plots = [
+        *class_metric_plots,
         _as_confidence_histogram("Confidence Distribution (All)", confidence_all, confidence_range),
         _as_confidence_histogram("Confidence Distribution (Correct)", confidence_correct, confidence_range),
         _as_confidence_histogram("Confidence Distribution (Incorrect)", confidence_incorrect, confidence_range),
     ]
+
     roc_curve_plot = _compute_test_case_ovr_roc_curve(labels, ground_truths, inferences)
     if roc_curve_plot:
         plots.append(roc_curve_plot)
     confusion_matrix = _compute_test_case_confusion_matrix(test_case_name, ground_truths, metrics)
     if confusion_matrix:
         plots.append(confusion_matrix)
     return plots
@@ -183,16 +209,16 @@
         fpr_values, tpr_values = roc_curve(y_true, y_score)
         if len(fpr_values) > 0 and len(tpr_values) > 0:
             curves.append(Curve(x=fpr_values, y=tpr_values, label=label))
 
     if len(curves) > 0:
         return CurvePlot(
             title="Receiver Operating Characteristic (One-vs-Rest)",
-            x_label="False Positive Rate",
-            y_label="True Positive Rate",
+            x_label="False Positive Rate (FPR)",
+            y_label="True Positive Rate (TPR)",
             curves=curves,
         )
     return None
 
 
 def _aggregate_label_metrics(
     labels: List[str],
@@ -219,62 +245,50 @@
             if gt_label != base_label and predicted_label != base_label:
                 n_tn += 1
         precision = n_tp / (n_tp + n_fp) if n_tp + n_fp > 0 else 0
         recall = n_tp / (n_tp + n_fn) if n_tp + n_fn > 0 else 0
         fpr = n_fp / (n_fp + n_tn) if n_fp + n_tn > 0 else 0
         f1_score = (2 * precision * recall) / (precision + recall) if precision + recall > 0 else 0
         aggregated_metrics[base_label] = AggregatedMetrics(
-            Count=n_tp + n_fn,
             F1=f1_score,
             Precision=precision,
             Recall=recall,
-            TPR=recall,
             FPR=fpr,
         )
     return aggregated_metrics
 
 
 def _compute_test_case_metrics(
-    labels: List[str],
     test_samples: List[TestSample],
     ground_truths: List[GroundTruth],
-    inferences: List[Inference],
     metrics_test_samples: List[TestSampleMetrics],
+    metrics_by_label: Dict[str, AggregatedMetrics],
 ) -> TestCaseMetrics:
     n_correct = len([metric for metric in metrics_test_samples if metric.is_correct])
     n_images = len(test_samples)
+    n_incorrect = n_images - n_correct
     accuracy = n_correct / n_images
-    values: Dict[str, Any] = dict(
-        n_correct=n_correct,
-        accuracy=accuracy,
-    )
-    fields: Dict[str, Type] = {}
+    labels = {gt.classification.label for gt in ground_truths}
 
-    aggregated_label_metrics = _aggregate_label_metrics(
-        labels,
-        test_samples,
-        ground_truths,
-        inferences,
-        metrics_test_samples,
-    )
-    for label, aggregated_metrics in aggregated_label_metrics.items():
-        label_name = _clean_variable_name(label)
-        for field in dataclasses.fields(AggregatedMetrics):
-            key = f"{label_name}_{field.name}"
-            value = getattr(aggregated_metrics, field.name)
-            values[key] = value
-            fields[key] = float
+    macro_metrics_by_name: Dict[str, float] = {}
+    for field in dataclasses.fields(AggregatedMetrics):
+        metric_name = field.name
+        metrics = [getattr(metrics_by_label[label], metric_name) for label in labels]
+        macro_metrics_by_name[metric_name] = sum(metrics) / len(metrics)
 
-    dc = make_dataclass(
-        "WorkflowTestCaseMetrics",
-        bases=(TestCaseMetrics,),
-        fields=list(fields.items()),
-        frozen=True,
+    return TestCaseMetrics(
+        n_correct=n_correct,
+        n_incorrect=n_incorrect,
+        accuracy=accuracy,
+        macro_precision=macro_metrics_by_name["Precision"],
+        macro_recall=macro_metrics_by_name["Recall"],
+        macro_f1=macro_metrics_by_name["F1"],
+        macro_tpr=macro_metrics_by_name["Recall"],
+        macro_fpr=macro_metrics_by_name["FPR"],
     )
-    return dc(**values)
 
 
 def _compute_test_suite_metrics(
     labels: List[str],
     test_samples: List[TestSample],
     ground_truths: List[GroundTruth],
     inferences: List[Inference],
@@ -291,16 +305,14 @@
         mean_test_case_accuracy=mean_test_case_accuracy,
     )
     fields: Dict[str, Type] = {}
 
     metrics_by_label = _aggregate_label_metrics(labels, test_samples, ground_truths, inferences, test_sample_metrics)
     for field in dataclasses.fields(AggregatedMetrics):
         attr = field.name
-        if attr == "Count":
-            continue  # mean and variance for Count not really meaningful
         label_values = [getattr(metric, attr) for metric in metrics_by_label.values()]
         mean_field_name = f"mean_{attr}"
         var_field_name = f"variance_{attr}"
         fields[mean_field_name] = float
         fields[var_field_name] = float
         values[mean_field_name] = np.mean(label_values)
         values[var_field_name] = np.var(label_values)
@@ -341,17 +353,26 @@
     plots_test_case: List[Tuple[TestCase, List[Plot]]] = []
     for tc, tc_samples, tc_gts, tc_infs, tc_metrics in test_cases.iter(
         test_samples,
         ground_truths,
         inferences,
         test_sample_metrics,
     ):
-        test_case_metrics = _compute_test_case_metrics(labels, tc_samples, tc_gts, tc_infs, tc_metrics)
+        aggregated_label_metrics = _aggregate_label_metrics(labels, tc_samples, tc_gts, tc_infs, tc_metrics)
+        test_case_metrics = _compute_test_case_metrics(tc_samples, tc_gts, tc_metrics, aggregated_label_metrics)
         metrics_test_case.append((tc, test_case_metrics))
-        test_case_plots = _compute_test_case_plots(tc.name, labels, tc_gts, tc_infs, tc_metrics, confidence_range)
+        test_case_plots = _compute_test_case_plots(
+            tc.name,
+            labels,
+            tc_gts,
+            tc_infs,
+            tc_metrics,
+            aggregated_label_metrics,
+            confidence_range,
+        )
         plots_test_case.append((tc, test_case_plots))
 
     all_test_case_metrics = [metric for _, metric in metrics_test_case]
     metrics_test_suite = _compute_test_suite_metrics(
         labels,
         test_samples,
         ground_truths,
```

### Comparing `kolena_client-0.67.0/kolena/classification/multiclass/test_run.py` & `kolena_client-0.68.0/kolena/classification/multiclass/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/classification/multiclass/workflow.py` & `kolena_client-0.68.0/kolena/classification/multiclass/workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,26 +57,30 @@
     classification: Optional[InferenceLabel]
     margin: Optional[float]
     is_correct: bool
 
 
 @dataclass(frozen=True)
 class AggregatedMetrics:
-    Count: int
     F1: float
     Precision: float
     Recall: float
-    TPR: float
     FPR: float
 
 
 @dataclass(frozen=True)
 class TestCaseMetrics(MetricsTestCase):
     n_correct: int
+    n_incorrect: int
     accuracy: float
+    macro_precision: float
+    macro_recall: float
+    macro_f1: float
+    macro_tpr: float
+    macro_fpr: float
 
 
 @dataclass(frozen=True)
 class TestSuiteMetrics(MetricsTestSuite):
     n_images: int
     n_correct: int
     mean_test_case_accuracy: float
```

### Comparing `kolena_client-0.67.0/kolena/classification/test_case.py` & `kolena_client-0.68.0/kolena/classification/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/classification/test_config.py` & `kolena_client-0.68.0/kolena/classification/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/classification/test_image.py` & `kolena_client-0.68.0/kolena/classification/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/classification/test_run.py` & `kolena_client-0.68.0/kolena/classification/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/classification/test_suite.py` & `kolena_client-0.68.0/kolena/classification/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/detection/__init__.py` & `kolena_client-0.68.0/kolena/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/detection/_datatypes.py` & `kolena_client-0.68.0/kolena/detection/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/detection/_internal/__init__.py` & `kolena_client-0.68.0/kolena/detection/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/detection/_internal/datatypes.py` & `kolena_client-0.68.0/kolena/detection/_internal/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/detection/_internal/ground_truth.py` & `kolena_client-0.68.0/kolena/detection/_internal/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/detection/_internal/inference.py` & `kolena_client-0.68.0/kolena/detection/_internal/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/detection/_internal/metadata.py` & `kolena_client-0.68.0/kolena/detection/_internal/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/detection/_internal/model.py` & `kolena_client-0.68.0/kolena/detection/_internal/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/detection/_internal/test_case.py` & `kolena_client-0.68.0/kolena/detection/_internal/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/detection/_internal/test_config.py` & `kolena_client-0.68.0/kolena/detection/_internal/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/detection/_internal/test_image.py` & `kolena_client-0.68.0/kolena/detection/_internal/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/detection/_internal/test_run.py` & `kolena_client-0.68.0/kolena/detection/_internal/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/detection/_internal/test_suite.py` & `kolena_client-0.68.0/kolena/detection/_internal/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/detection/ground_truth.py` & `kolena_client-0.68.0/kolena/detection/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/detection/inference.py` & `kolena_client-0.68.0/kolena/detection/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/detection/metadata.py` & `kolena_client-0.68.0/kolena/detection/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/detection/model.py` & `kolena_client-0.68.0/kolena/detection/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/detection/test_case.py` & `kolena_client-0.68.0/kolena/detection/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/detection/test_config.py` & `kolena_client-0.68.0/kolena/detection/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/detection/test_image.py` & `kolena_client-0.68.0/kolena/detection/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/detection/test_run.py` & `kolena_client-0.68.0/kolena/detection/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/detection/test_suite.py` & `kolena_client-0.68.0/kolena/detection/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/errors.py` & `kolena_client-0.68.0/kolena/errors.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/fr/__init__.py` & `kolena_client-0.68.0/kolena/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/fr/_consts.py` & `kolena_client-0.68.0/kolena/fr/_consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from enum import Enum
 
 
 class _BatchSize(int, Enum):
-    UPLOAD_CHIPS = 5_000
+    UPLOAD_CHIPS = 1_000
     UPLOAD_RECORDS = 10_000_000
```

### Comparing `kolena_client-0.67.0/kolena/fr/datatypes.py` & `kolena_client-0.68.0/kolena/fr/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/fr/model.py` & `kolena_client-0.68.0/kolena/fr/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/fr/test_case.py` & `kolena_client-0.68.0/kolena/fr/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/fr/test_images.py` & `kolena_client-0.68.0/kolena/fr/test_images.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/fr/test_run.py` & `kolena_client-0.68.0/kolena/fr/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/fr/test_suite.py` & `kolena_client-0.68.0/kolena/fr/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/initialize.py` & `kolena_client-0.68.0/kolena/initialize.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/workflow/__init__.py` & `kolena_client-0.68.0/kolena/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/workflow/_datatypes.py` & `kolena_client-0.68.0/kolena/workflow/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/workflow/_helpers.py` & `kolena_client-0.68.0/kolena/workflow/_helpers.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/workflow/_validators.py` & `kolena_client-0.68.0/kolena/workflow/_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/workflow/asset.py` & `kolena_client-0.68.0/kolena/workflow/asset.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/workflow/evaluator.py` & `kolena_client-0.68.0/kolena/workflow/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/workflow/evaluator_function.py` & `kolena_client-0.68.0/kolena/workflow/evaluator_function.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/workflow/ground_truth.py` & `kolena_client-0.68.0/kolena/workflow/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/workflow/inference.py` & `kolena_client-0.68.0/kolena/workflow/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/workflow/metrics/__init__.py` & `kolena_client-0.68.0/kolena/workflow/metrics/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,10 +7,16 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from ._geometry import InferenceMatches
 from ._geometry import iou
+from ._geometry import match_inferences
 
-__all__ = ["iou"]
+__all__ = [
+    "iou",
+    "InferenceMatches",
+    "match_inferences",
+]
```

### Comparing `kolena_client-0.67.0/kolena/workflow/model.py` & `kolena_client-0.68.0/kolena/workflow/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/workflow/test_case.py` & `kolena_client-0.68.0/kolena/workflow/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/workflow/test_run.py` & `kolena_client-0.68.0/kolena/workflow/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/workflow/test_sample.py` & `kolena_client-0.68.0/kolena/workflow/test_sample.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/workflow/test_suite.py` & `kolena_client-0.68.0/kolena/workflow/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/kolena/workflow/workflow.py` & `kolena_client-0.68.0/kolena/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.67.0/pyproject.toml` & `kolena_client-0.68.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "kolena-client"
-version = "0.67.0"
+version = "0.68.0"
 description = "Client for Kolena's machine learning (ML) testing and debugging platform."
 authors = ["Kolena Engineering <eng@kolena.io>"]
 homepage = "https://kolena.io"
 documentation = "https://docs.kolena.io"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["Kolena", "ML", "testing"]
-classifiers = [  # license, versions set automatically during build
+classifiers = [# license, versions set automatically during build
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Natural Language :: English",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -28,15 +28,15 @@
 python = ">=3.7.1,<3.11"
 numpy = ">=1.19"
 pandas = ">=1.1,<1.6"
 pandera = ">=0.9.0"
 pydantic = ">=1.8"
 dacite = ">=1.6"
 requests = ">=2.20"
-requests-toolbelt = "^0.9.1"
+requests-toolbelt = "^1.0.0"
 importlib-metadata = { version = "<5.0", python = "<3.8" }
 tqdm = ">=4,<5"
 Pillow = "^9.1.1"
 retrying = "^1.3.3"
 Shapely = "^1.8.5"
 deprecation = "^2.1.0"
 termcolor = "^1.1.0"
```

### Comparing `kolena_client-0.67.0/setup.py` & `kolena_client-0.68.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,30 +25,30 @@
  'dacite>=1.6',
  'deprecation>=2.1.0,<3.0.0',
  'numpy>=1.19',
  'pandas>=1.1,<1.6',
  'pandera>=0.9.0',
  'pyarrow>=8',
  'pydantic>=1.8',
- 'requests-toolbelt>=0.9.1,<0.10.0',
+ 'requests-toolbelt>=1.0.0,<2.0.0',
  'requests>=2.20',
  'retrying>=1.3.3,<2.0.0',
  'termcolor>=1.1.0,<2.0.0',
  'tqdm>=4,<5']
 
 extras_require = \
 {':python_version < "3.8"': ['importlib-metadata<5.0',
                              'typing-extensions>=4.5.0,<5.0.0']}
 
 entry_points = \
 {'console_scripts': ['kolena = kolena._utils.cli:run']}
 
 setup_kwargs = {
     'name': 'kolena-client',
-    'version': '0.67.0',
+    'version': '0.68.0',
     'description': "Client for Kolena's machine learning (ML) testing and debugging platform.",
     'long_description': '<p align="center">\n  <img src="https://app.kolena.io/api/developer/docs/html/_static/wordmark-purple.svg" width="400" alt="Kolena" />\n</p>\n\n<p align=\'center\'>\n  <a href="https://pypi.python.org/pypi/kolena-client"><img src="https://img.shields.io/pypi/v/kolena-client" /></a>\n  <a href="https://www.apache.org/licenses/LICENSE-2.0"><img src="https://img.shields.io/pypi/l/kolena-client" /></a>\n  <a href="https://docs.kolena.io"><img src="https://img.shields.io/badge/docs-Tutorial%20%26%20Usage-6434c1" /></a>\n  <a href="https://app.kolena.io/api/developer/docs/html/index.html"><img src="https://img.shields.io/badge/docs-API%20Reference-6434c1" /></a>\n</p>\n\n---\n\n[Kolena](https://www.kolena.io) is a comprehensive machine learning testing and debugging platform to surface hidden\nmodel behaviors and take the mystery out of model development. Kolena helps you:\n\n- Perform high-resolution model evaluation\n- Understand and track behavioral improvements and regressions\n- Meaningfully communicate model capabilities\n- Automate model testing and deployment workflows\n\n`kolena-client` is the Python client library for programmatic interaction with Kolena.\n\n## Documentation\n\nVisit [docs.kolena.io](https://docs.kolena.io/) for tutorial and usage documentation and the\n[API Reference](https://app.kolena.io/api/developer/docs/html/index.html) for detailed `kolena-client` typing and\nfunction documentation.\n',
     'author': 'Kolena Engineering',
     'author_email': 'eng@kolena.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kolena.io',
```

#### html2text {}

```diff
@@ -2,20 +2,20 @@
 'kolena._api', 'kolena._api.v1', 'kolena._utils', 'kolena._utils.dataframes',
 'kolena.classification', 'kolena.classification.multiclass',
 'kolena.detection', 'kolena.detection._internal', 'kolena.fr',
 'kolena.workflow', 'kolena.workflow.metrics'] package_data = \ {'': ['*']}
 install_requires = \ ['Pillow>=9.1.1,<10.0.0', 'Shapely>=1.8.5,<2.0.0',
 'click>=8.1.3,<9.0.0', 'dacite>=1.6', 'deprecation>=2.1.0,<3.0.0',
 'numpy>=1.19', 'pandas>=1.1,<1.6', 'pandera>=0.9.0', 'pyarrow>=8',
-'pydantic>=1.8', 'requests-toolbelt>=0.9.1,<0.10.0', 'requests>=2.20',
+'pydantic>=1.8', 'requests-toolbelt>=1.0.0,<2.0.0', 'requests>=2.20',
 'retrying>=1.3.3,<2.0.0', 'termcolor>=1.1.0,<2.0.0', 'tqdm>=4,<5']
 extras_require = \ {':python_version < "3.8"': ['importlib-metadata<5.0',
 'typing-extensions>=4.5.0,<5.0.0']} entry_points = \ {'console_scripts':
 ['kolena = kolena._utils.cli:run']} setup_kwargs = { 'name': 'kolena-client',
-'version': '0.67.0', 'description': "Client for Kolena's machine learning (ML)
+'version': '0.68.0', 'description': "Client for Kolena's machine learning (ML)
 testing and debugging platform.", 'long_description': '
                                  \n [Kolena]\n
 \n\n
 \n [https://img.shields.io/pypi/v/kolena-client]\n [https://img.shields.io/
 pypi/l/kolena-client]\n [https://img.shields.io/badge/docs-
 Tutorial%20%26%20Usage-6434c1]\n [https://img.shields.io/badge/docs-
 API%20Reference-6434c1]\n
```

### Comparing `kolena_client-0.67.0/PKG-INFO` & `kolena_client-0.68.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolena-client
-Version: 0.67.0
+Version: 0.68.0
 Summary: Client for Kolena's machine learning (ML) testing and debugging platform.
 Home-page: https://kolena.io
 License: Apache-2.0
 Keywords: Kolena,ML,testing
 Author: Kolena Engineering
 Author-email: eng@kolena.io
 Requires-Python: >=3.7.1,<3.11
@@ -31,15 +31,15 @@
 Requires-Dist: importlib-metadata (<5.0); python_version < "3.8"
 Requires-Dist: numpy (>=1.19)
 Requires-Dist: pandas (>=1.1,<1.6)
 Requires-Dist: pandera (>=0.9.0)
 Requires-Dist: pyarrow (>=8)
 Requires-Dist: pydantic (>=1.8)
 Requires-Dist: requests (>=2.20)
-Requires-Dist: requests-toolbelt (>=0.9.1,<0.10.0)
+Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
 Requires-Dist: retrying (>=1.3.3,<2.0.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Requires-Dist: tqdm (>=4,<5)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0); python_version < "3.8"
 Project-URL: Documentation, https://docs.kolena.io
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kolena-client Version: 0.67.0 Summary: Client for
+Metadata-Version: 2.1 Name: kolena-client Version: 0.68.0 Summary: Client for
 Kolena's machine learning (ML) testing and debugging platform. Home-page:
 https://kolena.io License: Apache-2.0 Keywords: Kolena,ML,testing Author:
 Kolena Engineering Author-email: eng@kolena.io Requires-Python: >=3.7.1,<3.11
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
@@ -15,15 +15,15 @@
 Testing Classifier: Typing :: Typed Requires-Dist: Pillow (>=9.1.1,<10.0.0)
 Requires-Dist: Shapely (>=1.8.5,<2.0.0) Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dacite (>=1.6) Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: importlib-metadata (<5.0); python_version < "3.8" Requires-Dist:
 numpy (>=1.19) Requires-Dist: pandas (>=1.1,<1.6) Requires-Dist: pandera
 (>=0.9.0) Requires-Dist: pyarrow (>=8) Requires-Dist: pydantic (>=1.8)
 Requires-Dist: requests (>=2.20) Requires-Dist: requests-toolbelt
-(>=0.9.1,<0.10.0) Requires-Dist: retrying (>=1.3.3,<2.0.0) Requires-Dist:
+(>=1.0.0,<2.0.0) Requires-Dist: retrying (>=1.3.3,<2.0.0) Requires-Dist:
 termcolor (>=1.1.0,<2.0.0) Requires-Dist: tqdm (>=4,<5) Requires-Dist: typing-
 extensions (>=4.5.0,<5.0.0); python_version < "3.8" Project-URL: Documentation,
 https://docs.kolena.io Description-Content-Type: text/markdown
                                    [Kolena]
  [https://img.shields.io/pypi/v/kolena-client] [https://img.shields.io/pypi/l/
    kolena-client] [https://img.shields.io/badge/docs-Tutorial%20%26%20Usage-
       6434c1] [https://img.shields.io/badge/docs-API%20Reference-6434c1]
```

