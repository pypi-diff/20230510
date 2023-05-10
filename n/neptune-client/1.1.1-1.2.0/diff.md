# Comparing `tmp/neptune_client-1.1.1.tar.gz` & `tmp/neptune_client-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune_client-1.1.1.tar", max compression
+gzip compressed data, was "neptune_client-1.2.0.tar", max compression
```

## Comparing `neptune_client-1.1.1.tar` & `neptune_client-1.2.0.tar`

### file list

```diff
@@ -1,322 +1,323 @@
--rw-r--r--   0        0        0    24339 2023-03-22 09:15:58.802336 neptune_client-1.1.1/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-03-22 09:15:58.802336 neptune_client-1.1.1/LICENSE
--rw-r--r--   0        0        0    14441 2023-03-22 09:15:58.802336 neptune_client-1.1.1/README.md
--rw-r--r--   0        0        0     4932 2023-03-22 09:16:14.723039 neptune_client-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1178 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/__init__.py
--rw-r--r--   0        0        0     1218 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/__init__.py
--rw-r--r--   0        0        0     1011 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/atoms/__init__.py
--rw-r--r--   0        0        0     3048 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/atoms/artifact.py
--rw-r--r--   0        0        0      701 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/atoms/atom.py
--rw-r--r--   0        0        0     1709 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/atoms/boolean.py
--rw-r--r--   0        0        0     2121 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/atoms/copiable_atom.py
--rw-r--r--   0        0        0     2075 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/atoms/datetime.py
--rw-r--r--   0        0        0     1788 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/atoms/file.py
--rw-r--r--   0        0        0     1704 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/atoms/float.py
--rw-r--r--   0        0        0      696 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/atoms/git_ref.py
--rw-r--r--   0        0        0     1710 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/atoms/integer.py
--rw-r--r--   0        0        0      707 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/atoms/notebook_ref.py
--rw-r--r--   0        0        0      700 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/atoms/run_state.py
--rw-r--r--   0        0        0     2658 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/atoms/string.py
--rw-r--r--   0        0        0     2159 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/attribute.py
--rw-r--r--   0        0        0     2538 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/constants.py
--rw-r--r--   0        0        0     2642 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/file_set.py
--rw-r--r--   0        0        0     4266 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/namespace.py
--rw-r--r--   0        0        0      782 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/series/__init__.py
--rw-r--r--   0        0        0     1949 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/series/fetchable_series.py
--rw-r--r--   0        0        0     4292 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/series/file_series.py
--rw-r--r--   0        0        0     2802 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/series/float_series.py
--rw-r--r--   0        0        0     6364 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/series/series.py
--rw-r--r--   0        0        0     3255 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/series/string_series.py
--rw-r--r--   0        0        0      662 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/sets/__init__.py
--rw-r--r--   0        0        0      699 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/sets/set.py
--rw-r--r--   0        0        0     2627 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/sets/string_set.py
--rw-r--r--   0        0        0     2157 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/attributes/utils.py
--rw-r--r--   0        0        0      686 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/cli/__init__.py
--rw-r--r--   0        0        0     1017 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/cli/__main__.py
--rw-r--r--   0        0        0      866 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/cli/abstract_backend_runner.py
--rw-r--r--   0        0        0     3436 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/cli/clear.py
--rw-r--r--   0        0        0     5574 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/cli/commands.py
--rw-r--r--   0        0        0     2814 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/cli/container_manager.py
--rw-r--r--   0        0        0     1947 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/cli/path_option.py
--rw-r--r--   0        0        0     3899 2023-03-22 09:15:58.802336 neptune_client-1.1.1/src/neptune/cli/status.py
--rw-r--r--   0        0        0     9995 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/cli/sync.py
--rw-r--r--   0        0        0     5028 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/cli/utils.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/__init__.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/backends/__init__.py
--rw-r--r--   0        0        0     1038 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/backends/api_model.py
--rw-r--r--   0        0        0     4230 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/backends/utils.py
--rw-r--r--   0        0        0      859 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/envs.py
--rw-r--r--   0        0        0    14106 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/exceptions.py
--rw-r--r--   0        0        0      629 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/experiments.py
--rw-r--r--   0        0        0     2490 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/git_info.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/__init__.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/cgroup/__init__.py
--rw-r--r--   0        0        0     2638 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py
--rw-r--r--   0        0        0     3212 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/cgroup/cgroup_monitor.py
--rw-r--r--   0        0        0      694 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/constants.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/gauges/__init__.py
--rw-r--r--   0        0        0     1554 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/gauges/cpu.py
--rw-r--r--   0        0        0      979 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/gauges/gauge.py
--rw-r--r--   0        0        0     2023 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/gauges/gauge_factory.py
--rw-r--r--   0        0        0      667 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/gauges/gauge_mode.py
--rw-r--r--   0        0        0     1766 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/gauges/gpu.py
--rw-r--r--   0        0        0     1748 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/gauges/memory.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/gpu/__init__.py
--rw-r--r--   0        0        0     2568 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/gpu/gpu_monitor.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/metrics/__init__.py
--rw-r--r--   0        0        0     2432 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/metrics/metric.py
--rw-r--r--   0        0        0     1216 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/metrics/metrics_container.py
--rw-r--r--   0        0        0     3490 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/metrics/metrics_factory.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/metrics/reports/__init__.py
--rw-r--r--   0        0        0      792 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/metrics/reports/metric_report.py
--rw-r--r--   0        0        0     1679 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/metrics/reports/metric_reporter.py
--rw-r--r--   0        0        0      947 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/metrics/service/__init__.py
--rw-r--r--   0        0        0     1106 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/metrics/service/metric_service.py
--rw-r--r--   0        0        0     2309 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/metrics/service/metric_service_factory.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/resources/__init__.py
--rw-r--r--   0        0        0     1821 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/resources/gpu_card_indices_provider.py
--rw-r--r--   0        0        0     1574 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/resources/system_resource_info.py
--rw-r--r--   0        0        0     2504 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/resources/system_resource_info_factory.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/system/__init__.py
--rw-r--r--   0        0        0      964 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/hardware/system/system_monitor.py
--rw-r--r--   0        0        0     4772 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/oauth.py
--rw-r--r--   0        0        0      884 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/patches/__init__.py
--rw-r--r--   0        0        0     2731 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/patches/bravado.py
--rw-r--r--   0        0        0      726 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/patterns.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/storage/__init__.py
--rw-r--r--   0        0        0     3223 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/storage/datastream.py
--rw-r--r--   0        0        0     7335 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/storage/storage_utils.py
--rw-r--r--   0        0        0     7075 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/utils.py
--rw-r--r--   0        0        0     2206 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/warnings.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/websockets/__init__.py
--rw-r--r--   0        0        0     3589 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/websockets/reconnecting_websocket.py
--rw-r--r--   0        0        0     2693 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/common/websockets/websocket_client_adapter.py
--rw-r--r--   0        0        0      985 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/constants.py
--rw-r--r--   0        0        0     1863 2023-03-22 09:15:58.806336 neptune_client-1.1.1/src/neptune/envs.py
--rw-r--r--   0        0        0    41966 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/exceptions.py
--rw-r--r--   0        0        0    29698 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/handler.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/integrations/__init__.py
--rw-r--r--   0        0        0      973 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/integrations/aws/__init__.py
--rw-r--r--   0        0        0     1014 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/integrations/detectron2/__init__.py
--rw-r--r--   0        0        0      985 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/integrations/fastai/__init__.py
--rw-r--r--   0        0        0      976 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/integrations/kedro/__init__.py
--rw-r--r--   0        0        0      993 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/integrations/lightgbm/__init__.py
--rw-r--r--   0        0        0      985 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/integrations/optuna/__init__.py
--rw-r--r--   0        0        0      989 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/integrations/prophet/__init__.py
--rw-r--r--   0        0        0     3084 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/integrations/python_logger.py
--rw-r--r--   0        0        0     1042 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/integrations/pytorch_lightning/__init__.py
--rw-r--r--   0        0        0      985 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/integrations/sacred/__init__.py
--rw-r--r--   0        0        0      989 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/integrations/sklearn/__init__.py
--rw-r--r--   0        0        0     1038 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/integrations/tensorflow_keras/__init__.py
--rw-r--r--   0        0        0     1032 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/integrations/transformers/__init__.py
--rw-r--r--   0        0        0     1164 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/integrations/utils.py
--rw-r--r--   0        0        0      989 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/integrations/xgboost/__init__.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/__init__.py
--rw-r--r--   0        0        0      760 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/artifacts/__init__.py
--rw-r--r--   0        0        0      791 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/artifacts/drivers/__init__.py
--rw-r--r--   0        0        0     4240 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/artifacts/drivers/local.py
--rw-r--r--   0        0        0     4810 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/artifacts/drivers/s3.py
--rw-r--r--   0        0        0     4017 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/artifacts/file_hasher.py
--rw-r--r--   0        0        0     2318 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/artifacts/local_file_hash_storage.py
--rw-r--r--   0        0        0     3578 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/artifacts/types.py
--rw-r--r--   0        0        0      999 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/artifacts/utils.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/backends/__init__.py
--rw-r--r--   0        0        0     7169 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/backends/api_model.py
--rw-r--r--   0        0        0     1703 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/backends/factory.py
--rw-r--r--   0        0        0     6700 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/backends/hosted_artifact_operations.py
--rw-r--r--   0        0        0     5942 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/backends/hosted_client.py
--rw-r--r--   0        0        0    17136 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/backends/hosted_file_operations.py
--rw-r--r--   0        0        0    40705 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/backends/hosted_neptune_backend.py
--rw-r--r--   0        0        0     8506 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/backends/neptune_backend.py
--rw-r--r--   0        0        0    31714 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/backends/neptune_backend_mock.py
--rw-r--r--   0        0        0     1942 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/backends/nql.py
--rw-r--r--   0        0        0     4471 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/backends/offline_neptune_backend.py
--rw-r--r--   0        0        0     3946 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/backends/operation_api_name_visitor.py
--rw-r--r--   0        0        0     5003 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/backends/operation_api_object_converter.py
--rw-r--r--   0        0        0    13841 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/backends/operations_preprocessor.py
--rw-r--r--   0        0        0     1619 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/backends/project_name_lookup.py
--rw-r--r--   0        0        0     5282 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/backends/swagger_client_wrapper.py
--rw-r--r--   0        0        0     8765 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/backends/utils.py
--rw-r--r--   0        0        0     1381 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/backgroud_job_list.py
--rw-r--r--   0        0        0     1035 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/background_job.py
--rw-r--r--   0        0        0      350 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/constants.py
--rw-r--r--   0        0        0     4486 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/container_structure.py
--rw-r--r--   0        0        0     1302 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/container_type.py
--rw-r--r--   0        0        0     2345 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/credentials.py
--rw-r--r--   0        0        0     8468 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/disk_queue.py
--rw-r--r--   0        0        0      689 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/exceptions.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/hardware/__init__.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/hardware/gpu/__init__.py
--rw-r--r--   0        0        0     2466 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/hardware/gpu/gpu_monitor.py
--rw-r--r--   0        0        0     4997 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/hardware/hardware_metric_reporting_job.py
--rw-r--r--   0        0        0      933 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/id_formats.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/init/__init__.py
--rw-r--r--   0        0        0      796 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/init/parameters.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/notebooks/__init__.py
--rw-r--r--   0        0        0     1572 2023-03-22 09:15:58.810336 neptune_client-1.1.1/src/neptune/internal/notebooks/comm.py
--rw-r--r--   0        0        0     1831 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/notebooks/notebooks.py
--rw-r--r--   0        0        0    17310 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/operation.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/operation_processors/__init__.py
--rw-r--r--   0        0        0    10851 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/operation_processors/async_operation_processor.py
--rw-r--r--   0        0        0     2177 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/operation_processors/factory.py
--rw-r--r--   0        0        0     2136 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/operation_processors/offline_operation_processor.py
--rw-r--r--   0        0        0     1140 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/operation_processors/operation_processor.py
--rw-r--r--   0        0        0     1998 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/operation_processors/operation_storage.py
--rw-r--r--   0        0        0     1577 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/operation_processors/read_only_operation_processor.py
--rw-r--r--   0        0        0     2483 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/operation_processors/sync_operation_processor.py
--rw-r--r--   0        0        0     3724 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/operation_visitor.py
--rw-r--r--   0        0        0      776 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/state.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/streams/__init__.py
--rw-r--r--   0        0        0     1815 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/streams/std_capture_background_job.py
--rw-r--r--   0        0        0     2418 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/streams/std_stream_capture_logger.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/threading/__init__.py
--rw-r--r--   0        0        0     3567 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/threading/daemon.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/types/__init__.py
--rw-r--r--   0        0        0     4584 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/types/file_types.py
--rw-r--r--   0        0        0     1665 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/types/stringify_value.py
--rw-r--r--   0        0        0     4856 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/utils/__init__.py
--rw-r--r--   0        0        0     2114 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/utils/deprecation.py
--rw-r--r--   0        0        0     2374 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/utils/generic_attribute_mapper.py
--rw-r--r--   0        0        0     2568 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/utils/git.py
--rw-r--r--   0        0        0      849 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/utils/hashing.py
--rw-r--r--   0        0        0     9732 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/utils/images.py
--rw-r--r--   0        0        0     1288 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/utils/iteration.py
--rw-r--r--   0        0        0     3053 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/utils/json_file_splitter.py
--rw-r--r--   0        0        0     1633 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/utils/limits.py
--rw-r--r--   0        0        0     1488 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/utils/logger.py
--rw-r--r--   0        0        0     1042 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/utils/paths.py
--rw-r--r--   0        0        0     2049 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/utils/ping_background_job.py
--rw-r--r--   0        0        0     1809 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/utils/process_killer.py
--rw-r--r--   0        0        0     1564 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/utils/run_state.py
--rw-r--r--   0        0        0     1207 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/utils/runningmode.py
--rw-r--r--   0        0        0     1340 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/utils/s3.py
--rw-r--r--   0        0        0     2270 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/utils/source_code.py
--rw-r--r--   0        0        0     1457 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/utils/sync_offset_file.py
--rw-r--r--   0        0        0     1927 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/utils/traceback_job.py
--rw-r--r--   0        0        0     2426 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/utils/uncaught_exception_handler.py
--rw-r--r--   0        0        0     4462 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/value_to_attribute_visitor.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/websockets/__init__.py
--rw-r--r--   0        0        0     5188 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/websockets/websocket_signals_background_job.py
--rw-r--r--   0        0        0     1229 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/internal/websockets/websockets_factory.py
--rw-r--r--   0        0        0    13821 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/legacy/__init__.py
--rw-r--r--   0        0        0    11218 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/legacy/api_exceptions.py
--rw-r--r--   0        0        0     4710 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/legacy/backend.py
--rw-r--r--   0        0        0      737 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/legacy/checkpoint.py
--rw-r--r--   0        0        0      859 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/legacy/constants.py
--rw-r--r--   0        0        0      860 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/legacy/envs.py
--rw-r--r--   0        0        0    12780 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/legacy/exceptions.py
--rw-r--r--   0        0        0    42888 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/legacy/experiments.py
--rw-r--r--   0        0        0      663 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/legacy/git_info.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/legacy/internal/__init__.py
--rw-r--r--   0        0        0     1999 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/legacy/internal/abort.py
--rw-r--r--   0        0        0      888 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/legacy/internal/api_clients/__init__.py
--rw-r--r--   0        0        0     1148 2023-03-22 09:15:58.814336 neptune_client-1.1.1/src/neptune/legacy/internal/api_clients/backend_factory.py
--rw-r--r--   0        0        0     1826 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/api_clients/client_config.py
--rw-r--r--   0        0        0     3103 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/api_clients/credentials.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py
--rw-r--r--   0        0        0    46556 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py
--rw-r--r--   0        0        0     8710 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py
--rw-r--r--   0        0        0     4456 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py
--rw-r--r--   0        0        0     3857 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py
--rw-r--r--   0        0        0     4631 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/api_clients/offline_backend.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/backends/__init__.py
--rw-r--r--   0        0        0      776 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/backends/hosted_neptune_backend.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/channels/__init__.py
--rw-r--r--   0        0        0     3903 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/channels/channels.py
--rw-r--r--   0        0        0     7087 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/channels/channels_values_sender.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/execution/__init__.py
--rw-r--r--   0        0        0     6126 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/execution/execution_context.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/experiments/__init__.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/notebooks/__init__.py
--rw-r--r--   0        0        0     1510 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/notebooks/comm.py
--rw-r--r--   0        0        0     1711 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/notebooks/notebooks.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/streams/__init__.py
--rw-r--r--   0        0        0     2805 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/streams/channel_writer.py
--rw-r--r--   0        0        0     1945 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/streams/stdstream_uploader.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/threads/__init__.py
--rw-r--r--   0        0        0     2363 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/threads/aborting_thread.py
--rw-r--r--   0        0        0     1816 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py
--rw-r--r--   0        0        0     1334 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/threads/neptune_thread.py
--rw-r--r--   0        0        0     1556 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/threads/ping_thread.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/utils/__init__.py
--rw-r--r--   0        0        0     8091 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/utils/alpha_integration.py
--rw-r--r--   0        0        0      997 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/utils/deprecation.py
--rw-r--r--   0        0        0     2597 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/utils/http.py
--rw-r--r--   0        0        0     2597 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/utils/http_utils.py
--rw-r--r--   0        0        0     2990 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/utils/image.py
--rw-r--r--   0        0        0     3145 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/utils/source_code.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/websockets/__init__.py
--rw-r--r--   0        0        0     3542 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/websockets/message.py
--rw-r--r--   0        0        0     1097 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py
--rw-r--r--   0        0        0     1228 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/internal/websockets/websocket_message_processor.py
--rw-r--r--   0        0        0     3938 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/model.py
--rw-r--r--   0        0        0     2807 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/notebook.py
--rw-r--r--   0        0        0      691 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/oauth.py
--rw-r--r--   0        0        0      678 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/patterns.py
--rw-r--r--   0        0        0    26377 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/projects.py
--rw-r--r--   0        0        0     8992 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/sessions.py
--rw-r--r--   0        0        0     1162 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/legacy/utils.py
--rw-r--r--   0        0        0      660 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/logging/__init__.py
--rw-r--r--   0        0        0      976 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/logging/logger.py
--rw-r--r--   0        0        0     1457 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/management/__init__.py
--rw-r--r--   0        0        0     5352 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/management/exceptions.py
--rw-r--r--   0        0        0      596 2023-03-22 09:15:58.818336 neptune_client-1.1.1/src/neptune/management/internal/__init__.py
--rw-r--r--   0        0        0    33764 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/management/internal/api.py
--rw-r--r--   0        0        0     2853 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/management/internal/dto.py
--rw-r--r--   0        0        0     1069 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/management/internal/types.py
--rw-r--r--   0        0        0     1797 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/management/internal/utils.py
--rw-r--r--   0        0        0      995 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/metadata_containers/__init__.py
--rw-r--r--   0        0        0     2063 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/metadata_containers/abstract.py
--rw-r--r--   0        0        0    12913 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/metadata_containers/metadata_container.py
--rw-r--r--   0        0        0     9194 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/metadata_containers/metadata_containers_table.py
--rw-r--r--   0        0        0     8568 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/metadata_containers/model.py
--rw-r--r--   0        0        0     6240 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/metadata_containers/model_version.py
--rw-r--r--   0        0        0    21071 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/metadata_containers/project.py
--rw-r--r--   0        0        0    30401 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/metadata_containers/run.py
--rw-r--r--   0        0        0     2606 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/new/__init__.py
--rw-r--r--   0        0        0     1476 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/new/_compatibility.py
--rw-r--r--   0        0        0      974 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/new/constants.py
--rw-r--r--   0        0        0     1378 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/new/envs.py
--rw-r--r--   0        0        0     5846 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/new/exceptions.py
--rw-r--r--   0        0        0      655 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/new/handler.py
--rw-r--r--   0        0        0      694 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/new/project.py
--rw-r--r--   0        0        0     1672 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/new/run.py
--rw-r--r--   0        0        0     1426 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/new/runs_table.py
--rw-r--r--   0        0        0      681 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/new/utils.py
--rw-r--r--   0        0        0      696 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/new/version.py
--rw-r--r--   0        0        0     1071 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/__init__.py
--rw-r--r--   0        0        0      914 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/atoms/__init__.py
--rw-r--r--   0        0        0     1626 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/atoms/artifact.py
--rw-r--r--   0        0        0      936 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/atoms/atom.py
--rw-r--r--   0        0        0     1302 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/atoms/boolean.py
--rw-r--r--   0        0        0     1435 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/atoms/datetime.py
--rw-r--r--   0        0        0    11695 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/atoms/file.py
--rw-r--r--   0        0        0     1297 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/atoms/float.py
--rw-r--r--   0        0        0     1902 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/atoms/git_ref.py
--rw-r--r--   0        0        0     1299 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/atoms/integer.py
--rw-r--r--   0        0        0     1473 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/atoms/string.py
--rw-r--r--   0        0        0     1485 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/file_set.py
--rw-r--r--   0        0        0      831 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/mode.py
--rw-r--r--   0        0        0      777 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/model_version_stage.py
--rw-r--r--   0        0        0     1144 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/namespace.py
--rw-r--r--   0        0        0      783 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/series/__init__.py
--rw-r--r--   0        0        0     1794 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/series/file_series.py
--rw-r--r--   0        0        0     1912 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/series/float_series.py
--rw-r--r--   0        0        0     1070 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/series/series.py
--rw-r--r--   0        0        0     1353 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/series/series_value.py
--rw-r--r--   0        0        0     1923 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/series/string_series.py
--rw-r--r--   0        0        0      655 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/sets/__init__.py
--rw-r--r--   0        0        0      934 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/sets/set.py
--rw-r--r--   0        0        0     1119 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/sets/string_set.py
--rw-r--r--   0        0        0     3551 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/type_casting.py
--rw-r--r--   0        0        0      892 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/value.py
--rw-r--r--   0        0        0     1634 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/value_copy.py
--rw-r--r--   0        0        0     2596 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/types/value_visitor.py
--rw-r--r--   0        0        0      698 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/typing.py
--rw-r--r--   0        0        0     1681 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/utils.py
--rw-r--r--   0        0        0        0 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/vendor/__init__.py
--rw-r--r--   0        0        0     6306 2023-03-22 09:15:58.822337 neptune_client-1.1.1/src/neptune/vendor/lib_programname.py
--rw-r--r--   0        0        0    68552 2023-03-22 09:15:58.826337 neptune_client-1.1.1/src/neptune/vendor/pynvml.py
--rw-r--r--   0        0        0     2228 2023-03-22 09:15:58.826337 neptune_client-1.1.1/src/neptune/version.py
--rw-r--r--   0        0        0    18724 1970-01-01 00:00:00.000000 neptune_client-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    25159 2023-05-10 07:50:40.387131 neptune_client-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-05-10 07:50:40.387131 neptune_client-1.2.0/LICENSE
+-rw-r--r--   0        0        0    14357 2023-05-10 07:50:40.387131 neptune_client-1.2.0/README.md
+-rw-r--r--   0        0        0     4932 2023-05-10 07:50:58.483814 neptune_client-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3532 2023-05-10 07:50:40.387131 neptune_client-1.2.0/src/neptune/__init__.py
+-rw-r--r--   0        0        0     1218 2023-05-10 07:50:40.387131 neptune_client-1.2.0/src/neptune/attributes/__init__.py
+-rw-r--r--   0        0        0     1011 2023-05-10 07:50:40.387131 neptune_client-1.2.0/src/neptune/attributes/atoms/__init__.py
+-rw-r--r--   0        0        0     3048 2023-05-10 07:50:40.387131 neptune_client-1.2.0/src/neptune/attributes/atoms/artifact.py
+-rw-r--r--   0        0        0      701 2023-05-10 07:50:40.387131 neptune_client-1.2.0/src/neptune/attributes/atoms/atom.py
+-rw-r--r--   0        0        0     1709 2023-05-10 07:50:40.387131 neptune_client-1.2.0/src/neptune/attributes/atoms/boolean.py
+-rw-r--r--   0        0        0     2121 2023-05-10 07:50:40.387131 neptune_client-1.2.0/src/neptune/attributes/atoms/copiable_atom.py
+-rw-r--r--   0        0        0     2075 2023-05-10 07:50:40.387131 neptune_client-1.2.0/src/neptune/attributes/atoms/datetime.py
+-rw-r--r--   0        0        0     1788 2023-05-10 07:50:40.387131 neptune_client-1.2.0/src/neptune/attributes/atoms/file.py
+-rw-r--r--   0        0        0     1704 2023-05-10 07:50:40.387131 neptune_client-1.2.0/src/neptune/attributes/atoms/float.py
+-rw-r--r--   0        0        0      696 2023-05-10 07:50:40.387131 neptune_client-1.2.0/src/neptune/attributes/atoms/git_ref.py
+-rw-r--r--   0        0        0     2395 2023-05-10 07:50:40.387131 neptune_client-1.2.0/src/neptune/attributes/atoms/integer.py
+-rw-r--r--   0        0        0      707 2023-05-10 07:50:40.387131 neptune_client-1.2.0/src/neptune/attributes/atoms/notebook_ref.py
+-rw-r--r--   0        0        0      700 2023-05-10 07:50:40.387131 neptune_client-1.2.0/src/neptune/attributes/atoms/run_state.py
+-rw-r--r--   0        0        0     2658 2023-05-10 07:50:40.387131 neptune_client-1.2.0/src/neptune/attributes/atoms/string.py
+-rw-r--r--   0        0        0     2159 2023-05-10 07:50:40.387131 neptune_client-1.2.0/src/neptune/attributes/attribute.py
+-rw-r--r--   0        0        0     2538 2023-05-10 07:50:40.387131 neptune_client-1.2.0/src/neptune/attributes/constants.py
+-rw-r--r--   0        0        0     2642 2023-05-10 07:50:40.387131 neptune_client-1.2.0/src/neptune/attributes/file_set.py
+-rw-r--r--   0        0        0     4266 2023-05-10 07:50:40.387131 neptune_client-1.2.0/src/neptune/attributes/namespace.py
+-rw-r--r--   0        0        0      782 2023-05-10 07:50:40.387131 neptune_client-1.2.0/src/neptune/attributes/series/__init__.py
+-rw-r--r--   0        0        0     1949 2023-05-10 07:50:40.387131 neptune_client-1.2.0/src/neptune/attributes/series/fetchable_series.py
+-rw-r--r--   0        0        0     4292 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/attributes/series/file_series.py
+-rw-r--r--   0        0        0     2656 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/attributes/series/float_series.py
+-rw-r--r--   0        0        0     6003 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/attributes/series/series.py
+-rw-r--r--   0        0        0     3498 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/attributes/series/string_series.py
+-rw-r--r--   0        0        0      662 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/attributes/sets/__init__.py
+-rw-r--r--   0        0        0      699 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/attributes/sets/set.py
+-rw-r--r--   0        0        0     2627 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/attributes/sets/string_set.py
+-rw-r--r--   0        0        0     2157 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/attributes/utils.py
+-rw-r--r--   0        0        0      686 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/cli/__init__.py
+-rw-r--r--   0        0        0     1017 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/cli/__main__.py
+-rw-r--r--   0        0        0      866 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/cli/abstract_backend_runner.py
+-rw-r--r--   0        0        0     3436 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/cli/clear.py
+-rw-r--r--   0        0        0     5574 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/cli/commands.py
+-rw-r--r--   0        0        0     2814 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/cli/container_manager.py
+-rw-r--r--   0        0        0     1947 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/cli/path_option.py
+-rw-r--r--   0        0        0     3899 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/cli/status.py
+-rw-r--r--   0        0        0     9995 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/cli/sync.py
+-rw-r--r--   0        0        0     5028 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/cli/utils.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/common/__init__.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/common/backends/__init__.py
+-rw-r--r--   0        0        0     1038 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/common/backends/api_model.py
+-rw-r--r--   0        0        0     4230 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/common/backends/utils.py
+-rw-r--r--   0        0        0      859 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/common/envs.py
+-rw-r--r--   0        0        0    14106 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/common/exceptions.py
+-rw-r--r--   0        0        0      629 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/common/experiments.py
+-rw-r--r--   0        0        0     2490 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/common/git_info.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/common/hardware/__init__.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/common/hardware/cgroup/__init__.py
+-rw-r--r--   0        0        0     2638 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py
+-rw-r--r--   0        0        0     3212 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/common/hardware/cgroup/cgroup_monitor.py
+-rw-r--r--   0        0        0      694 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/common/hardware/constants.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/common/hardware/gauges/__init__.py
+-rw-r--r--   0        0        0     1554 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/common/hardware/gauges/cpu.py
+-rw-r--r--   0        0        0      979 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/common/hardware/gauges/gauge.py
+-rw-r--r--   0        0        0     2023 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/common/hardware/gauges/gauge_factory.py
+-rw-r--r--   0        0        0      667 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/common/hardware/gauges/gauge_mode.py
+-rw-r--r--   0        0        0     1766 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/common/hardware/gauges/gpu.py
+-rw-r--r--   0        0        0     1748 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/common/hardware/gauges/memory.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/common/hardware/gpu/__init__.py
+-rw-r--r--   0        0        0     2568 2023-05-10 07:50:40.391131 neptune_client-1.2.0/src/neptune/common/hardware/gpu/gpu_monitor.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/hardware/metrics/__init__.py
+-rw-r--r--   0        0        0     2432 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/hardware/metrics/metric.py
+-rw-r--r--   0        0        0     1216 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/hardware/metrics/metrics_container.py
+-rw-r--r--   0        0        0     3490 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/hardware/metrics/metrics_factory.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/hardware/metrics/reports/__init__.py
+-rw-r--r--   0        0        0      792 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/hardware/metrics/reports/metric_report.py
+-rw-r--r--   0        0        0     1679 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/hardware/metrics/reports/metric_reporter.py
+-rw-r--r--   0        0        0      947 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/hardware/metrics/service/__init__.py
+-rw-r--r--   0        0        0     1106 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/hardware/metrics/service/metric_service.py
+-rw-r--r--   0        0        0     2309 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/hardware/metrics/service/metric_service_factory.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/hardware/resources/__init__.py
+-rw-r--r--   0        0        0     1821 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/hardware/resources/gpu_card_indices_provider.py
+-rw-r--r--   0        0        0     1574 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/hardware/resources/system_resource_info.py
+-rw-r--r--   0        0        0     2504 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/hardware/resources/system_resource_info_factory.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/hardware/system/__init__.py
+-rw-r--r--   0        0        0      964 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/hardware/system/system_monitor.py
+-rw-r--r--   0        0        0     4772 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/oauth.py
+-rw-r--r--   0        0        0      884 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/patches/__init__.py
+-rw-r--r--   0        0        0     2731 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/patches/bravado.py
+-rw-r--r--   0        0        0      726 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/patterns.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/storage/__init__.py
+-rw-r--r--   0        0        0     3223 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/storage/datastream.py
+-rw-r--r--   0        0        0     7335 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/storage/storage_utils.py
+-rw-r--r--   0        0        0     7075 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/utils.py
+-rw-r--r--   0        0        0     2206 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/warnings.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/websockets/__init__.py
+-rw-r--r--   0        0        0     3589 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/websockets/reconnecting_websocket.py
+-rw-r--r--   0        0        0     2693 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/common/websockets/websocket_client_adapter.py
+-rw-r--r--   0        0        0      985 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/constants.py
+-rw-r--r--   0        0        0     1863 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/envs.py
+-rw-r--r--   0        0        0    41966 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/exceptions.py
+-rw-r--r--   0        0        0    29698 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/handler.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/integrations/__init__.py
+-rw-r--r--   0        0        0      973 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/integrations/aws/__init__.py
+-rw-r--r--   0        0        0     1014 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/integrations/detectron2/__init__.py
+-rw-r--r--   0        0        0      985 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/integrations/fastai/__init__.py
+-rw-r--r--   0        0        0      976 2023-05-10 07:50:40.395131 neptune_client-1.2.0/src/neptune/integrations/kedro/__init__.py
+-rw-r--r--   0        0        0      993 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/integrations/lightgbm/__init__.py
+-rw-r--r--   0        0        0      985 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/integrations/optuna/__init__.py
+-rw-r--r--   0        0        0      989 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/integrations/prophet/__init__.py
+-rw-r--r--   0        0        0     3084 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/integrations/python_logger.py
+-rw-r--r--   0        0        0     1006 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/integrations/pytorch/__init__.py
+-rw-r--r--   0        0        0     1042 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/integrations/pytorch_lightning/__init__.py
+-rw-r--r--   0        0        0      985 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/integrations/sacred/__init__.py
+-rw-r--r--   0        0        0      989 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/integrations/sklearn/__init__.py
+-rw-r--r--   0        0        0     1038 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/integrations/tensorflow_keras/__init__.py
+-rw-r--r--   0        0        0     1032 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/integrations/transformers/__init__.py
+-rw-r--r--   0        0        0     1164 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/integrations/utils.py
+-rw-r--r--   0        0        0      989 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/integrations/xgboost/__init__.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/internal/__init__.py
+-rw-r--r--   0        0        0      760 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/internal/artifacts/__init__.py
+-rw-r--r--   0        0        0      791 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/internal/artifacts/drivers/__init__.py
+-rw-r--r--   0        0        0     4240 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/internal/artifacts/drivers/local.py
+-rw-r--r--   0        0        0     4810 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/internal/artifacts/drivers/s3.py
+-rw-r--r--   0        0        0     4017 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/internal/artifacts/file_hasher.py
+-rw-r--r--   0        0        0     2318 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/internal/artifacts/local_file_hash_storage.py
+-rw-r--r--   0        0        0     3578 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/internal/artifacts/types.py
+-rw-r--r--   0        0        0      999 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/internal/artifacts/utils.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/internal/backends/__init__.py
+-rw-r--r--   0        0        0     7169 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/internal/backends/api_model.py
+-rw-r--r--   0        0        0     1703 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/internal/backends/factory.py
+-rw-r--r--   0        0        0     6700 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/internal/backends/hosted_artifact_operations.py
+-rw-r--r--   0        0        0     5942 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/internal/backends/hosted_client.py
+-rw-r--r--   0        0        0    17136 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/internal/backends/hosted_file_operations.py
+-rw-r--r--   0        0        0    40705 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/internal/backends/hosted_neptune_backend.py
+-rw-r--r--   0        0        0     8506 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/internal/backends/neptune_backend.py
+-rw-r--r--   0        0        0    31714 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/internal/backends/neptune_backend_mock.py
+-rw-r--r--   0        0        0     1942 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/internal/backends/nql.py
+-rw-r--r--   0        0        0     4471 2023-05-10 07:50:40.399131 neptune_client-1.2.0/src/neptune/internal/backends/offline_neptune_backend.py
+-rw-r--r--   0        0        0     3946 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/backends/operation_api_name_visitor.py
+-rw-r--r--   0        0        0     5003 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/backends/operation_api_object_converter.py
+-rw-r--r--   0        0        0    13841 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/backends/operations_preprocessor.py
+-rw-r--r--   0        0        0     1619 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/backends/project_name_lookup.py
+-rw-r--r--   0        0        0     5282 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/backends/swagger_client_wrapper.py
+-rw-r--r--   0        0        0     8765 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/backends/utils.py
+-rw-r--r--   0        0        0     1381 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/backgroud_job_list.py
+-rw-r--r--   0        0        0     1035 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/background_job.py
+-rw-r--r--   0        0        0      350 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/constants.py
+-rw-r--r--   0        0        0     4486 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/container_structure.py
+-rw-r--r--   0        0        0     1302 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/container_type.py
+-rw-r--r--   0        0        0     2345 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/credentials.py
+-rw-r--r--   0        0        0     8468 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/disk_queue.py
+-rw-r--r--   0        0        0      689 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/exceptions.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/hardware/__init__.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/hardware/gpu/__init__.py
+-rw-r--r--   0        0        0     2466 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/hardware/gpu/gpu_monitor.py
+-rw-r--r--   0        0        0     4997 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/hardware/hardware_metric_reporting_job.py
+-rw-r--r--   0        0        0      933 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/id_formats.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/init/__init__.py
+-rw-r--r--   0        0        0      796 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/init/parameters.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/notebooks/__init__.py
+-rw-r--r--   0        0        0     1572 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/notebooks/comm.py
+-rw-r--r--   0        0        0     1831 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/notebooks/notebooks.py
+-rw-r--r--   0        0        0    17310 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/operation.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/operation_processors/__init__.py
+-rw-r--r--   0        0        0    10851 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/operation_processors/async_operation_processor.py
+-rw-r--r--   0        0        0     2177 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/operation_processors/factory.py
+-rw-r--r--   0        0        0     2136 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/operation_processors/offline_operation_processor.py
+-rw-r--r--   0        0        0     1140 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/operation_processors/operation_processor.py
+-rw-r--r--   0        0        0     1998 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/operation_processors/operation_storage.py
+-rw-r--r--   0        0        0     1577 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/operation_processors/read_only_operation_processor.py
+-rw-r--r--   0        0        0     2483 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/operation_processors/sync_operation_processor.py
+-rw-r--r--   0        0        0     3724 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/operation_visitor.py
+-rw-r--r--   0        0        0      776 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/state.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/streams/__init__.py
+-rw-r--r--   0        0        0     1815 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/streams/std_capture_background_job.py
+-rw-r--r--   0        0        0     2418 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/streams/std_stream_capture_logger.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/threading/__init__.py
+-rw-r--r--   0        0        0     3567 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/threading/daemon.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/types/__init__.py
+-rw-r--r--   0        0        0     4584 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/types/file_types.py
+-rw-r--r--   0        0        0     1665 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/types/stringify_value.py
+-rw-r--r--   0        0        0     4856 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/utils/__init__.py
+-rw-r--r--   0        0        0     2114 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/utils/deprecation.py
+-rw-r--r--   0        0        0     2374 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/utils/generic_attribute_mapper.py
+-rw-r--r--   0        0        0     2568 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/utils/git.py
+-rw-r--r--   0        0        0      849 2023-05-10 07:50:40.403131 neptune_client-1.2.0/src/neptune/internal/utils/hashing.py
+-rw-r--r--   0        0        0     9732 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/internal/utils/images.py
+-rw-r--r--   0        0        0     1288 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/internal/utils/iteration.py
+-rw-r--r--   0        0        0     3053 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/internal/utils/json_file_splitter.py
+-rw-r--r--   0        0        0     1633 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/internal/utils/limits.py
+-rw-r--r--   0        0        0     1488 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/internal/utils/logger.py
+-rw-r--r--   0        0        0     1042 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/internal/utils/paths.py
+-rw-r--r--   0        0        0     2049 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/internal/utils/ping_background_job.py
+-rw-r--r--   0        0        0     1809 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/internal/utils/process_killer.py
+-rw-r--r--   0        0        0     1564 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/internal/utils/run_state.py
+-rw-r--r--   0        0        0     1207 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/internal/utils/runningmode.py
+-rw-r--r--   0        0        0     1340 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/internal/utils/s3.py
+-rw-r--r--   0        0        0     2270 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/internal/utils/source_code.py
+-rw-r--r--   0        0        0     1457 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/internal/utils/sync_offset_file.py
+-rw-r--r--   0        0        0     1927 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/internal/utils/traceback_job.py
+-rw-r--r--   0        0        0     2426 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/internal/utils/uncaught_exception_handler.py
+-rw-r--r--   0        0        0     4462 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/internal/value_to_attribute_visitor.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/internal/websockets/__init__.py
+-rw-r--r--   0        0        0     5188 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/internal/websockets/websocket_signals_background_job.py
+-rw-r--r--   0        0        0     1229 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/internal/websockets/websockets_factory.py
+-rw-r--r--   0        0        0    13821 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/legacy/__init__.py
+-rw-r--r--   0        0        0    11218 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/legacy/api_exceptions.py
+-rw-r--r--   0        0        0     4710 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/legacy/backend.py
+-rw-r--r--   0        0        0      737 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/legacy/checkpoint.py
+-rw-r--r--   0        0        0      859 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/legacy/constants.py
+-rw-r--r--   0        0        0      860 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/legacy/envs.py
+-rw-r--r--   0        0        0    12780 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/legacy/exceptions.py
+-rw-r--r--   0        0        0    42888 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/legacy/experiments.py
+-rw-r--r--   0        0        0      663 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/legacy/git_info.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/legacy/internal/__init__.py
+-rw-r--r--   0        0        0     1999 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/legacy/internal/abort.py
+-rw-r--r--   0        0        0      888 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/legacy/internal/api_clients/__init__.py
+-rw-r--r--   0        0        0     1148 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/legacy/internal/api_clients/backend_factory.py
+-rw-r--r--   0        0        0     1826 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/legacy/internal/api_clients/client_config.py
+-rw-r--r--   0        0        0     3103 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/legacy/internal/api_clients/credentials.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py
+-rw-r--r--   0        0        0    46556 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py
+-rw-r--r--   0        0        0     8710 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py
+-rw-r--r--   0        0        0     4456 2023-05-10 07:50:40.407131 neptune_client-1.2.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py
+-rw-r--r--   0        0        0     3857 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py
+-rw-r--r--   0        0        0     4631 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/api_clients/offline_backend.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/backends/__init__.py
+-rw-r--r--   0        0        0      776 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/backends/hosted_neptune_backend.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/channels/__init__.py
+-rw-r--r--   0        0        0     3903 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/channels/channels.py
+-rw-r--r--   0        0        0     7087 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/channels/channels_values_sender.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/execution/__init__.py
+-rw-r--r--   0        0        0     6126 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/execution/execution_context.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/experiments/__init__.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/notebooks/__init__.py
+-rw-r--r--   0        0        0     1510 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/notebooks/comm.py
+-rw-r--r--   0        0        0     1711 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/notebooks/notebooks.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/streams/__init__.py
+-rw-r--r--   0        0        0     2805 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/streams/channel_writer.py
+-rw-r--r--   0        0        0     1945 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/streams/stdstream_uploader.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/threads/__init__.py
+-rw-r--r--   0        0        0     2363 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/threads/aborting_thread.py
+-rw-r--r--   0        0        0     1816 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py
+-rw-r--r--   0        0        0     1334 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/threads/neptune_thread.py
+-rw-r--r--   0        0        0     1556 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/threads/ping_thread.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/utils/__init__.py
+-rw-r--r--   0        0        0     8091 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/utils/alpha_integration.py
+-rw-r--r--   0        0        0      997 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/utils/deprecation.py
+-rw-r--r--   0        0        0     2597 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/utils/http.py
+-rw-r--r--   0        0        0     2597 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/utils/http_utils.py
+-rw-r--r--   0        0        0     2990 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/utils/image.py
+-rw-r--r--   0        0        0     3145 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/utils/source_code.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/websockets/__init__.py
+-rw-r--r--   0        0        0     3542 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/websockets/message.py
+-rw-r--r--   0        0        0     1097 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py
+-rw-r--r--   0        0        0     1228 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/internal/websockets/websocket_message_processor.py
+-rw-r--r--   0        0        0     3938 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/model.py
+-rw-r--r--   0        0        0     2807 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/notebook.py
+-rw-r--r--   0        0        0      691 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/oauth.py
+-rw-r--r--   0        0        0      678 2023-05-10 07:50:40.411131 neptune_client-1.2.0/src/neptune/legacy/patterns.py
+-rw-r--r--   0        0        0    26377 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/legacy/projects.py
+-rw-r--r--   0        0        0     8992 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/legacy/sessions.py
+-rw-r--r--   0        0        0     1162 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/legacy/utils.py
+-rw-r--r--   0        0        0      660 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/logging/__init__.py
+-rw-r--r--   0        0        0      976 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/logging/logger.py
+-rw-r--r--   0        0        0     4454 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/management/__init__.py
+-rw-r--r--   0        0        0     5669 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/management/exceptions.py
+-rw-r--r--   0        0        0      596 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/management/internal/__init__.py
+-rw-r--r--   0        0        0    37199 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/management/internal/api.py
+-rw-r--r--   0        0        0     2853 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/management/internal/dto.py
+-rw-r--r--   0        0        0     1069 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/management/internal/types.py
+-rw-r--r--   0        0        0     2013 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/management/internal/utils.py
+-rw-r--r--   0        0        0      995 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/metadata_containers/__init__.py
+-rw-r--r--   0        0        0     2063 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/metadata_containers/abstract.py
+-rw-r--r--   0        0        0    20007 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/metadata_containers/metadata_container.py
+-rw-r--r--   0        0        0     9194 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/metadata_containers/metadata_containers_table.py
+-rw-r--r--   0        0        0    12337 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/metadata_containers/model.py
+-rw-r--r--   0        0        0    11428 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/metadata_containers/model_version.py
+-rw-r--r--   0        0        0    15433 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/metadata_containers/project.py
+-rw-r--r--   0        0        0    22678 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/metadata_containers/run.py
+-rw-r--r--   0        0        0     2606 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/new/__init__.py
+-rw-r--r--   0        0        0     1476 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/new/_compatibility.py
+-rw-r--r--   0        0        0      974 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/new/constants.py
+-rw-r--r--   0        0        0     1378 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/new/envs.py
+-rw-r--r--   0        0        0     5846 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/new/exceptions.py
+-rw-r--r--   0        0        0      655 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/new/handler.py
+-rw-r--r--   0        0        0      694 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/new/project.py
+-rw-r--r--   0        0        0     1672 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/new/run.py
+-rw-r--r--   0        0        0     1426 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/new/runs_table.py
+-rw-r--r--   0        0        0      681 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/new/utils.py
+-rw-r--r--   0        0        0      696 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/new/version.py
+-rw-r--r--   0        0        0     1071 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/types/__init__.py
+-rw-r--r--   0        0        0      914 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/types/atoms/__init__.py
+-rw-r--r--   0        0        0     1626 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/types/atoms/artifact.py
+-rw-r--r--   0        0        0      936 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/types/atoms/atom.py
+-rw-r--r--   0        0        0     1302 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/types/atoms/boolean.py
+-rw-r--r--   0        0        0     1435 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/types/atoms/datetime.py
+-rw-r--r--   0        0        0    11695 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/types/atoms/file.py
+-rw-r--r--   0        0        0     1297 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/types/atoms/float.py
+-rw-r--r--   0        0        0     1902 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/types/atoms/git_ref.py
+-rw-r--r--   0        0        0     1299 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/types/atoms/integer.py
+-rw-r--r--   0        0        0     1473 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/types/atoms/string.py
+-rw-r--r--   0        0        0     1485 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/types/file_set.py
+-rw-r--r--   0        0        0      831 2023-05-10 07:50:40.415131 neptune_client-1.2.0/src/neptune/types/mode.py
+-rw-r--r--   0        0        0      777 2023-05-10 07:50:40.419131 neptune_client-1.2.0/src/neptune/types/model_version_stage.py
+-rw-r--r--   0        0        0     1144 2023-05-10 07:50:40.419131 neptune_client-1.2.0/src/neptune/types/namespace.py
+-rw-r--r--   0        0        0      783 2023-05-10 07:50:40.419131 neptune_client-1.2.0/src/neptune/types/series/__init__.py
+-rw-r--r--   0        0        0     2447 2023-05-10 07:50:40.419131 neptune_client-1.2.0/src/neptune/types/series/file_series.py
+-rw-r--r--   0        0        0     2553 2023-05-10 07:50:40.419131 neptune_client-1.2.0/src/neptune/types/series/float_series.py
+-rw-r--r--   0        0        0     1221 2023-05-10 07:50:40.419131 neptune_client-1.2.0/src/neptune/types/series/series.py
+-rw-r--r--   0        0        0     1353 2023-05-10 07:50:40.419131 neptune_client-1.2.0/src/neptune/types/series/series_value.py
+-rw-r--r--   0        0        0     2601 2023-05-10 07:50:40.419131 neptune_client-1.2.0/src/neptune/types/series/string_series.py
+-rw-r--r--   0        0        0      655 2023-05-10 07:50:40.419131 neptune_client-1.2.0/src/neptune/types/sets/__init__.py
+-rw-r--r--   0        0        0      934 2023-05-10 07:50:40.419131 neptune_client-1.2.0/src/neptune/types/sets/set.py
+-rw-r--r--   0        0        0     1119 2023-05-10 07:50:40.419131 neptune_client-1.2.0/src/neptune/types/sets/string_set.py
+-rw-r--r--   0        0        0     3551 2023-05-10 07:50:40.419131 neptune_client-1.2.0/src/neptune/types/type_casting.py
+-rw-r--r--   0        0        0      892 2023-05-10 07:50:40.419131 neptune_client-1.2.0/src/neptune/types/value.py
+-rw-r--r--   0        0        0     1634 2023-05-10 07:50:40.419131 neptune_client-1.2.0/src/neptune/types/value_copy.py
+-rw-r--r--   0        0        0     2596 2023-05-10 07:50:40.419131 neptune_client-1.2.0/src/neptune/types/value_visitor.py
+-rw-r--r--   0        0        0      698 2023-05-10 07:50:40.419131 neptune_client-1.2.0/src/neptune/typing.py
+-rw-r--r--   0        0        0     1755 2023-05-10 07:50:40.419131 neptune_client-1.2.0/src/neptune/utils.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:50:40.419131 neptune_client-1.2.0/src/neptune/vendor/__init__.py
+-rw-r--r--   0        0        0     6306 2023-05-10 07:50:40.419131 neptune_client-1.2.0/src/neptune/vendor/lib_programname.py
+-rw-r--r--   0        0        0    68552 2023-05-10 07:50:40.419131 neptune_client-1.2.0/src/neptune/vendor/pynvml.py
+-rw-r--r--   0        0        0     2228 2023-05-10 07:50:40.419131 neptune_client-1.2.0/src/neptune/version.py
+-rw-r--r--   0        0        0    18640 1970-01-01 00:00:00.000000 neptune_client-1.2.0/PKG-INFO
```

### Comparing `neptune_client-1.1.1/CHANGELOG.md` & `neptune_client-1.2.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+## neptune 1.2.0
+
+### Changes
+- Neptune objects and universal methods covered with docstrings ([#1309](https://github.com/neptune-ai/neptune-client/pull/1309))
+- Added docstrings for Neptune packages and modules ([#1332](https://github.com/neptune-ai/neptune-client/pull/1332))
+
+### Features
+- Series objects accept `timestamps` and `steps` in their constructors ([#1318](https://github.com/neptune-ai/neptune-client/pull/1318))
+- Users can be invited to the workspace with `management` api ([#1333](https://github.com/neptune-ai/neptune-client/pull/1333))
+- Added support for `pytorch` integration ([#1337](https://github.com/neptune-ai/neptune-client/pull/1337))
+
+### Fixes
+- Print warning instead of crashing syncing thread when logging big integers ([#1336](https://github.com/neptune-ai/neptune-client/pull/1336))
+
 ## neptune 1.1.1
 
 ### Fixes
 - Fixed handling errors in case of too long filenames provided with `sys.argv` ([#1305](https://github.com/neptune-ai/neptune-client/pull/1305))
 
 ## neptune 1.1.0
```

### Comparing `neptune_client-1.1.1/LICENSE` & `neptune_client-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/README.md` & `neptune_client-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,14 @@
   <a href="https://docs.neptune.ai/">Docs</a>
   <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
   <a href="https://github.com/neptune-ai/examples">Examples</a>
   <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
   <a href="https://neptune.ai/resources">Resource center</a>
   <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
   <a href="https://neptune.ai/blog">Blog</a>
-  <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
-  <a href="https://neptune.ai/events">Podcast</a>
 &nbsp;
   <hr />
 </div>
 
 ## What is neptune.ai?
 
 neptune.ai makes it easy to log, store, organize, compare, register, and share <b>all your ML model metadata in a single place</b>.
@@ -29,15 +27,15 @@
 * Automate and standardize as your modeling team grows.
 * Collaborate on models and results with your team and across the org.
 * Use hosted, deploy on-premises, or in a private cloud. Integrate with any MLOps stack.
 &nbsp;
 
 &nbsp;
 <div align="center">
-    <a href="https://youtu.be/mv9jxexmbBk">
+    <a href="https://youtu.be/L2CAYip0DmI">
       <img border="0" alt="neptune.ai explainer video" src="https://raw.githubusercontent.com/neptune-ai/neptune-client/assets/readme/github-explainer-video.png" width="600">
     </a>
 </div>
 &nbsp;
 
 &nbsp;
 <a href="https://app.neptune.ai/showcase/example-project-tensorflow-keras/experiments?split=tbl&dash=charts&viewId=eccd5adf-42b3-497e-9cc2-9fa2655429b3"><b>Play with a live neptune.ai app →</b></a>
@@ -235,8 +233,8 @@
 &nbsp;
 
 &nbsp;
 ## People behind
 
 Created with :heart: by the [neptune.ai team](https://neptune.ai/about-us):
 
-Piotr, Paulina, Chaz, Prince, Parth, Kshitij, Siddhant, Jakub, Patrycja, Dominika, Karolina, Stephen, Artur, Aleksiej, Martyna, Małgorzata, Magdalena, Karolina, Marcin, Michał, Tymoteusz, Rafał, Aleksandra, Sabine, Tomek, Piotr, Adam, Rafał, Hubert, Marcin, Jakub, Paweł, Jakub, Franciszek, Bartosz, Aleksander, Dawid, Patryk, Krzysztof, Aurimas, and [you?](https://neptune.ai/jobs)
+Piotr, Paulina, Chaz, Prince, Parth, Kshitij, Siddhant, Jakub, Patrycja, Dominika, Karolina, Stephen, Artur, Aleksiej, Martyna, Małgorzata, Magdalena, Karolina, Marcin, Michał, Tymoteusz, Rafał, Aleksandra, Sabine, Tomek, Piotr, Rafał, Adam, Hubert, Marcin, Jakub, Paweł, Franciszek, Bartosz, Aleksander, Dawid, Patryk, Krzysztof, Aurimas, Jakub, Bartosz, and [you?](https://neptune.ai/jobs)
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
   [https://raw.githubusercontent.com/neptune-ai/neptune-client/assets/readme/
                              github-banner.jpeg]  
                            ****** neptune.ai ******
    Quickstart   â¢   Website   â¢   Docs   â¢   Examples   â¢   Resource
-                    center   â¢   Blog   â¢   Podcast  
+                            center   â¢   Blog  
 ===============================================================================
 ## What is neptune.ai? neptune.ai makes it easy to log, store, organize,
 compare, register, and share all your ML model metadata in a single place. *
 Automate and standardize as your modeling team grows. * Collaborate on models
 and results with your team and across the org. * Use hosted, deploy on-
 premises, or in a private cloud. Integrate with any MLOps stack.    
                          [neptune.ai_explainer_video]
@@ -129,10 +129,10 @@
 Chat! In the app, click the blue_message_icon in the bottom-right corner and
 send a message. A real person will talk to you ASAP (typically very ASAP). *
 You can just shoot us an email at [support@neptune.ai](mailto:
 support@neptune.ai).     ## People behind Created with :heart: by the
 [neptune.ai team](https://neptune.ai/about-us): Piotr, Paulina, Chaz, Prince,
 Parth, Kshitij, Siddhant, Jakub, Patrycja, Dominika, Karolina, Stephen, Artur,
 Aleksiej, Martyna, MaÅgorzata, Magdalena, Karolina, Marcin, MichaÅ,
-Tymoteusz, RafaÅ, Aleksandra, Sabine, Tomek, Piotr, Adam, RafaÅ, Hubert,
-Marcin, Jakub, PaweÅ, Jakub, Franciszek, Bartosz, Aleksander, Dawid, Patryk,
-Krzysztof, Aurimas, and [you?](https://neptune.ai/jobs)
+Tymoteusz, RafaÅ, Aleksandra, Sabine, Tomek, Piotr, RafaÅ, Adam, Hubert,
+Marcin, Jakub, PaweÅ, Franciszek, Bartosz, Aleksander, Dawid, Patryk,
+Krzysztof, Aurimas, Jakub, Bartosz, and [you?](https://neptune.ai/jobs)
```

### Comparing `neptune_client-1.1.1/pyproject.toml` & `neptune_client-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 repository = "https://github.com/neptune-ai/neptune-client"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune-client"
 readme = "README.md"
-version = "1.1.1"
+version = "1.2.0"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `neptune_client-1.1.1/src/neptune/__init__.py` & `neptune_client-1.2.0/src/neptune/types/sets/string_set.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 #
-# Copyright (c) 2023, Neptune Labs Sp. z o.o.
+# Copyright (c) 2022, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = [
-    "ANONYMOUS_API_TOKEN",
-    "init_model",
-    "init_model_version",
-    "init_project",
-    "init_run",
-    "Run",
-    "Model",
-    "ModelVersion",
-    "Project",
-    "__version__",
-]
-
-
-from neptune.common.patches import apply_patches
-from neptune.constants import ANONYMOUS_API_TOKEN
-from neptune.metadata_containers import (
-    Model,
-    ModelVersion,
-    Project,
-    Run,
+__all__ = ["StringSet"]
+
+from typing import (
+    TYPE_CHECKING,
+    Iterable,
+    TypeVar,
 )
-from neptune.version import __version__
 
-# Apply patches of external libraries
-apply_patches()
+from neptune.types.sets.set import Set
+
+if TYPE_CHECKING:
+    from neptune.types.value_visitor import ValueVisitor
+
+Ret = TypeVar("Ret")
+
+
+class StringSet(Set):
+    def __init__(self, values: Iterable[str]):
+        self.values = set(values)
+
+    def accept(self, visitor: "ValueVisitor[Ret]") -> Ret:
+        return visitor.visit_string_set(self)
 
-init_run = Run
-init_model = Model
-init_model_version = ModelVersion
-init_project = Project
+    def __str__(self):
+        return "StringSet({})".format(str(self.values))
```

### Comparing `neptune_client-1.1.1/src/neptune/attributes/__init__.py` & `neptune_client-1.2.0/src/neptune/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/atoms/__init__.py` & `neptune_client-1.2.0/src/neptune/attributes/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/atoms/artifact.py` & `neptune_client-1.2.0/src/neptune/attributes/atoms/artifact.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/atoms/atom.py` & `neptune_client-1.2.0/src/neptune/attributes/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/atoms/boolean.py` & `neptune_client-1.2.0/src/neptune/attributes/atoms/boolean.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/atoms/copiable_atom.py` & `neptune_client-1.2.0/src/neptune/attributes/atoms/copiable_atom.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/atoms/datetime.py` & `neptune_client-1.2.0/src/neptune/attributes/atoms/datetime.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/atoms/file.py` & `neptune_client-1.2.0/src/neptune/attributes/atoms/file.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/atoms/float.py` & `neptune_client-1.2.0/src/neptune/attributes/atoms/float.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/atoms/git_ref.py` & `neptune_client-1.2.0/src/neptune/attributes/atoms/git_ref.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/atoms/integer.py` & `neptune_client-1.2.0/src/neptune/attributes/atoms/integer.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,21 +16,26 @@
 __all__ = ["Integer"]
 
 import typing
 
 from neptune.attributes.atoms.copiable_atom import CopiableAtom
 from neptune.internal.container_type import ContainerType
 from neptune.internal.operation import AssignInt
+from neptune.internal.utils.logger import logger
 from neptune.types.atoms.integer import Integer as IntegerVal
 
 if typing.TYPE_CHECKING:
     from neptune.internal.backends.neptune_backend import NeptuneBackend
 
 
 class Integer(CopiableAtom):
+
+    MAX_32_BIT_INT = 2147483647
+    MIN_32_BIT_INT = -2147483648
+
     @staticmethod
     def create_assignment_operation(path, value: int):
         return AssignInt(path, value)
 
     @staticmethod
     def getter(
         backend: "NeptuneBackend",
@@ -41,9 +46,21 @@
         val = backend.get_int_attribute(container_id, container_type, path)
         return val.value
 
     def assign(self, value: typing.Union[IntegerVal, float, int], *, wait: bool = False):
         if not isinstance(value, IntegerVal):
             value = IntegerVal(value)
 
+        if value.value < Integer.MIN_32_BIT_INT or value.value > Integer.MAX_32_BIT_INT:
+            logger.warning(
+                "WARNING: The value you're trying to log is outside the range of 32-bit integers "
+                "(%s to %s) and will be skipped. "
+                "We'll support 64-bit integers in the future. "
+                'For now, try logging the value as a float instead: run["field"] = float(%s)',
+                Integer.MIN_32_BIT_INT,
+                Integer.MAX_32_BIT_INT,
+                value.value,
+            )
+            return
+
         with self._container.lock():
             self._enqueue_operation(self.create_assignment_operation(self._path, value.value), wait=wait)
```

### Comparing `neptune_client-1.1.1/src/neptune/attributes/atoms/notebook_ref.py` & `neptune_client-1.2.0/src/neptune/attributes/atoms/notebook_ref.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/atoms/run_state.py` & `neptune_client-1.2.0/src/neptune/attributes/atoms/run_state.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/atoms/string.py` & `neptune_client-1.2.0/src/neptune/attributes/atoms/string.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/attribute.py` & `neptune_client-1.2.0/src/neptune/attributes/attribute.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/constants.py` & `neptune_client-1.2.0/src/neptune/attributes/constants.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/file_set.py` & `neptune_client-1.2.0/src/neptune/attributes/file_set.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/namespace.py` & `neptune_client-1.2.0/src/neptune/attributes/namespace.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/series/__init__.py` & `neptune_client-1.2.0/src/neptune/attributes/series/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/series/fetchable_series.py` & `neptune_client-1.2.0/src/neptune/attributes/series/fetchable_series.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/series/file_series.py` & `neptune_client-1.2.0/src/neptune/attributes/series/file_series.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/series/float_series.py` & `neptune_client-1.2.0/src/neptune/attributes/series/float_series.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from neptune.internal.operation import (
     ClearFloatLog,
     ConfigFloatSeries,
     LogFloats,
     Operation,
 )
 from neptune.internal.utils import verify_type
-from neptune.internal.utils.logger import logger
 from neptune.types.series.float_series import FloatSeries as FloatSeriesVal
 
 Val = FloatSeriesVal
 Data = Union[float, int]
 LogOperation = LogFloats
 
 
@@ -58,17 +57,15 @@
     def _get_clear_operation(self) -> Operation:
         return ClearFloatLog(self._path)
 
     def _get_config_operation_from_value(self, value: Val) -> Optional[Operation]:
         return ConfigFloatSeries(self._path, value.min, value.max, value.unit)
 
     def _data_to_value(self, values: Iterable, **kwargs) -> Val:
-        if kwargs:
-            logger.warning("Warning: unexpected arguments (%s) in FloatSeries", kwargs)
-        return FloatSeriesVal(values)
+        return FloatSeriesVal(values, **kwargs)
 
     def _is_value_type(self, value) -> bool:
         return isinstance(value, FloatSeriesVal)
 
     def fetch_last(self) -> float:
         val = self._backend.get_float_series_attribute(self._container_id, self._container_type, self._path)
         return val.last
```

### Comparing `neptune_client-1.1.1/src/neptune/attributes/series/series.py` & `neptune_client-1.2.0/src/neptune/attributes/series/series.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,65 +12,51 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 __all__ = ["Series"]
 
 import abc
-import time
-from itertools import cycle
 from typing import (
     Collection,
     Generic,
     Iterable,
     List,
     Optional,
     TypeVar,
     Union,
 )
 
 from neptune.attributes.attribute import Attribute
 from neptune.internal.operation import LogOperation
-from neptune.internal.types.stringify_value import StringifyValue
 from neptune.internal.utils import (
     is_collection,
+    is_stringify_value,
     verify_collection_type,
     verify_type,
 )
 from neptune.internal.utils.iteration import get_batches
 from neptune.types.series.series import Series as SeriesVal
-from neptune.utils import stringify_unsupported
 
 ValTV = TypeVar("ValTV", bound=SeriesVal)
 DataTV = TypeVar("DataTV")
 LogOperationTV = TypeVar("LogOperationTV", bound=LogOperation)
 
 
 class Series(Attribute, Generic[ValTV, DataTV, LogOperationTV]):
     def __init_subclass__(cls, max_batch_size: int, operation_cls: type(LogOperationTV)):
         cls.max_batch_size = max_batch_size
         cls.operation_cls = operation_cls
 
     def clear(self, *, wait: bool = False) -> None:
         self._clear_impl(wait)
 
-    def _get_log_operations_from_value(
-        self, value: ValTV, *, steps: Union[None, Collection[float]], timestamps: Union[None, Collection[float]]
-    ) -> List[LogOperationTV]:
-        if steps is None:
-            steps = cycle([None])
-        else:
-            assert len(value) == len(steps)
-        if timestamps is None:
-            timestamps = cycle([time.time()])
-        else:
-            assert len(value) == len(timestamps)
-
+    def _get_log_operations_from_value(self, value: ValTV) -> List[LogOperationTV]:
         mapped_values = self._map_series_val(value)
-        values_with_step_and_ts = zip(mapped_values, steps, timestamps)
+        values_with_step_and_ts = zip(mapped_values, value.steps, value.timestamps)
         log_values = [self.operation_cls.ValueType(val, step=step, ts=ts) for val, step, ts in values_with_step_and_ts]
         return [
             self.operation_cls(self._path, chunk) for chunk in get_batches(log_values, batch_size=self.max_batch_size)
         ]
 
     @classmethod
     def _map_series_val(cls, value: ValTV) -> List[DataTV]:
@@ -87,91 +73,88 @@
     def _data_to_value(self, values: Iterable, **kwargs) -> ValTV:
         pass
 
     @abc.abstractmethod
     def _is_value_type(self, value) -> bool:
         pass
 
-    def assign(self, value, *, wait: bool = False) -> None:
+    def _handle_stringified_value(self, value):
+        return value.value
+
+    def assign(self, value, wait: bool = False) -> None:
         if not self._is_value_type(value):
             value = self._data_to_value(value)
         clear_op = self._get_clear_operation()
         config_op = self._get_config_operation_from_value(value)
         with self._container.lock():
             if config_op:
                 self._enqueue_operation(config_op, wait=False)
             if not value.values:
                 self._enqueue_operation(clear_op, wait=wait)
             else:
                 self._enqueue_operation(clear_op, wait=False)
-                ops = self._get_log_operations_from_value(value, steps=None, timestamps=None)
+                ops = self._get_log_operations_from_value(value)
                 for op in ops:
                     self._enqueue_operation(op, wait=wait)
 
     def log(
         self,
         value: Union[DataTV, Iterable[DataTV]],
         step: Optional[float] = None,
         timestamp: Optional[float] = None,
         wait: bool = False,
         **kwargs,
     ) -> None:
         """log is a deprecated method, this code should be removed in future"""
-        from_stringify_value = False
-        if isinstance(value, StringifyValue):
-            from_stringify_value, value = True, value.value
-
-        if is_collection(value):
-            if step is not None and len(value) > 1:
-                raise ValueError("Collection of values are not supported for explicitly defined 'step'.")
-        else:
-            value = [value]
-
-        if from_stringify_value:
-            value = stringify_unsupported(value)
-
-        value = self._data_to_value(value, **kwargs)
-
         if step is not None:
             verify_type("step", step, (float, int))
         if timestamp is not None:
             verify_type("timestamp", timestamp, (float, int))
 
-        steps = None if step is None else [step]
-        timestamps = None if timestamp is None else [timestamp] * len(value)
+        if is_stringify_value(value):
+            value = self._handle_stringified_value(value)
+
+        if is_collection(value):
+            if step is not None and len(value) > 1:
+                raise ValueError("Collection of values is not supported for explicitly defined 'step'.")
+            steps = None if step is None else [step] * len(value)
+            timestamps = None if timestamp is None else [timestamp] * len(value)
+            value = self._data_to_value(value, steps=steps, timestamps=timestamps, **kwargs)
+        else:
+            steps = None if step is None else [step]
+            timestamps = None if timestamp is None else [timestamp]
+            value = self._data_to_value([value], steps=steps, timestamps=timestamps, **kwargs)
 
-        ops = self._get_log_operations_from_value(value, steps=steps, timestamps=timestamps)
+        ops = self._get_log_operations_from_value(value)
 
         with self._container.lock():
             for op in ops:
                 self._enqueue_operation(op, wait=wait)
 
     def extend(
         self,
         values: Collection[DataTV],
-        *,
         steps: Optional[Collection[float]] = None,
         timestamps: Optional[Collection[float]] = None,
         wait: bool = False,
         **kwargs,
     ) -> None:
-        value = self._data_to_value(values, **kwargs)
-
         if steps is not None:
             verify_collection_type("steps", steps, (float, int))
-            if len(steps) != len(value):
-                raise ValueError(f"Number of steps must be equal to number of values ({len(steps)} != {len(value)}")
+            if len(steps) != len(values):
+                raise ValueError(f"Number of steps must be equal to number of values ({len(steps)} != {len(values)}")
         if timestamps is not None:
             verify_collection_type("timestamps", timestamps, (float, int))
-            if len(timestamps) != len(value):
+            if len(timestamps) != len(values):
                 raise ValueError(
-                    f"Number of timestamps must be equal to number of values ({len(timestamps)} != {len(value)}"
+                    f"Number of timestamps must be equal to number of values ({len(timestamps)} != {len(values)}"
                 )
 
-        ops = self._get_log_operations_from_value(value, steps=steps, timestamps=timestamps)
+        value = self._data_to_value(values, steps=steps, timestamps=timestamps, **kwargs)
+        ops = self._get_log_operations_from_value(value)
 
         with self._container.lock():
             for op in ops:
                 self._enqueue_operation(op, wait=wait)
 
     def _clear_impl(self, wait: bool = False) -> None:
         op = self._get_clear_operation()
```

### Comparing `neptune_client-1.1.1/src/neptune/attributes/series/string_series.py` & `neptune_client-1.2.0/src/neptune/attributes/series/string_series.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 __all__ = ["StringSeries"]
 
 from typing import (
     TYPE_CHECKING,
-    Collection,
     Iterable,
     List,
     Union,
 )
 
 from neptune.attributes.series.fetchable_series import FetchableSeries
 from neptune.attributes.series.series import Series
 from neptune.internal.backends.api_model import StringSeriesValues
 from neptune.internal.operation import (
     ClearStringLog,
     LogStrings,
     Operation,
 )
+from neptune.internal.utils import is_collection
 from neptune.internal.utils.logger import logger
 from neptune.internal.utils.paths import path_to_str
 from neptune.types.series.string_series import MAX_STRING_SERIES_VALUE_LENGTH
 from neptune.types.series.string_series import StringSeries as StringSeriesVal
 
 if TYPE_CHECKING:
     from neptune.metadata_containers import MetadataContainer
@@ -48,41 +48,50 @@
     Series[Val, Data, LogOperation], FetchableSeries[StringSeriesValues], max_batch_size=10, operation_cls=LogOperation
 ):
     def __init__(self, container: "MetadataContainer", path: List[str]):
         super().__init__(container, path)
         self._value_truncation_occurred = False
 
     def _get_log_operations_from_value(
-        self, value: Val, *, steps: Union[None, Collection[float]], timestamps: Union[None, Collection[float]]
+        self,
+        value: Val,
     ) -> List[LogOperation]:
         if not self._value_truncation_occurred and value.truncated:
             # the first truncation
             self._value_truncation_occurred = True
             logger.warning(
                 "Warning: string series '%s' value was"
                 " longer than %s characters and was truncated."
                 " This warning is printed only once per series.",
                 path_to_str(self._path),
                 MAX_STRING_SERIES_VALUE_LENGTH,
             )
 
-        return super()._get_log_operations_from_value(value, steps=steps, timestamps=timestamps)
+        return super()._get_log_operations_from_value(value)
 
     def _get_clear_operation(self) -> Operation:
         return ClearStringLog(self._path)
 
     def _data_to_value(self, values: Iterable, **kwargs) -> Val:
+        steps = kwargs.pop("steps", None)
+        timestamps = kwargs.pop("timestamps", None)
+
         if kwargs:
             logger.warning("Warning: unexpected arguments (%s) in StringSeries", kwargs)
 
-        return StringSeriesVal(values)
+        return StringSeriesVal(values, steps=steps, timestamps=timestamps)
 
     def _is_value_type(self, value) -> bool:
         return isinstance(value, StringSeriesVal)
 
+    def _handle_stringified_value(self, value) -> Union[List[str], str]:
+        if is_collection(value.value):
+            return list(map(str, value.value))
+        return str(value.value)
+
     def fetch_last(self) -> str:
         val = self._backend.get_string_series_attribute(self._container_id, self._container_type, self._path)
         return val.last
 
     def _fetch_values_from_backend(self, offset, limit) -> StringSeriesValues:
         return self._backend.get_string_series_values(
             self._container_id, self._container_type, self._path, offset, limit
```

### Comparing `neptune_client-1.1.1/src/neptune/attributes/sets/__init__.py` & `neptune_client-1.2.0/src/neptune/attributes/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/sets/set.py` & `neptune_client-1.2.0/src/neptune/attributes/sets/set.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/sets/string_set.py` & `neptune_client-1.2.0/src/neptune/attributes/sets/string_set.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/attributes/utils.py` & `neptune_client-1.2.0/src/neptune/attributes/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/cli/__init__.py` & `neptune_client-1.2.0/src/neptune/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/cli/__main__.py` & `neptune_client-1.2.0/src/neptune/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/cli/abstract_backend_runner.py` & `neptune_client-1.2.0/src/neptune/cli/abstract_backend_runner.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/cli/clear.py` & `neptune_client-1.2.0/src/neptune/cli/clear.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/cli/commands.py` & `neptune_client-1.2.0/src/neptune/cli/commands.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/cli/container_manager.py` & `neptune_client-1.2.0/src/neptune/cli/container_manager.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/cli/path_option.py` & `neptune_client-1.2.0/src/neptune/cli/path_option.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/cli/status.py` & `neptune_client-1.2.0/src/neptune/cli/status.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/cli/sync.py` & `neptune_client-1.2.0/src/neptune/cli/sync.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/cli/utils.py` & `neptune_client-1.2.0/src/neptune/cli/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/__init__.py` & `neptune_client-1.2.0/src/neptune/common/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/backends/__init__.py` & `neptune_client-1.2.0/src/neptune/common/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/backends/api_model.py` & `neptune_client-1.2.0/src/neptune/common/backends/api_model.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/backends/utils.py` & `neptune_client-1.2.0/src/neptune/common/backends/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/envs.py` & `neptune_client-1.2.0/src/neptune/common/envs.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/exceptions.py` & `neptune_client-1.2.0/src/neptune/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/experiments.py` & `neptune_client-1.2.0/src/neptune/common/experiments.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/git_info.py` & `neptune_client-1.2.0/src/neptune/common/git_info.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/__init__.py` & `neptune_client-1.2.0/src/neptune/common/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/cgroup/__init__.py` & `neptune_client-1.2.0/src/neptune/common/hardware/cgroup/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py` & `neptune_client-1.2.0/src/neptune/common/hardware/cgroup/cgroup_filesystem_reader.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/cgroup/cgroup_monitor.py` & `neptune_client-1.2.0/src/neptune/common/hardware/cgroup/cgroup_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/constants.py` & `neptune_client-1.2.0/src/neptune/common/hardware/constants.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/gauges/__init__.py` & `neptune_client-1.2.0/src/neptune/common/hardware/gauges/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/gauges/cpu.py` & `neptune_client-1.2.0/src/neptune/common/hardware/gauges/cpu.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/gauges/gauge.py` & `neptune_client-1.2.0/src/neptune/common/hardware/gauges/gauge.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/gauges/gauge_factory.py` & `neptune_client-1.2.0/src/neptune/common/hardware/gauges/gauge_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/gauges/gauge_mode.py` & `neptune_client-1.2.0/src/neptune/common/hardware/gauges/gauge_mode.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/gauges/gpu.py` & `neptune_client-1.2.0/src/neptune/common/hardware/gauges/gpu.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/gauges/memory.py` & `neptune_client-1.2.0/src/neptune/common/hardware/gauges/memory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/gpu/__init__.py` & `neptune_client-1.2.0/src/neptune/common/hardware/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/gpu/gpu_monitor.py` & `neptune_client-1.2.0/src/neptune/common/hardware/gpu/gpu_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/metrics/__init__.py` & `neptune_client-1.2.0/src/neptune/common/hardware/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/metrics/metric.py` & `neptune_client-1.2.0/src/neptune/common/hardware/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/metrics/metrics_container.py` & `neptune_client-1.2.0/src/neptune/common/hardware/metrics/metrics_container.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/metrics/metrics_factory.py` & `neptune_client-1.2.0/src/neptune/common/hardware/metrics/metrics_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/metrics/reports/__init__.py` & `neptune_client-1.2.0/src/neptune/common/hardware/metrics/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/metrics/reports/metric_report.py` & `neptune_client-1.2.0/src/neptune/common/hardware/metrics/reports/metric_report.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/metrics/reports/metric_reporter.py` & `neptune_client-1.2.0/src/neptune/common/hardware/metrics/reports/metric_reporter.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py` & `neptune_client-1.2.0/src/neptune/common/hardware/metrics/reports/metric_reporter_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/metrics/service/__init__.py` & `neptune_client-1.2.0/src/neptune/common/hardware/metrics/service/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/metrics/service/metric_service.py` & `neptune_client-1.2.0/src/neptune/common/hardware/metrics/service/metric_service.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/metrics/service/metric_service_factory.py` & `neptune_client-1.2.0/src/neptune/common/hardware/metrics/service/metric_service_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/resources/__init__.py` & `neptune_client-1.2.0/src/neptune/common/hardware/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/resources/gpu_card_indices_provider.py` & `neptune_client-1.2.0/src/neptune/common/hardware/resources/gpu_card_indices_provider.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/resources/system_resource_info.py` & `neptune_client-1.2.0/src/neptune/common/hardware/resources/system_resource_info.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/resources/system_resource_info_factory.py` & `neptune_client-1.2.0/src/neptune/common/hardware/resources/system_resource_info_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/system/__init__.py` & `neptune_client-1.2.0/src/neptune/common/hardware/system/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/hardware/system/system_monitor.py` & `neptune_client-1.2.0/src/neptune/common/hardware/system/system_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/oauth.py` & `neptune_client-1.2.0/src/neptune/common/oauth.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/patches/__init__.py` & `neptune_client-1.2.0/src/neptune/common/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/patches/bravado.py` & `neptune_client-1.2.0/src/neptune/common/patches/bravado.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/patterns.py` & `neptune_client-1.2.0/src/neptune/common/patterns.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/storage/__init__.py` & `neptune_client-1.2.0/src/neptune/common/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/storage/datastream.py` & `neptune_client-1.2.0/src/neptune/common/storage/datastream.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/storage/storage_utils.py` & `neptune_client-1.2.0/src/neptune/common/storage/storage_utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/utils.py` & `neptune_client-1.2.0/src/neptune/common/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/warnings.py` & `neptune_client-1.2.0/src/neptune/common/warnings.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/websockets/__init__.py` & `neptune_client-1.2.0/src/neptune/common/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/websockets/reconnecting_websocket.py` & `neptune_client-1.2.0/src/neptune/common/websockets/reconnecting_websocket.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/common/websockets/websocket_client_adapter.py` & `neptune_client-1.2.0/src/neptune/common/websockets/websocket_client_adapter.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/constants.py` & `neptune_client-1.2.0/src/neptune/constants.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/envs.py` & `neptune_client-1.2.0/src/neptune/envs.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/exceptions.py` & `neptune_client-1.2.0/src/neptune/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/handler.py` & `neptune_client-1.2.0/src/neptune/handler.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/integrations/__init__.py` & `neptune_client-1.2.0/src/neptune/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/integrations/aws/__init__.py` & `neptune_client-1.2.0/src/neptune/integrations/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/integrations/detectron2/__init__.py` & `neptune_client-1.2.0/src/neptune/integrations/detectron2/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/integrations/fastai/__init__.py` & `neptune_client-1.2.0/src/neptune/integrations/fastai/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/integrations/kedro/__init__.py` & `neptune_client-1.2.0/src/neptune/integrations/kedro/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/integrations/lightgbm/__init__.py` & `neptune_client-1.2.0/src/neptune/integrations/lightgbm/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/integrations/optuna/__init__.py` & `neptune_client-1.2.0/src/neptune/integrations/optuna/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/integrations/prophet/__init__.py` & `neptune_client-1.2.0/src/neptune/integrations/prophet/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/integrations/python_logger.py` & `neptune_client-1.2.0/src/neptune/integrations/python_logger.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/integrations/pytorch_lightning/__init__.py` & `neptune_client-1.2.0/src/neptune/integrations/pytorch_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/integrations/sacred/__init__.py` & `neptune_client-1.2.0/src/neptune/integrations/sacred/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/integrations/sklearn/__init__.py` & `neptune_client-1.2.0/src/neptune/integrations/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/integrations/tensorflow_keras/__init__.py` & `neptune_client-1.2.0/src/neptune/integrations/tensorflow_keras/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/integrations/transformers/__init__.py` & `neptune_client-1.2.0/src/neptune/integrations/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/integrations/utils.py` & `neptune_client-1.2.0/src/neptune/integrations/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/integrations/xgboost/__init__.py` & `neptune_client-1.2.0/src/neptune/integrations/xgboost/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/__init__.py` & `neptune_client-1.2.0/src/neptune/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/artifacts/__init__.py` & `neptune_client-1.2.0/src/neptune/internal/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/artifacts/drivers/__init__.py` & `neptune_client-1.2.0/src/neptune/internal/artifacts/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/artifacts/drivers/local.py` & `neptune_client-1.2.0/src/neptune/internal/artifacts/drivers/local.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/artifacts/drivers/s3.py` & `neptune_client-1.2.0/src/neptune/internal/artifacts/drivers/s3.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/artifacts/file_hasher.py` & `neptune_client-1.2.0/src/neptune/internal/artifacts/file_hasher.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/artifacts/local_file_hash_storage.py` & `neptune_client-1.2.0/src/neptune/internal/artifacts/local_file_hash_storage.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/artifacts/types.py` & `neptune_client-1.2.0/src/neptune/internal/artifacts/types.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/artifacts/utils.py` & `neptune_client-1.2.0/src/neptune/internal/artifacts/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/backends/__init__.py` & `neptune_client-1.2.0/src/neptune/internal/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/backends/api_model.py` & `neptune_client-1.2.0/src/neptune/internal/backends/api_model.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/backends/factory.py` & `neptune_client-1.2.0/src/neptune/internal/backends/factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/backends/hosted_artifact_operations.py` & `neptune_client-1.2.0/src/neptune/internal/backends/hosted_artifact_operations.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/backends/hosted_client.py` & `neptune_client-1.2.0/src/neptune/internal/backends/hosted_client.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/backends/hosted_file_operations.py` & `neptune_client-1.2.0/src/neptune/internal/backends/hosted_file_operations.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/backends/hosted_neptune_backend.py` & `neptune_client-1.2.0/src/neptune/internal/backends/hosted_neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/backends/neptune_backend.py` & `neptune_client-1.2.0/src/neptune/internal/backends/neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/backends/neptune_backend_mock.py` & `neptune_client-1.2.0/src/neptune/internal/backends/neptune_backend_mock.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/backends/nql.py` & `neptune_client-1.2.0/src/neptune/internal/backends/nql.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/backends/offline_neptune_backend.py` & `neptune_client-1.2.0/src/neptune/internal/backends/offline_neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/backends/operation_api_name_visitor.py` & `neptune_client-1.2.0/src/neptune/internal/backends/operation_api_name_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/backends/operation_api_object_converter.py` & `neptune_client-1.2.0/src/neptune/internal/backends/operation_api_object_converter.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/backends/operations_preprocessor.py` & `neptune_client-1.2.0/src/neptune/internal/backends/operations_preprocessor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/backends/project_name_lookup.py` & `neptune_client-1.2.0/src/neptune/internal/backends/project_name_lookup.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/backends/swagger_client_wrapper.py` & `neptune_client-1.2.0/src/neptune/internal/backends/swagger_client_wrapper.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/backends/utils.py` & `neptune_client-1.2.0/src/neptune/internal/backends/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/backgroud_job_list.py` & `neptune_client-1.2.0/src/neptune/internal/backgroud_job_list.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/background_job.py` & `neptune_client-1.2.0/src/neptune/internal/background_job.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/container_structure.py` & `neptune_client-1.2.0/src/neptune/internal/container_structure.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/container_type.py` & `neptune_client-1.2.0/src/neptune/internal/container_type.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/credentials.py` & `neptune_client-1.2.0/src/neptune/internal/credentials.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/disk_queue.py` & `neptune_client-1.2.0/src/neptune/internal/disk_queue.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/exceptions.py` & `neptune_client-1.2.0/src/neptune/internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/hardware/__init__.py` & `neptune_client-1.2.0/src/neptune/internal/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/hardware/gpu/__init__.py` & `neptune_client-1.2.0/src/neptune/internal/hardware/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/hardware/gpu/gpu_monitor.py` & `neptune_client-1.2.0/src/neptune/internal/hardware/gpu/gpu_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/hardware/hardware_metric_reporting_job.py` & `neptune_client-1.2.0/src/neptune/internal/hardware/hardware_metric_reporting_job.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/id_formats.py` & `neptune_client-1.2.0/src/neptune/internal/id_formats.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/init/__init__.py` & `neptune_client-1.2.0/src/neptune/internal/init/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/init/parameters.py` & `neptune_client-1.2.0/src/neptune/internal/init/parameters.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/notebooks/__init__.py` & `neptune_client-1.2.0/src/neptune/internal/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/notebooks/comm.py` & `neptune_client-1.2.0/src/neptune/internal/notebooks/comm.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/notebooks/notebooks.py` & `neptune_client-1.2.0/src/neptune/internal/notebooks/notebooks.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/operation.py` & `neptune_client-1.2.0/src/neptune/internal/operation.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/operation_processors/__init__.py` & `neptune_client-1.2.0/src/neptune/internal/operation_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/operation_processors/async_operation_processor.py` & `neptune_client-1.2.0/src/neptune/internal/operation_processors/async_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/operation_processors/factory.py` & `neptune_client-1.2.0/src/neptune/internal/operation_processors/factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/operation_processors/offline_operation_processor.py` & `neptune_client-1.2.0/src/neptune/internal/operation_processors/offline_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/operation_processors/operation_processor.py` & `neptune_client-1.2.0/src/neptune/internal/operation_processors/operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/operation_processors/operation_storage.py` & `neptune_client-1.2.0/src/neptune/internal/operation_processors/operation_storage.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/operation_processors/read_only_operation_processor.py` & `neptune_client-1.2.0/src/neptune/internal/operation_processors/read_only_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/operation_processors/sync_operation_processor.py` & `neptune_client-1.2.0/src/neptune/internal/operation_processors/sync_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/operation_visitor.py` & `neptune_client-1.2.0/src/neptune/internal/operation_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/state.py` & `neptune_client-1.2.0/src/neptune/internal/state.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/streams/__init__.py` & `neptune_client-1.2.0/src/neptune/internal/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/streams/std_capture_background_job.py` & `neptune_client-1.2.0/src/neptune/internal/streams/std_capture_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/streams/std_stream_capture_logger.py` & `neptune_client-1.2.0/src/neptune/internal/streams/std_stream_capture_logger.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/threading/__init__.py` & `neptune_client-1.2.0/src/neptune/internal/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/threading/daemon.py` & `neptune_client-1.2.0/src/neptune/internal/threading/daemon.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/types/__init__.py` & `neptune_client-1.2.0/src/neptune/internal/types/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/types/file_types.py` & `neptune_client-1.2.0/src/neptune/internal/types/file_types.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/types/stringify_value.py` & `neptune_client-1.2.0/src/neptune/internal/types/stringify_value.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/utils/__init__.py` & `neptune_client-1.2.0/src/neptune/internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/utils/deprecation.py` & `neptune_client-1.2.0/src/neptune/internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/utils/generic_attribute_mapper.py` & `neptune_client-1.2.0/src/neptune/internal/utils/generic_attribute_mapper.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/utils/git.py` & `neptune_client-1.2.0/src/neptune/internal/utils/git.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/utils/hashing.py` & `neptune_client-1.2.0/src/neptune/internal/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/utils/images.py` & `neptune_client-1.2.0/src/neptune/internal/utils/images.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/utils/iteration.py` & `neptune_client-1.2.0/src/neptune/internal/utils/iteration.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/utils/json_file_splitter.py` & `neptune_client-1.2.0/src/neptune/internal/utils/json_file_splitter.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/utils/limits.py` & `neptune_client-1.2.0/src/neptune/internal/utils/limits.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/utils/logger.py` & `neptune_client-1.2.0/src/neptune/internal/utils/logger.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/utils/paths.py` & `neptune_client-1.2.0/src/neptune/internal/utils/paths.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/utils/ping_background_job.py` & `neptune_client-1.2.0/src/neptune/internal/utils/ping_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/utils/process_killer.py` & `neptune_client-1.2.0/src/neptune/internal/utils/process_killer.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/utils/run_state.py` & `neptune_client-1.2.0/src/neptune/internal/utils/run_state.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/utils/runningmode.py` & `neptune_client-1.2.0/src/neptune/internal/utils/runningmode.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/utils/s3.py` & `neptune_client-1.2.0/src/neptune/internal/utils/s3.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/utils/source_code.py` & `neptune_client-1.2.0/src/neptune/internal/utils/source_code.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/utils/sync_offset_file.py` & `neptune_client-1.2.0/src/neptune/internal/utils/sync_offset_file.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/utils/traceback_job.py` & `neptune_client-1.2.0/src/neptune/internal/utils/traceback_job.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/utils/uncaught_exception_handler.py` & `neptune_client-1.2.0/src/neptune/internal/utils/uncaught_exception_handler.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/value_to_attribute_visitor.py` & `neptune_client-1.2.0/src/neptune/internal/value_to_attribute_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/websockets/__init__.py` & `neptune_client-1.2.0/src/neptune/internal/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/websockets/websocket_signals_background_job.py` & `neptune_client-1.2.0/src/neptune/internal/websockets/websocket_signals_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/internal/websockets/websockets_factory.py` & `neptune_client-1.2.0/src/neptune/internal/websockets/websockets_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/__init__.py` & `neptune_client-1.2.0/src/neptune/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/api_exceptions.py` & `neptune_client-1.2.0/src/neptune/legacy/api_exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/backend.py` & `neptune_client-1.2.0/src/neptune/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/checkpoint.py` & `neptune_client-1.2.0/src/neptune/legacy/checkpoint.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/constants.py` & `neptune_client-1.2.0/src/neptune/legacy/constants.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/envs.py` & `neptune_client-1.2.0/src/neptune/legacy/envs.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/exceptions.py` & `neptune_client-1.2.0/src/neptune/legacy/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/experiments.py` & `neptune_client-1.2.0/src/neptune/legacy/experiments.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/git_info.py` & `neptune_client-1.2.0/src/neptune/legacy/git_info.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/__init__.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/abort.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/abort.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/api_clients/__init__.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/api_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/api_clients/backend_factory.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/api_clients/backend_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/api_clients/client_config.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/api_clients/client_config.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/api_clients/credentials.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/api_clients/credentials.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_alpha_leaderboard_api_client.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/hosted_backend_api_client.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/mixins.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/api_clients/hosted_api_clients/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/api_clients/offline_backend.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/api_clients/offline_backend.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/backends/__init__.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/backends/hosted_neptune_backend.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/backends/hosted_neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/channels/__init__.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/channels/channels.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/channels/channels.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/channels/channels_values_sender.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/channels/channels_values_sender.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/execution/__init__.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/execution/execution_context.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/execution/execution_context.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/experiments/__init__.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/notebooks/__init__.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/notebooks/comm.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/notebooks/comm.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/notebooks/notebooks.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/notebooks/notebooks.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/streams/__init__.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/streams/channel_writer.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/streams/channel_writer.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/streams/stdstream_uploader.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/streams/stdstream_uploader.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/threads/__init__.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/threads/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/threads/aborting_thread.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/threads/aborting_thread.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/threads/hardware_metric_reporting_thread.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/threads/neptune_thread.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/threads/neptune_thread.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/threads/ping_thread.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/threads/ping_thread.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/utils/__init__.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/utils/alpha_integration.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/utils/alpha_integration.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/utils/deprecation.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/utils/http.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/utils/http.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/utils/http_utils.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/utils/http_utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/utils/image.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/utils/image.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/utils/source_code.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/utils/source_code.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/websockets/__init__.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/websockets/message.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/websockets/message.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/websockets/reconnecting_websocket_factory.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/internal/websockets/websocket_message_processor.py` & `neptune_client-1.2.0/src/neptune/legacy/internal/websockets/websocket_message_processor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/model.py` & `neptune_client-1.2.0/src/neptune/legacy/model.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/notebook.py` & `neptune_client-1.2.0/src/neptune/legacy/notebook.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/oauth.py` & `neptune_client-1.2.0/src/neptune/legacy/oauth.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/patterns.py` & `neptune_client-1.2.0/src/neptune/legacy/patterns.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/projects.py` & `neptune_client-1.2.0/src/neptune/legacy/projects.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/sessions.py` & `neptune_client-1.2.0/src/neptune/legacy/sessions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/legacy/utils.py` & `neptune_client-1.2.0/src/neptune/legacy/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/logging/__init__.py` & `neptune_client-1.2.0/src/neptune/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/logging/logger.py` & `neptune_client-1.2.0/src/neptune/logging/logger.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/management/exceptions.py` & `neptune_client-1.2.0/src/neptune/management/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,7 +164,17 @@
     code = 21
     description = "Can not parse '{identifier}' as identifier."
 
 
 class ObjectNotFound(ManagementOperationFailure):
     code = 22
     description = "Object not found."
+
+
+class WorkspaceOrUserNotFound(ManagementOperationFailure):
+    code = 23
+    description = "Workspace '{workspace}' or user '{user}' could not be found."
+
+
+class UserAlreadyInvited(ManagementOperationFailure):
+    code = 24
+    description = "User '{user}' has already been invited to the workspace '{workspace}'."
```

### Comparing `neptune_client-1.1.1/src/neptune/management/internal/__init__.py` & `neptune_client-1.2.0/src/neptune/management/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/management/internal/api.py` & `neptune_client-1.2.0/src/neptune/management/internal/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     "get_project_list",
     "create_project",
     "delete_project",
     "get_project_member_list",
     "add_project_member",
     "remove_project_member",
     "get_workspace_member_list",
+    "invite_to_workspace",
+    "WorkspaceMemberRole",
     "add_project_service_account",
     "remove_project_service_account",
     "get_project_service_account_list",
     "get_workspace_service_account_list",
     "trash_objects",
 ]
 
@@ -75,25 +77,28 @@
     ProjectAlreadyExists,
     ProjectNotFound,
     ProjectsLimitReached,
     ServiceAccountAlreadyHasAccess,
     ServiceAccountNotExistsOrWithoutAccess,
     ServiceAccountNotFound,
     UserAlreadyHasAccess,
+    UserAlreadyInvited,
     UserNotExistsOrWithoutAccess,
     WorkspaceNotFound,
+    WorkspaceOrUserNotFound,
 )
 from neptune.management.internal.dto import (
     ProjectMemberRoleDTO,
     ProjectVisibilityDTO,
     ServiceAccountDTO,
     WorkspaceMemberRoleDTO,
 )
 from neptune.management.internal.types import ProjectVisibility
 from neptune.management.internal.utils import (
+    WorkspaceMemberRole,
     extract_project_and_workspace,
     normalize_project_name,
 )
 
 TRASH_BATCH_SIZE = 100
 
 
@@ -560,14 +565,101 @@
     return {
         service_account_name: WorkspaceMemberRoleDTO.to_domain("member")
         for service_account_name, _ in service_accounts.items()
     }
 
 
 @with_api_exceptions_handler
+def invite_to_workspace(
+    *,
+    username: Optional[str] = None,
+    email: Optional[str] = None,
+    workspace: str,
+    api_token: Optional[str] = None,
+    role: Union[WorkspaceMemberRole, str] = WorkspaceMemberRole.MEMBER,
+    add_to_all_projects: bool = False,
+) -> None:
+    """Creates invitation to Neptune workspace.
+
+    Args:
+        username: username of the user to invite.
+        email: email of the user to invite.
+            Note: at least one of the above parameters are needed.
+            If neither the username nor the email is passed, will raise ValueError.
+            If both are filled, will raise ValueError.
+        workspace: Name of your Neptune workspace.
+        api_token: Account's API token.
+            If None, the value of the NEPTUNE_API_TOKEN environment variable is used.
+            Note: To keep your token secure, use the NEPTUNE_API_TOKEN environment variable rather than placing your
+            API token in plain text in your source code.
+        role: The workspace role that is to be granted to the invited user.
+        You can choose between the following values:
+        - Administrator: `WorkspaceMemberRole.ADMIN`
+        - Member: `WorkspaceMemberRole.MEMBER`
+        add_to_all_projects: Whether to add the user to all projects in the workspace.
+
+    Example:
+        >>> from neptune import management
+        >>> from management import WorkspaceMemberRole
+        >>> management.invite_to_workspace(
+        ...     username="user",
+        ...     workspace="ml-team",
+        ...     role=WorkspaceMemberRole.ADMIN,
+        ... )
+
+    You may also want to check the management API reference:
+    https://docs.neptune.ai/api/management
+    """
+    verify_type("workspace", workspace, str)
+    verify_type("role", role, (WorkspaceMemberRole, str))
+    verify_type("add_to_all_projects", add_to_all_projects, bool)
+    verify_type("username", username, (str, type(None)))
+    verify_type("email", email, (str, type(None)))
+    verify_type("api_token", api_token, (str, type(None)))
+
+    if username and email:
+        raise ValueError("Cannot specify both `username` and `email`.")
+
+    if username:
+        invitee = username
+        invitation_type = "user"
+    elif email:
+        invitee = email
+        invitation_type = "emailRecipient"
+    else:
+        raise ValueError("Neither `username` nor `email` arguments filled. At least one needs to be passed")
+
+    if isinstance(role, str):
+        role = WorkspaceMemberRole(role)
+
+    params = {
+        "newOrganizationInvitations": {
+            "invitationsEntries": [
+                {
+                    "invitee": invitee,
+                    "invitationType": invitation_type,
+                    "roleGrant": role.to_api(),
+                    "addToAllProjects": add_to_all_projects,
+                }
+            ],
+            "organizationIdentifier": workspace,
+        },
+        **DEFAULT_REQUEST_KWARGS,
+    }
+
+    backend_client = _get_backend_client(api_token=api_token)
+    try:
+        backend_client.api.createOrganizationInvitations(**params)
+    except HTTPNotFound:
+        raise WorkspaceOrUserNotFound(workspace=workspace, user=invitee)
+    except HTTPConflict:
+        raise UserAlreadyInvited(user=invitee, workspace=workspace)
+
+
+@with_api_exceptions_handler
 def get_project_service_account_list(
     project: str, *, workspace: Optional[str] = None, api_token: Optional[str] = None
 ) -> Dict[str, str]:
     """Lists service accounts assigned to a Neptune project.
 
     Args:
         project: The name of the project in Neptune in the form 'workspace-name/project-name'.
```

### Comparing `neptune_client-1.1.1/src/neptune/management/internal/dto.py` & `neptune_client-1.2.0/src/neptune/management/internal/dto.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/management/internal/types.py` & `neptune_client-1.2.0/src/neptune/management/internal/types.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/management/internal/utils.py` & `neptune_client-1.2.0/src/neptune/management/internal/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import re
+from enum import Enum
 from typing import Optional
 
 from neptune.common.patterns import PROJECT_QUALIFIED_NAME_PATTERN
 from neptune.management.exceptions import (
     ConflictingWorkspaceName,
     InvalidProjectName,
     MissingWorkspaceName,
@@ -46,7 +47,17 @@
     return final_workspace_name, extracted_project_name
 
 
 def normalize_project_name(name: str, workspace: Optional[str] = None):
     extracted_workspace_name, extracted_project_name = extract_project_and_workspace(name=name, workspace=workspace)
 
     return f"{extracted_workspace_name}/{extracted_project_name}"
+
+
+class WorkspaceMemberRole(Enum):
+    MEMBER = "member"
+    ADMIN = "admin"
+
+    def to_api(self) -> str:
+        if self.value == "admin":
+            return "owner"
+        return self.value
```

### Comparing `neptune_client-1.1.1/src/neptune/metadata_containers/__init__.py` & `neptune_client-1.2.0/src/neptune/metadata_containers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/metadata_containers/abstract.py` & `neptune_client-1.2.0/src/neptune/metadata_containers/abstract.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/metadata_containers/metadata_containers_table.py` & `neptune_client-1.2.0/src/neptune/metadata_containers/metadata_containers_table.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/metadata_containers/model.py` & `neptune_client-1.2.0/src/neptune/metadata_containers/model.py`

 * *Files 27% similar despite different names*

```diff
@@ -52,21 +52,15 @@
 from neptune.internal.utils.ping_background_job import PingBackgroundJob
 from neptune.metadata_containers import MetadataContainer
 from neptune.metadata_containers.metadata_containers_table import Table
 from neptune.types.mode import Mode
 
 
 class Model(MetadataContainer):
-    """A class for managing a Neptune model and retrieving information from it.
-
-    You may also want to check `Model docs page`_.
-
-    .. _Model docs page:
-       https://docs.neptune.ai/api/model
-    """
+    """Class for registering a model to neptune.ai and retrieving information from it."""
 
     container_type = ContainerType.MODEL
 
     def __init__(
         self,
         with_id: Optional[str] = None,
         *,
@@ -74,14 +68,89 @@
         key: Optional[str] = None,
         project: Optional[str] = None,
         api_token: Optional[str] = None,
         mode: Optional[str] = None,
         flush_period: float = DEFAULT_FLUSH_PERIOD,
         proxies: Optional[dict] = None,
     ):
+        """Initializes a Model object from an existing or new model.
+
+        You can use this to create a new model from code or to perform actions on existing models.
+
+        A Model object is suitable for storing model metadata that is common to all versions (you can use ModelVersion
+        objects to track version-specific metadata). It does not track background metrics or logs automatically,
+        but you can assign metadata to the Model object just like you can for runs.
+        To learn more about model registry, see the docs: https://docs.neptune.ai/model_registry/overview/
+
+        You can also use the Model object as a context manager (see examples).
+
+        Args:
+             with_id: The Neptune identifier of an existing model to resume, such as "CLS-PRE".
+                The identifier is stored in the object's "sys/id" field.
+                If omitted or `None` is passed, a new model is created.
+            name: A custom name for the model.
+            key: Key for the new model. Required when creating a new model version.
+                Used together with the project key to form the model identifier.
+                Must be uppercase and unique within the project.
+            project: Name of a project in the form `workspace-name/project-name`.
+                If None, the value of the NEPTUNE_PROJECT environment variable is used.
+            api_token: User's API token.
+                If None (default), the value of the NEPTUNE_API_TOKEN environment variable is used.
+                Note: To keep your API token secure, save it to the NEPTUNE_API_TOKEN environment variable rather than
+                placing it in plain text in the source code.
+            mode: Connection mode in which the tracking will work.
+                If `None` (default), the value of the NEPTUNE_MODE environment variable is used.
+                If no value was set for the environment variable, "async" is used by default.
+                Possible values are `async`, `sync`, `offline`, `read-only`, and `debug`.
+            flush_period: In the asynchronous (default) connection mode, how often disk flushing is triggered
+                (in seconds).
+            proxies: Argument passed to HTTP calls made via the Requests library, as dictionary of strings.
+                For more information about proxies, see the Requests documentation.
+
+        Returns:
+            Model object that is used to manage the model and log metadata to it.
+
+        Examples:
+
+            >>> import neptune
+
+            Creating a new model:
+
+            >>> model = neptune.init_model(key="PRE")
+            >>> model["metadata"] = some_metadata
+
+            >>> # Or initialize with the constructor
+            ... model = Model(key="PRE")
+
+            >>> # You can provide the project parameter as an environment variable
+            ... # or as an argument to the init_model() function:
+            ... model = neptune.init_model(key="PRE", project="workspace-name/project-name")
+
+            >>> # When creating a model, you can give it a name:
+            ... model = neptune.init_model(key="PRE", name="Pre-trained model")
+
+            Connecting to an existing model:
+
+            >>> # Initialize existing model with identifier "CLS-PRE"
+            ... model = neptune.init_model(with_id="CLS-PRE")
+
+            >>> # To prevent modifications when connecting to an existing model, you can connect in read-only mode
+            ... model = neptune.init_model(with_id="CLS-PRE", mode="read-only")
+
+            Using the Model object as context manager:
+
+            >>> with Model(key="PRE") as model:
+            ...     model["metadata"] = some_metadata
+
+        For details, see the docs:
+            Initializing a model:
+                https://docs.neptune.ai/api/neptune#init_model
+            Model class reference:
+                https://docs.neptune.ai/api/model
+        """
         verify_type("with_id", with_id, (str, type(None)))
         verify_type("name", name, (str, type(None)))
         verify_type("key", key, (str, type(None)))
         verify_type("project", project, (str, type(None)))
         verify_type("mode", mode, (str, type(None)))
 
         self._key: Optional[str] = key
@@ -184,15 +253,15 @@
 
             >>> # Sort model versions by creation time
             ... model_versions_df = model_versions_df.sort_values(by="sys/creation_time", ascending=False)
 
             >>> # Extract the last model version ID
             ... last_model_version_id = model_versions_df["sys/id"].values[0]
 
-        You may also want to check the API referene in the docs:
+        See also the API referene:
             https://docs.neptune.ai/api/model/#fetch_model_versions_table
         """
         return MetadataContainer._fetch_entries(
             self,
             child_type=ContainerType.MODEL_VERSION,
             query=NQLQueryAggregate(
                 items=[
```

### Comparing `neptune_client-1.1.1/src/neptune/metadata_containers/project.py` & `neptune_client-1.2.0/src/neptune/metadata_containers/metadata_container.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,476 +9,506 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["Project"]
+__all__ = ["MetadataContainer"]
 
-import os
+import abc
+import atexit
+import itertools
+import threading
+import time
+import traceback
+from contextlib import AbstractContextManager
+from functools import wraps
 from typing import (
     Any,
     Dict,
     Iterable,
+    List,
     Optional,
     Union,
 )
 
-from neptune.common.exceptions import NeptuneException
-from neptune.envs import CONNECTION_MODE
-from neptune.exceptions import InactiveProjectException
-from neptune.internal.backends.api_model import ApiExperiment
-from neptune.internal.backends.nql import (
-    NQLAggregator,
-    NQLAttributeOperator,
-    NQLAttributeType,
-    NQLQueryAggregate,
-    NQLQueryAttribute,
+from neptune.attributes import create_attribute_from_type
+from neptune.attributes.attribute import Attribute
+from neptune.attributes.namespace import Namespace as NamespaceAttr
+from neptune.attributes.namespace import NamespaceBuilder
+from neptune.common.exceptions import UNIX_STYLES
+from neptune.common.warnings import warn_about_unsupported_type
+from neptune.exceptions import (
+    MetadataInconsistency,
+    NeptunePossibleLegacyUsageException,
 )
+from neptune.handler import Handler
+from neptune.internal.backends.api_model import (
+    ApiExperiment,
+    AttributeType,
+    Project,
+)
+from neptune.internal.backends.factory import get_backend
+from neptune.internal.backends.neptune_backend import NeptuneBackend
+from neptune.internal.backends.nql import NQLQuery
+from neptune.internal.backends.project_name_lookup import project_name_lookup
+from neptune.internal.backgroud_job_list import BackgroundJobList
+from neptune.internal.container_structure import ContainerStructure
 from neptune.internal.container_type import ContainerType
+from neptune.internal.id_formats import (
+    QualifiedName,
+    SysId,
+    UniqueId,
+    conform_optional,
+)
 from neptune.internal.init.parameters import DEFAULT_FLUSH_PERIOD
+from neptune.internal.operation import DeleteAttribute
+from neptune.internal.operation_processors.factory import get_operation_processor
+from neptune.internal.operation_processors.operation_processor import OperationProcessor
 from neptune.internal.state import ContainerState
-from neptune.internal.utils import (
-    as_list,
-    verify_type,
-)
-from neptune.internal.utils.run_state import RunState
-from neptune.metadata_containers import MetadataContainer
+from neptune.internal.utils import verify_type
+from neptune.internal.utils.logger import logger
+from neptune.internal.utils.paths import parse_path
+from neptune.internal.utils.uncaught_exception_handler import instance as uncaught_exception_handler
+from neptune.internal.value_to_attribute_visitor import ValueToAttributeVisitor
+from neptune.metadata_containers.abstract import SupportsNamespaces
 from neptune.metadata_containers.metadata_containers_table import Table
 from neptune.types.mode import Mode
+from neptune.types.type_casting import cast_value
+
 
+def ensure_not_stopped(fun):
+    @wraps(fun)
+    def inner_fun(self: "MetadataContainer", *args, **kwargs):
+        self._raise_if_stopped()
+        return fun(self, *args, **kwargs)
 
-class Project(MetadataContainer):
-    """A class for managing a Neptune project and retrieving information from it.
+    return inner_fun
 
-    You may also want to check `Project docs page`_.
 
-    .. _Project docs page:
-       https://docs.neptune.ai/api/project
-    """
+class MetadataContainer(AbstractContextManager, SupportsNamespaces):
+    container_type: ContainerType
 
-    container_type = ContainerType.PROJECT
+    LEGACY_METHODS = set()
 
     def __init__(
         self,
-        project: Optional[str] = None,
         *,
+        project: Optional[str] = None,
         api_token: Optional[str] = None,
-        mode: Optional[str] = None,
+        mode: Mode = Mode.ASYNC,
         flush_period: float = DEFAULT_FLUSH_PERIOD,
         proxies: Optional[dict] = None,
     ):
-        verify_type("mode", mode, (str, type(None)))
-
-        # make mode proper Enum instead of string
-        mode = Mode(mode or os.getenv(CONNECTION_MODE) or Mode.ASYNC.value)
-
-        if mode == Mode.OFFLINE:
-            raise NeptuneException("Project can't be initialized in OFFLINE mode")
-
-        super().__init__(project=project, api_token=api_token, mode=mode, flush_period=flush_period, proxies=proxies)
-
-    def _get_or_create_api_object(self) -> ApiExperiment:
-        return ApiExperiment(
-            id=self._project_api_object.id,
-            type=ContainerType.PROJECT,
-            sys_id=self._project_api_object.sys_id,
-            workspace=self._project_api_object.workspace,
-            project_name=self._project_api_object.name,
+        verify_type("project", project, (str, type(None)))
+        verify_type("api_token", api_token, (str, type(None)))
+        verify_type("mode", mode, Mode)
+        verify_type("flush_period", flush_period, (int, float))
+        verify_type("proxies", proxies, (dict, type(None)))
+
+        self._mode: Mode = mode
+        self._lock: threading.RLock = threading.RLock()
+        self._state: ContainerState = ContainerState.CREATED
+
+        self._backend: NeptuneBackend = get_backend(mode=mode, api_token=api_token, proxies=proxies)
+
+        self._project_qualified_name: Optional[str] = conform_optional(project, QualifiedName)
+        self._project_api_object: Project = project_name_lookup(
+            backend=self._backend, name=self._project_qualified_name
         )
+        self._project_id: UniqueId = self._project_api_object.id
 
-    def _raise_if_stopped(self):
-        if self._state == ContainerState.STOPPED:
-            raise InactiveProjectException(label=f"{self._workspace}/{self._project_name}")
-
-    def get_url(self) -> str:
-        """Returns the URL that can be accessed within the browser"""
-        return self._backend.get_project_url(
-            project_id=self._id,
-            workspace=self._workspace,
-            project_name=self._project_name,
+        self._api_object: ApiExperiment = self._get_or_create_api_object()
+        self._id: UniqueId = self._api_object.id
+        self._sys_id: SysId = self._api_object.sys_id
+        self._workspace: str = self._api_object.workspace
+        self._project_name: str = self._api_object.project_name
+
+        self._op_processor: OperationProcessor = get_operation_processor(
+            mode=mode,
+            container_id=self._id,
+            container_type=self.container_type,
+            backend=self._backend,
+            lock=self._lock,
+            flush_period=flush_period,
         )
+        self._bg_job: BackgroundJobList = self._prepare_background_jobs_if_non_read_only()
+        self._structure: ContainerStructure[Attribute, NamespaceAttr] = ContainerStructure(NamespaceBuilder(self))
 
-    @staticmethod
-    def _prepare_nql_query(ids, states, owners, tags):
-        query_items = [
-            NQLQueryAttribute(
-                name="sys/trashed",
-                type=NQLAttributeType.BOOLEAN,
-                operator=NQLAttributeOperator.EQUALS,
-                value=False,
-            )
-        ]
-
-        if ids:
-            query_items.append(
-                NQLQueryAggregate(
-                    items=[
-                        NQLQueryAttribute(
-                            name="sys/id",
-                            type=NQLAttributeType.STRING,
-                            operator=NQLAttributeOperator.EQUALS,
-                            value=api_id,
-                        )
-                        for api_id in ids
-                    ],
-                    aggregator=NQLAggregator.OR,
-                )
-            )
-
-        if states:
-            query_items.append(
-                NQLQueryAggregate(
-                    items=[
-                        NQLQueryAttribute(
-                            name="sys/state",
-                            type=NQLAttributeType.EXPERIMENT_STATE,
-                            operator=NQLAttributeOperator.EQUALS,
-                            value=RunState.from_string(state).to_api(),
-                        )
-                        for state in states
-                    ],
-                    aggregator=NQLAggregator.OR,
-                )
-            )
+        if self._mode != Mode.OFFLINE:
+            self.sync(wait=False)
 
-        if owners:
-            query_items.append(
-                NQLQueryAggregate(
-                    items=[
-                        NQLQueryAttribute(
-                            name="sys/owner",
-                            type=NQLAttributeType.STRING,
-                            operator=NQLAttributeOperator.EQUALS,
-                            value=owner,
-                        )
-                        for owner in owners
-                    ],
-                    aggregator=NQLAggregator.OR,
-                )
-            )
+        if self._mode != Mode.READ_ONLY:
+            self._write_initial_attributes()
 
-        if tags:
-            query_items.append(
-                NQLQueryAggregate(
-                    items=[
-                        NQLQueryAttribute(
-                            name="sys/tags",
-                            type=NQLAttributeType.STRING_SET,
-                            operator=NQLAttributeOperator.CONTAINS,
-                            value=tag,
-                        )
-                        for tag in tags
-                    ],
-                    aggregator=NQLAggregator.AND,
-                )
-            )
+        self._startup(debug_mode=mode == Mode.DEBUG)
 
-        query = NQLQueryAggregate(items=query_items, aggregator=NQLAggregator.AND)
-        return query
+    def _prepare_background_jobs_if_non_read_only(self) -> BackgroundJobList:
+        if self._mode != Mode.READ_ONLY:
+            return self._prepare_background_jobs()
+        return BackgroundJobList([])
 
-    def fetch_runs_table(
-        self,
-        *,
-        id: Optional[Union[str, Iterable[str]]] = None,
-        state: Optional[Union[str, Iterable[str]]] = None,
-        owner: Optional[Union[str, Iterable[str]]] = None,
-        tag: Optional[Union[str, Iterable[str]]] = None,
-        columns: Optional[Iterable[str]] = None,
-    ) -> Table:
-        """Retrieve runs matching the specified criteria.
+    @abc.abstractmethod
+    def _get_or_create_api_object(self) -> ApiExperiment:
+        raise NotImplementedError
 
-        All parameters are optional. Each of them specifies a single criterion.
-        Only runs matching all of the criteria will be returned.
+    def _prepare_background_jobs(self) -> BackgroundJobList:
+        return BackgroundJobList([])
 
-        Args:
-            id: Neptune ID of a run, or list of several IDs.
-                Example: `"SAN-1"` or `["SAN-1", "SAN-2"]`.
-                Matching any element of the list is sufficient to pass the criterion.
-                Defaults to `None`.
-            state: Run state, or list of states.
-                Example: `"active"`.
-                Possible values: "inactive", "active".
-                Defaults to `None`.
-                Matching any element of the list is sufficient to pass the criterion.
-            owner: Username of the run owner, or a list of owners.
-                Example: `"josh"` or `["frederic", "josh"]`.
-                The owner is the user who created the run.
-                Defaults to `None`.
-                Matching any element of the list is sufficient to pass the criterion.
-            tag: A tag or list of tags applied to the run.
-                Example: `"lightGBM"` or `["pytorch", "cycleLR"]`.
-                Defaults to `None`.
-                Only runs that have all specified tags will match this criterion.
-            columns: Names of columns to include in the table, as a list of namespace or field names.
-                The Neptune ID ("sys/id") is included automatically.
-                Examples:
-                    Fields: `["params/lr", "params/batch", "train/acc"]` - these fields are included as columns.
-                    Namespaces: `["params", "train"]` - all the fields inside the namespaces are included as columns.
-                If `None` (default), all the columns of the runs table are included.
+    def _write_initial_attributes(self):
+        pass
 
-        Returns:
-            `Table` object containing `Run` objects matching the specified criteria.
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        if exc_tb is not None:
+            traceback.print_exception(exc_type, exc_val, exc_tb)
+        self.stop()
 
-            Use `to_pandas()` to convert the table to a pandas DataFrame.
+    def __getattr__(self, item):
+        if item in self.LEGACY_METHODS:
+            raise NeptunePossibleLegacyUsageException()
+        raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{item}'")
 
-        Examples:
-            >>> import neptune
-
-            >>> # Fetch project "jackie/sandbox"
-            ... project = neptune.init_project(mode="read-only", project="jackie/sandbox")
+    @abc.abstractmethod
+    def _raise_if_stopped(self):
+        raise NotImplementedError
 
-            >>> # Fetch the metadata of all runs as a pandas DataFrame
-            ... runs_table_df = project.fetch_runs_table().to_pandas()
+    def _get_subpath_suggestions(self, path_prefix: str = None, limit: int = 1000) -> List[str]:
+        parsed_path = parse_path(path_prefix or "")
+        return list(itertools.islice(self._structure.iterate_subpaths(parsed_path), limit))
 
-            >>> # Fetch the metadata of all runs as a pandas DataFrame, including only the field "train/loss"
-            ... # and the fields from the "params" namespace as columns:
-            ... runs_table_df = project.fetch_runs_table(columns=["params", "train/loss"]).to_pandas()
+    def _ipython_key_completions_(self):
+        return self._get_subpath_suggestions()
 
-            >>> # Sort runs by creation time
-            ... runs_table_df = runs_table_df.sort_values(by="sys/creation_time", ascending=False)
+    @ensure_not_stopped
+    def __getitem__(self, path: str) -> "Handler":
+        return Handler(self, path)
 
-            >>> # Extract the id of the last run
-            ... last_run_id = runs_table_df["sys/id"].values[0]
+    @ensure_not_stopped
+    def __setitem__(self, key: str, value) -> None:
+        self.__getitem__(key).assign(value)
 
-            You can also filter the runs table by state, owner, tag, or a combination of these:
+    @ensure_not_stopped
+    def __delitem__(self, path) -> None:
+        self.pop(path)
 
-            >>> # Fetch only inactive runs
-            ... runs_table_df = project.fetch_runs_table(state="Inactive").to_pandas()
+    @ensure_not_stopped
+    def assign(self, value, *, wait: bool = False) -> None:
+        """Assigns values to multiple fields from a dictionary.
 
-            >>> # Fetch only runs created by CI service
-            ... runs_table_df = project.fetch_runs_table(owner="my_company_ci_service").to_pandas()
+        You can use this method to quickly log all parameters at once.
 
-            >>> # Fetch only runs that have both "Exploration" and "Optuna" tags
-            ... runs_table_df = project.fetch_runs_table(tag=["Exploration", "Optuna"]).to_pandas()
+        Args:
+            value (dict): A dictionary with values to assign, where keys become paths of the fields.
+                The dictionary can be nested, in which case the path will be a combination of all the keys.
+            wait: If `True`, Neptune waits to send all tracked metadata to the server before executing the call.
 
-            >>> # You can combine conditions. Runs satisfying all conditions will be fetched
-            ... runs_table_df = project.fetch_runs_table(state="Inactive", tag="Exploration").to_pandas()
+        Examples:
+            >>> import neptune
+            >>> run = neptune.init_run()
+            >>> # Assign a single value with the Python "=" operator
+            >>> run["parameters/learning_rate"] = 0.8
+            >>> # or the assign() method
+            >>> run["parameters/learning_rate"].assign(0.8)
+            >>> # Assign a dictionary with the Python "=" operator
+            >>> run["parameters"] = {"max_epochs": 10, "optimizer": "Adam", "learning_rate": 0.8}
+            >>> # or the assign() method
+            >>> run.assign({"parameters": {"max_epochs": 10, "optimizer": "Adam", "learning_rate": 0.8}})
+
+            When operating on a handler object, you can use assign() to circumvent normal Python variable assignment.
+            >>> params = run["params"]
+            >>> params.assign({"max_epochs": 10, "optimizer": "Adam", "learning_rate": 0.8})
 
-        You may also want to check the API reference in the docs:
-            https://docs.neptune.ai/api/project#fetch_runs_table
+        See also the API reference:
+            https://docs.neptune.ai/api/universal/#assign
         """
-        ids = as_list("id", id)
-        states = as_list("state", state)
-        owners = as_list("owner", owner)
-        tags = as_list("tag", tag)
-
-        nql_query = self._prepare_nql_query(ids, states, owners, tags)
-
-        return MetadataContainer._fetch_entries(
-            self,
-            child_type=ContainerType.RUN,
-            query=nql_query,
-            columns=columns,
-        )
+        self._get_root_handler().assign(value, wait=wait)
 
-    def fetch_models_table(self, *, columns: Optional[Iterable[str]] = None) -> Table:
-        """Retrieve models stored in the project.
+    @ensure_not_stopped
+    def fetch(self) -> dict:
+        """Fetch values of all non-File Atom fields as a dictionary.
 
-        Args:
-            columns: Names of columns to include in the table, as a list of namespace or field names.
-                The Neptune ID ("sys/id") is included automatically.
-                Examples:
-                    Fields: `["datasets/test", "info/size"]` - these fields are included as columns.
-                    Namespaces: `["datasets", "info"]` - all the fields inside the namespaces are included as columns.
-                If `None` (default), all the columns of the models table are included.
+        You can use this method to retrieve metadata from a started or resumed run.
+        The result preserves the hierarchical structure of the run's metadata, but only contains Atom fields.
+        This means fields that contain single values, as opposed to series, files, or sets.
 
         Returns:
-            `Table` object containing `Model` objects.
-
-            Use `to_pandas()` to convert the table to a pandas DataFrame.
+            `dict` containing the values of all non-File Atom fields.
 
         Examples:
+            Resuming an existing run and fetching metadata from it:
             >>> import neptune
+            >>> resumed_run = neptune.init_run(with_id="CLS-3")
+            >>> params = resumed_run["model/parameters"].fetch()
+            >>> run_data = resumed_run.fetch()
+            >>> print(run_data)
+            >>> # prints all Atom attributes stored in run as a dict
+
+            Fetching metadata from an existing model version:
+            >>> model_version = neptune.init_model_version(with_id="CLS-TREE-45")
+            >>> optimizer = model["parameters/optimizer"].fetch()
 
-            >>> # Fetch project "jackie/sandbox"
-            ... project = neptune.init_project(mode="read-only", project="jackie/sandbox")
+        See also the API reference:
+            https://docs.neptune.ai/api/universal#fetch
+        """
+        return self._get_root_handler().fetch()
 
-            >>> # Fetch the metadata of all models as a pandas DataFrame
-            ... models_table_df = project.fetch_models_table().to_pandas()
+    def ping(self):
+        self._backend.ping(self._id, self.container_type)
 
-            >>> # Fetch the metadata of all models as a pandas DataFrame,
-            ... # including only the "datasets" namespace and "info/size" field as columns:
-            ... models_table_df = project.fetch_models_table(columns=["datasets", "info/size"]).to_pandas()
+    def start(self):
+        atexit.register(self._shutdown_hook)
+        self._op_processor.start()
+        self._bg_job.start(self)
+        self._state = ContainerState.STARTED
 
-            >>> # Sort model objects by size
-            ... models_table_df = models_table_df.sort_values(by="sys/size")
+    def stop(self, *, seconds: Optional[Union[float, int]] = None) -> None:
+        """Stops the connection and ends the synchronization thread.
 
-            >>> # Sort models by creation time
-            ... models_table_df = models_table_df.sort_values(by="sys/creation_time", ascending=False)
+        You should stop any initialized runs or other objects when the connection to them is no longer needed.
 
-            >>> # Extract the last model id
-            ... last_model_id = models_table_df["sys/id"].values[0]
+        This method is automatically called:
+        - when the script that created the run or other object finishes execution.
+        - if using a context manager, on destruction of the Neptune context.
 
-        You may also want to check the API referene in the docs:
-            https://docs.neptune.ai/api/project#fetch_models_table
-        """
-        return MetadataContainer._fetch_entries(
-            self,
-            child_type=ContainerType.MODEL,
-            query=NQLQueryAttribute(
-                name="sys/trashed",
-                type=NQLAttributeType.BOOLEAN,
-                operator=NQLAttributeOperator.EQUALS,
-                value=False,
-            ),
-            columns=columns,
-        )
+        Note: In interactive sessions, such as Jupyter Notebook, objects are stopped automatically only when
+        the Python kernel stops. However, background monitoring of system metrics and standard streams is disabled
+        unless explicitly enabled when initializing Neptune.
 
-    def assign(self, value, *, wait: bool = False) -> None:
-        """Assign values to multiple fields from a dictionary.
-        You can use this method to log multiple pieces of information with one command.
         Args:
-            value (dict): A dictionary with values to assign, where keys become the paths of the fields.
-                The dictionary can be nested - in such case the path will be a combination of all keys.
-            wait (bool, optional): If `True` the client will first wait to send all tracked metadata to the server.
-                This makes the call synchronous. Defaults to `False`.
-        Examples:
-            >>> import neptune
-            >>> project = neptune.init_project(project="MY_WORKSPACE/MY_PROJECT")
-            >>> # Assign multiple fields from a dictionary
-            ... general_info = {"brief": URL_TO_PROJECT_BRIEF, "deadline": "2049-06-30"}
-            >>> project["general"] = general_info
-            >>> # You can always log explicitly parameters one by one
-            ... project["general/brief"] = URL_TO_PROJECT_BRIEF
-            >>> project["general/deadline"] = "2049-06-30"
-            >>> # Dictionaries can be nested
-            ... general_info = {"brief": {"url": URL_TO_PROJECT_BRIEF}}
-            >>> project["general"] = general_info
-            >>> # This will log the url under path "general/brief/url"
-        You may also want to check `assign docs page`_.
-        .. _assign docs page:
-            https://docs.neptune.ai/api/project#assign
-        """
-        return MetadataContainer.assign(self, value=value, wait=wait)
+            seconds: Seconds to wait for all metadata tracking calls to finish before stopping the object.
+                If `None`, waits for all tracking calls to finish.
 
-    def fetch(self) -> dict:
-        """Fetch values of all non-File Atom fields as a dictionary.
-        The result will preserve the hierarchical structure of the projects's metadata
-        but will contain only non-File Atom fields.
-        Returns:
-            `dict` containing all non-File Atom fields values.
-        Examples:
-            >>> import neptune
-            >>> project = neptune.init_project(project="MY_WORKSPACE/MY_PROJECT")
-            >>> # Fetch all the project metrics
-            >>> project_metrics = project["metrics"].fetch()
-        You may also want to check `fetch docs page`_.
-        .. _fetch docs page:
-            https://docs.neptune.ai/api/project#fetch
-        """
-        return MetadataContainer.fetch(self)
-
-    def stop(self, *, seconds: Optional[Union[float, int]] = None) -> None:
-        """Stops the connection to the project and kills the synchronization thread.
-        `.stop()` will be automatically called when a script that initialized the connection finishes
-        or on the destruction of Neptune context.
-        When using Neptune with Jupyter notebooks it's a good practice to stop the connection manually as it
-        will be stopped automatically only when the Jupyter kernel stops.
-        Args:
-            seconds (int or float, optional): Seconds to wait for all tracking calls to finish
-                before stopping the tracked run.
-                If `None` will wait for all tracking calls to finish. Defaults to `True`.
-        Examples:
-            If you are initializing the connection from a script you don't need to call `.stop()`:
-            >>> import neptune
-            >>> project = neptune.init_project(project="MY_WORKSPACE/MY_PROJECT")
-            >>> # Your code
-            ... pass
-            ... # If you are executing Python script .stop()
-            ... # is automatically called at the end for every Neptune object
-            If you are initializing multiple connection from one script it is a good practice
-            to .stop() the unneeded connections. You can also use Context Managers - Neptune
-            will automatically call .stop() on the destruction of Project context:
+        Example:
             >>> import neptune
-            >>> # If you are initializing multiple connections from the same script
-            ... # stop the connection manually once not needed
-            ... for project_name in projects:
-            ...   project = neptune.init_project(project=project_name)
-            ...   # Your code
-            ...   pass
-            ...   project.stop()
-            >>> # You can also use with statement and context manager
-            ... for project_name in projects:
-            ...   with neptune.init_project(project=project_name) as project:
-            ...     # Your code
-            ...     pass
-            ...     # .stop() is automatically called
-            ...     # when code execution exits the with statement
-        .. warning::
-            If you are using Jupyter notebooks for connecting to a project you need to manually invoke `.stop()`
-            once the connection is not needed.
-        You may also want to check `stop docs page`_.
-        .. _stop docs page:
-            https://docs.neptune.ai/api/project#stop
+            >>> run = neptune.init_run()
+            >>> # Your training or monitoring code
+            >>> run.stop()
+
+        See also the docs:
+            Best practices - Stopping objects
+                https://docs.neptune.ai/usage/best_practices/#stopping-runs-and-other-objects
+            API reference:
+                https://docs.neptune.ai/api/universal/#stop
         """
-        return MetadataContainer.stop(self, seconds=seconds)
+        verify_type("seconds", seconds, (float, int, type(None)))
+        if self._state != ContainerState.STARTED:
+            return
+
+        self._state = ContainerState.STOPPING
+        ts = time.time()
+        logger.info("Shutting down background jobs, please wait a moment...")
+        self._bg_job.stop()
+        self._bg_job.join(seconds)
+        logger.info("Done!")
+
+        sec_left = None if seconds is None else seconds - (time.time() - ts)
+        self._op_processor.stop(sec_left)
+
+        if self._mode not in {Mode.OFFLINE, Mode.DEBUG}:
+            logger.info("Explore the metadata in the Neptune app:")
+            logger.info(self.get_url().rstrip("/") + "/metadata")
+        self._backend.close()
+        self._state = ContainerState.STOPPED
 
     def get_structure(self) -> Dict[str, Any]:
-        """Returns a project's metadata structure in form of a dictionary.
-        This method can be used to traverse the project's metadata structure programmatically
-        when using Neptune in automated workflows.
-        .. danger::
-            The returned object is a shallow copy of an internal structure.
-            Any modifications to it may result in tracking malfunction.
-        Returns:
-            ``dict``: with the project's metadata structure.
+        """Returns the object's metadata structure as a dictionary.
+
+        This method can be used to programmatically traverse the metadata structure of a run, model,
+        or project object when using Neptune in automated workflows.
+
+        Note: The returned object is a deep copy of the structure of the internal object.
+
+        See also the API reference:
+            https://docs.neptune.ai/api/universal/#get_structure
         """
-        return MetadataContainer.get_structure(self)
+        return self._structure.get_structure().to_dict()
 
     def print_structure(self) -> None:
-        """Pretty prints the structure of the project's metadata.
+        """Pretty-prints the structure of the object's metadata.
+
         Paths are ordered lexicographically and the whole structure is neatly colored.
+
+        See also: https://docs.neptune.ai/api/universal/#print_structure
         """
-        return MetadataContainer.print_structure(self)
+        self._print_structure_impl(self.get_structure(), indent=0)
+
+    def _print_structure_impl(self, struct: dict, indent: int) -> None:
+        for key in sorted(struct.keys()):
+            print("    " * indent, end="")
+            if isinstance(struct[key], dict):
+                print("{blue}'{key}'{end}:".format(blue=UNIX_STYLES["blue"], key=key, end=UNIX_STYLES["end"]))
+                self._print_structure_impl(struct[key], indent=indent + 1)
+            else:
+                print(
+                    "{blue}'{key}'{end}: {type}".format(
+                        blue=UNIX_STYLES["blue"],
+                        key=key,
+                        end=UNIX_STYLES["end"],
+                        type=type(struct[key]).__name__,
+                    )
+                )
+
+    def define(
+        self,
+        path: str,
+        value: Any,
+        *,
+        wait: bool = False,
+    ) -> Optional[Attribute]:
+        with self._lock:
+            old_attr = self.get_attribute(path)
+            if old_attr is not None:
+                raise MetadataInconsistency("Attribute or namespace {} is already defined".format(path))
+
+            neptune_value = cast_value(value)
+            if neptune_value is None:
+                warn_about_unsupported_type(type_str=str(type(value)))
+                return None
+
+            attr = ValueToAttributeVisitor(self, parse_path(path)).visit(neptune_value)
+            self.set_attribute(path, attr)
+            attr.process_assignment(neptune_value, wait=wait)
+            return attr
+
+    def get_attribute(self, path: str) -> Optional[Attribute]:
+        with self._lock:
+            return self._structure.get(parse_path(path))
+
+    def set_attribute(self, path: str, attribute: Attribute) -> Optional[Attribute]:
+        with self._lock:
+            return self._structure.set(parse_path(path), attribute)
+
+    def exists(self, path: str) -> bool:
+        """Checks if there is a field or namespace under the specified path."""
+        verify_type("path", path, str)
+        return self.get_attribute(path) is not None
 
+    @ensure_not_stopped
     def pop(self, path: str, *, wait: bool = False) -> None:
-        """Removes the field or whole namespace stored under the path completely and all data associated with them.
+        """Removes the field stored under the path and all data associated with it.
+
         Args:
-            path (str): Path of the field or namespace to be removed.
-            wait (bool, optional): If `True` the client will first wait to send all tracked metadata to the server.
-                This makes the call synchronous. Defaults to `False`.
+            path: Path of the field to be removed.
+            wait: If `True`, Neptune waits to send all tracked metadata to the server before executing the call.
+
         Examples:
             >>> import neptune
-            >>> project = neptune.init_project(project="MY_WORKSPACE/MY_PROJECT")
-            >>> # Delete a field along with it's data
-            ... project.pop("datasets/v0.4")
-            >>> # .pop() can be invoked directly on fields and namespaces
-            >>> project['parameters/learning_rate'] = 0.3
-            >>> # Following line
-            ... project.pop("datasets/v0.4")
-            >>> # is equiavlent to this line
-            ... project["datasets/v0.4"].pop()
-            >>> # or this line
-            ... project["datasets"].pop("v0.4")
-            >>> # You can also delete in batch whole namespace
-            ... project["datasets"].pop()
-        You may also want to check `pop docs page`_.
-        .. _pop docs page:
-           https://docs.neptune.ai/api/project#pop
+            >>> run = neptune.init_run()
+            >>> run["parameters/learninggg_rata"] = 0.3
+            >>> # Let's delete that misspelled field along with its data
+            ... run.pop("parameters/learninggg_rata")
+            >>> run["parameters/learning_rate"] = 0.3
+            >>> # Training finished
+            ... run["trained_model"].upload("model.pt")
+            >>> # "model_checkpoint" is a File field
+            ... run.pop("model_checkpoint")
+
+        See also the API reference:
+           https://docs.neptune.ai/api/universal/#pop
         """
-        return MetadataContainer.pop(self, path=path, wait=wait)
+        verify_type("path", path, str)
+        self._get_root_handler().pop(path, wait=wait)
+
+    def _pop_impl(self, parsed_path: List[str], *, wait: bool):
+        self._structure.pop(parsed_path)
+        self._op_processor.enqueue_operation(DeleteAttribute(parsed_path), wait=wait)
+
+    def lock(self) -> threading.RLock:
+        return self._lock
 
     def wait(self, *, disk_only=False) -> None:
-        """Wait for all the tracking calls to finish.
+        """Wait for all the queued metadata tracking calls to reach the Neptune servers.
+
         Args:
-            disk_only (bool, optional, default is False): If `True` the process will only wait for data to be saved
+            disk_only: If `True`, the process will only wait for data to be saved
                 locally from memory, but will not wait for them to reach Neptune servers.
-                Defaults to `False`.
-        You may also want to check `wait docs page`_.
-        .. _wait docs page:
-            https://docs.neptune.ai/api/project#wait
+
+        See also the API reference:
+            https://docs.neptune.ai/api/universal/#wait
         """
-        return MetadataContainer.wait(self, disk_only=disk_only)
+        with self._lock:
+            if disk_only:
+                self._op_processor.flush()
+            else:
+                self._op_processor.wait()
 
     def sync(self, *, wait: bool = True) -> None:
-        """Synchronizes local representation of the project with Neptune servers.
+        """Synchronizes the local representation of the object with the representation on the Neptune servers.
+
         Args:
-            wait (bool, optional, default is True): If `True` the process will only wait for data to be saved
+            wait: If `True`, the process will only wait for data to be saved
                 locally from memory, but will not wait for them to reach Neptune servers.
-                Defaults to `True`.
-        You may also want to check `sync docs page`_.
-        .. _sync docs page:
-            https://docs.neptune.ai/api/project#sync
+
+        Example:
+            >>> import neptune
+            >>> # Connect to a run from Worker #3
+            ... worker_id = 3
+            >>> run = neptune.init_run(with_id="DIST-43", monitoring_namespace=f"monitoring/{worker_id}")
+            >>> # Try to access logs that were created in the meantime by Worker #2
+            ... worker_2_status = run["status/2"].fetch()
+            ... # Error if this field was created after this script starts
+            >>> run.sync() # Synchronizes local representation with Neptune servers
+            >>> worker_2_status = run["status/2"].fetch()
+            ... # No error
+
+        See also the API reference:
+            https://docs.neptune.ai/api/universal/#sync
+        """
+        with self._lock:
+            if wait:
+                self._op_processor.wait()
+            attributes = self._backend.get_attributes(self._id, self.container_type)
+            self._structure.clear()
+            for attribute in attributes:
+                self._define_attribute(parse_path(attribute.path), attribute.type)
+
+    def _define_attribute(self, _path: List[str], _type: AttributeType):
+        attr = create_attribute_from_type(_type, self, _path)
+        self._structure.set(_path, attr)
+
+    def _get_root_handler(self):
+        return Handler(self, "")
+
+    @abc.abstractmethod
+    def get_url(self) -> str:
+        """Returns a link to the object in the Neptune app.
+
+        The same link is printed in the console once the object has been initialized.
+
+        API reference: https://docs.neptune.ai/api/universal/#get_url
         """
-        return MetadataContainer.sync(self, wait=wait)
+        ...
+
+    def _startup(self, debug_mode):
+        if not debug_mode:
+            logger.info(self.get_url())
+
+        self.start()
+
+        uncaught_exception_handler.activate()
+
+    def _shutdown_hook(self):
+        self.stop()
+
+    def _fetch_entries(self, child_type: ContainerType, query: NQLQuery, columns: Optional[Iterable[str]]) -> Table:
+        if columns is not None:
+            # always return entries with `sys/id` column when filter applied
+            columns = set(columns)
+            columns.add("sys/id")
+
+        leaderboard_entries = self._backend.search_leaderboard_entries(
+            project_id=self._project_id,
+            types=[child_type],
+            query=query,
+            columns=columns,
+        )
+
+        return Table(
+            backend=self._backend,
+            container_type=child_type,
+            entries=leaderboard_entries,
+        )
+
+    def get_root_object(self) -> "MetadataContainer":
+        """Returns the same Neptune object."""
+        return self
```

### Comparing `neptune_client-1.1.1/src/neptune/metadata_containers/run.py` & `neptune_client-1.2.0/src/neptune/metadata_containers/run.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 #
 __all__ = ["Run"]
 
 import os
 import threading
 from platform import node as get_hostname
 from typing import (
-    Any,
-    Dict,
     List,
     Optional,
     Tuple,
     Union,
 )
 
 from neptune.attributes.constants import (
@@ -89,54 +87,15 @@
     StringSeries,
 )
 from neptune.types.atoms.git_ref import GitRefDisabled
 from neptune.types.mode import Mode
 
 
 class Run(MetadataContainer):
-    """A Run in Neptune is a representation of all metadata that you log to Neptune.
-
-    Beginning when you start a tracked run with `neptune.init_run()` and ending when the script finishes
-    or when you explicitly stop the experiment with `.stop()`.
-
-    You can log many ML metadata types, including:
-        * metrics
-        * losses
-        * model weights
-        * images
-        * interactive charts
-        * predictions
-        * and much more
-
-    Examples:
-        >>> import neptune
-
-        >>> # Create new experiment
-        ... run = neptune.init_run(project='my_workspace/my_project')
-
-        >>> # Log parameters
-        ... params = {'max_epochs': 10, 'optimizer': 'Adam'}
-        ... run['parameters'] = params
-
-        >>> # Log metadata
-        ... run['train/metric_name'].log()
-        >>> run['predictions'].log(image)
-        >>> run['model'].upload(path_to_model)
-
-        >>> # Log whatever else you want
-        ... pass
-
-        >>> # Stop tracking and clean up
-        ... run.stop()
-
-    You may also want to check `Run docs page`_.
-
-    .. _Run docs page:
-       https://docs.neptune.ai/api/run
-    """
+    """Starts a tracked run that logs ML model-building metadata to neptune.ai."""
 
     container_type = ContainerType.RUN
 
     LEGACY_METHODS = (
         "create_experiment",
         "send_metric",
         "log_metric",
@@ -178,68 +137,87 @@
         monitoring_namespace: Optional[str] = None,
         flush_period: float = DEFAULT_FLUSH_PERIOD,
         proxies: Optional[dict] = None,
         capture_traceback: bool = True,
         git_ref: Optional[Union[GitRef, GitRefDisabled]] = None,
         **kwargs,
     ):
-        """Starts a new tracked run and adds it to the top of the runs table.
+        """Starts a new tracked run that logs ML model-building metadata to neptune.ai.
+
+        You can log metadata by assigning it to the initialized Run object:
+
+        ```
+        run = neptune.init_run()
+        run["your/structure"] = some_metadata
+        ```
+
+        Examples of metadata you can log: metrics, losses, scores, artifact versions, images, predictions,
+        model weights, parameters, checkpoints, and interactive visualizations.
+
+        By default, the run automatically tracks hardware consumption, stdout/stderr, source code, and Git information.
+        If you're using Neptune in an interactive session, however, some background monitoring needs to be enabled
+        explicitly.
 
-        If you provide the ID of an existing run, that run is resumed and no new run is created.
+        If you provide the ID of an existing run, that run is resumed and no new run is created. You may resume a run
+        either to log more metadata or to fetch metadata from it.
+
+        The run ends either when its `stop()` method is called or when the script finishes execution.
+
+        You can also use the Run object as a context manager (see examples).
 
         Args:
-            project: Name of the project where the run should go, in the form "workspace-name/project_name".
+            project: Name of the project where the run should go, in the form `workspace-name/project_name`.
             If None (default), the value of the NEPTUNE_PROJECT environment variable is used.
-            api_token: User's API token. Defaults to None.
+            api_token: User's API token.
                 If None (default), the value of the NEPTUNE_API_TOKEN environment variable is used.
                 Note: To keep your API token secure, save it to the NEPTUNE_API_TOKEN environment variable rather than
                 placing it in plain text in the source code.
-            with_id: If you want to resume a run, the identifier of the existing run.
-                For example, 'SAN-1'. A run with such an ID must exist.
+            with_id: If you want to resume a run, pass the identifier of an existing run. For example, "SAN-1".
                 If None (default) is passed, starts a new tracked run.
-            custom_run_id: A unique identifier to be used when running Neptune in pipelines.
+            custom_run_id: A unique identifier to be used when running Neptune in distributed training jobs.
                 Make sure to use the same identifier throughout the whole pipeline execution.
             mode: Connection mode in which the tracking will work.
                 If None (default), the value of the NEPTUNE_MODE environment variable is used.
-                If no value was set for the environment variable, 'async' is used by default.
-                Possible values are 'async', 'sync', 'offline', 'read-only', and 'debug'.
-            name: Editable name of the run. Defaults to 'Untitled'.
+                If no value was set for the environment variable, "async" is used by default.
+                Possible values are `async`, `sync`, `offline`, `read-only`, and `debug`.
+            name: Editable name of the run. Defaults to "Untitled".
                 The name is displayed in the run details and as a column in the runs table.
-            description: Editable description of the run. Defaults to `''`.
+            description: Editable description of the run. Defaults to `""`.
                 The description is displayed in the run details and can be added to the runs table as a column.
             tags: Tags of the run as a list of strings. Defaults to `[]`.
                 Tags are displayed in the run details and in the runs table as a column.
                 You can edit the tags after the run is created, either through the app or the API.
             source_files: List of source files to be uploaded.
-                Uploaded source files are displayed in the 'Source code' tab of the run view.
+                Uploaded source files are displayed in the "Source code" tab of the run view.
                 To not upload anything, pass an empty list (`[]`).
                 Unix style pathname pattern expansion is supported. For example, you can pass `*.py` to upload
                 all Python files from the current directory.
                 If None is passed, the Python file from which the run was created will be uploaded.
-            capture_stdout: Whether to log the stdout of the run. Defaults to True.
-                The data is logged under the monitoring namespace (see the 'monitoring_namespace' parameter).
-            capture_stderr:  Whether to log the stderr of the run. Defaults to True.
-                The data is logged under the monitoring namespace (see the 'monitoring_namespace' parameter).
+            capture_stdout: Whether to log the stdout of the run.
+                Defaults to `False` in interactive sessions and `True` otherwise.
+                The data is logged under the monitoring namespace (see the `monitoring_namespace` parameter).
+            capture_stderr: Whether to log the stderr of the run.
+                Defaults to `False` in interactive sessions and `True` otherwise.
+                The data is logged under the monitoring namespace (see the `monitoring_namespace` parameter).
             capture_hardware_metrics: Whether to send hardware monitoring logs (CPU, GPU, and memory utilization).
-                Defaults to True.
-                The data is logged under the monitoring namespace (see the 'monitoring_namespace' parameter).
+                Defaults to `False` in interactive sessions and `True` otherwise.
+                The data is logged under the monitoring namespace (see the `monitoring_namespace` parameter).
             fail_on_exception: Whether to register an uncaught exception handler to this process and,
-                in case of an exception, set the 'sys/failed' field of the run to True.
+                in case of an exception, set the "sys/failed" field of the run to `True`.
                 An exception is always logged.
             monitoring_namespace: Namespace inside which all hardware monitoring logs are stored.
-                Defaults to 'monitoring/<hash>', where the hash is generated based on environment information,
+                Defaults to "monitoring/<hash>", where the hash is generated based on environment information,
                 to ensure that it's unique for each process.
-            flush_period: In the asynchronous (default) connection mode, how often disk flushing is triggered.
-                Defaults to 5 (every 5 seconds).
+            flush_period: In the asynchronous (default) connection mode, how often disk flushing is triggered
+                (in seconds).
             proxies: Argument passed to HTTP calls made via the Requests library, as dictionary of strings.
-                For more information, see the 'Proxies' section in the Requests documentation.
-            capture_traceback:  Whether to log the traceback of the run in case of an exception.
-                Defaults to True.
-                The tracked metadata is stored in the '<monitoring_namespace>/traceback' namespace (see the
-                'monitoring_namespace' parameter).
+                For more information about proxies, see the Requests documentation.
+            capture_traceback: Whether to log the traceback of the run in case of an exception.
+                The tracked metadata is stored in the "<monitoring_namespace>/traceback" namespace (see the
+                `monitoring_namespace` parameter).
             git_ref: GitRef object containing information about the Git repository path.
                 If None, Neptune looks for a repository in the path of the script that is executed.
                 To specify a different location, set to GitRef(repository_path="path/to/repo").
                 To turn off Git tracking for the run, set to GitRef.DISABLED.
 
         Returns:
             Run object that is used to manage the tracked run and log metadata to it.
@@ -250,14 +228,17 @@
 
             >>> import neptune
 
             >>> # Minimal invoke
             ... # (creates a run in the project specified by the NEPTUNE_PROJECT environment variable)
             ... run = neptune.init_run()
 
+            >>> # Or initialize with the constructor
+            ... run = Run(project="ml-team/classification")
+
             >>> # Create a run with a name and description, with no sources files or Git info tracked:
             >>> run = neptune.init_run(
             ...     name="neural-net-mnist",
             ...     description="neural net trained on MNIST",
             ...     source_files=[],
             ...     git_ref=GitRef.DISABLED,
             ... )
@@ -286,16 +267,34 @@
             ... run = neptune.init_run(with_id="SAN-3")
             ... run["parameters/lr"] = 0.1  # modify or add metadata
 
             >>> # Initialize an existing run in read-only mode (logging new data is not possible, only fetching)
             ... run = neptune.init_run(with_id="SAN-4", mode="read-only")
             ... learning_rate = run["parameters/lr"].fetch()
 
-        For more, see the API reference:
-        https://docs.neptune.ai/api/neptune#init_run
+            Using the Run object as context manager:
+
+            >>> with Run() as run:
+            ...     run["metric"].append(value)
+
+        For more, see the docs:
+            Initializing a run:
+                https://docs.neptune.ai/api/neptune#init_run
+            Run class reference:
+                https://docs.neptune.ai/api/run/
+            Essential logging methods:
+                https://docs.neptune.ai/logging/methods/
+            Resuming a run:
+                https://docs.neptune.ai/logging/to_existing_object/
+            Setting a custom run ID:
+                https://docs.neptune.ai/logging/custom_run_id/
+            Logging to multiple runs at once:
+                https://docs.neptune.ai/logging/to_multiple_objects/
+            Accessing the run from multiple places:
+                https://docs.neptune.ai/logging/from_multiple_places/
         """
         check_for_extra_kwargs("Run", kwargs)
 
         verify_type("with_id", with_id, (str, type(None)))
         verify_type("project", project, (str, type(None)))
         verify_type("custom_run_id", custom_run_id, (str, type(None)))
         verify_type("mode", mode, (str, type(None)))
@@ -465,180 +464,14 @@
         return self._backend.get_run_url(
             run_id=self._id,
             workspace=self._workspace,
             project_name=self._project_name,
             sys_id=self._sys_id,
         )
 
-    def assign(self, value, *, wait: bool = False) -> None:
-        """Assign values to multiple fields from a dictionary.
-        You can use this method to quickly log all run's parameters.
-        Args:
-            value (dict): A dictionary with values to assign, where keys become the paths of the fields.
-                The dictionary can be nested - in such case the path will be a combination of all keys.
-            wait (bool, optional): If `True` the client will first wait to send all tracked metadata to the server.
-                This makes the call synchronous. Defaults to `False`.
-        Examples:
-            >>> import neptune
-            >>> run = neptune.init_run()
-            >>> # Assign multiple fields from a dictionary
-            ... params = {"max_epochs": 10, "optimizer": "Adam"}
-            >>> run["parameters"] = params
-            >>> # You can always log explicitly parameters one by one
-            ... run["parameters/max_epochs"] = 10
-            >>> run["parameters/optimizer"] = "Adam"
-            >>> # Dictionaries can be nested
-            ... params = {"train": {"max_epochs": 10}}
-            >>> run["parameters"] = params
-            >>> # This will log 10 under path "parameters/train/max_epochs"
-        You may also want to check `assign docs page`_.
-        .. _assign docs page:
-            https://docs.neptune.ai/api/run#assign
-        """
-        return super().assign(value=value, wait=wait)
-
-    def fetch(self) -> dict:
-        """Fetch values of all non-File Atom fields as a dictionary.
-        The result will preserve the hierarchical structure of the run's metadata, but will contain only non-File Atom
-        fields.
-        You can use this method to quickly retrieve previous run's parameters.
-        Returns:
-            `dict` containing all non-File Atom fields values.
-        Examples:
-            >>> import neptune
-            >>> resumed_run = neptune.init_run(with_id="HEL-3")
-            >>> params = resumed_run['model/parameters'].fetch()
-            >>> run_data = resumed_run.fetch()
-            >>> print(run_data)
-            >>> # this will print out all Atom attributes stored in run as a dict
-        You may also want to check `fetch docs page`_.
-        .. _fetch docs page:
-            https://docs.neptune.ai/api/run#fetch
-        """
-        return super().fetch()
-
-    def stop(self, *, seconds: Optional[Union[float, int]] = None) -> None:
-        """Stops the tracked run and kills the synchronization thread.
-        `.stop()` will be automatically called when a script that created the run finishes or on the destruction
-        of Neptune context.
-        When using Neptune with Jupyter notebooks it's a good practice to stop the tracked run manually as it
-        will be stopped automatically only when the Jupyter kernel stops.
-        Args:
-            seconds (int or float, optional): Seconds to wait for all tracking calls to finish
-                before stopping the tracked run.
-                If `None` will wait for all tracking calls to finish. Defaults to `True`.
-        Examples:
-            If you are creating tracked runs from the script you don't need to call `.stop()`:
-            >>> import neptune
-            >>> run = neptune.init_run()
-            >>> # Your training or monitoring code
-            ... pass
-            ... # If you are executing Python script .stop()
-            ... # is automatically called at the end for every run
-            If you are performing multiple training jobs from one script one after the other it is a good practice
-            to `.stop()` the finished tracked runs as every open run keeps an open connection with Neptune,
-            monitors hardware usage, etc. You can also use Context Managers - Neptune will automatically call `.stop()`
-            on the destruction of Run context:
-            >>> import neptune
-            >>> # If you are running consecutive training jobs from the same script
-            ... # stop the tracked runs manually at the end of single training job
-            ... for config in configs:
-            ...   run = neptune.init_run()
-            ...   # Your training or monitoring code
-            ...   pass
-            ...   run.stop()
-            >>> # You can also use with statement and context manager
-            ... for config in configs:
-            ...   with neptune.init_run() as run:
-            ...     # Your training or monitoring code
-            ...     pass
-            ...     # .stop() is automatically called
-            ...     # when code execution exits the with statement
-        .. warning::
-            If you are using Jupyter notebooks for creating your runs you need to manually invoke `.stop()` once the
-            training and evaluation is done.
-        You may also want to check `stop docs page`_.
-        .. _stop docs page:
-            https://docs.neptune.ai/api/run#stop
-        """
-        return super().stop(seconds=seconds)
-
-    def get_structure(self) -> Dict[str, Any]:
-        """Returns a run's metadata structure in form of a dictionary.
-        This method can be used to traverse the run's metadata structure programmatically
-        when using Neptune in automated workflows.
-        .. danger::
-            The returned object is a deep copy of an internal run's structure.
-        Returns:
-            ``dict``: with the run's metadata structure.
-        """
-        return super().get_structure()
-
-    def print_structure(self) -> None:
-        """Pretty prints the structure of the run's metadata.
-        Paths are ordered lexicographically and the whole structure is neatly colored.
-        """
-        return super().print_structure()
-
-    def pop(self, path: str, *, wait: bool = False) -> None:
-        """Removes the field stored under the path completely and all data associated with it.
-        Args:
-            path (str): Path of the field to be removed.
-            wait (bool, optional): If `True` the client will first wait to send all tracked metadata to the server.
-                This makes the call synchronous. Defaults to `True`.
-        Examples:
-            >>> import neptune
-            >>> run = neptune.init_run()
-            >>> run['parameters/learninggg_rata'] = 0.3
-            >>> # Delete a field along with it's data
-            ... run.pop('parameters/learninggg_rata')
-            >>> run['parameters/learning_rate'] = 0.3
-            >>> # Training finished
-            ... run['trained_model'].upload('model.pt')
-            >>> # 'model_checkpoint' is a File field
-            ... run.pop('model_checkpoint')
-        You may also want to check `pop docs page`_.
-        .. _pop docs page:
-           https://docs.neptune.ai/api/run#pop
-        """
-        return super().pop(path=path, wait=wait)
-
-    def wait(self, *, disk_only=False) -> None:
-        """Wait for all the tracking calls to finish.
-        Args:
-            disk_only (bool, optional, default is False): If `True` the process will only wait for data to be saved
-                locally from memory, but will not wait for them to reach Neptune servers.
-                Defaults to `False`.
-        You may also want to check `wait docs page`_.
-        .. _wait docs page:
-            https://docs.neptune.ai/api/run#wait
-        """
-        return super().wait(disk_only=disk_only)
-
-    def sync(self, *, wait: bool = True) -> None:
-        """Synchronizes local representation of the run with Neptune servers.
-        Args:
-            wait (bool, optional, default is True): If `True` the process will only wait for data to be saved
-                locally from memory, but will not wait for them to reach Neptune servers.
-                Defaults to `True`.
-        Examples:
-            >>> import neptune
-            >>> # Connect to a run from Worker #3
-            ... worker_id = 3
-            >>> run = neptune.init_run(with_id='DIST-43', monitoring_namespace='monitoring/{}'.format(worker_id))
-            >>> # Try to access logs that were created in meantime by Worker #2
-            ... worker_2_status = run['status/2'].fetch() # Error if this field was created after this script starts
-            >>> run.sync() # Synchronizes local representation with Neptune servers.
-            >>> worker_2_status = run['status/2'].fetch() # No error
-        You may also want to check `sync docs page`_.
-        .. _sync docs page:
-            https://docs.neptune.ai/api/run#sync
-        """
-        return super().sync(wait=wait)
-
 
 def capture_only_if_non_interactive(mode) -> bool:
     if in_interactive() or in_notebook():
         if mode in {Mode.OFFLINE, Mode.SYNC, Mode.ASYNC}:
             warn_once(
                 "To avoid unintended consumption of logging hours during interactive sessions, the"
                 " following monitoring options are disabled unless set to 'True' when initializing"
```

### Comparing `neptune_client-1.1.1/src/neptune/new/__init__.py` & `neptune_client-1.2.0/src/neptune/new/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/new/_compatibility.py` & `neptune_client-1.2.0/src/neptune/new/_compatibility.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/new/constants.py` & `neptune_client-1.2.0/src/neptune/new/constants.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/new/envs.py` & `neptune_client-1.2.0/src/neptune/new/envs.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/new/exceptions.py` & `neptune_client-1.2.0/src/neptune/new/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/new/handler.py` & `neptune_client-1.2.0/src/neptune/new/handler.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/new/project.py` & `neptune_client-1.2.0/src/neptune/new/project.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/new/run.py` & `neptune_client-1.2.0/src/neptune/new/run.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/new/runs_table.py` & `neptune_client-1.2.0/src/neptune/new/runs_table.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/new/utils.py` & `neptune_client-1.2.0/src/neptune/new/utils.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/new/version.py` & `neptune_client-1.2.0/src/neptune/new/version.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/types/__init__.py` & `neptune_client-1.2.0/src/neptune/types/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/types/atoms/__init__.py` & `neptune_client-1.2.0/src/neptune/types/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/types/atoms/artifact.py` & `neptune_client-1.2.0/src/neptune/types/atoms/artifact.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/types/atoms/atom.py` & `neptune_client-1.2.0/src/neptune/types/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/types/atoms/boolean.py` & `neptune_client-1.2.0/src/neptune/types/atoms/boolean.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/types/atoms/datetime.py` & `neptune_client-1.2.0/src/neptune/types/atoms/datetime.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/types/atoms/file.py` & `neptune_client-1.2.0/src/neptune/types/atoms/file.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/types/atoms/float.py` & `neptune_client-1.2.0/src/neptune/types/atoms/float.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/types/atoms/git_ref.py` & `neptune_client-1.2.0/src/neptune/types/atoms/git_ref.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/types/atoms/integer.py` & `neptune_client-1.2.0/src/neptune/types/atoms/integer.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/types/atoms/string.py` & `neptune_client-1.2.0/src/neptune/types/atoms/string.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/types/file_set.py` & `neptune_client-1.2.0/src/neptune/types/file_set.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/types/mode.py` & `neptune_client-1.2.0/src/neptune/types/mode.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/types/model_version_stage.py` & `neptune_client-1.2.0/src/neptune/types/model_version_stage.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/types/namespace.py` & `neptune_client-1.2.0/src/neptune/types/namespace.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/types/series/__init__.py` & `neptune_client-1.2.0/src/neptune/types/series/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/types/series/file_series.py` & `neptune_client-1.2.0/src/neptune/types/series/file_series.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,17 +11,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 __all__ = ["FileSeries"]
 
+import time
+from itertools import cycle
 from typing import (
     TYPE_CHECKING,
     List,
+    Optional,
+    Sequence,
     TypeVar,
 )
 
 from neptune.internal.types.stringify_value import extract_if_stringify_value
 from neptune.internal.utils import is_collection
 from neptune.internal.utils.logger import logger
 from neptune.types import File
@@ -30,26 +34,48 @@
 if TYPE_CHECKING:
     from neptune.types.value_visitor import ValueVisitor
 
 Ret = TypeVar("Ret")
 
 
 class FileSeries(Series):
-    def __init__(self, values, **kwargs):
+    def __init__(
+        self, values, timestamps: Optional[Sequence[float]] = None, steps: Optional[Sequence[float]] = None, **kwargs
+    ):
         values = extract_if_stringify_value(values)
 
         if not is_collection(values):
             raise TypeError("`values` is not a collection")
 
         self._values = [File.create_from(value) for value in values]
         self.name = kwargs.pop("name", None)
         self.description = kwargs.pop("description", None)
         if kwargs:
             logger.error("Warning: unexpected arguments (%s) in FileSeries", kwargs)
 
+        if steps is None:
+            self._steps = cycle([None])
+        else:
+            assert len(values) == len(steps)
+            self._steps = steps
+
+        if timestamps is None:
+            self._timestamps = cycle([time.time()])
+        else:
+            assert len(values) == len(timestamps)
+            self._timestamps = timestamps
+
+    @property
+    def steps(self):
+        return self._steps
+
+    @property
+    def timestamps(self):
+        return self._timestamps
+
     def accept(self, visitor: "ValueVisitor[Ret]") -> Ret:
         return visitor.visit_image_series(self)
 
     @property
     def values(self) -> List[File]:
         return self._values
```

### Comparing `neptune_client-1.1.1/src/neptune/types/series/float_series.py` & `neptune_client-1.2.0/src/neptune/types/series/float_series.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,17 +11,20 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 __all__ = ["FloatSeries"]
 
+import time
+from itertools import cycle
 from typing import (
     TYPE_CHECKING,
     Optional,
+    Sequence,
     TypeVar,
     Union,
 )
 
 from neptune.internal.types.stringify_value import extract_if_stringify_value
 from neptune.internal.utils import is_collection
 from neptune.types.series.series import Series
@@ -35,25 +38,47 @@
 class FloatSeries(Series):
     def __init__(
         self,
         values,
         min: Optional[Union[float, int]] = None,
         max: Optional[Union[float, int]] = None,
         unit: Optional[str] = None,
+        timestamps: Optional[Sequence[float]] = None,
+        steps: Optional[Sequence[float]] = None,
     ):
         values = extract_if_stringify_value(values)
 
         if not is_collection(values):
             raise TypeError("`values` is not a collection")
 
         self._values = [float(value) for value in values]
         self._min = min
         self._max = max
         self._unit = unit
 
+        if steps is None:
+            self._steps = cycle([None])
+        else:
+            assert len(values) == len(steps)
+            self._steps = steps
+
+        if timestamps is None:
+            self._timestamps = cycle([time.time()])
+        else:
+            assert len(values) == len(timestamps)
+            self._timestamps = timestamps
+
+    @property
+    def steps(self):
+        return self._steps
+
+    @property
+    def timestamps(self):
+        return self._timestamps
+
     def accept(self, visitor: "ValueVisitor[Ret]") -> Ret:
         return visitor.visit_float_series(self)
 
     @property
     def values(self):
         return self._values
```

### Comparing `neptune_client-1.1.1/src/neptune/types/series/series.py` & `neptune_client-1.2.0/src/neptune/types/value.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,35 +9,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["Series"]
+__all__ = ["Value"]
 
 import abc
 from typing import (
     TYPE_CHECKING,
     TypeVar,
 )
 
-from neptune.types.value import Value
-
 if TYPE_CHECKING:
     from neptune.types.value_visitor import ValueVisitor
 
 Ret = TypeVar("Ret")
 
 
-class Series(Value):
+class Value:
     @abc.abstractmethod
     def accept(self, visitor: "ValueVisitor[Ret]") -> Ret:
         pass
-
-    @property
-    @abc.abstractmethod
-    def values(self):
-        pass
-
-    def __len__(self):
-        return len(self.values)
```

### Comparing `neptune_client-1.1.1/src/neptune/types/series/series_value.py` & `neptune_client-1.2.0/src/neptune/types/series/series_value.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/types/sets/__init__.py` & `neptune_client-1.2.0/src/neptune/types/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/types/sets/set.py` & `neptune_client-1.2.0/src/neptune/types/sets/set.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/types/sets/string_set.py` & `neptune_client-1.2.0/src/neptune/types/value_copy.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,32 +9,43 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["StringSet"]
+__all__ = ["ValueCopy"]
 
+from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
-    Iterable,
     TypeVar,
 )
 
-from neptune.types.sets.set import Set
+from neptune.internal.utils.paths import parse_path
+from neptune.types.value import Value
 
 if TYPE_CHECKING:
+    from neptune.handler import Handler
     from neptune.types.value_visitor import ValueVisitor
 
 Ret = TypeVar("Ret")
 
 
-class StringSet(Set):
-    def __init__(self, values: Iterable[str]):
-        self.values = set(values)
+@dataclass
+class ValueCopy(Value):
+
+    source_handler: "Handler"
+
+    def __init__(self, source_handler: "Handler"):
+        self.source_handler = source_handler
 
     def accept(self, visitor: "ValueVisitor[Ret]") -> Ret:
-        return visitor.visit_string_set(self)
+        source_path = self.source_handler._path
+        source_attr = self.source_handler._container.get_attribute(source_path)
+        if source_attr and source_attr.supports_copy:
+            return visitor.copy_value(source_type=type(source_attr), source_path=parse_path(source_path))
+        else:
+            raise Exception(f"{type(source_attr).__name__} doesn't support copying")
 
     def __str__(self):
-        return "StringSet({})".format(str(self.values))
+        return "Copy({})".format(str(self.source_handler))
```

### Comparing `neptune_client-1.1.1/src/neptune/types/type_casting.py` & `neptune_client-1.2.0/src/neptune/types/type_casting.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/types/value.py` & `neptune_client-1.2.0/src/neptune/typing.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,18 @@
 #
-# Copyright (c) 2022, Neptune Labs Sp. z o.o.
+# Copyright (c) 2023, Neptune Labs Sp. z o.o.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["Value"]
+__all__ = ["SupportsNamespaces"]
 
-import abc
-from typing import (
-    TYPE_CHECKING,
-    TypeVar,
-)
-
-if TYPE_CHECKING:
-    from neptune.types.value_visitor import ValueVisitor
-
-Ret = TypeVar("Ret")
-
-
-class Value:
-    @abc.abstractmethod
-    def accept(self, visitor: "ValueVisitor[Ret]") -> Ret:
-        pass
+from neptune.metadata_containers.abstract import SupportsNamespaces
```

### Comparing `neptune_client-1.1.1/src/neptune/types/value_visitor.py` & `neptune_client-1.2.0/src/neptune/types/value_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/typing.py` & `neptune_client-1.2.0/src/neptune/integrations/pytorch/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,10 +9,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["SupportsNamespaces"]
 
-from neptune.metadata_containers.abstract import SupportsNamespaces
+try:
+    from neptune_pytorch.impl import *  # noqa: F401,F403
+except ModuleNotFoundError as e:
+    if e.name == "neptune_pytorch":
+        from neptune.new.exceptions import NeptuneIntegrationNotInstalledException
+
+        raise NeptuneIntegrationNotInstalledException(
+            integration_package_name="neptune-pytorch",
+            framework_name="pytorch",
+        ) from None
+    else:
+        raise
```

### Comparing `neptune_client-1.1.1/src/neptune/utils.py` & `neptune_client-1.2.0/src/neptune/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,29 +9,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+"""Utility functions to support ML metadata logging with neptune.ai."""
 __all__ = ["stringify_unsupported"]
 
 from typing import (
     Any,
     Mapping,
     Union,
 )
 
 from neptune.internal.types.stringify_value import StringifyValue
 
 
 def stringify_unsupported(value: Any) -> Union[StringifyValue, Mapping]:
     """Helper function that converts unsupported values in a collection or dictionary to strings.
+
     Args:
         value (Any): A dictionary with values or a collection
+
     Example:
         >>> import neptune
         >>> run = neptune.init_run()
         >>> complex_dict = {"tuple": ("hi", 1), "metric": 0.87}
         >>> run["complex_dict"] = complex_dict
         >>> # (as of 1.0.0) error - tuple is not a supported type
         ... from neptune.utils import stringify_unsupported
```

### Comparing `neptune_client-1.1.1/src/neptune/vendor/lib_programname.py` & `neptune_client-1.2.0/src/neptune/vendor/lib_programname.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/vendor/pynvml.py` & `neptune_client-1.2.0/src/neptune/vendor/pynvml.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/src/neptune/version.py` & `neptune_client-1.2.0/src/neptune/version.py`

 * *Files identical despite different names*

### Comparing `neptune_client-1.1.1/PKG-INFO` & `neptune_client-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neptune-client
-Version: 1.1.1
+Version: 1.2.0
 Summary: Neptune Client
 Home-page: https://neptune.ai/
 License: Apache-2.0
 Keywords: MLOps,ML Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store
 Author: neptune.ai
 Author-email: contact@neptune.ai
 Requires-Python: >=3.7,<4.0
@@ -115,16 +115,14 @@
   <a href="https://docs.neptune.ai/">Docs</a>
   <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
   <a href="https://github.com/neptune-ai/examples">Examples</a>
   <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
   <a href="https://neptune.ai/resources">Resource center</a>
   <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
   <a href="https://neptune.ai/blog">Blog</a>
-  <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
-  <a href="https://neptune.ai/events">Podcast</a>
 &nbsp;
   <hr />
 </div>
 
 ## What is neptune.ai?
 
 neptune.ai makes it easy to log, store, organize, compare, register, and share <b>all your ML model metadata in a single place</b>.
@@ -132,15 +130,15 @@
 * Automate and standardize as your modeling team grows.
 * Collaborate on models and results with your team and across the org.
 * Use hosted, deploy on-premises, or in a private cloud. Integrate with any MLOps stack.
 &nbsp;
 
 &nbsp;
 <div align="center">
-    <a href="https://youtu.be/mv9jxexmbBk">
+    <a href="https://youtu.be/L2CAYip0DmI">
       <img border="0" alt="neptune.ai explainer video" src="https://raw.githubusercontent.com/neptune-ai/neptune-client/assets/readme/github-explainer-video.png" width="600">
     </a>
 </div>
 &nbsp;
 
 &nbsp;
 <a href="https://app.neptune.ai/showcase/example-project-tensorflow-keras/experiments?split=tbl&dash=charts&viewId=eccd5adf-42b3-497e-9cc2-9fa2655429b3"><b>Play with a live neptune.ai app →</b></a>
@@ -338,9 +336,9 @@
 &nbsp;
 
 &nbsp;
 ## People behind
 
 Created with :heart: by the [neptune.ai team](https://neptune.ai/about-us):
 
-Piotr, Paulina, Chaz, Prince, Parth, Kshitij, Siddhant, Jakub, Patrycja, Dominika, Karolina, Stephen, Artur, Aleksiej, Martyna, Małgorzata, Magdalena, Karolina, Marcin, Michał, Tymoteusz, Rafał, Aleksandra, Sabine, Tomek, Piotr, Adam, Rafał, Hubert, Marcin, Jakub, Paweł, Jakub, Franciszek, Bartosz, Aleksander, Dawid, Patryk, Krzysztof, Aurimas, and [you?](https://neptune.ai/jobs)
+Piotr, Paulina, Chaz, Prince, Parth, Kshitij, Siddhant, Jakub, Patrycja, Dominika, Karolina, Stephen, Artur, Aleksiej, Martyna, Małgorzata, Magdalena, Karolina, Marcin, Michał, Tymoteusz, Rafał, Aleksandra, Sabine, Tomek, Piotr, Rafał, Adam, Hubert, Marcin, Jakub, Paweł, Franciszek, Bartosz, Aleksander, Dawid, Patryk, Krzysztof, Aurimas, Jakub, Bartosz, and [you?](https://neptune.ai/jobs)
```

