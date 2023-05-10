# Comparing `tmp/mlfoundry-0.7.9.tar.gz` & `tmp/mlfoundry-0.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlfoundry-0.7.9.tar", max compression
+gzip compressed data, was "mlfoundry-0.8.0rc1.tar", max compression
```

## Comparing `mlfoundry-0.7.9.tar` & `mlfoundry-0.8.0rc1.tar`

### file list

```diff
@@ -1,113 +1,113 @@
--rw-r--r--   0        0        0     3158 2023-04-26 11:54:04.850183 mlfoundry-0.7.9/README.md
--rw-r--r--   0        0        0      991 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/__init__.py
--rw-r--r--   0        0        0     1211 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/__main__.py
--rw-r--r--   0        0        0     3713 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/amplitude.py
--rw-r--r--   0        0        0        0 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/artifact/__init__.py
--rw-r--r--   0        0        0     7069 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/artifact/truefoundry_artifact_repo.py
--rw-r--r--   0        0        0        0 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/background/__init__.py
--rw-r--r--   0        0        0      287 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/background/events.py
--rw-r--r--   0        0        0     3032 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/background/interface.py
--rw-r--r--   0        0        0     4016 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/background/sender.py
--rw-r--r--   0        0        0     8756 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/background/system_metrics.py
--rw-r--r--   0        0        0     4028 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/background/utils.py
--rw-r--r--   0        0        0        0 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/cli/__init__.py
--rw-r--r--   0        0        0      918 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/cli/cli_interface.py
--rw-r--r--   0        0        0      100 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/cli/commands/__init__.py
--rw-r--r--   0        0        0      731 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/cli/commands/download.py
--rw-r--r--   0        0        0      739 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/cli/commands/login.py
--rw-r--r--   0        0        0     2724 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/constants.py
--rw-r--r--   0        0        0      103 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/dataset/__init__.py
--rw-r--r--   0        0        0     7854 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/dataset/dataset.py
--rw-r--r--   0        0        0     2255 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/dataset/schema.py
--rw-r--r--   0        0        0    13138 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/dataset/serde.py
--rw-r--r--   0        0        0     2028 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/dataset/serde_utils.py
--rw-r--r--   0        0        0     2078 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/dataset/stats.py
--rw-r--r--   0        0        0     1903 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/dataset/types.py
--rw-r--r--   0        0        0     2588 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/dataset/validation.py
--rw-r--r--   0        0        0       69 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/dataset/whylogs_types/__init__.py
--rw-r--r--   0        0        0     4025 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/dataset/whylogs_types/summary.py
--rw-r--r--   0        0        0     1358 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/enums.py
--rw-r--r--   0        0        0      325 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/env_vars.py
--rw-r--r--   0        0        0      365 2023-04-26 11:54:04.866184 mlfoundry-0.7.9/mlfoundry/exceptions.py
--rw-r--r--   0        0        0     1906 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/__init__.py
--rw-r--r--   0        0        0      301 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/base_registry.py
--rw-r--r--   0        0        0      718 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/fastai_registry.py
--rw-r--r--   0        0        0      892 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/gluon_registry.py
--rw-r--r--   0        0        0      700 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/h2o_registry.py
--rw-r--r--   0        0        0      712 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/keras_registry.py
--rw-r--r--   0        0        0      730 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/lightgbm_registry.py
--rw-r--r--   0        0        0      706 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/onnx_registry.py
--rw-r--r--   0        0        0      775 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/paddle_registry.py
--rw-r--r--   0        0        0      744 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/pytorch_registry.py
--rw-r--r--   0        0        0      724 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/sklearn_registry.py
--rw-r--r--   0        0        0      712 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/spacy_registry.py
--rw-r--r--   0        0        0      748 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/statsmodel_registry.py
--rw-r--r--   0        0        0     3077 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/tensorflow_registry.py
--rw-r--r--   0        0        0      724 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/frameworks/xgboost_registry.py
--rw-r--r--   0        0        0     2349 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/git_info.py
--rw-r--r--   0        0        0        0 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/integrations/__init__.py
--rw-r--r--   0        0        0    15215 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/integrations/lightning.py
--rw-r--r--   0        0        0    22189 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/integrations/transformers.py
--rw-r--r--   0        0        0     1785 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/internal_namespace.py
--rw-r--r--   0        0        0      571 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/__init__.py
--rw-r--r--   0        0        0     7521 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/artifacts/artifact.py
--rw-r--r--   0        0        0     1019 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/artifacts/constants.py
--rw-r--r--   0        0        0     2871 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/artifacts/general_artifact.py
--rw-r--r--   0        0        0    14349 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/artifacts/model.py
--rw-r--r--   0        0        0     5983 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/artifacts/utils.py
--rw-r--r--   0        0        0     1281 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/dataset_artifact.py
--rw-r--r--   0        0        0      222 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/dataset_schema.py
--rw-r--r--   0        0        0      318 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/dataset_stats.py
--rw-r--r--   0        0        0       50 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/image/__init__.py
--rw-r--r--   0        0        0      255 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/image/constants.py
--rw-r--r--   0        0        0    11446 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/image/image.py
--rw-r--r--   0        0        0     2767 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/image/image_normalizer.py
--rw-r--r--   0        0        0     1566 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/image/types.py
--rw-r--r--   0        0        0      271 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/model_artifact.py
--rw-r--r--   0        0        0     7125 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/plot.py
--rw-r--r--   0        0        0     2486 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/pydantic_base.py
--rw-r--r--   0        0        0     1332 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/log_types/utils.py
--rw-r--r--   0        0        0      453 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/logger.py
--rw-r--r--   0        0        0     9286 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/login.py
--rw-r--r--   0        0        0        0 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/__init__.py
--rw-r--r--   0        0        0     1065 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v1/__init__.py
--rw-r--r--   0        0        0     2080 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v1/base_metrics.py
--rw-r--r--   0        0        0     6852 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v1/binary_classification_metrics.py
--rw-r--r--   0        0        0     6736 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v1/multiclass_classification_metrics.py
--rw-r--r--   0        0        0     4419 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v1/regression_metrics.py
--rw-r--r--   0        0        0     3976 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v1/timeseries_metrics.py
--rw-r--r--   0        0        0     1026 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v2/__init__.py
--rw-r--r--   0        0        0     1898 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v2/base_metrics.py
--rw-r--r--   0        0        0      566 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v2/custom_metric_types.py
--rw-r--r--   0        0        0     6192 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v2/multiclass_classification_metrics.py
--rw-r--r--   0        0        0     2718 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v2/regression_metrics.py
--rw-r--r--   0        0        0     2251 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v2/timeseries_metrics.py
--rw-r--r--   0        0        0      295 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/metrics/v2/utils.py
--rw-r--r--   0        0        0    30890 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/mlfoundry_api.py
--rw-r--r--   0        0        0    46245 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/mlfoundry_run.py
--rw-r--r--   0        0        0        0 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/monitoring/__init__.py
--rw-r--r--   0        0        0     1994 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/monitoring/entities.py
--rw-r--r--   0        0        0       63 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/monitoring/store/__init__.py
--rw-r--r--   0        0        0     6630 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/monitoring/store/client.py
--rw-r--r--   0        0        0      169 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/monitoring/store/constants.py
--rw-r--r--   0        0        0      336 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/monitoring/store/repositories/__init__.py
--rw-r--r--   0        0        0     1351 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/monitoring/store/repositories/dto.py
--rw-r--r--   0        0        0     6529 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py
--rw-r--r--   0        0        0     2178 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/monitoring/store/worker.py
--rw-r--r--   0        0        0     4304 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/run_utils.py
--rw-r--r--   0        0        0      492 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/schema.py
--rw-r--r--   0        0        0     9979 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/session.py
--rw-r--r--   0        0        0        0 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/tracking/__init__.py
--rw-r--r--   0        0        0     2766 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/tracking/auth_service.py
--rw-r--r--   0        0        0     2629 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/tracking/entities.py
--rw-r--r--   0        0        0     1175 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/tracking/servicefoundry_service.py
--rw-r--r--   0        0        0     4308 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/tracking/truefoundry_rest_store.py
--rw-r--r--   0        0        0        0 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/vendor/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/vendor/pynvml/__init__.py
--rw-r--r--   0        0        0    56147 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/vendor/pynvml/pynvml.py
--rw-r--r--   0        0        0      253 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/version.py
--rw-r--r--   0        0        0        0 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/webapp/__init__.py
--rw-r--r--   0        0        0       38 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/webapp/inputs.py
--rw-r--r--   0        0        0       39 2023-04-26 11:54:04.870184 mlfoundry-0.7.9/mlfoundry/webapp/outputs.py
--rw-r--r--   0        0        0     3549 2023-04-26 11:54:16.574302 mlfoundry-0.7.9/pyproject.toml
--rw-r--r--   0        0        0     4925 1970-01-01 00:00:00.000000 mlfoundry-0.7.9/PKG-INFO
+-rw-r--r--   0        0        0     3158 2023-05-10 17:03:51.918163 mlfoundry-0.8.0rc1/README.md
+-rw-r--r--   0        0        0      991 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/__init__.py
+-rw-r--r--   0        0        0     1211 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/__main__.py
+-rw-r--r--   0        0        0     3713 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/amplitude.py
+-rw-r--r--   0        0        0        0 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/artifact/__init__.py
+-rw-r--r--   0        0        0     7069 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/artifact/truefoundry_artifact_repo.py
+-rw-r--r--   0        0        0        0 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/background/__init__.py
+-rw-r--r--   0        0        0      287 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/background/events.py
+-rw-r--r--   0        0        0     3032 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/background/interface.py
+-rw-r--r--   0        0        0     4016 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/background/sender.py
+-rw-r--r--   0        0        0     8756 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/background/system_metrics.py
+-rw-r--r--   0        0        0     4028 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/background/utils.py
+-rw-r--r--   0        0        0        0 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/cli/__init__.py
+-rw-r--r--   0        0        0      918 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/cli/cli_interface.py
+-rw-r--r--   0        0        0      100 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/cli/commands/__init__.py
+-rw-r--r--   0        0        0      731 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/cli/commands/download.py
+-rw-r--r--   0        0        0      739 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/cli/commands/login.py
+-rw-r--r--   0        0        0     2724 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/constants.py
+-rw-r--r--   0        0        0      103 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/dataset/__init__.py
+-rw-r--r--   0        0        0     7854 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/dataset/dataset.py
+-rw-r--r--   0        0        0     2255 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/dataset/schema.py
+-rw-r--r--   0        0        0    13138 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/dataset/serde.py
+-rw-r--r--   0        0        0     2028 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/dataset/serde_utils.py
+-rw-r--r--   0        0        0     2078 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/dataset/stats.py
+-rw-r--r--   0        0        0     1903 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/dataset/types.py
+-rw-r--r--   0        0        0     2588 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/dataset/validation.py
+-rw-r--r--   0        0        0       69 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/dataset/whylogs_types/__init__.py
+-rw-r--r--   0        0        0     4025 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/dataset/whylogs_types/summary.py
+-rw-r--r--   0        0        0     1358 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/enums.py
+-rw-r--r--   0        0        0      325 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/env_vars.py
+-rw-r--r--   0        0        0      365 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/exceptions.py
+-rw-r--r--   0        0        0     1906 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/frameworks/__init__.py
+-rw-r--r--   0        0        0      301 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/frameworks/base_registry.py
+-rw-r--r--   0        0        0      718 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/frameworks/fastai_registry.py
+-rw-r--r--   0        0        0      892 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/frameworks/gluon_registry.py
+-rw-r--r--   0        0        0      700 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/frameworks/h2o_registry.py
+-rw-r--r--   0        0        0      712 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/frameworks/keras_registry.py
+-rw-r--r--   0        0        0      730 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/frameworks/lightgbm_registry.py
+-rw-r--r--   0        0        0      706 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/frameworks/onnx_registry.py
+-rw-r--r--   0        0        0      775 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/frameworks/paddle_registry.py
+-rw-r--r--   0        0        0      744 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/frameworks/pytorch_registry.py
+-rw-r--r--   0        0        0      724 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/frameworks/sklearn_registry.py
+-rw-r--r--   0        0        0      712 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/frameworks/spacy_registry.py
+-rw-r--r--   0        0        0      748 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/frameworks/statsmodel_registry.py
+-rw-r--r--   0        0        0     3077 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/frameworks/tensorflow_registry.py
+-rw-r--r--   0        0        0      724 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/frameworks/xgboost_registry.py
+-rw-r--r--   0        0        0     2349 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/git_info.py
+-rw-r--r--   0        0        0        0 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/integrations/__init__.py
+-rw-r--r--   0        0        0    15399 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/integrations/lightning.py
+-rw-r--r--   0        0        0    22386 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/integrations/transformers.py
+-rw-r--r--   0        0        0     1785 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/internal_namespace.py
+-rw-r--r--   0        0        0      571 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/log_types/__init__.py
+-rw-r--r--   0        0        0     7978 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/log_types/artifacts/artifact.py
+-rw-r--r--   0        0        0     1019 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/log_types/artifacts/constants.py
+-rw-r--r--   0        0        0     3068 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/log_types/artifacts/general_artifact.py
+-rw-r--r--   0        0        0    14875 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/log_types/artifacts/model.py
+-rw-r--r--   0        0        0     5983 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/log_types/artifacts/utils.py
+-rw-r--r--   0        0        0     1281 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/log_types/dataset_artifact.py
+-rw-r--r--   0        0        0      222 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/log_types/dataset_schema.py
+-rw-r--r--   0        0        0      318 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/log_types/dataset_stats.py
+-rw-r--r--   0        0        0       50 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/log_types/image/__init__.py
+-rw-r--r--   0        0        0      255 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/log_types/image/constants.py
+-rw-r--r--   0        0        0    11446 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/log_types/image/image.py
+-rw-r--r--   0        0        0     2767 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/log_types/image/image_normalizer.py
+-rw-r--r--   0        0        0     1566 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/log_types/image/types.py
+-rw-r--r--   0        0        0      271 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/log_types/model_artifact.py
+-rw-r--r--   0        0        0     7125 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/log_types/plot.py
+-rw-r--r--   0        0        0     2486 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/log_types/pydantic_base.py
+-rw-r--r--   0        0        0     1332 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/log_types/utils.py
+-rw-r--r--   0        0        0      453 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/logger.py
+-rw-r--r--   0        0        0     9286 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/login.py
+-rw-r--r--   0        0        0        0 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/metrics/__init__.py
+-rw-r--r--   0        0        0     1065 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/metrics/v1/__init__.py
+-rw-r--r--   0        0        0     2080 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/metrics/v1/base_metrics.py
+-rw-r--r--   0        0        0     6852 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/metrics/v1/binary_classification_metrics.py
+-rw-r--r--   0        0        0     6736 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/metrics/v1/multiclass_classification_metrics.py
+-rw-r--r--   0        0        0     4419 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/metrics/v1/regression_metrics.py
+-rw-r--r--   0        0        0     3976 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/metrics/v1/timeseries_metrics.py
+-rw-r--r--   0        0        0     1026 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/metrics/v2/__init__.py
+-rw-r--r--   0        0        0     1898 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/metrics/v2/base_metrics.py
+-rw-r--r--   0        0        0      566 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/metrics/v2/custom_metric_types.py
+-rw-r--r--   0        0        0     6192 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/metrics/v2/multiclass_classification_metrics.py
+-rw-r--r--   0        0        0     2718 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/metrics/v2/regression_metrics.py
+-rw-r--r--   0        0        0     2251 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/metrics/v2/timeseries_metrics.py
+-rw-r--r--   0        0        0      295 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/metrics/v2/utils.py
+-rw-r--r--   0        0        0    42544 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/mlfoundry_api.py
+-rw-r--r--   0        0        0    46176 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/mlfoundry_run.py
+-rw-r--r--   0        0        0        0 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/monitoring/__init__.py
+-rw-r--r--   0        0        0     1994 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/monitoring/entities.py
+-rw-r--r--   0        0        0       63 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/monitoring/store/__init__.py
+-rw-r--r--   0        0        0     6630 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/monitoring/store/client.py
+-rw-r--r--   0        0        0      169 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/monitoring/store/constants.py
+-rw-r--r--   0        0        0      336 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/monitoring/store/repositories/__init__.py
+-rw-r--r--   0        0        0     1351 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/monitoring/store/repositories/dto.py
+-rw-r--r--   0        0        0     6529 2023-05-10 17:03:51.934163 mlfoundry-0.8.0rc1/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py
+-rw-r--r--   0        0        0     2178 2023-05-10 17:03:51.938163 mlfoundry-0.8.0rc1/mlfoundry/monitoring/store/worker.py
+-rw-r--r--   0        0        0     4304 2023-05-10 17:03:51.938163 mlfoundry-0.8.0rc1/mlfoundry/run_utils.py
+-rw-r--r--   0        0        0      492 2023-05-10 17:03:51.938163 mlfoundry-0.8.0rc1/mlfoundry/schema.py
+-rw-r--r--   0        0        0    10031 2023-05-10 17:03:51.938163 mlfoundry-0.8.0rc1/mlfoundry/session.py
+-rw-r--r--   0        0        0        0 2023-05-10 17:03:51.938163 mlfoundry-0.8.0rc1/mlfoundry/tracking/__init__.py
+-rw-r--r--   0        0        0     2766 2023-05-10 17:03:51.938163 mlfoundry-0.8.0rc1/mlfoundry/tracking/auth_service.py
+-rw-r--r--   0        0        0     2629 2023-05-10 17:03:51.938163 mlfoundry-0.8.0rc1/mlfoundry/tracking/entities.py
+-rw-r--r--   0        0        0     1175 2023-05-10 17:03:51.938163 mlfoundry-0.8.0rc1/mlfoundry/tracking/servicefoundry_service.py
+-rw-r--r--   0        0        0     4308 2023-05-10 17:03:51.938163 mlfoundry-0.8.0rc1/mlfoundry/tracking/truefoundry_rest_store.py
+-rw-r--r--   0        0        0        0 2023-05-10 17:03:51.938163 mlfoundry-0.8.0rc1/mlfoundry/vendor/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 17:03:51.938163 mlfoundry-0.8.0rc1/mlfoundry/vendor/pynvml/__init__.py
+-rw-r--r--   0        0        0    56147 2023-05-10 17:03:51.938163 mlfoundry-0.8.0rc1/mlfoundry/vendor/pynvml/pynvml.py
+-rw-r--r--   0        0        0      253 2023-05-10 17:03:51.938163 mlfoundry-0.8.0rc1/mlfoundry/version.py
+-rw-r--r--   0        0        0        0 2023-05-10 17:03:51.938163 mlfoundry-0.8.0rc1/mlfoundry/webapp/__init__.py
+-rw-r--r--   0        0        0       38 2023-05-10 17:03:51.938163 mlfoundry-0.8.0rc1/mlfoundry/webapp/inputs.py
+-rw-r--r--   0        0        0       39 2023-05-10 17:03:51.938163 mlfoundry-0.8.0rc1/mlfoundry/webapp/outputs.py
+-rw-r--r--   0        0        0     3552 2023-05-10 17:04:06.266286 mlfoundry-0.8.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     4928 1970-01-01 00:00:00.000000 mlfoundry-0.8.0rc1/PKG-INFO
```

### Comparing `mlfoundry-0.7.9/README.md` & `mlfoundry-0.8.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/__init__.py` & `mlfoundry-0.8.0rc1/mlfoundry/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/__main__.py` & `mlfoundry-0.8.0rc1/mlfoundry/__main__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/amplitude.py` & `mlfoundry-0.8.0rc1/mlfoundry/amplitude.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/artifact/truefoundry_artifact_repo.py` & `mlfoundry-0.8.0rc1/mlfoundry/artifact/truefoundry_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/background/interface.py` & `mlfoundry-0.8.0rc1/mlfoundry/background/interface.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/background/sender.py` & `mlfoundry-0.8.0rc1/mlfoundry/background/sender.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/background/system_metrics.py` & `mlfoundry-0.8.0rc1/mlfoundry/background/system_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/background/utils.py` & `mlfoundry-0.8.0rc1/mlfoundry/background/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/cli/cli_interface.py` & `mlfoundry-0.8.0rc1/mlfoundry/cli/cli_interface.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/cli/commands/download.py` & `mlfoundry-0.8.0rc1/mlfoundry/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/cli/commands/login.py` & `mlfoundry-0.8.0rc1/mlfoundry/cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/constants.py` & `mlfoundry-0.8.0rc1/mlfoundry/constants.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/dataset/dataset.py` & `mlfoundry-0.8.0rc1/mlfoundry/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/dataset/schema.py` & `mlfoundry-0.8.0rc1/mlfoundry/dataset/schema.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/dataset/serde.py` & `mlfoundry-0.8.0rc1/mlfoundry/dataset/serde.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/dataset/serde_utils.py` & `mlfoundry-0.8.0rc1/mlfoundry/dataset/serde_utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/dataset/stats.py` & `mlfoundry-0.8.0rc1/mlfoundry/dataset/stats.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/dataset/types.py` & `mlfoundry-0.8.0rc1/mlfoundry/dataset/types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/dataset/validation.py` & `mlfoundry-0.8.0rc1/mlfoundry/dataset/validation.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/dataset/whylogs_types/summary.py` & `mlfoundry-0.8.0rc1/mlfoundry/dataset/whylogs_types/summary.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/enums.py` & `mlfoundry-0.8.0rc1/mlfoundry/enums.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/frameworks/__init__.py` & `mlfoundry-0.8.0rc1/mlfoundry/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/frameworks/fastai_registry.py` & `mlfoundry-0.8.0rc1/mlfoundry/frameworks/fastai_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/frameworks/gluon_registry.py` & `mlfoundry-0.8.0rc1/mlfoundry/frameworks/gluon_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/frameworks/h2o_registry.py` & `mlfoundry-0.8.0rc1/mlfoundry/frameworks/h2o_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/frameworks/keras_registry.py` & `mlfoundry-0.8.0rc1/mlfoundry/frameworks/keras_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/frameworks/lightgbm_registry.py` & `mlfoundry-0.8.0rc1/mlfoundry/frameworks/lightgbm_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/frameworks/onnx_registry.py` & `mlfoundry-0.8.0rc1/mlfoundry/frameworks/onnx_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/frameworks/paddle_registry.py` & `mlfoundry-0.8.0rc1/mlfoundry/frameworks/paddle_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/frameworks/pytorch_registry.py` & `mlfoundry-0.8.0rc1/mlfoundry/frameworks/pytorch_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/frameworks/sklearn_registry.py` & `mlfoundry-0.8.0rc1/mlfoundry/frameworks/sklearn_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/frameworks/spacy_registry.py` & `mlfoundry-0.8.0rc1/mlfoundry/frameworks/spacy_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/frameworks/statsmodel_registry.py` & `mlfoundry-0.8.0rc1/mlfoundry/frameworks/statsmodel_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/frameworks/tensorflow_registry.py` & `mlfoundry-0.8.0rc1/mlfoundry/frameworks/tensorflow_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/frameworks/xgboost_registry.py` & `mlfoundry-0.8.0rc1/mlfoundry/frameworks/xgboost_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/git_info.py` & `mlfoundry-0.8.0rc1/mlfoundry/git_info.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/integrations/lightning.py` & `mlfoundry-0.8.0rc1/mlfoundry/integrations/lightning.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 from pytorch_lightning.utilities.distributed import rank_zero_only
 from pytorch_lightning.utilities.logger import (
     _add_prefix,
     _convert_params,
     _sanitize_callable_params,
 )
 
