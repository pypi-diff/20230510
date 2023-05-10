# Comparing `tmp/aqueduct-sdk-0.3.1.tar.gz` & `tmp/aqueduct-sdk-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqueduct-sdk-0.3.1.tar", last modified: Thu May  4 10:50:06 2023, max compression
+gzip compressed data, was "aqueduct-sdk-0.3.2.tar", last modified: Wed May 10 18:31:38 2023, max compression
```

## Comparing `aqueduct-sdk-0.3.1.tar` & `aqueduct-sdk-0.3.2.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:50:06.779054 aqueduct-sdk-0.3.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       34 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7511 2023-05-04 10:50:06.779054 aqueduct-sdk-0.3.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:50:06.763054 aqueduct-sdk-0.3.1/aqueduct/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1530 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:50:06.767053 aqueduct-sdk-0.3.1/aqueduct/artifacts/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/artifacts/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/artifacts/_create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1815 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/artifacts/base_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4188 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/artifacts/bool_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3729 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/artifacts/create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4688 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/artifacts/generic_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11713 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/artifacts/numeric_artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6599 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/artifacts/preview.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4124 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/artifacts/system_metric.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24895 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/artifacts/table_artifact.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:50:06.767053 aqueduct-sdk-0.3.1/aqueduct/backend/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/backend/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24487 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/backend/api_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6091 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/backend/response_helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34643 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:50:06.767053 aqueduct-sdk-0.3.1/aqueduct/constants/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/constants/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6666 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/constants/enums.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/constants/exports.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/constants/metrics.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    52868 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/decorator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3930 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/error.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5525 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/flow.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7295 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/flow_run.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8269 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/github.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:50:06.767053 aqueduct-sdk-0.3.1/aqueduct/globals/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      200 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/globals/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/globals/api_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      477 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/globals/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      192 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/globals/dag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8354 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/llm_wrapper.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/logger.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:50:06.767053 aqueduct-sdk-0.3.1/aqueduct/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      574 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/models/artifact.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1647 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/models/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19371 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/models/dag.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2925 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/models/dag_rules.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      554 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/models/execution_state.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3099 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/models/integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7640 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/models/operators.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9747 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/models/response_models.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      176 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/models/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:50:06.771054 aqueduct-sdk-0.3.1/aqueduct/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      285 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      474 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/resources/airflow.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      624 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/resources/aws.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      464 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/resources/aws_lambda.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13077 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/resources/connect_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      486 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/resources/databricks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7518 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/resources/dynamic_k8s.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1787 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/resources/ecr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4878 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/resources/google_sheets.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      458 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/resources/k8s.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8993 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/resources/mongodb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2596 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/resources/parameters.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9035 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/resources/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5519 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/resources/salesforce.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3199 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/resources/save.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      466 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/resources/spark.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12065 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/resources/sql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      687 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/resources/validation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3846 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/schedule.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:50:06.775054 aqueduct-sdk-0.3.1/aqueduct/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      451 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/tests/connect_config_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19133 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/tests/dag_delta_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4058 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/tests/dag_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3040 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/tests/decorator_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3811 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/tests/decorators_with_without_parentheses_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      218 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/tests/enum_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1094 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/tests/flow_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1398 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/tests/helpers_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4498 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/tests/metric_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      488 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/tests/naming_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15641 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/tests/serialization_test.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:50:06.775054 aqueduct-sdk-0.3.1/aqueduct/tests/test_files/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/tests/test_files/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:50:06.775054 aqueduct-sdk-0.3.1/aqueduct/tests/test_files/python_function/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/tests/test_files/python_function/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      170 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/tests/test_files/python_function/python_function.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:50:06.775054 aqueduct-sdk-0.3.1/aqueduct/tests/test_files/python_function/test_dependency_folder/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/tests/test_files/python_function/test_dependency_folder/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/tests/test_files/python_function/test_dependency_folder/helper_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6071 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/tests/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/type_annotations.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:50:06.775054 aqueduct-sdk-0.3.1/aqueduct/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10504 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/utils/dag_deltas.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1271 2023-02-07 07:49:15.000000 aqueduct-sdk-0.3.1/aqueduct/utils/describe.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/utils/format.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11492 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/utils/function_packaging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1446 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/utils/integration_validation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1706 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/utils/local_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1234 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/utils/naming.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16432 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/utils/serialization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2148 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/utils/type_inference.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8505 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/aqueduct/utils/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:50:06.775054 aqueduct-sdk-0.3.1/aqueduct_sdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7511 2023-05-04 10:50:06.000000 aqueduct-sdk-0.3.1/aqueduct_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3124 2023-05-04 10:50:06.000000 aqueduct-sdk-0.3.1/aqueduct_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-04 10:50:06.000000 aqueduct-sdk-0.3.1/aqueduct_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-05-04 10:50:06.000000 aqueduct-sdk-0.3.1/aqueduct_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-04 10:50:06.000000 aqueduct-sdk-0.3.1/aqueduct_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:50:06.779054 aqueduct-sdk-0.3.1/requirements/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/requirements/python-3-10.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/requirements/python-3-7.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/requirements/python-3-8.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/requirements/python-3-9.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-04 10:50:06.779054 aqueduct-sdk-0.3.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1197 2023-05-04 10:16:29.000000 aqueduct-sdk-0.3.1/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-05-04 10:16:31.000000 aqueduct-sdk-0.3.1/version
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.157794 aqueduct-sdk-0.3.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       34 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7511 2023-05-10 18:31:38.157794 aqueduct-sdk-0.3.2/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.145794 aqueduct-sdk-0.3.2/aqueduct/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1530 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.145794 aqueduct-sdk-0.3.2/aqueduct/artifacts/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/artifacts/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1258 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/artifacts/_create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1815 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/artifacts/base_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4188 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/artifacts/bool_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3729 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/artifacts/create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4688 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/artifacts/generic_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11713 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/artifacts/numeric_artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6599 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/artifacts/preview.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4124 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/artifacts/system_metric.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24895 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/artifacts/table_artifact.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.149794 aqueduct-sdk-0.3.2/aqueduct/backend/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/backend/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24525 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/backend/api_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6091 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/backend/response_helpers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35841 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.149794 aqueduct-sdk-0.3.2/aqueduct/constants/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/constants/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6596 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/constants/enums.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/constants/exports.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/constants/metrics.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    52868 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/decorator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3930 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/error.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5525 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/flow.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7295 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/flow_run.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8260 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/github.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.149794 aqueduct-sdk-0.3.2/aqueduct/globals/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      200 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/globals/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      194 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/globals/api_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      477 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/globals/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      192 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/globals/dag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8506 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/llm_wrapper.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/logger.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.149794 aqueduct-sdk-0.3.2/aqueduct/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      574 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/models/artifact.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1647 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/models/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19371 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/models/dag.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2925 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/models/dag_rules.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      554 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/models/execution_state.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3061 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/models/integration.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7640 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/models/operators.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9747 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/models/response_models.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      176 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/models/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.153794 aqueduct-sdk-0.3.2/aqueduct/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      285 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      474 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/airflow.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      624 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/aws.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      464 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/aws_lambda.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13077 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/connect_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      486 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/databricks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7518 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/dynamic_k8s.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1789 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/ecr.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4878 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/google_sheets.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      458 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/k8s.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8993 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/mongodb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2596 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/parameters.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9035 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5519 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/salesforce.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3199 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/save.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      466 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/spark.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12027 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/sql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      687 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/resources/validation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3846 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/schedule.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.153794 aqueduct-sdk-0.3.2/aqueduct/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      451 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/connect_config_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19133 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/dag_delta_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4058 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/dag_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3040 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/decorator_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3811 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/decorators_with_without_parentheses_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      218 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/enum_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1094 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/flow_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1398 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/helpers_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4498 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/metric_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      488 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/naming_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15641 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/serialization_test.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.153794 aqueduct-sdk-0.3.2/aqueduct/tests/test_files/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/test_files/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.153794 aqueduct-sdk-0.3.2/aqueduct/tests/test_files/python_function/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/test_files/python_function/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      170 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/test_files/python_function/python_function.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.153794 aqueduct-sdk-0.3.2/aqueduct/tests/test_files/python_function/test_dependency_folder/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/test_files/python_function/test_dependency_folder/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/test_files/python_function/test_dependency_folder/helper_function.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6071 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/tests/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      225 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/type_annotations.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.153794 aqueduct-sdk-0.3.2/aqueduct/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10504 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/utils/dag_deltas.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1271 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/utils/describe.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/utils/format.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11492 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/utils/function_packaging.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1446 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/utils/integration_validation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1706 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/utils/local_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1234 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/utils/naming.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16432 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/utils/serialization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2148 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/utils/type_inference.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8505 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/aqueduct/utils/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.153794 aqueduct-sdk-0.3.2/aqueduct_sdk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7511 2023-05-10 18:31:38.000000 aqueduct-sdk-0.3.2/aqueduct_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3124 2023-05-10 18:31:38.000000 aqueduct-sdk-0.3.2/aqueduct_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-10 18:31:38.000000 aqueduct-sdk-0.3.2/aqueduct_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-05-10 18:31:38.000000 aqueduct-sdk-0.3.2/aqueduct_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-05-10 18:31:38.000000 aqueduct-sdk-0.3.2/aqueduct_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:31:38.153794 aqueduct-sdk-0.3.2/requirements/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/requirements/python-3-10.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/requirements/python-3-7.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/requirements/python-3-8.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/requirements/python-3-9.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-10 18:31:38.157794 aqueduct-sdk-0.3.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1197 2023-05-09 23:15:33.000000 aqueduct-sdk-0.3.2/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-05-09 23:19:59.000000 aqueduct-sdk-0.3.2/version
```

### Comparing `aqueduct-sdk-0.3.1/PKG-INFO` & `aqueduct-sdk-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-sdk
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python SDK for Aqueduct
 Home-page: https://github.com/aqueducthq/aqueduct
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `aqueduct-sdk-0.3.1/aqueduct/__init__.py` & `aqueduct-sdk-0.3.2/aqueduct/__init__.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/artifacts/_create.py` & `aqueduct-sdk-0.3.2/aqueduct/artifacts/_create.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/artifacts/base_artifact.py` & `aqueduct-sdk-0.3.2/aqueduct/artifacts/base_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/artifacts/bool_artifact.py` & `aqueduct-sdk-0.3.2/aqueduct/artifacts/bool_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/artifacts/create.py` & `aqueduct-sdk-0.3.2/aqueduct/artifacts/create.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/artifacts/generic_artifact.py` & `aqueduct-sdk-0.3.2/aqueduct/artifacts/generic_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/artifacts/numeric_artifact.py` & `aqueduct-sdk-0.3.2/aqueduct/artifacts/numeric_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/artifacts/preview.py` & `aqueduct-sdk-0.3.2/aqueduct/artifacts/preview.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/artifacts/system_metric.py` & `aqueduct-sdk-0.3.2/aqueduct/artifacts/system_metric.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/artifacts/table_artifact.py` & `aqueduct-sdk-0.3.2/aqueduct/artifacts/table_artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/backend/api_client.py` & `aqueduct-sdk-0.3.2/aqueduct/backend/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,16 +144,17 @@
                 "Unable to connect to server. Double check that both your API key `%s` and your specified address `%s` are correct. "
                 % (self.api_key, self.aqueduct_address),
             )
 
     def _check_config(self) -> None:
         if not self.configured:
             raise Exception(
-                "API client has not been configured, please complete the configuration \
-                by initializing an Aqueduct client with the api key and the server address."
+                "API client has not been configured, please complete the configuration "
+                "by initializing an Aqueduct client via: "
+                "`client = aqueduct.Client(api_key, aqueduct_address)`"
             )
 
     def _generate_auth_headers(self) -> Dict[str, str]:
         self._check_config()
         return {self.API_KEY_HEADER: self.api_key}
 
     def construct_base_url(self, use_https: Optional[bool] = None) -> str:
```

