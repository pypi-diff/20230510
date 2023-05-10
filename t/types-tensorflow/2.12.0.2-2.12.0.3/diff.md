# Comparing `tmp/types-tensorflow-2.12.0.2.tar.gz` & `tmp/types-tensorflow-2.12.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-tensorflow-2.12.0.2.tar", last modified: Thu Apr 27 12:28:34 2023, max compression
+gzip compressed data, was "types-tensorflow-2.12.0.3.tar", last modified: Wed May 10 15:23:36 2023, max compression
```

## Comparing `types-tensorflow-2.12.0.2.tar` & `types-tensorflow-2.12.0.3.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.069185 types-tensorflow-2.12.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-27 12:28:31.000000 types-tensorflow-2.12.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 12:28:31.000000 types-tensorflow-2.12.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-27 12:28:34.069185 types-tensorflow-2.12.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 12:28:34.069185 types-tensorflow-2.12.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-04-27 12:28:31.000000 types-tensorflow-2.12.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.057185 types-tensorflow-2.12.0.2/tensorflow-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-27 12:28:31.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/_aliases.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.057185 types-tensorflow-2.12.0.2/tensorflow-stubs/compiler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.057185 types-tensorflow-2.12.0.2/tensorflow-stubs/compiler/xla/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.057185 types-tensorflow-2.12.0.2/tensorflow-stubs/compiler/xla/service/
--rw-r--r--   0 runner    (1001) docker     (123)    78294 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    78920 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.057185 types-tensorflow-2.12.0.2/tensorflow-stubs/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.057185 types-tensorflow-2.12.0.2/tensorflow-stubs/core/example/
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/example/example_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/example/feature_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.061185 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/allocation_description_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/api_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/attr_value_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/cost_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22095 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/dataset_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/device_attributes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23251 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/full_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/function_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/kernel_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/log_memory_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12658 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/node_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15381 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/op_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/reader_base_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/resource_handle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/step_stats_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/summary_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/tensor_description_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/tensor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/variable_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/versions_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.065185 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/cluster_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    77923 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/coordination_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/data_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    26277 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/debug_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/distributed_runtime_payloads_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    28896 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27624 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27163 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/saver_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/service_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19704 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/struct_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.065185 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/tpu/
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    51042 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.065185 types-tensorflow-2.12.0.2/tensorflow-stubs/core/util/
--rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/util/event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/core/util/test_log_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/dtypes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.065185 types-tensorflow-2.12.0.2/tensorflow-stubs/feature_column/
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/feature_column/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/initializers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.065185 types-tensorflow-2.12.0.2/tensorflow-stubs/io/
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/io/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/io/gfile.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.065185 types-tensorflow-2.12.0.2/tensorflow-stubs/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/keras/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/keras/activations.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/keras/constraints.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/keras/initializers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/keras/layers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.065185 types-tensorflow-2.12.0.2/tensorflow-stubs/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/keras/optimizers/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.065185 types-tensorflow-2.12.0.2/tensorflow-stubs/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/keras/optimizers/schedules.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/keras/regularizers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/math.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.065185 types-tensorflow-2.12.0.2/tensorflow-stubs/python/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/python/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.065185 types-tensorflow-2.12.0.2/tensorflow-stubs/python/feature_column/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/python/feature_column/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/python/feature_column/feature_column_v2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.065185 types-tensorflow-2.12.0.2/tensorflow-stubs/python/keras/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/python/keras/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.065185 types-tensorflow-2.12.0.2/tensorflow-stubs/python/keras/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.069185 types-tensorflow-2.12.0.2/tensorflow-stubs/python/trackable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/python/trackable/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/python/trackable/autotrackable.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/python/trackable/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/sparse.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.057185 types-tensorflow-2.12.0.2/tensorflow-stubs/tsl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.069185 types-tensorflow-2.12.0.2/tensorflow-stubs/tsl/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-27 12:28:16.000000 types-tensorflow-2.12.0.2/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 12:28:34.069185 types-tensorflow-2.12.0.2/types_tensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-27 12:28:34.000000 types-tensorflow-2.12.0.2/types_tensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-04-27 12:28:34.000000 types-tensorflow-2.12.0.2/types_tensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 12:28:34.000000 types-tensorflow-2.12.0.2/types_tensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 12:28:34.000000 types-tensorflow-2.12.0.2/types_tensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 12:28:34.000000 types-tensorflow-2.12.0.2/types_tensorflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-10 15:23:35.000000 types-tensorflow-2.12.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:23:35.000000 types-tensorflow-2.12.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-05-10 15:23:35.000000 types-tensorflow-2.12.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.270543 types-tensorflow-2.12.0.3/tensorflow-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-10 15:23:35.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/_aliases.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.266543 types-tensorflow-2.12.0.3/tensorflow-stubs/compiler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.270543 types-tensorflow-2.12.0.3/tensorflow-stubs/compiler/xla/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.270543 types-tensorflow-2.12.0.3/tensorflow-stubs/compiler/xla/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    78294 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    78920 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.270543 types-tensorflow-2.12.0.3/tensorflow-stubs/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.270543 types-tensorflow-2.12.0.3/tensorflow-stubs/core/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/example/example_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/example/feature_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.274543 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/allocation_description_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/api_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/attr_value_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/cost_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22095 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/dataset_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/device_attributes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23251 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/full_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/function_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/kernel_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/log_memory_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12658 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/node_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15381 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/op_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/reader_base_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/resource_handle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/step_stats_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/summary_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/tensor_description_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/tensor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/variable_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/versions_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.278544 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/cluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    77923 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/coordination_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/data_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    26277 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/debug_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/distributed_runtime_payloads_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    28896 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27624 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27163 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/saver_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/service_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19704 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/struct_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.278544 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    51042 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.278544 types-tensorflow-2.12.0.3/tensorflow-stubs/core/util/
+-rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/util/event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/core/util/test_log_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/dtypes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.278544 types-tensorflow-2.12.0.3/tensorflow-stubs/feature_column/
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/feature_column/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/initializers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.278544 types-tensorflow-2.12.0.3/tensorflow-stubs/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/io/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/io/gfile.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/activations.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/constraints.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/initializers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/layers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/optimizers/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/optimizers/schedules.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/keras/regularizers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/math.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/tensorflow-stubs/python/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/python/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/tensorflow-stubs/python/feature_column/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/python/feature_column/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/python/feature_column/feature_column_v2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/tensorflow-stubs/python/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/python/keras/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/tensorflow-stubs/python/keras/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/tensorflow-stubs/python/trackable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/python/trackable/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/python/trackable/autotrackable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/python/trackable/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/sparse.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.270543 types-tensorflow-2.12.0.3/tensorflow-stubs/tsl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/tensorflow-stubs/tsl/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-10 15:19:44.000000 types-tensorflow-2.12.0.3/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:36.282544 types-tensorflow-2.12.0.3/types_tensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-10 15:23:36.000000 types-tensorflow-2.12.0.3/types_tensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-05-10 15:23:36.000000 types-tensorflow-2.12.0.3/types_tensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:23:36.000000 types-tensorflow-2.12.0.3/types_tensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 15:23:36.000000 types-tensorflow-2.12.0.3/types_tensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 15:23:36.000000 types-tensorflow-2.12.0.3/types_tensorflow.egg-info/top_level.txt
```

### Comparing `types-tensorflow-2.12.0.2/CHANGELOG.md` & `types-tensorflow-2.12.0.3/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 2.12.0.3 (2023-05-10)
+
+Add `partial_stub` metadata field (#10157)
+
 ## 2.12.0.2 (2023-04-27)
 
 tensorflow: feature columns (#10052)
 
 Co-authored-by: Mehdi Drissi <mdrissi@snapchat.com>
 Co-authored-by: Jelle Zijlstra <jelle.zijlstra@gmail.com>
```

### Comparing `types-tensorflow-2.12.0.2/PKG-INFO` & `types-tensorflow-2.12.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tensorflow
-Version: 2.12.0.2
+Version: 2.12.0.3
 Summary: Typing stubs for tensorflow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tensorflow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tensorflow. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `11f5858f0bdde716b05e9fc1cd35c8de5d6cc74c`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-tensorflow-2.12.0.2/setup.py` & `types-tensorflow-2.12.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tensorflow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tensorflow. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `11f5858f0bdde716b05e9fc1cd35c8de5d6cc74c`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
 '''.lstrip()
 
 setup(name=name,
-      version="2.12.0.2",
+      version="2.12.0.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md",
```

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/__init__.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/_aliases.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/_aliases.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/example/example_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/example/example_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/example/feature_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/example/feature_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/allocation_description_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/allocation_description_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/api_def_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/api_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/attr_value_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/attr_value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/cost_graph_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/cost_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/dataset_options_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/dataset_options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/device_attributes_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/device_attributes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/full_type_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/full_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/function_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/graph_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/kernel_def_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/kernel_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/log_memory_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/log_memory_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/model_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/node_def_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/node_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/op_def_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/op_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/reader_base_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/reader_base_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/resource_handle_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/resource_handle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/step_stats_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/step_stats_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/summary_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/summary_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/tensor_description_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/tensor_description_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/tensor_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/tensor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/types_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/variable_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/variable_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/framework/versions_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/framework/versions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/cluster_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/cluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/config_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/coordination_config_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/coordination_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/data_service_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/data_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/debug_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/debug_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/distributed_runtime_payloads_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/distributed_runtime_payloads_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/saver_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/saver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/service_config_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/service_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/struct_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/struct_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/util/event_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/util/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/core/util/test_log_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/core/util/test_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/dtypes.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/dtypes.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/feature_column/__init__.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/feature_column/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/io/__init__.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/io/gfile.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/io/gfile.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/keras/constraints.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/keras/constraints.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/keras/initializers.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/keras/initializers.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/keras/layers.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/keras/layers.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/keras/optimizers/schedules.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/keras/optimizers/schedules.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/keras/regularizers.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/keras/regularizers.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/math.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/math.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/python/feature_column/feature_column_v2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/python/feature_column/feature_column_v2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/sparse.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/sparse.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi` & `types-tensorflow-2.12.0.3/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.2/types_tensorflow.egg-info/PKG-INFO` & `types-tensorflow-2.12.0.3/types_tensorflow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tensorflow
-Version: 2.12.0.2
+Version: 2.12.0.3
 Summary: Typing stubs for tensorflow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tensorflow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tensorflow. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `11f5858f0bdde716b05e9fc1cd35c8de5d6cc74c`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-tensorflow-2.12.0.2/types_tensorflow.egg-info/SOURCES.txt` & `types-tensorflow-2.12.0.3/types_tensorflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

