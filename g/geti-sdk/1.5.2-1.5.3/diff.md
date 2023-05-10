# Comparing `tmp/geti-sdk-1.5.2.tar.gz` & `tmp/geti-sdk-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geti-sdk-1.5.2.tar", last modified: Mon May  8 12:17:15 2023, max compression
+gzip compressed data, was "geti-sdk-1.5.3.tar", last modified: Wed May 10 12:10:18 2023, max compression
```

## Comparing `geti-sdk-1.5.2.tar` & `geti-sdk-1.5.3.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.146379 geti-sdk-1.5.2/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10174 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/LICENSE
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      178 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/MANIFEST.in
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17322 2023-05-08 12:17:15.146379 geti-sdk-1.5.2/PKG-INFO
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16457 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/README.md
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.130379 geti-sdk-1.5.2/geti_sdk/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2231 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.130379 geti-sdk-1.5.2/geti_sdk/annotation_readers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1948 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/annotation_readers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4239 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/annotation_readers/base_annotation_reader.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.130379 geti-sdk-1.5.2/geti_sdk/annotation_readers/datumaro_annotation_reader/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    12680 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11868 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10558 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/annotation_readers/directory_tree_annotation_reader.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9911 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/annotation_readers/geti_annotation_reader.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.134379 geti-sdk-1.5.2/geti_sdk/data_models/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5033 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1689 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/algorithms.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14951 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/annotation_scene.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6286 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/annotations.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2564 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/code_deployment_info.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6065 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/configurable_parameter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10440 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/configurable_parameter_group.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14304 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/configuration.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3321 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/configuration_identifiers.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.134379 geti-sdk-1.5.2/geti_sdk/data_models/containers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/containers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5250 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/containers/algorithm_list.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3608 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/containers/media_list.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.134379 geti-sdk-1.5.2/geti_sdk/data_models/enums/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1382 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/enums/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/enums/annotation_kind.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1035 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/enums/annotation_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2192 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/enums/configuration_enums.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      987 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/enums/deployment_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1587 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/enums/domain.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1707 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/enums/job_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1061 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/enums/job_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1062 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/enums/media_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1031 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/enums/model_status.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      943 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/enums/optimization_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/enums/prediction_mode.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1013 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/enums/shape_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4225 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/enums/task_type.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8506 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/job.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5736 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/label.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16509 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/media.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2520 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/media_identifiers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8547 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/model.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     7302 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/model_group.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1132 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/performance.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9330 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/predictions.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11975 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/project.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    31421 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/shapes.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6635 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/status.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5705 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/task.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1019 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/task_annotation_state.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9823 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/data_models/utils.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.134379 geti-sdk-1.5.2/geti_sdk/demos/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1921 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/demos/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      909 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/demos/constants.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.126379 geti-sdk-1.5.2/geti_sdk/demos/data/
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.134379 geti-sdk-1.5.2/geti_sdk/demos/data/example/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)   724731 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/demos/data/example/dogs.png
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.138379 geti-sdk-1.5.2/geti_sdk/demos/data_helpers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      925 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/demos/data_helpers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6177 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/demos/data_helpers/anomaly_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9179 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/demos/data_helpers/coco_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5361 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/demos/data_helpers/download_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1945 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/demos/data_helpers/video_helpers.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.138379 geti-sdk-1.5.2/geti_sdk/demos/demo_projects/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1438 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/demos/demo_projects/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5247 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/demos/demo_projects/anomaly_demos.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16855 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/demos/demo_projects/coco_demos.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3058 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/demos/demo_projects/utils.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.138379 geti-sdk-1.5.2/geti_sdk/deployment/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2684 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/deployment/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.138379 geti-sdk-1.5.2/geti_sdk/deployment/data_models/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      753 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/deployment/data_models/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4715 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/deployment/data_models/intermediate_inference_result.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2064 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/deployment/data_models/region_of_interest.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    26479 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/deployment/deployed_model.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    22564 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/deployment/deployment.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.138379 geti-sdk-1.5.2/geti_sdk/deployment/resources/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2669 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/deployment/resources/OVMS_README.md
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      653 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/deployment/resources/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3306 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/deployment/utils.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    55063 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/geti.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.138379 geti-sdk-1.5.2/geti_sdk/http_session/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2120 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/http_session/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2504 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/http_session/exception.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18039 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/http_session/geti_session.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4421 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/http_session/server_config.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6021 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/platform_versions.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.142379 geti-sdk-1.5.2/geti_sdk/rest_clients/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3575 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_clients/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.142379 geti-sdk-1.5.2/geti_sdk/rest_clients/annotation_clients/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      676 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_clients/annotation_clients/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14474 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_clients/annotation_clients/annotation_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    19255 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16462 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_clients/configuration_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4949 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_clients/dataset_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18377 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_clients/deployment_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.142379 geti-sdk-1.5.2/geti_sdk/rest_clients/media_client/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_clients/media_client/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8558 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_clients/media_client/image_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16827 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_clients/media_client/media_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6260 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_clients/media_client/video_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17521 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_clients/model_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24590 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_clients/prediction_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.142379 geti-sdk-1.5.2/geti_sdk/rest_clients/project_client/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      667 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_clients/project_client/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24906 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_clients/project_client/project_client.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2045 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_clients/project_client/task_templates.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    15014 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_clients/training_client.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.142379 geti-sdk-1.5.2/geti_sdk/rest_converters/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2016 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_converters/__init__.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.142379 geti-sdk-1.5.2/geti_sdk/rest_converters/annotation_rest_converter/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_converters/annotation_rest_converter/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6317 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6871 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10877 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_converters/configuration_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1722 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_converters/job_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1554 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_converters/media_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2361 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_converters/model_rest_converter.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.142379 geti-sdk-1.5.2/geti_sdk/rest_converters/prediction_rest_converter/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_converters/prediction_rest_converter/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3977 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3471 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2292 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_converters/project_rest_converter.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1400 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/rest_converters/status_rest_converter.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.146379 geti-sdk-1.5.2/geti_sdk/utils/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1784 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/utils/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2007 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/utils/algorithm_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6398 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/utils/credentials_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1259 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/utils/dictionary_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3836 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/utils/label_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6661 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/utils/plot_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1408 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/utils/project_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3455 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/utils/serialization_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1669 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/geti_sdk/utils/workspace_helpers.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.130379 geti-sdk-1.5.2/geti_sdk.egg-info/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17322 2023-05-08 12:17:15.000000 geti-sdk-1.5.2/geti_sdk.egg-info/PKG-INFO
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5718 2023-05-08 12:17:15.000000 geti-sdk-1.5.2/geti_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)        1 2023-05-08 12:17:15.000000 geti-sdk-1.5.2/geti_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-05-08 12:17:15.000000 geti-sdk-1.5.2/geti_sdk.egg-info/requires.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       15 2023-05-08 12:17:15.000000 geti-sdk-1.5.2/geti_sdk.egg-info/top_level.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       94 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/pyproject.toml
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.146379 geti-sdk-1.5.2/requirements/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      247 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/requirements/requirements-dev.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       98 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/requirements/requirements-docs.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      121 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/requirements/requirements-notebooks.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      353 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/requirements/requirements.txt
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       38 2023-05-08 12:17:15.146379 geti-sdk-1.5.2/setup.cfg
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2844 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/setup.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.146379 geti-sdk-1.5.2/tests/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      581 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/tests/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8562 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/tests/conftest.py
-drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-08 12:17:15.146379 geti-sdk-1.5.2/tests/helpers/
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1351 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/tests/helpers/__init__.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1002 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/tests/helpers/constants.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1709 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/tests/helpers/enums.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2326 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/tests/helpers/finalizers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2412 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/tests/helpers/fixtures.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2761 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/tests/helpers/plotting.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4417 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/tests/helpers/project_helpers.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18968 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/tests/helpers/project_service.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1866 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/tests/helpers/training.py
--rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3068 2023-05-08 11:51:42.000000 geti-sdk-1.5.2/tests/helpers/vcr_helpers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.317252 geti-sdk-1.5.3/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10174 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/LICENSE
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      178 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/MANIFEST.in
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17322 2023-05-10 12:10:18.317252 geti-sdk-1.5.3/PKG-INFO
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16457 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/README.md
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.301252 geti-sdk-1.5.3/geti_sdk/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2231 2023-05-10 11:48:55.000000 geti-sdk-1.5.3/geti_sdk/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.301252 geti-sdk-1.5.3/geti_sdk/annotation_readers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1948 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/annotation_readers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4239 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/annotation_readers/base_annotation_reader.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.301252 geti-sdk-1.5.3/geti_sdk/annotation_readers/datumaro_annotation_reader/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    12680 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11868 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10558 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/annotation_readers/directory_tree_annotation_reader.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9911 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/annotation_readers/geti_annotation_reader.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.305253 geti-sdk-1.5.3/geti_sdk/data_models/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5033 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1689 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/algorithms.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14951 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/annotation_scene.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6286 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/annotations.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2564 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/code_deployment_info.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6065 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/configurable_parameter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10440 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/configurable_parameter_group.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14304 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/configuration.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3321 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/configuration_identifiers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.305253 geti-sdk-1.5.3/geti_sdk/data_models/containers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/containers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5250 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/containers/algorithm_list.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3608 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/containers/media_list.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.305253 geti-sdk-1.5.3/geti_sdk/data_models/enums/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1382 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/enums/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/enums/annotation_kind.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1035 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/enums/annotation_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2192 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/enums/configuration_enums.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      987 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/enums/deployment_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1587 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/enums/domain.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1707 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/enums/job_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1061 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/enums/job_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1062 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/enums/media_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1031 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/enums/model_status.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      961 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/enums/optimization_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      957 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/enums/prediction_mode.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1013 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/enums/shape_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4225 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/enums/task_type.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8506 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/job.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5736 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/label.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16509 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/media.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2520 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/media_identifiers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8547 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/model.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     7302 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/model_group.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1132 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/performance.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9330 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/predictions.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    11975 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/project.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    31421 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/shapes.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6635 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/status.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5705 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/task.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1019 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/task_annotation_state.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9823 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/data_models/utils.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.305253 geti-sdk-1.5.3/geti_sdk/demos/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1921 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/demos/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      909 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/demos/constants.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.297253 geti-sdk-1.5.3/geti_sdk/demos/data/
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.305253 geti-sdk-1.5.3/geti_sdk/demos/data/example/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)   724731 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/demos/data/example/dogs.png
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.309253 geti-sdk-1.5.3/geti_sdk/demos/data_helpers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      925 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/demos/data_helpers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6177 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/demos/data_helpers/anomaly_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     9179 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/demos/data_helpers/coco_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5361 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/demos/data_helpers/download_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1945 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/demos/data_helpers/video_helpers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.309253 geti-sdk-1.5.3/geti_sdk/demos/demo_projects/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1438 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/demos/demo_projects/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5247 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/demos/demo_projects/anomaly_demos.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16855 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/demos/demo_projects/coco_demos.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3058 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/demos/demo_projects/utils.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.309253 geti-sdk-1.5.3/geti_sdk/deployment/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2684 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/deployment/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.309253 geti-sdk-1.5.3/geti_sdk/deployment/data_models/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      753 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/deployment/data_models/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4715 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/deployment/data_models/intermediate_inference_result.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2064 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/deployment/data_models/region_of_interest.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    26479 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/deployment/deployed_model.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    22564 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/deployment/deployment.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.309253 geti-sdk-1.5.3/geti_sdk/deployment/resources/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2669 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/deployment/resources/OVMS_README.md
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      653 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/deployment/resources/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3306 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/deployment/utils.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    55063 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/geti.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.309253 geti-sdk-1.5.3/geti_sdk/http_session/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2120 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/http_session/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2504 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/http_session/exception.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18039 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/http_session/geti_session.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4421 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/http_session/server_config.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6083 2023-05-10 11:03:58.000000 geti-sdk-1.5.3/geti_sdk/platform_versions.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.313253 geti-sdk-1.5.3/geti_sdk/rest_clients/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3575 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_clients/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.313253 geti-sdk-1.5.3/geti_sdk/rest_clients/annotation_clients/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      676 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_clients/annotation_clients/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    14474 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_clients/annotation_clients/annotation_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    19255 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16462 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_clients/configuration_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4949 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_clients/dataset_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18377 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_clients/deployment_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.313253 geti-sdk-1.5.3/geti_sdk/rest_clients/media_client/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      714 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_clients/media_client/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8558 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_clients/media_client/image_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    16826 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_clients/media_client/media_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6260 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_clients/media_client/video_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17521 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_clients/model_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24590 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_clients/prediction_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.313253 geti-sdk-1.5.3/geti_sdk/rest_clients/project_client/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      667 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_clients/project_client/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    24906 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_clients/project_client/project_client.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2045 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_clients/project_client/task_templates.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    15014 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_clients/training_client.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.313253 geti-sdk-1.5.3/geti_sdk/rest_converters/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2016 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_converters/__init__.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.313253 geti-sdk-1.5.3/geti_sdk/rest_converters/annotation_rest_converter/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_converters/annotation_rest_converter/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6317 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6871 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    10877 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_converters/configuration_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1722 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_converters/job_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1554 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_converters/media_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2361 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_converters/model_rest_converter.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.313253 geti-sdk-1.5.3/geti_sdk/rest_converters/prediction_rest_converter/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      819 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_converters/prediction_rest_converter/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3977 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3471 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2292 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_converters/project_rest_converter.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1400 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/rest_converters/status_rest_converter.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.317252 geti-sdk-1.5.3/geti_sdk/utils/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1784 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/utils/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2007 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/utils/algorithm_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6398 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/utils/credentials_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1259 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/utils/dictionary_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3836 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/utils/label_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     6661 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/utils/plot_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1408 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/utils/project_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3455 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/utils/serialization_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1669 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/geti_sdk/utils/workspace_helpers.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.301252 geti-sdk-1.5.3/geti_sdk.egg-info/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    17322 2023-05-10 12:10:18.000000 geti-sdk-1.5.3/geti_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     5718 2023-05-10 12:10:18.000000 geti-sdk-1.5.3/geti_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)        1 2023-05-10 12:10:18.000000 geti-sdk-1.5.3/geti_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      695 2023-05-10 12:10:18.000000 geti-sdk-1.5.3/geti_sdk.egg-info/requires.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       15 2023-05-10 12:10:18.000000 geti-sdk-1.5.3/geti_sdk.egg-info/top_level.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       94 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/pyproject.toml
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.317252 geti-sdk-1.5.3/requirements/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      247 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/requirements/requirements-dev.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       98 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/requirements/requirements-docs.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      121 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/requirements/requirements-notebooks.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      353 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/requirements/requirements.txt
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)       38 2023-05-10 12:10:18.317252 geti-sdk-1.5.3/setup.cfg
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2844 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/setup.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.317252 geti-sdk-1.5.3/tests/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)      581 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/tests/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     8562 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/tests/conftest.py
+drwxr-xr-x   0 ljcornel  (1002) ljcornel  (1002)        0 2023-05-10 12:10:18.317252 geti-sdk-1.5.3/tests/helpers/
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1351 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/tests/helpers/__init__.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1002 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/tests/helpers/constants.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1709 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/tests/helpers/enums.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2326 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/tests/helpers/finalizers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2412 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/tests/helpers/fixtures.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     2761 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/tests/helpers/plotting.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     4417 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/tests/helpers/project_helpers.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)    18968 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/tests/helpers/project_service.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     1866 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/tests/helpers/training.py
+-rw-r--r--   0 ljcornel  (1002) ljcornel  (1002)     3068 2023-05-10 11:03:57.000000 geti-sdk-1.5.3/tests/helpers/vcr_helpers.py
```

### Comparing `geti-sdk-1.5.2/LICENSE` & `geti-sdk-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/PKG-INFO` & `geti-sdk-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geti-sdk
-Version: 1.5.2
+Version: 1.5.3
 Summary: Software Development Kit for the Intel® Geti™ platform
 Home-page: https://github.com/openvinotoolkit/geti-sdk
 Author: Intel OpenVINO
 Author-email: ludo.cornelissen@intel.com
 License: Copyright (C) 2022 Intel Corporation - All Rights Reserved. Licensed under the Apache License, Version 2.0 (the 'License'). See LICENSE file for more details.
 Project-URL: Documentation, https://openvinotoolkit.github.io/geti-sdk
 Project-URL: Bug Tracker, https://github.com/openvinotoolkit/geti-sdk/issues