-import mlfoundry as mlf
+import mlfoundry
 from mlfoundry.enums import EnumMissingMixin
 from mlfoundry.logger import logger
+from mlfoundry.mlfoundry_api import resolve_ml_repo_name
 from mlfoundry.mlfoundry_run import MlFoundryRun
 
 LIGHTNING_ARTIFACTS_PATH = "lightning/"
 LIGHTNING_MODELS_PATH = os.path.join(LIGHTNING_ARTIFACTS_PATH, "models")
 
 
 class LogModelStrategy(EnumMissingMixin, enum.Enum):
@@ -41,16 +42,16 @@
 class MlFoundryLightningLogger(LightningLoggerBase):
     """
     Pytorch Lightning Logger for tracking training run on MLFoundry
 
     Examples:
 
         ```
-        import mlfoundry as mlf
-        mlf.login()
+        import mlfoundry
+        mlfoundry.login()
         # or set API key via `TFY_API_KEY` env variable
 
         from pytorch_lightning import Trainer
         from pytorch_lightning.callbacks import ModelCheckpoint
         from mlfoundry.integrations.lightning import MlFoundryLightningLogger, LogModelStrategy
 
         mlf_logger = MlFoundryLightningLogger(
@@ -73,23 +74,23 @@
             )
         trainer.fit(model, training_loader, validation_loader)
         ```
 
         Logger can also be created from an existing run
 
         ```
-        import mlfoundry as mlf
-        mlf.login()
+        import mlfoundry
+        mlfoundry.login()
         # or set API key via `TFY_API_KEY` env variable
 
         from pytorch_lightning import Trainer
         from pytorch_lightning.callbacks import ModelCheckpoint
         from mlfoundry.integrations.lightning import MlFoundryLightningLogger, LogModelStrategy
 
-        client = mlf.get_client()
+        client = mlfoundry.get_client()
         run = client.create_run(project_name="lightning")
 
         mlf_logger = MlFoundryLightningLogger.from_run(
             run=run,
             auto_end_run=False,
             flatten_params=True,
             log_model_strategy=LogModelStrategy.BEST_PLUS_LATEST,
@@ -110,28 +111,29 @@
 
         run.end()
         ```
     """
 
     def __init__(
         self,
-        project_name: str,
+        ml_repo: Optional[str] = None,
         run_name: Optional[str] = None,
         log_model_strategy: Union[str, LogModelStrategy] = LogModelStrategy.NO,
         flatten_params: Optional[bool] = False,
         prefix: str = "",
         agg_key_funcs: Optional[
             Mapping[str, Callable[[Sequence[float]], float]]
         ] = None,
         agg_default_func: Optional[Callable[[Sequence[float]], float]] = None,
+        project_name: Optional[str] = None,
         **kwargs,
     ):
         """
         Args:
-            project_name (str): name of the project to create the run under
+            ml_repo (str): name of the ML repo to create the run under
             run_name (Optional[str], optional): name of the run. When not provided a run name is automatically generated
             log_model_strategy (LogModelStrategy, optional): The strategy to use for logging models
                 - LogModelStrategy.NO (default): Do not log any models
                 - LogModelStrategy.BEST_ONLY: Log only the best model checkpoint.
                 - LogModelStrategy.BEST_PLUS_LATEST: Log both the latest checkpoint and the best checkpoint (if
                     available) and different from the latest checkpoint. Note that `save_last` argument must be set
                     in the `ModelCheckpoint` callback, else latest checkpoints wont be saved/logged.
@@ -155,44 +157,44 @@
             prefix (str, optional): This prefix will be added in front of all metric_name logged.
 
         """
         super().__init__(agg_key_funcs=agg_key_funcs, agg_default_func=agg_default_func)
 
         log_model_strategy = LogModelStrategy(log_model_strategy)
 