### Comparing `aqueduct-sdk-0.3.1/aqueduct/backend/response_helpers.py` & `aqueduct-sdk-0.3.2/aqueduct/backend/response_helpers.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/client.py` & `aqueduct-sdk-0.3.2/aqueduct/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,18 @@
         except yaml.YAMLError as exc:
             logger().error(
                 "This API works only when you are running the server and the SDK on the same machine."
             )
             exit(1)
 
 
+DEPRECATED_AQUEDUCT_DEMO_DB_NAME = "aqueduct_demo"
+AQUEDUCT_DEMO_DB_NAME = "Demo"
+
+
 class Client:
     """This class allows users to interact with flows on their Aqueduct cluster."""
 
     def __init__(
         self,
         api_key: str = "",
         aqueduct_address: str = "http://localhost:8080",
@@ -302,20 +306,27 @@
         """Deletes the integration from Aqueduct.
 
         Args:
             name:
                 The name of the integration to delete.
         """
         existing_integrations = globals.__GLOBAL_API_CLIENT__.list_resources()
+
+        # If the user uses the deprecated demo name, and there isn't a resource for this, that means they actually
+        # want to use the new demo name.
+        if (
+            name == DEPRECATED_AQUEDUCT_DEMO_DB_NAME
+            and DEPRECATED_AQUEDUCT_DEMO_DB_NAME not in existing_integrations.keys()
+        ) or name == AQUEDUCT_DEMO_DB_NAME:
+            raise InvalidUserActionException("Cannot delete the Aqueduct demo database: %s" % name)
         if name not in existing_integrations.keys():
             raise InvalidIntegrationException("Not connected to integration %s!" % name)
 
-        globals.__GLOBAL_API_CLIENT__.delete_integration(existing_integrations[name].id)
-
         # Update the connected integrations cached on this object.
+        globals.__GLOBAL_API_CLIENT__.delete_integration(existing_integrations[name].id)
         self._connected_integrations = globals.__GLOBAL_API_CLIENT__.list_resources()
 
     def list_integrations(self) -> Dict[str, ResourceInfo]:
         """Deprecated. Use `client.list_resources()` instead."""
         logger().warning(
             "client.list_integrations() will be deprecated soon. Use `client.list_resources() instead."
         )
@@ -381,16 +392,27 @@
         Raises:
             InvalidIntegrationException:
                 An error occurred because the cluster is not connected to the
                 provided integration or the provided integration is of an
                 incompatible type.
         """
         self._connected_integrations = globals.__GLOBAL_API_CLIENT__.list_resources()
+        connected_names = self._connected_integrations.keys()
+
+        if name == DEPRECATED_AQUEDUCT_DEMO_DB_NAME:
+            # If the user uses the deprecated demo name, and there isn't a resource for this, that means they actually
+            # want to use the new demo name. We implicitly convert this for them, with a warning.
+            if DEPRECATED_AQUEDUCT_DEMO_DB_NAME not in connected_names:
+                logger().warning(
+                    "`%s` is the deprecated name for the aqueduct demo db. Please use `%s` instead."
+                    % (DEPRECATED_AQUEDUCT_DEMO_DB_NAME, AQUEDUCT_DEMO_DB_NAME)
+                )
+                name = AQUEDUCT_DEMO_DB_NAME
 
-        if name not in self._connected_integrations.keys():
+        if name not in connected_names:
             raise InvalidIntegrationException("Not connected to integration %s!" % name)
 
         integration_info = self._connected_integrations[name]
         if integration_info.service in RelationalDBServices:
             return RelationalDBResource(
                 dag=self._dag,
                 metadata=integration_info,
```

### Comparing `aqueduct-sdk-0.3.1/aqueduct/constants/enums.py` & `aqueduct-sdk-0.3.2/aqueduct/constants/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
     POSTGRES = "Postgres"
     SNOWFLAKE = "Snowflake"
     MYSQL = "MySQL"
     REDSHIFT = "Redshift"
     MARIADB = "MariaDB"
     SQLSERVER = "SQL Server"
     BIGQUERY = "BigQuery"
-    AQUEDUCTDEMO = "Aqueduct Demo"
     GITHUB = "Github"
     SALESFORCE = "Salesforce"
     GOOGLE_SHEETS = "Google Sheets"
     S3 = "S3"
     ATHENA = "Athena"
     SQLITE = "SQLite"
     AIRFLOW = "Airflow"
@@ -89,15 +88,14 @@
     POSTGRES = "Postgres"
     SNOWFLAKE = "Snowflake"
     MYSQL = "MySQL"
     REDSHIFT = "Redshift"
     MARIADB = "MariaDB"
     SQLSERVER = "SQL Server"
     BIGQUERY = "BigQuery"
-    AQUEDUCTDEMO = "Aqueduct Demo"
     SQLITE = "SQLite"
     ATHENA = "Athena"
 
 
 class ExecutionStatus(str, Enum, metaclass=MetaEnum):
     UNKNOWN = "unknown"
     SUCCEEDED = "succeeded"
```

### Comparing `aqueduct-sdk-0.3.1/aqueduct/decorator.py` & `aqueduct-sdk-0.3.2/aqueduct/decorator.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/error.py` & `aqueduct-sdk-0.3.2/aqueduct/error.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/flow.py` & `aqueduct-sdk-0.3.2/aqueduct/flow.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/flow_run.py` & `aqueduct-sdk-0.3.2/aqueduct/flow_run.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/github.py` & `aqueduct-sdk-0.3.2/aqueduct/github.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
             Assuming a github repo structure:
             ```
             /queries
                 hotels.sql
             ```
             Then to use it:
             ```
-            warehouse = aqueduct_client.resource(name="aqueduct_demo")
+            warehouse = aqueduct_client.resource(name="Demo")
             gh = aqueduct_client.github(repo=<repo_name>, branch=<branch_name>)
             reviews = warehouse.sql(
                 query=gh.query(path="queries/hotel.sql")
             )
             ```
         """
         repo_config_content_type = GithubRepoConfigContentType.QUERY if query_name else None
```

### Comparing `aqueduct-sdk-0.3.1/aqueduct/llm_wrapper.py` & `aqueduct-sdk-0.3.2/aqueduct/llm_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -126,75 +126,74 @@
     output_column_name: Optional[str] = None,
     engine: Optional[Union[str, DynamicK8sResource]] = None,
 ) -> Union[
     Callable[..., Union[BaseArtifact, List[BaseArtifact]]], BaseArtifact, List[BaseArtifact]
 ]:
     """Generates an Aqueduct operator to run a LLM. Either both column_name and output_column_name must be provided,
     or neither must be provided. Please refer to the `Returns` section below for their differences.
-
     Args:
         name:
             The name of the LLM to use. Please see aqueduct.supported_llms for a list of supported LLMs.
         op_name:
             The name of the operator. If not provided, defaults to the name of the LLM.
         column_name:
             The name of the column of the Dataframe to use as input to the LLM. If this field is provided,
             output_column_name must also be provided.
         output_column_name:
             The name of the column of the Dataframe to store the output of the LLM. If this field is provided,
             column_name must also be provided.
+
         engine:
-            The name of the compute integration this operator will run on. Defaults to the Aqueduct engine.
+            The name of the compute resource this operator will run on. Defaults to the Aqueduct engine.
             We recommend using a Kubernetes engine to run LLM operators, as we have implemented performance
             optimizations for LLMs on Kubernetes.
-
     Returns:
         If column_name and output_column_name are both provided, returns a function that takes in a
         DataFrame and returns a DataFrame with the output of the LLM appended as a new column:
-
-        def llm_for_table(df: pd.DataFrame, parameters: Dict[str, Any] = {}) -> pd.DataFrame:
-
+        ```python
+        def use_llm_for_table(df: pd.DataFrame, parameters: Dict[str, Any] = {}) -> pd.DataFrame:
+        ```
         Otherwise, returns a function that takes in a string or list of strings, applies LLM, and
         returns a string or list of strings:
-
+        ```python
         def use_llm(messages: Union[str, List[str]], parameters: Dict[str, Any] = {}) -> Union[str, List[str]]:
-
+        ```
         In both cases, the function takes in an optional second argument, which is a dictionary of
         parameters to pass to the LLM. Please refer to the documentation for the LLM you are using
         for a list of supported parameters. For all LLMs, we support the "prompt" parameter. If the
         prompt contains {text}, we will replace {text} with the input string(s) before sending to
         the LLM. If the prompt does not contain {text}, we will prepend the prompt to the input
         string(s) before sending to the LLM.
-
     Examples:
+        ```python
+        >>> from aqueduct import Client
+        >>> client = Client()
         >>> snowflake = client.resource("snowflake")
         >>> reviews_table = snowflake.sql("select * from hotel_reviews;")
-
         >>> from aqueduct import llm_op
-        ... vicuna_table_op = llm_op(
+        >>> vicuna_table_op = llm_op(
         ...     name="vicuna_7b",
         ...     op_name="my_vicuna_operator",
         ...     column_name="review",
         ...     output_column_name="response",
         ...     engine=ondemand_k8s,
-        >>> )
-        ... params = client.create_param(
+        ... )
+        >>> params = client.create_param(
         ...     "vicuna_params",
         ...     default={
         ...         "prompt": "Respond to the following hotel review as a customer service agent: {text} ",
         ...         "max_gpu_memory": "13GiB",
         ...         "temperature": 0.7,
         ...         "max_new_tokens": 512,
         ...     }
-        >>> )
+        ... )
         >>> review_with_response = vicuna_table_op(reviews_table, params)
-
         `review_with_response` is a Table Artifact with the output of the LLM appended as a new column.
-
         >>> review_with_response.get()
+        ```
     """
     if name not in supported_llms:
         raise InvalidUserArgumentException(f"Unsupported LLM model {name}")
 
     kwargs: Dict[str, Any] = {}
     if engine is not None:
         kwargs["engine"] = engine