```

### Comparing `geti-sdk-1.5.2/README.md` & `geti-sdk-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/__init__.py` & `geti-sdk-1.5.3/geti_sdk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,10 +74,10 @@
 
    .. automethod:: upload_and_predict_media_folder
 
 """
 
 from .geti import Geti
 
-__version__ = "1.5.2"
+__version__ = "1.5.3"
 
 __all__ = ["Geti"]
```

### Comparing `geti-sdk-1.5.2/geti_sdk/annotation_readers/__init__.py` & `geti-sdk-1.5.3/geti_sdk/annotation_readers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/annotation_readers/base_annotation_reader.py` & `geti-sdk-1.5.3/geti_sdk/annotation_readers/base_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py` & `geti-sdk-1.5.3/geti_sdk/annotation_readers/datumaro_annotation_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py` & `geti-sdk-1.5.3/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py` & `geti-sdk-1.5.3/geti_sdk/annotation_readers/datumaro_annotation_reader/datumaro_dataset.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/annotation_readers/directory_tree_annotation_reader.py` & `geti-sdk-1.5.3/geti_sdk/annotation_readers/directory_tree_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/annotation_readers/geti_annotation_reader.py` & `geti-sdk-1.5.3/geti_sdk/annotation_readers/geti_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/__init__.py` & `geti-sdk-1.5.3/geti_sdk/data_models/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/algorithms.py` & `geti-sdk-1.5.3/geti_sdk/data_models/algorithms.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/annotation_scene.py` & `geti-sdk-1.5.3/geti_sdk/data_models/annotation_scene.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/annotations.py` & `geti-sdk-1.5.3/geti_sdk/data_models/annotations.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/code_deployment_info.py` & `geti-sdk-1.5.3/geti_sdk/data_models/code_deployment_info.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/configurable_parameter.py` & `geti-sdk-1.5.3/geti_sdk/data_models/configurable_parameter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/configurable_parameter_group.py` & `geti-sdk-1.5.3/geti_sdk/data_models/configurable_parameter_group.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/configuration.py` & `geti-sdk-1.5.3/geti_sdk/data_models/configuration.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/configuration_identifiers.py` & `geti-sdk-1.5.3/geti_sdk/data_models/configuration_identifiers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/containers/__init__.py` & `geti-sdk-1.5.3/geti_sdk/data_models/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/containers/algorithm_list.py` & `geti-sdk-1.5.3/geti_sdk/data_models/containers/algorithm_list.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/containers/media_list.py` & `geti-sdk-1.5.3/geti_sdk/data_models/containers/media_list.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/enums/__init__.py` & `geti-sdk-1.5.3/geti_sdk/data_models/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/enums/annotation_kind.py` & `geti-sdk-1.5.3/geti_sdk/data_models/enums/annotation_kind.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/enums/annotation_state.py` & `geti-sdk-1.5.3/geti_sdk/data_models/enums/annotation_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/enums/configuration_enums.py` & `geti-sdk-1.5.3/geti_sdk/data_models/enums/configuration_enums.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/enums/deployment_state.py` & `geti-sdk-1.5.3/geti_sdk/data_models/enums/deployment_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/enums/domain.py` & `geti-sdk-1.5.3/geti_sdk/data_models/enums/domain.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/enums/job_state.py` & `geti-sdk-1.5.3/geti_sdk/data_models/enums/job_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/enums/job_type.py` & `geti-sdk-1.5.3/geti_sdk/data_models/enums/job_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/enums/media_type.py` & `geti-sdk-1.5.3/geti_sdk/data_models/enums/media_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/enums/model_status.py` & `geti-sdk-1.5.3/geti_sdk/data_models/enums/model_status.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/enums/optimization_type.py` & `geti-sdk-1.5.3/geti_sdk/data_models/enums/optimization_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,13 +19,14 @@
     """
     Enum representing the optimization type for an OptimizedModel in Intel® Geti™.
     """
 
     NNCF = "NNCF"
     POT = "POT"
     MO = "MO"
+    ONNX = "ONNX"
 
     def __str__(self) -> str:
         """
         Return the string representation of the OptimizationType instance.
         """
         return self.value
```

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/enums/prediction_mode.py` & `geti-sdk-1.5.3/geti_sdk/data_models/enums/prediction_mode.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/enums/shape_type.py` & `geti-sdk-1.5.3/geti_sdk/data_models/enums/shape_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/enums/task_type.py` & `geti-sdk-1.5.3/geti_sdk/data_models/enums/task_type.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/job.py` & `geti-sdk-1.5.3/geti_sdk/data_models/job.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/label.py` & `geti-sdk-1.5.3/geti_sdk/data_models/label.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/media.py` & `geti-sdk-1.5.3/geti_sdk/data_models/media.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/media_identifiers.py` & `geti-sdk-1.5.3/geti_sdk/data_models/media_identifiers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/model.py` & `geti-sdk-1.5.3/geti_sdk/data_models/model.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/model_group.py` & `geti-sdk-1.5.3/geti_sdk/data_models/model_group.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/performance.py` & `geti-sdk-1.5.3/geti_sdk/data_models/performance.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/predictions.py` & `geti-sdk-1.5.3/geti_sdk/data_models/predictions.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/project.py` & `geti-sdk-1.5.3/geti_sdk/data_models/project.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/shapes.py` & `geti-sdk-1.5.3/geti_sdk/data_models/shapes.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/status.py` & `geti-sdk-1.5.3/geti_sdk/data_models/status.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/task.py` & `geti-sdk-1.5.3/geti_sdk/data_models/task.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/task_annotation_state.py` & `geti-sdk-1.5.3/geti_sdk/data_models/task_annotation_state.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/data_models/utils.py` & `geti-sdk-1.5.3/geti_sdk/data_models/utils.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/demos/__init__.py` & `geti-sdk-1.5.3/geti_sdk/demos/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/demos/constants.py` & `geti-sdk-1.5.3/geti_sdk/demos/constants.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/demos/data/example/dogs.png` & `geti-sdk-1.5.3/geti_sdk/demos/data/example/dogs.png`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/demos/data_helpers/__init__.py` & `geti-sdk-1.5.3/geti_sdk/demos/data_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/demos/data_helpers/anomaly_helpers.py` & `geti-sdk-1.5.3/geti_sdk/demos/data_helpers/anomaly_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/demos/data_helpers/coco_helpers.py` & `geti-sdk-1.5.3/geti_sdk/demos/data_helpers/coco_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/demos/data_helpers/download_helpers.py` & `geti-sdk-1.5.3/geti_sdk/demos/data_helpers/download_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/demos/data_helpers/video_helpers.py` & `geti-sdk-1.5.3/geti_sdk/demos/data_helpers/video_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/demos/demo_projects/__init__.py` & `geti-sdk-1.5.3/geti_sdk/demos/demo_projects/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/demos/demo_projects/anomaly_demos.py` & `geti-sdk-1.5.3/geti_sdk/demos/demo_projects/anomaly_demos.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/demos/demo_projects/coco_demos.py` & `geti-sdk-1.5.3/geti_sdk/demos/demo_projects/coco_demos.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/demos/demo_projects/utils.py` & `geti-sdk-1.5.3/geti_sdk/demos/demo_projects/utils.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/deployment/__init__.py` & `geti-sdk-1.5.3/geti_sdk/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/deployment/data_models/__init__.py` & `geti-sdk-1.5.3/geti_sdk/deployment/data_models/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/deployment/data_models/intermediate_inference_result.py` & `geti-sdk-1.5.3/geti_sdk/deployment/data_models/intermediate_inference_result.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/deployment/data_models/region_of_interest.py` & `geti-sdk-1.5.3/geti_sdk/deployment/data_models/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/deployment/deployed_model.py` & `geti-sdk-1.5.3/geti_sdk/deployment/deployed_model.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/deployment/deployment.py` & `geti-sdk-1.5.3/geti_sdk/deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/deployment/resources/OVMS_README.md` & `geti-sdk-1.5.3/geti_sdk/deployment/resources/OVMS_README.md`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/deployment/resources/__init__.py` & `geti-sdk-1.5.3/geti_sdk/deployment/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/deployment/utils.py` & `geti-sdk-1.5.3/geti_sdk/deployment/utils.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/geti.py` & `geti-sdk-1.5.3/geti_sdk/geti.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/http_session/__init__.py` & `geti-sdk-1.5.3/geti_sdk/http_session/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/http_session/exception.py` & `geti-sdk-1.5.3/geti_sdk/http_session/exception.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/http_session/geti_session.py` & `geti-sdk-1.5.3/geti_sdk/http_session/geti_session.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/http_session/server_config.py` & `geti-sdk-1.5.3/geti_sdk/http_session/server_config.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/platform_versions.py` & `geti-sdk-1.5.3/geti_sdk/platform_versions.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,7 +158,8 @@
 
 
 SC_MVP_VERSION = GetiVersion("1.0.0-release-20220129184214")
 SC_11_VERSION = GetiVersion("1.1.0-release-20220624125113")
 GETI_10_VERSION = GetiVersion("1.0.0-release-20221005164936")
 GETI_11_VERSION = GetiVersion("1.1.0-release-20221125121144")
 GETI_12_VERSION = GetiVersion("1.2.0-release-20230101120000")
+GETI_15_VERSION = GetiVersion("1.5.0-release-20230504111017")
```

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_clients/__init__.py` & `geti-sdk-1.5.3/geti_sdk/rest_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_clients/annotation_clients/__init__.py` & `geti-sdk-1.5.3/geti_sdk/rest_clients/annotation_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_clients/annotation_clients/annotation_client.py` & `geti-sdk-1.5.3/geti_sdk/rest_clients/annotation_clients/annotation_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py` & `geti-sdk-1.5.3/geti_sdk/rest_clients/annotation_clients/base_annotation_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_clients/configuration_client.py` & `geti-sdk-1.5.3/geti_sdk/rest_clients/configuration_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_clients/dataset_client.py` & `geti-sdk-1.5.3/geti_sdk/rest_clients/dataset_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_clients/deployment_client.py` & `geti-sdk-1.5.3/geti_sdk/rest_clients/deployment_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_clients/media_client/__init__.py` & `geti-sdk-1.5.3/geti_sdk/rest_clients/media_client/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_clients/media_client/image_client.py` & `geti-sdk-1.5.3/geti_sdk/rest_clients/media_client/image_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_clients/media_client/media_client.py` & `geti-sdk-1.5.3/geti_sdk/rest_clients/media_client/media_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     """
 
     _MEDIA_TYPE: ClassVar[MediaType]
 
     def __init__(self, session: GetiSession, workspace_id: str, project: Project):
         self.session = session
         self._workspace_id = workspace_id