-        self._project_name = project_name
+        self._ml_repo = resolve_ml_repo_name(ml_repo=ml_repo, project_name=project_name)
         self._run_name = run_name
         self._log_model_strategy = log_model_strategy
         self._flatten_params = flatten_params
         self._auto_end_run = True
         self._prefix = prefix
 
-        self._run = None
+        self._run: Optional[MlFoundryRun] = None
         self._checkpoint_callback = None
         self._available_model_paths: List[str] = []
 
     @property
     @rank_zero_experiment  # Returns the real experiment on rank 0 and otherwise the DummyExperiment
     def run(self) -> MlFoundryRun:
         if self._run:
             return self._run
 
         if not self._run:
-            self._run = mlf.get_client().create_run(
-                project_name=self._project_name,
+            self._run = mlfoundry.get_client().create_run(
+                ml_repo=self._ml_repo,
                 run_name=self._run_name,
             )
             self._run_name = self._run.run_name
             self._auto_end_run = True
 
         return self._run
 
     @property
     def name(self) -> str:
-        return self.run.project_name
+        return self.run.ml_repo
 
     @property
     def version(self) -> str:
         return self.run.run_name
 
     @classmethod
     def from_run(
@@ -230,15 +232,15 @@
                 `{'a': {'b': 'c'}}` will be logged as -> `{'a/b': 'c'}`
 
                 when set to `False`:
                 Individual keys will be logged ie) `'a':{'b':'c'}`
             auto_end_run (bool, optional): if to end the run when training finishes. By default, this is `False`
         """
         instance = cls(
-            project_name=run.project_name,
+            project_name=run.ml_repo,
             run_name=run.run_name,
             log_model_strategy=log_model_strategy,
             flatten_params=flatten_params,
             **kwargs,
         )
         instance._run = run
         instance._auto_end_run = auto_end_run
@@ -315,15 +317,15 @@
 
         for checkpoint_path in checkpoints_to_log:
             checkpoint_name = os.path.basename(checkpoint_path)
             artifact_path = os.path.join(LIGHTNING_MODELS_PATH, checkpoint_name)
             logger.debug(
                 f"Logging checkpoint at {checkpoint_path!r} to {artifact_path!r}"
             )
-            self._run.log_artifact(
+            self._run.log_artifact_deprecated(
                 local_path=checkpoint_path, artifact_path=artifact_path
             )
 
         if best_checkpoint_path:
             best_model_artifact_path = _get_artifact_path_for_checkpoint(
                 os.path.basename(best_checkpoint_path)
             )
@@ -335,15 +337,15 @@
             )
             metadata["checkpoints"]["latest"] = latest_model_artifact_path
 
         metadata_file_name = "metadata.json"
         metadata_path = os.path.join(temp_dir, metadata_file_name)
         with open(metadata_path, "w") as f:
             json.dump(metadata, f)
-        self._run.log_artifact(
+        self._run.log_artifact_deprecated(
             local_path=metadata_path,
             artifact_path=LIGHTNING_MODELS_PATH,
         )
 
     def after_save_checkpoint(
         self, checkpoint_callback: "ReferenceType[ModelCheckpoint]"
     ) -> None:
```

### Comparing `mlfoundry-0.7.9/mlfoundry/integrations/transformers.py` & `mlfoundry-0.8.0rc1/mlfoundry/integrations/transformers.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 
 import numpy as np
 from transformers import IntervalStrategy, Trainer
 from transformers.integrations import rewrite_logs
 from transformers.trainer_callback import TrainerCallback
 from transformers.utils import flatten_dict
 
-import mlfoundry as mlf
+import mlfoundry
 from mlfoundry.enums import EnumMissingMixin
 from mlfoundry.logger import logger
+from mlfoundry.mlfoundry_api import resolve_ml_repo_name
 from mlfoundry.mlfoundry_run import MlFoundryRun
 
 __all__ = ["HF_MODEL_PATH", "MlFoundryTrainerCallback", "LogModelStrategy"]
 
 
 HF_ARTIFACTS_PATH = "hf/"
 HF_MODELS_PATH = os.path.join(HF_ARTIFACTS_PATH, "models")
@@ -42,16 +43,16 @@
 class MlFoundryTrainerCallback(TrainerCallback):
     """
     Huggingface Transformers Trainer Callback for tracking training run on MLFoundry
 
     Examples:
 
         ```
-        import mlfoundry as mlf
-        mlf.login()
+        import mlfoundry
+        mlfoundry.login()
         # or set API key via `TFY_API_KEY` env variable
 
         from transformers import TrainingArguments, Trainer
         from mlfoundry.integrations.transformers import MlFoundryTrainerCallback, LogModelStrategy
 
         mlf_cb = MlFoundryTrainerCallback(
             project_name="huggingface",
@@ -64,23 +65,23 @@
         trainer = Trainer(..., args=args, callbacks=[mlf_cb])
         trainer.train()
         ```
 
         Callback can also be created from an existing run
 
         ```
-        import mlfoundry as mlf
-        mlf.login()
+        import mlfoundry
+        mlfoundry.login()
         # or set API key via `TFY_API_KEY` env variable
 
         from transformers import TrainingArguments, Trainer
-        import mlfoundry as mlf
+        import mlfoundry
         from mlfoundry.integrations.transformers import MlFoundryTrainerCallback, LogModelStrategy
 
-        client = mlf.get_client()
+        client = mlfoundry.get_client()
         run = client.create_run(project_name="huggingface", run_name="my-hf-run")
 
         mlf_cb = MlFoundryTrainerCallback.from_run(
             run=run,
             auto_end_run=False,
             flatten_params=True,
             log_model_strategy=LogModelStrategy.BEST_PLUS_LATEST,
@@ -92,23 +93,24 @@
 
         run.end()
         ```
     """
 
     def __init__(
         self,
-        project_name: str,
+        ml_repo: Optional[str] = None,
         run_name: Optional[str] = None,
         flatten_params: bool = False,
         log_model_strategy: Union[str, LogModelStrategy] = LogModelStrategy.NO,
+        project_name: Optional[str] = None,
         **kwargs,
     ):
         """
         Args:
-            project_name (str): name of the project to create the run under
+            ml_repo (str): name of the ML Repo to create the run under
             run_name (Optional[str], optional): name of the run. When not provided a run name is automatically generated
             flatten_params (bool, optional): if to flatten the args and model config dictionaries before logging them,
                 By default, this is `False`
 
                 For e.g.
 
                 when set to True,
@@ -149,15 +151,15 @@
                 f"`log_model` argument has been deprecated, please use the `log_model_strategy` argument instead. "
                 f"E.g. log_model_strategy={_option}",
                 FutureWarning,
             )
             if kwargs["log_model"] and log_model_strategy == LogModelStrategy.NO:
                 log_model_strategy = LogModelStrategy.BEST_PLUS_LATEST
 