```

### Comparing `aqueduct-sdk-0.3.1/aqueduct/models/artifact.py` & `aqueduct-sdk-0.3.2/aqueduct/models/artifact.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/models/config.py` & `aqueduct-sdk-0.3.2/aqueduct/models/config.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/models/dag.py` & `aqueduct-sdk-0.3.2/aqueduct/models/dag.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/models/dag_rules.py` & `aqueduct-sdk-0.3.2/aqueduct/models/dag_rules.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/models/execution_state.py` & `aqueduct-sdk-0.3.2/aqueduct/models/execution_state.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/models/integration.py` & `aqueduct-sdk-0.3.2/aqueduct/models/integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,14 @@
             ServiceType.POSTGRES,
             ServiceType.SNOWFLAKE,
             ServiceType.MYSQL,
             ServiceType.REDSHIFT,
             ServiceType.MARIADB,
             ServiceType.SQLSERVER,
             ServiceType.BIGQUERY,
-            ServiceType.AQUEDUCTDEMO,
             ServiceType.SQLITE,
             ServiceType.ATHENA,
         ]
 
 
 class BaseResource(ABC):
     """
```

### Comparing `aqueduct-sdk-0.3.1/aqueduct/models/operators.py` & `aqueduct-sdk-0.3.2/aqueduct/models/operators.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/models/response_models.py` & `aqueduct-sdk-0.3.2/aqueduct/models/response_models.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/resources/aws.py` & `aqueduct-sdk-0.3.2/aqueduct/resources/aws.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/resources/connect_config.py` & `aqueduct-sdk-0.3.2/aqueduct/resources/connect_config.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/resources/dynamic_k8s.py` & `aqueduct-sdk-0.3.2/aqueduct/resources/dynamic_k8s.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/resources/ecr.py` & `aqueduct-sdk-0.3.2/aqueduct/resources/ecr.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         """
         Returns a dictionary with the name of the ECR resource and the image URL, which can be
         used as input to the `image` field of an operator's decorator. This method also verifies
         that the image exists in the ECR repository.
 
         Args:
             image_name: The name of the image to retrieve. Should be in the form of `image:tag`.
