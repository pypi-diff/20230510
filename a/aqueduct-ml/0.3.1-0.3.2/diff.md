# Comparing `tmp/aqueduct-ml-0.3.1.tar.gz` & `tmp/aqueduct-ml-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqueduct-ml-0.3.1.tar", last modified: Thu May  4 10:51:42 2023, max compression
+gzip compressed data, was "aqueduct-ml-0.3.2.tar", last modified: Wed May 10 18:36:05 2023, max compression
```

## Comparing `aqueduct-ml-0.3.1.tar` & `aqueduct-ml-0.3.2.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:51:42.023181 aqueduct-ml-0.3.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7514 2023-05-04 10:51:42.023181 aqueduct-ml-0.3.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:51:41.995181 aqueduct-ml-0.3.1/aqueduct_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:51:41.995181 aqueduct-ml-0.3.1/aqueduct_executor/migrators/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/migrators/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:51:41.995181 aqueduct-ml-0.3.1/aqueduct_executor/migrators/artifact_migration_000016/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/migrators/artifact_migration_000016/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4538 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/migrators/artifact_migration_000016/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      441 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/migrators/artifact_migration_000016/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/migrators/artifact_migration_000016/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:51:41.995181 aqueduct-ml-0.3.1/aqueduct_executor/migrators/backfill_python_type_000022/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/migrators/backfill_python_type_000022/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      445 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/migrators/backfill_python_type_000022/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      437 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/migrators/backfill_python_type_000022/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:51:41.999181 aqueduct-ml-0.3.1/aqueduct_executor/migrators/parameter_val_type_inference_000019/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/migrators/parameter_val_type_inference_000019/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1039 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      598 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4168 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/migrators/parameter_val_type_inference_000019/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:51:41.999181 aqueduct-ml-0.3.1/aqueduct_executor/operators/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:51:41.999181 aqueduct-ml-0.3.1/aqueduct_executor/operators/airflow/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/airflow/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3010 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/airflow/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      405 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/airflow/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1122 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/airflow/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:51:41.999181 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:51:42.007181 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2680 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/athena.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      134 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/azure_sql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3297 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/bigquery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      694 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2892 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1829 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/connector.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15392 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6057 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/extract.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1462 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/gcs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      650 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/load.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      576 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/maria_db.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      825 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/models.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3821 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/mongodb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      798 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/mysql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1099 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/postgres.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      129 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/redshift.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4774 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/relational.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8690 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6878 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/s3_serialization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1808 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/snowflake.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:51:42.007181 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/spark/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/spark/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5385 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/spark/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2833 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/spark/snowflake.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5473 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/spec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1722 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/sql_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2434 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/sqlite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2728 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:51:42.011181 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2349 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/conf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      254 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/conftest.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1909 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/test_bigquery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1169 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/test_mariadb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/test_mysql.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/test_postgres.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/test_redshift.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/test_snowflake.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1173 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/test_sql_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1150 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/test_sqlite.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      925 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:51:42.015181 aqueduct-ml-0.3.1/aqueduct_executor/operators/function_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/function_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17252 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/function_executor/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2770 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/function_executor/extract_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      801 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/function_executor/get_extract_path.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3286 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/function_executor/install_requirements.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      594 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/function_executor/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1280 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/function_executor/set_conda_version.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1501 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/function_executor/spec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/function_executor/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:51:42.015181 aqueduct-ml-0.3.1/aqueduct_executor/operators/param_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/param_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3211 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/param_executor/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      419 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/param_executor/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/param_executor/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:51:42.015181 aqueduct-ml-0.3.1/aqueduct_executor/operators/spark/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/spark/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2683 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/spark/execute_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1020 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/spark/execute_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5401 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/spark/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:51:42.015181 aqueduct-ml-0.3.1/aqueduct_executor/operators/system_metric_executor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/system_metric_executor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2264 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/system_metric_executor/execute.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      435 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/system_metric_executor/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      837 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/system_metric_executor/spec.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:51:42.019181 aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2259 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/enums.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      465 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/exceptions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7531 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/execution.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/saved_object_delete.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:51:42.019181 aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/storage/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/storage/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      914 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/storage/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      948 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/storage/file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1354 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/storage/gcs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      720 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/storage/parse.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3780 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/storage/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      288 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/storage/storage.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      819 2023-02-07 07:49:15.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/timer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9254 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:51:42.019181 aqueduct-ml-0.3.1/aqueduct_ml.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7514 2023-05-04 10:51:41.000000 aqueduct-ml-0.3.1/aqueduct_ml.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5737 2023-05-04 10:51:41.000000 aqueduct-ml-0.3.1/aqueduct_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-04 10:51:41.000000 aqueduct-ml-0.3.1/aqueduct_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      248 2023-05-04 10:51:41.000000 aqueduct-ml-0.3.1/aqueduct_ml.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2023-05-04 10:51:41.000000 aqueduct-ml-0.3.1/aqueduct_ml.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 10:51:42.023181 aqueduct-ml-0.3.1/bin/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    29290 2023-05-04 10:16:31.000000 aqueduct-ml-0.3.1/bin/aqueduct
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2023-05-04 10:16:31.000000 aqueduct-ml-0.3.1/requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-04 10:51:42.023181 aqueduct-ml-0.3.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-05-04 10:16:29.000000 aqueduct-ml-0.3.1/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-05-04 10:16:31.000000 aqueduct-ml-0.3.1/version
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.923531 aqueduct-ml-0.3.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7514 2023-05-10 18:36:05.923531 aqueduct-ml-0.3.2/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.915531 aqueduct-ml-0.3.2/aqueduct_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.915531 aqueduct-ml-0.3.2/aqueduct_executor/migrators/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.915531 aqueduct-ml-0.3.2/aqueduct_executor/migrators/artifact_migration_000016/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/artifact_migration_000016/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4538 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/artifact_migration_000016/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      441 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/artifact_migration_000016/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      455 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/artifact_migration_000016/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.915531 aqueduct-ml-0.3.2/aqueduct_executor/migrators/backfill_python_type_000022/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/backfill_python_type_000022/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/backfill_python_type_000022/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      445 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/backfill_python_type_000022/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      437 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/backfill_python_type_000022/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.915531 aqueduct-ml-0.3.2/aqueduct_executor/migrators/parameter_val_type_inference_000019/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/parameter_val_type_inference_000019/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1039 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      598 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4168 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/migrators/parameter_val_type_inference_000019/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.915531 aqueduct-ml-0.3.2/aqueduct_executor/operators/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.915531 aqueduct-ml-0.3.2/aqueduct_executor/operators/airflow/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/airflow/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3010 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/airflow/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      405 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/airflow/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1122 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/airflow/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.915531 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.919531 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2680 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/athena.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      134 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/azure_sql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3297 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/bigquery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      658 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2892 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1829 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/connector.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15345 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6057 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/extract.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1462 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/gcs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      650 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/load.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      576 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      119 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/maria_db.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/models.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3821 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/mongodb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      798 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/mysql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1099 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/postgres.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      129 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/redshift.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4774 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/relational.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8690 2023-05-09 23:16:09.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6878 2023-05-09 23:16:09.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/s3_serialization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1808 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/snowflake.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.919531 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/spark/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/spark/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5385 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/spark/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2833 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/spark/snowflake.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5464 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/spec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1722 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/sql_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2434 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/sqlite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2728 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.919531 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2349 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/conf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      254 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/conftest.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1909 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_bigquery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1169 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_mariadb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_mysql.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_postgres.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1176 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_redshift.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_snowflake.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1173 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_sql_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1150 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_sqlite.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      925 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.919531 aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17252 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2770 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/extract_function.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      801 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/get_extract_path.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3286 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/install_requirements.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      594 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1280 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/set_conda_version.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1501 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/spec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.923531 aqueduct-ml-0.3.2/aqueduct_executor/operators/param_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/param_executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3211 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/param_executor/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      419 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/param_executor/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/param_executor/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.923531 aqueduct-ml-0.3.2/aqueduct_executor/operators/spark/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/spark/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2683 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/spark/execute_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1020 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/spark/execute_function.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5401 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/spark/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.923531 aqueduct-ml-0.3.2/aqueduct_executor/operators/system_metric_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/system_metric_executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2264 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/system_metric_executor/execute.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      435 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/system_metric_executor/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      837 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/system_metric_executor/spec.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.923531 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2259 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/enums.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      465 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/exceptions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7531 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/execution.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/saved_object_delete.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.923531 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      914 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      948 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1354 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/gcs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      720 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/parse.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3780 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      288 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/storage.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      819 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/timer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9254 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.923531 aqueduct-ml-0.3.2/aqueduct_ml.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7514 2023-05-10 18:36:05.000000 aqueduct-ml-0.3.2/aqueduct_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5737 2023-05-10 18:36:05.000000 aqueduct-ml-0.3.2/aqueduct_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-10 18:36:05.000000 aqueduct-ml-0.3.2/aqueduct_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      248 2023-05-10 18:36:05.000000 aqueduct-ml-0.3.2/aqueduct_ml.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2023-05-10 18:36:05.000000 aqueduct-ml-0.3.2/aqueduct_ml.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-10 18:36:05.923531 aqueduct-ml-0.3.2/bin/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    29290 2023-05-09 23:19:59.000000 aqueduct-ml-0.3.2/bin/aqueduct
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2023-05-09 23:19:59.000000 aqueduct-ml-0.3.2/requirements.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-10 18:36:05.923531 aqueduct-ml-0.3.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-05-09 23:15:33.000000 aqueduct-ml-0.3.2/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-05-09 23:19:59.000000 aqueduct-ml-0.3.2/version
```

### Comparing `aqueduct-ml-0.3.1/PKG-INFO` & `aqueduct-ml-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-ml
-Version: 0.3.1
+Version: 0.3.2
 Summary: The control center for ML in the cloud
 Home-page: https://www.aqueducthq.com/
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/migrators/artifact_migration_000016/execute.py` & `aqueduct-ml-0.3.2/aqueduct_executor/migrators/artifact_migration_000016/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/migrators/backfill_python_type_000022/execute.py` & `aqueduct-ml-0.3.2/aqueduct_executor/migrators/backfill_python_type_000022/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py` & `aqueduct-ml-0.3.2/aqueduct_executor/migrators/backfill_python_type_000022/serialize.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py` & `aqueduct-ml-0.3.2/aqueduct_executor/migrators/parameter_val_type_inference_000019/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py` & `aqueduct-ml-0.3.2/aqueduct_executor/migrators/parameter_val_type_inference_000019/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py` & `aqueduct-ml-0.3.2/aqueduct_executor/migrators/parameter_val_type_inference_000019/serialize.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/airflow/execute.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/airflow/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/airflow/spec.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/airflow/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/athena.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/athena.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/bigquery.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/bigquery.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/common.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     SQL_SERVER = "SQL Server"
     MYSQL = "MySQL"
     MARIA_DB = "MariaDB"
     AZURE_SQL = "AzureSQL"
     S3 = "S3"
     ATHENA = "Athena"
     SQLITE = "SQLite"