-        self._project_name = project_name
+        self._ml_repo = resolve_ml_repo_name(ml_repo=ml_repo, project_name=project_name)
         self._run_name = run_name
         self._run: Optional[MlFoundryRun] = None
         self._auto_end_run = True
 
         self._flatten_params = flatten_params
         self._log_model_strategy = log_model_strategy
         self._MAX_PARAM_VAL_LENGTH = 250
@@ -213,15 +215,15 @@
                 see the description for `log_model_strategy`
             **kwargs: Additional keyword arguments to pass to init
 
         Returns:
             MlFoundryTrainerCallback: an instance of `MlFoundryTrainerCallback`
         """
         instance = cls(
-            project_name=run.project_name,
+            ml_repo=run.ml_repo,
             run_name=run.run_name,
             flatten_params=flatten_params,
             log_model_strategy=log_model_strategy,
             **kwargs,
         )
         instance._run = run
         instance._auto_end_run = auto_end_run
@@ -268,16 +270,16 @@
             # If the current process is not the global main process in a distributed training setting do nothing
             return
 
         logger.info("Automatic MLFoundry logging enabled")
 
         if not self._run:
             self._auto_end_run = True
-            self._run = mlf.get_client().create_run(
-                project_name=self._project_name,
+            self._run = mlfoundry.get_client().create_run(
+                ml_repo=self._ml_repo,
                 run_name=self._run_name,
             )
 
         args_dict = {f"args/{k}": v for k, v in args.to_dict().items()}
         if self._flatten_params:
             args_dict = flatten_dict(args_dict)
 
@@ -377,20 +379,22 @@
     ):
         # TODO: this is kept only for backward compatibility and duplicates a checkpoint
         #       this should be removed
         checkpoint_path = best_checkpoint_path or latest_checkpoint_path
         if not checkpoint_path:
             return
 
-        self._run.log_artifact(local_path=checkpoint_path, artifact_path=HF_MODEL_PATH)
+        self._run.log_artifact_deprecated(
+            local_path=checkpoint_path, artifact_path=HF_MODEL_PATH
+        )
         metadata = {"checkpoint_name": os.path.basename(checkpoint_path)}
         metadata_filepath = os.path.join(temp_dir, ".mlfoundry.json")
         with open(metadata_filepath, "w") as f:
             json.dump(metadata, f)
-        self._run.log_artifact(
+        self._run.log_artifact_deprecated(
             local_path=metadata_filepath, artifact_path=HF_MODEL_PATH
         )
 
     def _log_model_on_train_end(
         self,
         temp_dir,
         args,
@@ -443,15 +447,15 @@
 
         for checkpoint_path in checkpoints_to_log:
             checkpoint_name = os.path.basename(checkpoint_path)
             artifact_path = os.path.join(HF_MODELS_PATH, checkpoint_name)
             logger.debug(
                 f"Logging checkpoint at {checkpoint_path!r} to {artifact_path!r}"
             )
-            self._run.log_artifact(
+            self._run.log_artifact_deprecated(
                 local_path=checkpoint_path, artifact_path=artifact_path
             )
 
         if best_checkpoint_path:
             metadata["checkpoints"]["best"] = _get_artifact_path_for_checkpoint(
                 best_checkpoint_path
             )
@@ -461,15 +465,15 @@
                 latest_checkpoint_path
             )
 
         metadata_file_name = "metadata.json"
         metadata_path = os.path.join(temp_dir, metadata_file_name)
         with open(metadata_path, "w") as f:
             json.dump(metadata, f)
-        self._run.log_artifact(
+        self._run.log_artifact_deprecated(
             local_path=metadata_path,
             artifact_path=HF_MODELS_PATH,
         )
 
         self._legacy_log_model(
             temp_dir=temp_dir,
             best_checkpoint_path=best_checkpoint_path,
```

### Comparing `mlfoundry-0.7.9/mlfoundry/internal_namespace.py` & `mlfoundry-0.8.0rc1/mlfoundry/internal_namespace.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/log_types/__init__.py` & `mlfoundry-0.8.0rc1/mlfoundry/log_types/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/log_types/artifacts/artifact.py` & `mlfoundry-0.8.0rc1/mlfoundry/log_types/artifacts/artifact.py`

 * *Files 3% similar despite different names*

```diff
@@ -186,21 +186,31 @@
 
 
 def _log_artifact_version_helper(
     run,
     name: str,
     artifact_type: ArtifactType,
     artifact_dir: tempfile.TemporaryDirectory,
+    mlflow_client: Optional[MlflowClient] = None,
+    ml_repo_id: Optional[str] = None,
     description: Optional[str] = None,
     metadata: Optional[Dict[str, Any]] = None,
     step: int = 0,
 ):
-    mlflow_client: MlflowClient = run.mlflow_client
+    if (run and mlflow_client) or (not run and not mlflow_client):
+        raise MlFoundryException("Exactly one of run, mlflow_client should be passed")
+    if mlflow_client and not ml_repo_id:
+        raise MlFoundryException(
+            "If mlflow_client is passed, ml_repo_id must also be passed"
+        )
+    if run:
+        mlflow_client: MlflowClient = run.mlflow_client
+
     version_id = mlflow_client.create_artifact_version(
-        experiment_id=int(run._experiment_id),
+        experiment_id=int(run._experiment_id) if run else ml_repo_id,
         artifact_type=artifact_type,
         name=name,
     )
     artifacts_repo = MlFoundryArtifactsRepository(
         version_id=version_id, mlflow_client=mlflow_client
     )
     total_size = calculate_artifact_size(artifact_dir)
@@ -213,15 +223,15 @@
     except Exception as e:
         mlflow_client.notify_failure_for_artifact_version(version_id=version_id)
         raise MlFoundryException("Failed to log Artifact") from e
     finally:
         artifact_dir.cleanup()
     artifact_version = mlflow_client.finalize_artifact_version(
         version_id=version_id,
-        run_uuid=run.run_id,
+        run_uuid=run.run_id if run else None,
         description=description,
         artifact_metadata=metadata,
         data_path=INTERNAL_METADATA_PATH,
         step=step,
         artifact_size=total_size,
     )
```

### Comparing `mlfoundry-0.7.9/mlfoundry/log_types/artifacts/constants.py` & `mlfoundry-0.8.0rc1/mlfoundry/log_types/artifacts/constants.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/log_types/artifacts/general_artifact.py` & `mlfoundry-0.8.0rc1/mlfoundry/log_types/artifacts/general_artifact.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import collections
 import json
 import os.path
 import tempfile
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from mlflow.entities import ArtifactType
+from mlflow.tracking import MlflowClient
 
 from mlfoundry.exceptions import MlFoundryException
 from mlfoundry.log_types.artifacts.artifact import (
     ArtifactPath,
     ArtifactVersion,
     ArtifactVersionInternalMetadata,
     _log_artifact_version_helper,
@@ -22,14 +23,16 @@
 from mlfoundry.logger import logger
 
 
 def _log_artifact_version(
     run,
     name: str,
     artifact_paths: List[Union[ArtifactPath, Tuple[str, Optional[str]]]],
+    mlflow_client: Optional[MlflowClient] = None,
+    ml_repo_id: Optional[str] = None,
     description: Optional[str] = None,
     metadata: Optional[Dict[str, Any]] = None,
     step: int = 0,
 ) -> ArtifactVersion:
 
     for i, artifact_path in enumerate(artifact_paths):
         if isinstance(artifact_path, ArtifactPath):
@@ -77,14 +80,16 @@
     local_internal_metadata_path = os.path.join(temp_dir.name, INTERNAL_METADATA_PATH)
     os.makedirs(os.path.dirname(local_internal_metadata_path), exist_ok=True)
     with open(local_internal_metadata_path, "w") as f:
         json.dump(internal_metadata.dict(), f)
 
     return _log_artifact_version_helper(
         run=run,
+        mlflow_client=mlflow_client,
+        ml_repo_id=ml_repo_id,
         name=name,
         artifact_type=ArtifactType.ARTIFACT,
         artifact_dir=temp_dir,
         description=description,
         metadata=metadata,
         step=step,
     )
```

### Comparing `mlfoundry-0.7.9/mlfoundry/log_types/artifacts/model.py` & `mlfoundry-0.8.0rc1/mlfoundry/log_types/artifacts/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,25 +257,35 @@
 
 
 def _log_model_version(
     run,
     name: str,
     model: Any,
     framework: ModelFramework,
+    mlflow_client: Optional[MlflowClient] = None,
+    ml_repo_id: Optional[str] = None,
     model_save_kwargs: Optional[Dict[str, Any]] = None,
     additional_files: Sequence[Tuple[Union[str, Path], Optional[str]]] = (),
     description: Optional[str] = None,
     metadata: Optional[Dict[str, Any]] = None,
     model_schema: Optional[Union[Dict[str, Any], ModelSchema]] = None,
     custom_metrics: Optional[Union[List[Dict[str, Any]], CustomMetric]] = None,
     step: int = 0,
 ) -> ModelVersion:
-
     from mlfoundry.frameworks import get_model_registry
 
+    if (run and mlflow_client) or (not run and not mlflow_client):
+        raise MlFoundryException("Exactly one of run, mlflow_client should be passed")
+    if mlflow_client and not ml_repo_id:
+        raise MlFoundryException(
+            "If mlflow_client is passed, ml_repo_id must also be passed"
+        )
+    if run:
+        mlflow_client: MlflowClient = run.mlflow_client
+
     custom_metrics = custom_metrics or []
     model_save_kwargs = model_save_kwargs or {}
     metadata = metadata or {}
     additional_files = additional_files or {}
     step = step or 0
 
     # validations
@@ -301,15 +311,14 @@
         )
     custom_metrics = [
         CustomMetric.parse_obj(cm) if not isinstance(cm, CustomMetric) else cm
         for cm in custom_metrics
     ]
 
     logger.info("Logging model and additional files, this might take a while ...")
-    mlflow_client: MlflowClient = run.mlflow_client
     temp_dir = tempfile.TemporaryDirectory(prefix="truefoundry-")
 
     internal_metadata = ModelVersionInternalMetadata(
         framework=framework,
         files_dir=FILES_DIR,
         model_dir=MODEL_DIR_NAME,
         model_is_null=model is None,
@@ -348,15 +357,15 @@
     local_internal_metadata_path = os.path.join(temp_dir.name, INTERNAL_METADATA_PATH)
     os.makedirs(os.path.dirname(local_internal_metadata_path), exist_ok=True)
     with open(local_internal_metadata_path, "w") as f:
         json.dump(internal_metadata.dict(), f)
 
     # create entry
     version_id = mlflow_client.create_artifact_version(
-        experiment_id=int(run._experiment_id),
+        experiment_id=int(run._experiment_id) if run else ml_repo_id,
         artifact_type=ArtifactType.MODEL,
         name=name,
     )
     artifacts_repo = MlFoundryArtifactsRepository(
         version_id=version_id, mlflow_client=mlflow_client
     )
     model_size = calculate_model_size(temp_dir)
@@ -368,22 +377,25 @@
         artifacts_repo.log_artifacts(local_dir=temp_dir.name, artifact_path=None)
     except Exception as e:
         mlflow_client.notify_failure_for_artifact_version(version_id=version_id)
         raise MlFoundryException("Failed to log model") from e
     finally:
         temp_dir.cleanup()
     mlflow_client.finalize_artifact_version(
-        version_id=version_id, run_uuid=run.run_id, artifact_size=model_size
+        version_id=version_id,
+        run_uuid=run.run_id if run else None,
+        artifact_size=model_size,
+        step=step if run else None,
     )
     model_version = mlflow_client.create_model_version(
         artifact_version_id=version_id,
         description=description,
         artifact_metadata=metadata,
         data_path=INTERNAL_METADATA_PATH,
-        step=step,
+        step=step if run else None,
     )
     # update model schema at end
     if model_schema is not None:
         try:
             model_version = mlflow_client.update_model_version(
                 version_id=version_id,
                 model_schema=model_schema,
```

### Comparing `mlfoundry-0.7.9/mlfoundry/log_types/artifacts/utils.py` & `mlfoundry-0.8.0rc1/mlfoundry/log_types/artifacts/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/log_types/dataset_artifact.py` & `mlfoundry-0.8.0rc1/mlfoundry/log_types/dataset_artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/log_types/image/image.py` & `mlfoundry-0.8.0rc1/mlfoundry/log_types/image/image.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/log_types/image/image_normalizer.py` & `mlfoundry-0.8.0rc1/mlfoundry/log_types/image/image_normalizer.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/log_types/image/types.py` & `mlfoundry-0.8.0rc1/mlfoundry/log_types/image/types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/log_types/plot.py` & `mlfoundry-0.8.0rc1/mlfoundry/log_types/plot.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/log_types/pydantic_base.py` & `mlfoundry-0.8.0rc1/mlfoundry/log_types/pydantic_base.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/log_types/utils.py` & `mlfoundry-0.8.0rc1/mlfoundry/log_types/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/login.py` & `mlfoundry-0.8.0rc1/mlfoundry/login.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/metrics/v1/__init__.py` & `mlfoundry-0.8.0rc1/mlfoundry/metrics/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/metrics/v1/base_metrics.py` & `mlfoundry-0.8.0rc1/mlfoundry/metrics/v1/base_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/metrics/v1/binary_classification_metrics.py` & `mlfoundry-0.8.0rc1/mlfoundry/metrics/v1/binary_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/metrics/v1/multiclass_classification_metrics.py` & `mlfoundry-0.8.0rc1/mlfoundry/metrics/v1/multiclass_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/metrics/v1/regression_metrics.py` & `mlfoundry-0.8.0rc1/mlfoundry/metrics/v1/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/metrics/v1/timeseries_metrics.py` & `mlfoundry-0.8.0rc1/mlfoundry/metrics/v1/timeseries_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/metrics/v2/__init__.py` & `mlfoundry-0.8.0rc1/mlfoundry/metrics/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/metrics/v2/base_metrics.py` & `mlfoundry-0.8.0rc1/mlfoundry/metrics/v2/base_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/metrics/v2/custom_metric_types.py` & `mlfoundry-0.8.0rc1/mlfoundry/metrics/v2/custom_metric_types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/metrics/v2/multiclass_classification_metrics.py` & `mlfoundry-0.8.0rc1/mlfoundry/metrics/v2/multiclass_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/metrics/v2/regression_metrics.py` & `mlfoundry-0.8.0rc1/mlfoundry/metrics/v2/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/metrics/v2/timeseries_metrics.py` & `mlfoundry-0.8.0rc1/mlfoundry/metrics/v2/timeseries_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/mlfoundry_api.py` & `mlfoundry-0.8.0rc1/mlfoundry/mlfoundry_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,31 +3,44 @@
 python examples/sklearn/iris_train.py
 
 Besides running pytest
 """
 from __future__ import annotations
 
 import os