-            No need to include the endpoint URL prefix such as 123456789012.dkr.ecr.us-east-1.amazonaws.com.
+            No need to include the endpoint URL prefix such as `123456789012.dkr.ecr.us-east-1.amazonaws.com`.
         """
         if len(image_name.split("/")) == 2:
             image_name = image_name.split("/")[1]
 
         if len(image_name.split(":")) != 2:
             if len(image_name.split(":")) == 1:
                 image_name = image_name + ":latest"
```

### Comparing `aqueduct-sdk-0.3.1/aqueduct/resources/google_sheets.py` & `aqueduct-sdk-0.3.2/aqueduct/resources/google_sheets.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/resources/mongodb.py` & `aqueduct-sdk-0.3.2/aqueduct/resources/mongodb.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/resources/parameters.py` & `aqueduct-sdk-0.3.2/aqueduct/resources/parameters.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/resources/s3.py` & `aqueduct-sdk-0.3.2/aqueduct/resources/s3.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/resources/salesforce.py` & `aqueduct-sdk-0.3.2/aqueduct/resources/salesforce.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/resources/save.py` & `aqueduct-sdk-0.3.2/aqueduct/resources/save.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/resources/sql.py` & `aqueduct-sdk-0.3.2/aqueduct/resources/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,14 @@
             # Use the list integration objects endpoint instead of
             # providing a hardcoded SQL query to execute
             tables = globals.__GLOBAL_API_CLIENT__.list_tables(str(self.id()))
             return pd.DataFrame(tables, columns=["tablename"])
 
         if self.type() in [
             ServiceType.POSTGRES,
-            ServiceType.AQUEDUCTDEMO,
             ServiceType.REDSHIFT,
         ]:
             list_tables_query = LIST_TABLES_QUERY_PG
         elif self.type() == ServiceType.MYSQL:
             list_tables_query = LIST_TABLES_QUERY_MYSQL
         elif self.type() == ServiceType.MARIADB:
             list_tables_query = LIST_TABLES_QUERY_MARIADB
```

### Comparing `aqueduct-sdk-0.3.1/aqueduct/resources/validation.py` & `aqueduct-sdk-0.3.2/aqueduct/resources/validation.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/schedule.py` & `aqueduct-sdk-0.3.2/aqueduct/schedule.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/tests/dag_delta_test.py` & `aqueduct-sdk-0.3.2/aqueduct/tests/dag_delta_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/tests/dag_test.py` & `aqueduct-sdk-0.3.2/aqueduct/tests/dag_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/tests/decorator_test.py` & `aqueduct-sdk-0.3.2/aqueduct/tests/decorator_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/tests/decorators_with_without_parentheses_test.py` & `aqueduct-sdk-0.3.2/aqueduct/tests/decorators_with_without_parentheses_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/tests/flow_test.py` & `aqueduct-sdk-0.3.2/aqueduct/tests/flow_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/tests/helpers_test.py` & `aqueduct-sdk-0.3.2/aqueduct/tests/helpers_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/tests/metric_test.py` & `aqueduct-sdk-0.3.2/aqueduct/tests/metric_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/tests/serialization_test.py` & `aqueduct-sdk-0.3.2/aqueduct/tests/serialization_test.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/tests/utils.py` & `aqueduct-sdk-0.3.2/aqueduct/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/utils/dag_deltas.py` & `aqueduct-sdk-0.3.2/aqueduct/utils/dag_deltas.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/utils/describe.py` & `aqueduct-sdk-0.3.2/aqueduct/utils/describe.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/utils/function_packaging.py` & `aqueduct-sdk-0.3.2/aqueduct/utils/function_packaging.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/utils/integration_validation.py` & `aqueduct-sdk-0.3.2/aqueduct/utils/integration_validation.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/utils/local_data.py` & `aqueduct-sdk-0.3.2/aqueduct/utils/local_data.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/utils/naming.py` & `aqueduct-sdk-0.3.2/aqueduct/utils/naming.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/utils/serialization.py` & `aqueduct-sdk-0.3.2/aqueduct/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/utils/type_inference.py` & `aqueduct-sdk-0.3.2/aqueduct/utils/type_inference.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct/utils/utils.py` & `aqueduct-sdk-0.3.2/aqueduct/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/aqueduct_sdk.egg-info/PKG-INFO` & `aqueduct-sdk-0.3.2/aqueduct_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-sdk
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python SDK for Aqueduct
 Home-page: https://github.com/aqueducthq/aqueduct
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `aqueduct-sdk-0.3.1/aqueduct_sdk.egg-info/SOURCES.txt` & `aqueduct-sdk-0.3.2/aqueduct_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aqueduct-sdk-0.3.1/setup.py` & `aqueduct-sdk-0.3.2/setup.py`

 * *Files identical despite different names*