-    AQUEDUCT_DEMO = "Aqueduct Demo"
     GCS = "GCS"
     MONGO_DB = "MongoDB"
 
 
 class UpdateMode(Enum, metaclass=enums.MetaEnum):
     APPEND = "append"
     REPLACE = "replace"
```

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/config.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/config.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/connector.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/connector.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/execute.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,15 @@
 
 
 def setup_connector(
     connector_name: common.Name, connector_config: config.Config
 ) -> connector.DataConnector:
     # prevent isort from moving around type: ignore comments which will cause mypy issues.
     # isort: off
-    if connector_name == common.Name.AQUEDUCT_DEMO or connector_name == common.Name.POSTGRES:
+    if connector_name == common.Name.POSTGRES:
         try:
             import psycopg2
         except:
             raise MissingConnectorDependencyException(
                 "Unable to initialize the Postgres connector. Have you run `aqueduct install postgres`?"
             )
```

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/extract.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/extract.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/gcs.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/gcs.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/load.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/load.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/main.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/models.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 from pydantic import BaseModel, Extra
 
 
 class BaseSpec(BaseModel):
     """
     BaseSpec defines the Pydantic Config shared by all connector Spec's, e.g.
     AuthenticateSpec, ExtractSpec, etc.
@@ -14,14 +16,16 @@
 
 class BaseConfig(BaseModel):
     """
     BaseConfig defines the Pydantic Config shared by all connector Config's, e.g.
     postgres.Config, mysql.Config, etc.
     """
 
+    exec_state: Optional[str]
+
     class Config:
         extra = Extra.forbid
 
 
 class BaseParams(BaseModel):
     """
     BaseParams defines the Pydantic Config shared by all ExtractParams and LoadParams, e.g.