+import warnings
 from datetime import datetime, timedelta, timezone
-from typing import Any, Dict, Generator, Iterator, List, Optional, Sequence, Union
+from pathlib import Path
+from typing import (
+    Any,
+    Dict,
+    Generator,
+    Iterator,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+)
 
 import coolname
 import mlflow
 import pandas as pd
-from mlflow.entities import Experiment
+from mlflow.entities import CustomMetric, Experiment, ModelSchema
 from mlflow.store.tracking import SEARCH_MAX_RESULTS_DEFAULT
 from mlflow.tracking import MlflowClient
 
 from mlfoundry import amplitude, constants, env_vars
-from mlfoundry.enums import ViewType
+from mlfoundry.enums import ModelFramework, ViewType
 from mlfoundry.env_vars import TRACKING_HOST_GLOBAL
 from mlfoundry.exceptions import MlflowException, MlFoundryException
 from mlfoundry.internal_namespace import NAMESPACE
-from mlfoundry.log_types.artifacts.artifact import ArtifactVersion
-from mlfoundry.log_types.artifacts.model import ModelVersion
+from mlfoundry.log_types.artifacts.artifact import ArtifactPath, ArtifactVersion
+from mlfoundry.log_types.artifacts.general_artifact import _log_artifact_version
+from mlfoundry.log_types.artifacts.model import ModelVersion, _log_model_version
 from mlfoundry.logger import logger
 from mlfoundry.mlfoundry_run import MlFoundryRun
 from mlfoundry.monitoring.entities import Actual, Prediction
 from mlfoundry.monitoring.store import MonitoringClient
 from mlfoundry.session import Session, get_active_session, init_session
 from mlfoundry.tracking.servicefoundry_service import ServicefoundryService
 