-        self._base_url = f"workspaces/{workspace_id}/projects/{project.id}/datasets/"
+        self._base_url = f"workspaces/{workspace_id}/projects/{project.id}/datasets"
         self._project = project
         self.__media_type: Type[MediaTypeVar] = self.__get_media_type(self._MEDIA_TYPE)
         self._dataset_client = DatasetClient(
             session=session, project=project, workspace_id=workspace_id
         )
 
     def base_url(self, dataset: Dataset) -> str:
```

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_clients/media_client/video_client.py` & `geti-sdk-1.5.3/geti_sdk/rest_clients/media_client/video_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_clients/model_client.py` & `geti-sdk-1.5.3/geti_sdk/rest_clients/model_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_clients/prediction_client.py` & `geti-sdk-1.5.3/geti_sdk/rest_clients/prediction_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_clients/project_client/__init__.py` & `geti-sdk-1.5.3/geti_sdk/rest_clients/project_client/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_clients/project_client/project_client.py` & `geti-sdk-1.5.3/geti_sdk/rest_clients/project_client/project_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_clients/project_client/task_templates.py` & `geti-sdk-1.5.3/geti_sdk/rest_clients/project_client/task_templates.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_clients/training_client.py` & `geti-sdk-1.5.3/geti_sdk/rest_clients/training_client.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_converters/__init__.py` & `geti-sdk-1.5.3/geti_sdk/rest_converters/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_converters/annotation_rest_converter/__init__.py` & `geti-sdk-1.5.3/geti_sdk/rest_converters/annotation_rest_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py` & `geti-sdk-1.5.3/geti_sdk/rest_converters/annotation_rest_converter/annotation_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py` & `geti-sdk-1.5.3/geti_sdk/rest_converters/annotation_rest_converter/normalized_annotation_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_converters/configuration_rest_converter.py` & `geti-sdk-1.5.3/geti_sdk/rest_converters/configuration_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_converters/job_rest_converter.py` & `geti-sdk-1.5.3/geti_sdk/rest_converters/job_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_converters/media_rest_converter.py` & `geti-sdk-1.5.3/geti_sdk/rest_converters/media_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_converters/model_rest_converter.py` & `geti-sdk-1.5.3/geti_sdk/rest_converters/model_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_converters/prediction_rest_converter/__init__.py` & `geti-sdk-1.5.3/geti_sdk/rest_converters/prediction_rest_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py` & `geti-sdk-1.5.3/geti_sdk/rest_converters/prediction_rest_converter/normalized_prediction_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py` & `geti-sdk-1.5.3/geti_sdk/rest_converters/prediction_rest_converter/prediction_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_converters/project_rest_converter.py` & `geti-sdk-1.5.3/geti_sdk/rest_converters/project_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/rest_converters/status_rest_converter.py` & `geti-sdk-1.5.3/geti_sdk/rest_converters/status_rest_converter.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/utils/__init__.py` & `geti-sdk-1.5.3/geti_sdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/utils/algorithm_helpers.py` & `geti-sdk-1.5.3/geti_sdk/utils/algorithm_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/utils/credentials_helpers.py` & `geti-sdk-1.5.3/geti_sdk/utils/credentials_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/utils/dictionary_helpers.py` & `geti-sdk-1.5.3/geti_sdk/utils/dictionary_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/utils/label_helpers.py` & `geti-sdk-1.5.3/geti_sdk/utils/label_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/utils/plot_helpers.py` & `geti-sdk-1.5.3/geti_sdk/utils/plot_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/utils/project_helpers.py` & `geti-sdk-1.5.3/geti_sdk/utils/project_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/utils/serialization_helpers.py` & `geti-sdk-1.5.3/geti_sdk/utils/serialization_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk/utils/workspace_helpers.py` & `geti-sdk-1.5.3/geti_sdk/utils/workspace_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk.egg-info/PKG-INFO` & `geti-sdk-1.5.3/geti_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geti-sdk
-Version: 1.5.2
+Version: 1.5.3
 Summary: Software Development Kit for the Intel® Geti™ platform
 Home-page: https://github.com/openvinotoolkit/geti-sdk
 Author: Intel OpenVINO
 Author-email: ludo.cornelissen@intel.com
 License: Copyright (C) 2022 Intel Corporation - All Rights Reserved. Licensed under the Apache License, Version 2.0 (the 'License'). See LICENSE file for more details.
 Project-URL: Documentation, https://openvinotoolkit.github.io/geti-sdk
 Project-URL: Bug Tracker, https://github.com/openvinotoolkit/geti-sdk/issues
```