```

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/mongodb.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/mongodb.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/mysql.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/mysql.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/postgres.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/postgres.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/relational.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/relational.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/s3.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/s3.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/s3_serialization.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/s3_serialization.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/snowflake.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/snowflake.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/spark/s3.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/spark/s3.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/spark/snowflake.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/spark/snowflake.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/spec.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import json
 
 from aqueduct_executor.operators.connectors.data import common, config, extract, load, models
 from aqueduct_executor.operators.utils import enums
 from aqueduct_executor.operators.utils.storage import config as sconfig
 from pydantic import parse_obj_as, validator
 
-AQUEDUCT_DEMO_NAME = "aqueduct_demo"
+AQUEDUCT_DEMO_NAME = "Demo"
 
 
 def unwrap_connector_config(cls, connector_config, values):  # type: ignore
     """
     TODO ENG-937: Remove this validator once connector config serialization is fixed.
 
     Unwraps the connector config before it can be parsed into a
```

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/sql_server.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/sql_server.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/sqlite.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/sqlite.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/data/utils.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/data/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/conf.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/conf.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/test_bigquery.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/test_mariadb.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_mariadb.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/test_mysql.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_mysql.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/test_postgres.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_postgres.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/test_redshift.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_redshift.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/test_snowflake.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_snowflake.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/test_sql_server.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_sql_server.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/test_sqlite.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/connectors/tests/utils.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/connectors/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/function_executor/execute.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/function_executor/extract_function.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/extract_function.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/function_executor/get_extract_path.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/get_extract_path.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/function_executor/install_requirements.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/install_requirements.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/function_executor/main.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/main.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/function_executor/set_conda_version.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/set_conda_version.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/function_executor/spec.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/function_executor/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/param_executor/execute.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/param_executor/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/param_executor/spec.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/param_executor/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/spark/execute_data.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/spark/execute_data.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/spark/execute_function.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/spark/execute_function.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/spark/utils.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/spark/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/system_metric_executor/execute.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/system_metric_executor/execute.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/system_metric_executor/spec.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/system_metric_executor/spec.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/enums.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/enums.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/execution.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/execution.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/storage/config.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/config.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/storage/file.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/file.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/storage/gcs.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/storage/parse.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/parse.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/storage/s3.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/storage/s3.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/timer.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/timer.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_executor/operators/utils/utils.py` & `aqueduct-ml-0.3.2/aqueduct_executor/operators/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/aqueduct_ml.egg-info/PKG-INFO` & `aqueduct-ml-0.3.2/aqueduct_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqueduct-ml
-Version: 0.3.1
+Version: 0.3.2
 Summary: The control center for ML in the cloud
 Home-page: https://www.aqueducthq.com/
 Author: Aqueduct, Inc.
 Author-email: hello@aqueducthq.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `aqueduct-ml-0.3.1/aqueduct_ml.egg-info/SOURCES.txt` & `aqueduct-ml-0.3.2/aqueduct_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aqueduct-ml-0.3.1/bin/aqueduct` & `aqueduct-ml-0.3.2/bin/aqueduct`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 MYSQL_CLIENT_VERSION_BOUND = "<=2.1.1"
 PYODBC_VERSION_BOUND = "<=4.0.35"
 
 base_directory = os.path.join(os.environ["HOME"], ".aqueduct")
 server_directory = os.path.join(os.environ["HOME"], ".aqueduct", "server")
 ui_directory = os.path.join(os.environ["HOME"], ".aqueduct", "ui")
 
-package_version = "0.3.1"
+package_version = "0.3.2"
 aws_credentials_path = os.path.join(os.environ["HOME"], ".aws", "credentials")
 
 default_server_port = 8080
 
 s3_server_prefix = (
     "https://aqueduct-ai.s3.us-east-2.amazonaws.com/assets/%s/server" % package_version
 )
```

### Comparing `aqueduct-ml-0.3.1/setup.py` & `aqueduct-ml-0.3.2/setup.py`

 * *Files identical despite different names*