@@ -86,22 +99,25 @@
 
 def resolve_ml_repo_name(
     ml_repo: Optional[str] = None,
     project_name: Optional[str] = None,
 ) -> str:
     if project_name and ml_repo:
         raise MlFoundryException(
-            f"Only one of field project_name or ml_repo should be passed"
+            f"Only one of `ml_repo` or `project_name` should be passed"
         )
     if not project_name and not ml_repo:
-        raise MlFoundryException(f"ml_repo must be string type and cannot be empty")
+        raise MlFoundryException(f"`ml_repo` must be string type and cannot be empty")
     if project_name:
-        logger.warning(
-            "Field project_name has been depricated and renamed to ml_repo. Please use ml_repo as we will remove project_name in the upcoming versions"
+        warning_message = (
+            "Argument `project_name` has been deprecated and renamed to `ml_repo`. "
+            "Please use `ml_repo` as `project_name` will be removed in the upcoming versions"
         )
+        warnings.warn(warning_message, FutureWarning)
+        logger.warning(warning_message)
     if ml_repo:
         project_name = ml_repo
     if project_name == "" or (not isinstance(project_name, str)):
         raise MlFoundryException(
             f"ml_repo must be string type and not empty. "
             f"Got {type(project_name)} type with value {project_name!r}"
         )
@@ -111,15 +127,15 @@
 class MlFoundry:
     """MlFoundry."""
 
     def __init__(self, session: Optional[Session] = None):
         """__init__.
 
         Args:
-            tracking_uri (Optional[str], optional): tracking_uri
+            session (Optional[Session], optional): Session instance to get auth credentials from
         """
         self.mlflow_client = MlflowClient()
         if session:
             self.monitoring_client = MonitoringClient(session=session)
 
     def _get_ml_repo(self, ml_repo: str) -> str:
         """_get_ml_repo.
@@ -204,18 +220,18 @@
                     f"{storage_integration_fqn}"
                 )
 
         return existing_ml_repo
 
     def create_run(
         self,
-        project_name: Optional[str] = None,
         ml_repo: Optional[str] = None,
         run_name: Optional[str] = None,
         tags: Optional[Dict[str, Any]] = None,
+        project_name: Optional[str] = None,
         **kwargs,
     ) -> MlFoundryRun:
         """Initialize a `run`.
 
         In a machine learning experiment `run` represents a single experiment
         conducted under a project.
         Args:
@@ -349,16 +365,16 @@
         return MlFoundryRun(
             experiment_id=run.info.experiment_id,
             run_id=run.info.run_id,
         )
 
     def get_all_runs(
         self,
-        project_name: Optional[str] = None,
         ml_repo: Optional[str] = None,
+        project_name: Optional[str] = None,
     ) -> pd.DataFrame:
         """Returns all the run name and id present under a project.
 
         The user must have `READ` access to the project.
         Args:
             ml_repo (str): Name of the project.
         Returns:
@@ -399,23 +415,23 @@
 
         return pd.DataFrame(
             runs, columns=[constants.RUN_ID_COL_NAME, constants.RUN_NAME_COL_NAME]
         )
 
     def search_runs(
         self,
-        project_name: Optional[str] = None,
         ml_repo: Optional[str] = None,
         filter_string: str = "",
         run_view_type: str = "ACTIVE_ONLY",
         order_by: Sequence[str] = ("attribute.start_time DESC",),
+        project_name: Optional[str] = None,
     ) -> Generator[MlFoundryRun, None, None]:
         """
         The user must have `READ` access to the project.
-        Returns an Generator that returns a MLFoundryRun on each next call.
+        Returns a Generator that returns a MLFoundryRun on each next call.
         All the runs under a project which matches the filter string and the run_view_type are returned.
 
         Args:
             ml_repo (str): Name of the project.
             filter_string (str, optional):
                 Filter query string, defaults to searching all runs. Identifier required in the LHS of a search expression.
                 Signifies an entity to compare against. An identifier has two parts separated by a period: the type of the entity and the name of the entity.
@@ -647,14 +663,242 @@
             for artifact_version in artifact_versions:
                 yield ArtifactVersion(
                     artifact_version=artifact_version, artifact=artifact
                 )
             if not artifact_versions or not page_token:
                 done = True
 
+    def log_artifact(
+        self,
+        ml_repo: str,
+        name: str,
+        artifact_paths: List[
+            Union[Tuple[str], Tuple[str, Optional[str]], ArtifactPath]
+        ],
+        description: Optional[str] = None,
+        metadata: Optional[Dict] = None,
+    ) -> ArtifactVersion | None:
+        """Logs an artifact for the current `ml_repo`.
+
+        An `artifact` is a list of local files and directories. This function packs the mentioned files and directories in `artifact_paths` and uploads them to remote storage linked to the ml_repo
+
+        Args:
+            ml_repo (str): Name of the ML Repo to which an artifact is to be logged.
+            name (str): Name of the Artifact. If an artifact with this name already exists under the current ml_repo,
+                the logged artifact will be added as a new version under that `name`. If no artifact exist with the given
+                `name`, the given artifact will be logged as version 1.
+            artifact_paths (List[mlfoundry.ArtifactPath], optional): A list of pairs
+                of (source path, destination path) to add files and folders
+                to the artifact version contents. The first member of the pair should be a file or directory path
+                and the second member should be the path inside the artifact contents to upload to.
+
+                E.g. >>> client.log_artifact(
+                     ...     ml_repo="sample-repo",
+                     ...     name="xyz",
+                     ...     artifact_paths=[
+                                mlfoundry.ArtifactPath("foo.txt", "foo/bar/foo.txt"),
+                                mlfoundry.ArtifactPath("tokenizer/", "foo/tokenizer/"),
+                                mlfoundry.ArtifactPath('bar.text'),
+                                ('bar.txt', ),
+                                ('foo.txt', 'a/foo.txt')
+                             ]
+                     ... )
+                would result in
+                .
+                └── foo/
+                    ├── bar/
+                    │   └── foo.txt
+                    └── tokenizer/
+                        └── # contents of tokenizer/ directory will be uploaded here
+            description (Optional[str], optional): arbitrary text upto 1024 characters to store as description.
+                This field can be updated at any time after logging. Defaults to `None`
+            metadata (Optional[Dict[str, Any]], optional): arbitrary json serializable dictionary to store metadata.
+                For example, you can use this to store metrics, params, notes.
+                This field can be updated at any time after logging. Defaults to `None`
+
+        Returns:
+            mlfoundry.ArtifactVersion: an instance of `ArtifactVersion` that can be used to download the files,
+            or update attributes like description, metadata.
+
+        Examples:
+        ```python
+        import os
+        import mlfoundry
+
+        with open("artifact.txt", "w") as f:
+            f.write("hello-world")
+
+        client = mlfoundry.get_client()
+        ml_repo = "sample-repo"
+
+        client.create_ml_repo(ml_repo=ml_repo)
+        client.log_artifact(
+            ml_repo=ml_repo,
+            name="hello-world-file",
+            artifact_paths=[mlfoundry.ArtifactPath('artifact.txt', 'a/b/')]
+        )
+        ```
+        """
+        if not artifact_paths:
+            raise MlFoundryException(
+                "artifact_paths cannot be empty, atleast one artifact_path must be passed"
+            )
+
+        ml_repo_id = self._get_ml_repo(ml_repo=ml_repo)
+        artifact_version = _log_artifact_version(
+            run=None,
+            mlflow_client=self.mlflow_client,
+            ml_repo_id=ml_repo_id,
+            name=name,
+            artifact_paths=artifact_paths,
+            description=description,
+            metadata=metadata,
+            step=None,
+        )
+        logger.info(f"Logged artifact successfully with fqn {artifact_version.fqn!r}")
+        return artifact_version
+
+    def log_model(
+        self,
+        *,
+        ml_repo: str,
+        name: str,
+        model: Any,
+        framework: Optional[Union[ModelFramework, str]],
+        model_save_kwargs: Optional[Dict[str, Any]] = None,
+        additional_files: Sequence[Tuple[Union[str, Path], Optional[str]]] = (),
+        description: Optional[str] = None,
+        metadata: Optional[Dict[str, Any]] = None,
+        model_schema: Optional[Union[Dict[str, Any], ModelSchema]] = None,
+        custom_metrics: Optional[List[Union[Dict[str, Any], CustomMetric]]] = None,
+    ) -> ModelVersion:
+        """
+        Serialize and log a versioned model under the current ml_repo. Each logged model generates a new version
+        associated with the given `name` and linked to the current run. Multiple versions of the model can be
+        logged as separate versions under the same `name`.
+
+        Args:
+            ml_repo (str): Name of the ML Repo to which an artifact is to be logged.
+            name (str): Name of the model. If a model with this name already exists under the current ml_repo,
+                the logged model will be added as a new version under that `name`. If no models exist with the given
+                `name`, the given model will be logged as version 1.
+            model (Any): model instance of any one of the supported frameworks under `mlfoundry.enums.ModelFramework`.
+                Can also be `None` which can be useful to create a reference entry without uploading any model files.
+            framework (Union[enums.ModelFramework, str]): Model Framework. Ex:- pytorch, sklearn, tensorflow etc.
+                The full list of supported frameworks can be found in `mlfoundry.enums.ModelFramework`.
+                Can also be `None` when `model` is `None`.
+            model_save_kwargs (Optional[Dict[str, Any]], optional): keyword arguments to pass to model serializer.
+                Defaults to `None`
+            additional_files (Sequence[Tuple[Union[str, Path], Optional[str]]], optional): A list of pairs
+                of (source path, destination path) to add additional files and folders
+                to the model version contents. The first member of the pair should be a file or directory path
+                and the second member should be the path inside the model versions contents to upload to.
+                The model version contents are arranged like follows
+                .
+                └── model/
+                    └── # model files are serialized here
+                └── # any additional files and folders can be added here
+
+                To avoid corrupting any model files, the "model/" directory is reserved and additional files cannot be
+                added to it.
+
+                E.g. >>> client.log_model(
+                     ...     ml_repo="sample-repo", name="xyz", model=clf, framework="sklearn",
+                     ...     additional_files=[("foo.txt", "foo/bar/foo.txt"), ("tokenizer/", "foo/tokenizer/")]
+                     ... )
+                would result in
+                .
+                ├── model/
+                │   └── # model files are serialized here e.g. model.joblib
+                └── foo/
+                    ├── bar/
+                    │   └── foo.txt
+                    └── tokenizer/
+                        └── # contents of tokenizer/ directory will be uploaded here
+            description (Optional[str], optional): arbitrary text upto 1024 characters to store as description.
+                This field can be updated at any time after logging. Defaults to `None`
+            metadata (Optional[Dict[str, Any]], optional): arbitrary json serializable dictionary to store metadata.
+                For example, you can use this to store metrics, params, notes.
+                This field can be updated at any time after logging. Defaults to `None`
+            model_schema (Optional[Union[Dict[str, Any], ModelSchema]], optional): instance of `mlfoundry.ModelSchema`.
+                This schema needs to be consistent with older versions of the model under the given `name` i.e.
+                a feature's value type and model's prediction type cannot be changed in the schema of new version.
+                Features can be removed or added between versions.
+                E.g. if there exists a v1 with
+                schema = {"features": {"name": "feat1": "int"}, "prediction": "categorical"}, then
+
+                schema = {"features": {"name": "feat1": "string"}, "prediction": "categorical"} or
+                schema = {"features": {"name": "feat1": "int"}, "prediction": "numerical"}
+                are invalid because they change the types of existing features and prediction
+
+                while
+                schema = {"features": {"name": "feat1": "int", "feat2": "string"}, "prediction": "categorical"} or
+                schema = {"features": {"feat2": "string"}, "prediction": "categorical"}
+                are valid
+
+                This field can be updated at any time after logging. Defaults to `None`
+            custom_metrics: (Optional[Union[List[Dict[str, Any]], CustomMetric]], optional): list of instances of
+                `mlfoundry.CustomMetric`
+                The custom metrics must be added according to the prediction type of schema.
+                custom_metrics = [{
+                    "name": "mean_square_error",
+                    "type": "metric",
+                    "value_type": "float"
+                }]
+
+        Returns:
+            mlfoundry.ModelVersion: an instance of `ModelVersion` that can be used to download the files,
+                load the model, or update attributes like description, metadata, schema.
+
+        Examples:
+
+        ### sklearn
+        ```python
+        import mlfoundry
+        import numpy as np
+        from sklearn.pipeline import make_pipeline
+        from sklearn.preprocessing import StandardScaler
+        from sklearn.svm import SVC
+
+        client = mlfoundry.get_client()
+        run = client.create_run(
+            ml_repo="my-classification-project"
+        )
+        X = np.array([[-1, -1], [-2, -1], [1, 1], [2, 1]])
+        y = np.array([1, 1, 2, 2])
+        clf = make_pipeline(StandardScaler(), SVC(gamma='auto'))
+        clf.fit(X, y)
+
+        model_version = run.log_model(
+            name="my-sklearn-model",
+            model=clf,
+            framework="sklearn"
+        )
+        print(model_version.fqn)
+        """
+        ml_repo_id = self._get_ml_repo(ml_repo=ml_repo)
+
+        model_version = _log_model_version(
+            run=None,
+            mlflow_client=self.mlflow_client,
+            ml_repo_id=ml_repo_id,
+            name=name,
+            model=model,
+            framework=framework,
+            model_save_kwargs=model_save_kwargs,
+            additional_files=additional_files,
+            description=description,
+            metadata=metadata,
+            model_schema=model_schema,
+            custom_metrics=custom_metrics,
+            step=None,
+        )
+        logger.info(f"Logged model successfully with fqn {model_version.fqn!r}")
+        return model_version
+
     def log_predictions(
         self, model_version_fqn: str, predictions: List[Union[Prediction, Dict]]
     ):
         """log_predictions.
 
         Args:
             model_version_fqn (str): fqn of model_version where data needs to be logged
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mlfoundry-0.7.9/mlfoundry/mlfoundry_run.py` & `mlfoundry-0.8.0rc1/mlfoundry/mlfoundry_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,14 @@
         """__init__.
 
         Args:
             experiment_id (str): experiment_id
             run_id (str): run_id
         """
 
-        # TODO (chiragjn): rename experiment to project everywhere
         self._experiment_id = str(experiment_id)
         # TODO (chiragjn): mlflow_client be a protected/private member
         self.mlflow_client = MlflowClient()
         self._project_name = self.mlflow_client.get_experiment(self._experiment_id).name
         self._run_id = run_id
         self._run_info: Optional[RunInfo] = None
 
@@ -368,20 +367,20 @@
         artifact_paths: List[
             Union[Tuple[str], Tuple[str, Optional[str]], ArtifactPath]
         ],
         description: Optional[str] = None,
         metadata: Optional[Dict] = None,
         step: Optional[int] = 0,
     ) -> ArtifactVersion:
-        """Logs an artifact for the current `project`.
+        """Logs an artifact for the current ML Repo.
 
         An `artifact` is a list of local files and directories. This function packs the mentioned files and directories in `artifact_paths` and uploads them to remote storage linked to the experiment
 
         Args:
-            name (str): Name of the Artifact. If an artifact with this name already exists under the current project,
+            name (str): Name of the Artifact. If an artifact with this name already exists under the current ML Repo,
                 the logged artifact will be added as a new version under that `name`. If no artifact exist with the given
                 `name`, the given artifact will be logged as version 1.
             artifact_paths (List[mlfoundry.ArtifactPath], optional): A list of pairs
                 of (source path, destination path) to add files and folders
                 to the artifact version contents. The first member of the pair should be a file or directory path
                 and the second member should be the path inside the artifact contents to upload to.
 
@@ -913,20 +912,20 @@
         model_schema: Optional[Union[Dict[str, Any], ModelSchema]] = None,
         custom_metrics: Optional[List[Union[Dict[str, Any], CustomMetric]]] = None,
         step: int = 0,
     ) -> ModelVersion:
         # TODO (chiragjn): Document mapping of framework to list of valid model save kwargs
         # TODO (chiragjn): Add more examples
         """
-        Serialize and log a versioned model under the current project. Each logged model generates a new version
+        Serialize and log a versioned model under the current ML Repo. Each logged model generates a new version
             associated with the given `name` and linked to the current run. Multiple versions of the model can be
             logged as separate versions under the same `name`.
 
         Args:
-            name (str): Name of the model. If a model with this name already exists under the current project,
+            name (str): Name of the model. If a model with this name already exists under the current ML Repo,
                 the logged model will be added as a new version under that `name`. If no models exist with the given
                 `name`, the given model will be logged as version 1.
             model (Any): model instance of any one of the supported frameworks under `mlfoundry.enums.ModelFramework`.
                 Can also be `None` which can be useful to create a reference entry without uploading any model files.
             framework (Union[enums.ModelFramework, str]): Model Framework. Ex:- pytorch, sklearn, tensorflow etc.
                 The full list of supported frameworks can be found in `mlfoundry.enums.ModelFramework`.
                 Can also be `None` when `model` is `None`.
```

### Comparing `mlfoundry-0.7.9/mlfoundry/monitoring/entities.py` & `mlfoundry-0.8.0rc1/mlfoundry/monitoring/entities.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/monitoring/store/client.py` & `mlfoundry-0.8.0rc1/mlfoundry/monitoring/store/client.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/monitoring/store/repositories/dto.py` & `mlfoundry-0.8.0rc1/mlfoundry/monitoring/store/repositories/dto.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py` & `mlfoundry-0.8.0rc1/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/monitoring/store/worker.py` & `mlfoundry-0.8.0rc1/mlfoundry/monitoring/store/worker.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/run_utils.py` & `mlfoundry-0.8.0rc1/mlfoundry/run_utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/session.py` & `mlfoundry-0.8.0rc1/mlfoundry/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,16 @@
 
     def add_run(self, run: MlFoundryRun):
         with SESSION_LOCK:
             self._active_runs[run.run_id] = weakref.ref(run)
 
     def remove_run(self, run: MlFoundryRun):
         with SESSION_LOCK:
-            del self._active_runs[run.run_id]
+            if run.run_id in self._active_runs:
+                del self._active_runs[run.run_id]
 
     def close_active_runs(self):
         with SESSION_LOCK:
             for run_ref in list(self._active_runs.values()):
                 run = run_ref()
                 if run:
                     run.end()
```

### Comparing `mlfoundry-0.7.9/mlfoundry/tracking/auth_service.py` & `mlfoundry-0.8.0rc1/mlfoundry/tracking/auth_service.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/tracking/entities.py` & `mlfoundry-0.8.0rc1/mlfoundry/tracking/entities.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/tracking/servicefoundry_service.py` & `mlfoundry-0.8.0rc1/mlfoundry/tracking/servicefoundry_service.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/tracking/truefoundry_rest_store.py` & `mlfoundry-0.8.0rc1/mlfoundry/tracking/truefoundry_rest_store.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/mlfoundry/vendor/pynvml/pynvml.py` & `mlfoundry-0.8.0rc1/mlfoundry/vendor/pynvml/pynvml.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.7.9/pyproject.toml` & `mlfoundry-0.8.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlfoundry"
-version = "0.7.9" # do not change, auto-generated by poetry-dynamic-versioning
+version = "0.8.0rc1" # do not change, auto-generated by poetry-dynamic-versioning
 description = "Truefoundry's Experiment Tracking, Model Registry and Model Monitoring Library"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 homepage = "https://github.com/truefoundry/mlfoundry"
 repository = "https://github.com/truefoundry/mlfoundry"
 readme = "README.md"
 packages = [
     { include = "mlfoundry" },
```

### Comparing `mlfoundry-0.7.9/PKG-INFO` & `mlfoundry-0.8.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlfoundry
-Version: 0.7.9
+Version: 0.8.0rc1
 Summary: Truefoundry's Experiment Tracking, Model Registry and Model Monitoring Library
 Home-page: https://github.com/truefoundry/mlfoundry
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.7,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