### Comparing `geti-sdk-1.5.2/geti_sdk.egg-info/SOURCES.txt` & `geti-sdk-1.5.3/geti_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/geti_sdk.egg-info/requires.txt` & `geti-sdk-1.5.3/geti_sdk.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 joblib>=1.1.1
 protobuf>=3.20.2
 ovmsclient>=2022.3
 orjson==3.8.8
 
 [dev]
 vcrpy==4.2.*
-pytest==7.2.*
+pytest==7.3.*
 pytest-recording==0.12.*
 pytest-cov==4.0.*
 pytest-env==0.8.*
 pytest-html==3.2.*
 flake8>=4.0
 pydocstyle>=6.1
 black>=22.6
```

### Comparing `geti-sdk-1.5.2/setup.py` & `geti-sdk-1.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/tests/__init__.py` & `geti-sdk-1.5.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/tests/conftest.py` & `geti-sdk-1.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/tests/helpers/__init__.py` & `geti-sdk-1.5.3/tests/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/tests/helpers/constants.py` & `geti-sdk-1.5.3/tests/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/tests/helpers/enums.py` & `geti-sdk-1.5.3/tests/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/tests/helpers/finalizers.py` & `geti-sdk-1.5.3/tests/helpers/finalizers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/tests/helpers/fixtures.py` & `geti-sdk-1.5.3/tests/helpers/fixtures.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/tests/helpers/plotting.py` & `geti-sdk-1.5.3/tests/helpers/plotting.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/tests/helpers/project_helpers.py` & `geti-sdk-1.5.3/tests/helpers/project_helpers.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/tests/helpers/project_service.py` & `geti-sdk-1.5.3/tests/helpers/project_service.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/tests/helpers/training.py` & `geti-sdk-1.5.3/tests/helpers/training.py`

 * *Files identical despite different names*

### Comparing `geti-sdk-1.5.2/tests/helpers/vcr_helpers.py` & `geti-sdk-1.5.3/tests/helpers/vcr_helpers.py`

 * *Files identical despite different names*

