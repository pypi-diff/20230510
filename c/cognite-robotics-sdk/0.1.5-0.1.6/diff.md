# Comparing `tmp/cognite_robotics_sdk-0.1.5.tar.gz` & `tmp/cognite_robotics_sdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_robotics_sdk-0.1.5.tar", max compression
+gzip compressed data, was "cognite_robotics_sdk-0.1.6.tar", max compression
```

## Comparing `cognite_robotics_sdk-0.1.5.tar` & `cognite_robotics_sdk-0.1.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1252 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/README.md
--rw-r--r--   0        0        0       74 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/__init__.py
--rw-r--r--   0        0        0     1190 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/config/config.py
--rw-r--r--   0        0        0      255 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/data_classes.py
--rw-r--r--   0        0        0       67 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/data_uploader/__init__.py
--rw-r--r--   0        0        0     3132 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/data_uploader/data_classes.py
--rw-r--r--   0        0        0    11895 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/data_uploader/data_uploader.py
--rw-r--r--   0        0        0     1660 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/data_uploader/data_uploader_task.py
--rw-r--r--   0        0        0    11648 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/data_uploader/helpers.py
--rw-r--r--   0        0        0     9030 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/grpc/clients/robot_interface_client.py
--rw-r--r--   0        0        0     1505 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/grpc/clients/web_interface_client.py
--rw-r--r--   0        0        0       62 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/grpc/helpers/__init__.py
--rw-r--r--   0        0        0      821 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/grpc/helpers/bearer_token_auth.py
--rw-r--r--   0        0        0      826 2023-04-28 12:15:24.574271 cognite_robotics_sdk-0.1.5/cognite_robotics/grpc/helpers/channel.py
--rw-r--r--   0        0        0    10275 2023-04-28 12:15:24.575271 cognite_robotics_sdk-0.1.5/cognite_robotics/grpc/helpers/messages.py
--rw-r--r--   0        0        0        0 2023-04-28 12:29:41.554947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/__init__.py
--rw-r--r--   0        0        0     1453 2023-04-28 12:29:41.556947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/common_pb2.py
--rw-r--r--   0        0        0     1702 2023-04-28 12:29:41.535945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/common_pb2.pyi
--rw-r--r--   0        0        0     2519 2023-04-28 12:29:41.556947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/connectivity_pb2.py
--rw-r--r--   0        0        0     6430 2023-04-28 12:29:41.535945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/connectivity_pb2.pyi
--rw-r--r--   0        0        0     3047 2023-04-28 12:29:41.556947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/control_authority_pb2.py
--rw-r--r--   0        0        0     7303 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/control_authority_pb2.pyi
--rw-r--r--   0        0        0     2302 2023-04-28 12:29:41.556947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/data_pb2.py
--rw-r--r--   0        0        0     4811 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/data_pb2.pyi
--rw-r--r--   0        0        0     3228 2023-04-28 12:29:41.557947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/geometry_pb2.py
--rw-r--r--   0        0        0     8503 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/geometry_pb2.pyi
--rw-r--r--   0        0        0     1444 2023-04-28 12:29:41.557947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/joint_state_pb2.py
--rw-r--r--   0        0        0     1705 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/joint_state_pb2.pyi
--rw-r--r--   0        0        0     2590 2023-04-28 12:29:41.557947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_event_pb2.py
--rw-r--r--   0        0        0     5930 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_event_pb2.pyi
--rw-r--r--   0        0        0     1842 2023-04-28 12:29:41.557947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_log_pb2.py
--rw-r--r--   0        0        0     2460 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_log_pb2.pyi
--rw-r--r--   0        0        0     2384 2023-04-28 12:29:41.557947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_pb2.py
--rw-r--r--   0        0        0     5977 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_pb2.pyi
--rw-r--r--   0        0        0     1461 2023-04-28 12:29:41.557947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/payloads_pb2.py
--rw-r--r--   0        0        0     1805 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/payloads_pb2.pyi
--rw-r--r--   0        0        0     8330 2023-04-28 12:29:41.558947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_control_pb2.py
--rw-r--r--   0        0        0    23660 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_control_pb2.pyi
--rw-r--r--   0        0        0     2549 2023-04-28 12:29:41.558947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_registration_pb2.py
--rw-r--r--   0        0        0     4966 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_registration_pb2.pyi
--rw-r--r--   0        0        0     4899 2023-04-28 12:29:41.558947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_state_pb2.py
--rw-r--r--   0        0        0    12598 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_state_pb2.pyi
--rw-r--r--   0        0        0     4507 2023-04-28 12:29:41.558947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/video_pb2.py
--rw-r--r--   0        0        0    15277 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/video_pb2.pyi
--rw-r--r--   0        0        0     1597 2023-04-28 12:29:41.558947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/web_pb2.py
--rw-r--r--   0        0        0     2003 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/web_pb2.pyi
--rw-r--r--   0        0        0     2845 2023-04-28 12:29:41.558947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/services/robot_interface_pb2.py
--rw-r--r--   0        0        0      165 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/services/robot_interface_pb2.pyi
--rw-r--r--   0        0        0    15062 2023-04-28 12:29:41.559947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/services/robot_interface_pb2_grpc.py
--rw-r--r--   0        0        0     2853 2023-04-28 12:29:41.559947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/services/web_interface_pb2.py
--rw-r--r--   0        0        0      165 2023-04-28 12:29:41.536945 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/services/web_interface_pb2.pyi
--rw-r--r--   0        0        0    14820 2023-04-28 12:29:41.559947 cognite_robotics_sdk-0.1.5/cognite_robotics/protos/services/web_interface_pb2_grpc.py
--rw-r--r--   0        0        0       60 2023-04-28 12:15:24.576271 cognite_robotics_sdk-0.1.5/cognite_robotics/rest/__init__.py
--rw-r--r--   0        0        0      943 2023-04-28 12:15:24.576271 cognite_robotics_sdk-0.1.5/cognite_robotics/rest/base_model.py
--rw-r--r--   0        0        0       64 2023-04-28 12:15:24.576271 cognite_robotics_sdk-0.1.5/cognite_robotics/rest/client.py
--rw-r--r--   0        0        0    45829 2023-04-28 12:29:43.799103 cognite_robotics_sdk-0.1.5/cognite_robotics/rest/models.py
--rw-r--r--   0        0        0       58 2023-04-28 12:15:24.577271 cognite_robotics_sdk-0.1.5/cognite_robotics/utils/__init__.py
--rw-r--r--   0        0        0      645 2023-04-28 12:15:24.577271 cognite_robotics_sdk-0.1.5/cognite_robotics/utils/env_utils.py
--rw-r--r--   0        0        0     3016 2023-04-28 12:15:24.577271 cognite_robotics_sdk-0.1.5/cognite_robotics/utils/token.py
--rw-r--r--   0        0        0     2766 2023-04-28 12:15:24.577271 cognite_robotics_sdk-0.1.5/cognite_robotics/utils/utils.py
--rw-r--r--   0        0        0     1452 2023-04-28 12:15:24.578271 cognite_robotics_sdk-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1896 1970-01-01 00:00:00.000000 cognite_robotics_sdk-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1252 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/README.md
+-rw-r--r--   0        0        0       74 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/__init__.py
+-rw-r--r--   0        0        0     1190 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/config/config.py
+-rw-r--r--   0        0        0      255 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/data_classes.py
+-rw-r--r--   0        0        0       67 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/data_uploader/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/data_uploader/data_classes.py
+-rw-r--r--   0        0        0    11878 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/data_uploader/data_uploader.py
+-rw-r--r--   0        0        0     1662 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/data_uploader/data_uploader_task.py
+-rw-r--r--   0        0        0    11675 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/data_uploader/helpers.py
+-rw-r--r--   0        0        0     9034 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/grpc/clients/robot_interface_client.py
+-rw-r--r--   0        0        0     1505 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/grpc/clients/web_interface_client.py
+-rw-r--r--   0        0        0       62 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/grpc/helpers/__init__.py
+-rw-r--r--   0        0        0      821 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/grpc/helpers/bearer_token_auth.py
+-rw-r--r--   0        0        0      826 2023-05-10 08:49:07.564107 cognite_robotics_sdk-0.1.6/cognite_robotics/grpc/helpers/channel.py
+-rw-r--r--   0        0        0    10327 2023-05-10 08:49:07.565107 cognite_robotics_sdk-0.1.6/cognite_robotics/grpc/helpers/messages.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:02:55.487861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/__init__.py
+-rw-r--r--   0        0        0     1453 2023-05-10 09:02:55.489861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/common_pb2.py
+-rw-r--r--   0        0        0     1702 2023-05-10 09:02:55.469859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/common_pb2.pyi
+-rw-r--r--   0        0        0     2519 2023-05-10 09:02:55.489861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/connectivity_pb2.py
+-rw-r--r--   0        0        0     6430 2023-05-10 09:02:55.469859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/connectivity_pb2.pyi
+-rw-r--r--   0        0        0     3047 2023-05-10 09:02:55.489861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/control_authority_pb2.py
+-rw-r--r--   0        0        0     7303 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/control_authority_pb2.pyi
+-rw-r--r--   0        0        0     2302 2023-05-10 09:02:55.489861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/data_pb2.py
+-rw-r--r--   0        0        0     4811 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/data_pb2.pyi
+-rw-r--r--   0        0        0     3228 2023-05-10 09:02:55.489861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/geometry_pb2.py
+-rw-r--r--   0        0        0     8503 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/geometry_pb2.pyi
+-rw-r--r--   0        0        0     1444 2023-05-10 09:02:55.490861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/joint_state_pb2.py
+-rw-r--r--   0        0        0     1705 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/joint_state_pb2.pyi
+-rw-r--r--   0        0        0     2590 2023-05-10 09:02:55.490861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_event_pb2.py
+-rw-r--r--   0        0        0     5930 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_event_pb2.pyi
+-rw-r--r--   0        0        0     1842 2023-05-10 09:02:55.490861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_log_pb2.py
+-rw-r--r--   0        0        0     2460 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_log_pb2.pyi
+-rw-r--r--   0        0        0     2384 2023-05-10 09:02:55.490861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_pb2.py
+-rw-r--r--   0        0        0     5977 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_pb2.pyi
+-rw-r--r--   0        0        0     1461 2023-05-10 09:02:55.490861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/payloads_pb2.py
+-rw-r--r--   0        0        0     1805 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/payloads_pb2.pyi
+-rw-r--r--   0        0        0     8330 2023-05-10 09:02:55.490861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_control_pb2.py
+-rw-r--r--   0        0        0    23660 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_control_pb2.pyi
+-rw-r--r--   0        0        0     2549 2023-05-10 09:02:55.492861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_registration_pb2.py
+-rw-r--r--   0        0        0     4966 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_registration_pb2.pyi
+-rw-r--r--   0        0        0     4899 2023-05-10 09:02:55.492861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_state_pb2.py
+-rw-r--r--   0        0        0    12598 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_state_pb2.pyi
+-rw-r--r--   0        0        0     4507 2023-05-10 09:02:55.492861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/video_pb2.py
+-rw-r--r--   0        0        0    15277 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/video_pb2.pyi
+-rw-r--r--   0        0        0     1597 2023-05-10 09:02:55.492861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/web_pb2.py
+-rw-r--r--   0        0        0     2003 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/web_pb2.pyi
+-rw-r--r--   0        0        0     2845 2023-05-10 09:02:55.492861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/services/robot_interface_pb2.py
+-rw-r--r--   0        0        0      165 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/services/robot_interface_pb2.pyi
+-rw-r--r--   0        0        0    15062 2023-05-10 09:02:55.492861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/services/robot_interface_pb2_grpc.py
+-rw-r--r--   0        0        0     2853 2023-05-10 09:02:55.492861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/services/web_interface_pb2.py
+-rw-r--r--   0        0        0      165 2023-05-10 09:02:55.470859 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/services/web_interface_pb2.pyi
+-rw-r--r--   0        0        0    14820 2023-05-10 09:02:55.493861 cognite_robotics_sdk-0.1.6/cognite_robotics/protos/services/web_interface_pb2_grpc.py
+-rw-r--r--   0        0        0       60 2023-05-10 08:49:07.567107 cognite_robotics_sdk-0.1.6/cognite_robotics/rest/__init__.py
+-rw-r--r--   0        0        0      943 2023-05-10 08:49:07.567107 cognite_robotics_sdk-0.1.6/cognite_robotics/rest/base_model.py
+-rw-r--r--   0        0        0       64 2023-05-10 08:49:07.567107 cognite_robotics_sdk-0.1.6/cognite_robotics/rest/client.py
+-rw-r--r--   0        0        0    50682 2023-05-10 09:02:57.518000 cognite_robotics_sdk-0.1.6/cognite_robotics/rest/models.py
+-rw-r--r--   0        0        0       58 2023-05-10 08:49:07.567107 cognite_robotics_sdk-0.1.6/cognite_robotics/utils/__init__.py
+-rw-r--r--   0        0        0      645 2023-05-10 08:49:07.567107 cognite_robotics_sdk-0.1.6/cognite_robotics/utils/env_utils.py
+-rw-r--r--   0        0        0     3016 2023-05-10 08:49:07.567107 cognite_robotics_sdk-0.1.6/cognite_robotics/utils/token.py
+-rw-r--r--   0        0        0     3153 2023-05-10 08:49:07.567107 cognite_robotics_sdk-0.1.6/cognite_robotics/utils/utils.py
+-rw-r--r--   0        0        0     1460 2023-05-10 08:49:07.568107 cognite_robotics_sdk-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1946 1970-01-01 00:00:00.000000 cognite_robotics_sdk-0.1.6/PKG-INFO
```

### Comparing `cognite_robotics_sdk-0.1.5/README.md` & `cognite_robotics_sdk-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/config/config.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/config/config.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/data_uploader/data_classes.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/data_uploader/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/data_uploader/data_uploader.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/data_uploader/data_uploader.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,23 @@
     flatten_dict,
     get_upload_request_from_json,
     move_files,
     remove_files,
 )
 from cognite_robotics.grpc.clients.robot_interface_client import CogniteRobotInterfaceClient
 from cognite_robotics.protos.messages import data_pb2
-from cognite_robotics.utils.utils import handle_grpc_error
+from cognite_robotics.utils.utils import handle_grpc_error, to_thread
 
 logger = logging.getLogger(__name__)
 mimetypes.add_type("application/octet-stream", ".raw")
 
 
 async def data_uploader(
     stop_task_trigger: asyncio.Event,
-    data_upload_event_queue: asyncio.Queue[data_pb2.DataUploadEvent],
+    data_upload_event_queue: "asyncio.Queue[data_pb2.DataUploadEvent]",
     cognite_client: CogniteClient,
     data_set_id: int,
     config: DataUploaderConfig,
     loop_time_step_s: float = 1.0,
 ) -> None:
     """Upload data to CDF and notify Robotics Services."""
     while not stop_task_trigger.is_set():
@@ -119,15 +119,15 @@
         finally:
             logger.info("Data uploader stopped.")
 
 
 async def data_upload_event_message_publisher(
     stop_task_trigger: asyncio.Event,
     robot_interface_client: CogniteRobotInterfaceClient,
-    data_upload_event_queue: asyncio.Queue[data_pb2.DataUploadEvent],
+    data_upload_event_queue: "asyncio.Queue[data_pb2.DataUploadEvent]",
 ) -> None:
     """Handle data upload event and response."""
     logger.info("Starting data upload event message handler.")
     while not stop_task_trigger.is_set():
         data_upload_event = await data_upload_event_queue.get()
         logger.info(
             f"Sending data upload event, mission_run_id: `{data_upload_event.mission_report_id}`,"
@@ -148,15 +148,15 @@
 ) -> Optional[data_pb2.DataUploadEvent]:
     """Upload file to CDF."""
     file_path = upload_request.file_path
     if not os.path.exists(file_path):
         raise FileNotFoundError(f"File `{file_path}` not found.")
 
     external_id = upload_request.external_id
-    retrieved_files = await asyncio.to_thread(cognite_client.files.retrieve, external_id=external_id)
+    retrieved_files = await to_thread(cognite_client.files.retrieve, external_id=external_id)
     if retrieved_files is not None:
         if isinstance(retrieved_files, unittest.mock.MagicMock):
             logger.debug(f"Mocked response, external_id: `{external_id}`.")
         else:
             message = f"File already exists in CDF, retaining the existing file, external_id: `{external_id}`."
             logger.debug(message)
             # TODO: implement robot log client
@@ -176,15 +176,15 @@
 
     name = upload_request.name
     external_id = upload_request.external_id
 
     (mime_type, _) = mimetypes.guess_type(file_path)
 
     result = await asyncio.shield(
-        asyncio.to_thread(
+        to_thread(
             cognite_client.files.upload,
             file_path,
             name=name,
             external_id=external_id,
             metadata=cdf_metadata,
             data_set_id=data_set_id,
             mime_type=mime_type,  # type: ignore
@@ -212,20 +212,20 @@
 ) -> data_pb2.DataUploadEvent:
     """Upload data to a timeseries."""
     timeseries_external_id = upload_request.timeseries_external_id
 
     def check_timeseries_exists() -> bool:
         return cognite_client.time_series.retrieve(external_id=timeseries_external_id) is None
 
-    if not await asyncio.to_thread(check_timeseries_exists):
+    if not await to_thread(check_timeseries_exists):
         raise Exception(f"Timeseries does not exist, external_id: `{timeseries_external_id}`.")
 
     data_points = [datapoint.dict() for datapoint in upload_request.datapoints]
     await asyncio.shield(
-        asyncio.to_thread(cognite_client.time_series.data.insert, datapoints=data_points, external_id=timeseries_external_id)
+        to_thread(cognite_client.time_series.data.insert, datapoints=data_points, external_id=timeseries_external_id)
     )
     message = f"Datapoints upload successful, timeseries_external_id: `{timeseries_external_id}`."
     logger.info(message)
     # TODO: implement robot log client
     # await create_robot_log(
     #     message=message,
     #     severity=INFO,
```

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/data_uploader/data_uploader_task.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/data_uploader/data_uploader_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 async def data_uploader_tasks(
     stop_task_trigger: asyncio.Event,
     robot_interface_client: CogniteRobotInterfaceClient,
     data_set_id: int,
     config: DataUploaderConfig,
 ) -> None:
     """Set up tasks for data uploader."""
-    data_upload_event_queue: asyncio.Queue[data_pb2.DataUploadEvent] = asyncio.Queue()
+    data_upload_event_queue: "asyncio.Queue[data_pb2.DataUploadEvent]" = asyncio.Queue()
     cognite_client = create_cognite_client(client_name="data_uploader")
 
     data_uploader_task = asyncio.create_task(
         data_uploader(
             stop_task_trigger=stop_task_trigger,
             data_upload_event_queue=data_upload_event_queue,
             cognite_client=cognite_client,
```

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/data_uploader/helpers.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/data_uploader/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     Datapoint,
     DatapointsUploadRequest,
     DataUploaderConfig,
     FileUploadRequest,
     UploadRequestParseError,
 )
 from cognite_robotics.protos.messages import common_pb2, data_pb2
+from cognite_robotics.utils.utils import to_thread
 
 logger = logging.getLogger(__name__)
 
 
 async def create_file_upload_request(
     file_path: str,
     data_type: str,
@@ -244,15 +245,15 @@
                 continue
             try:
                 os.remove(file)
                 logger.debug(f"Removed {file}.")
             except OSError as e:
                 logger.error(f"Failed to remove `{file}`: {str(e)}")
 
-    await asyncio.shield(asyncio.to_thread(_remove_files))
+    await asyncio.shield(to_thread(_remove_files))
 
 
 async def move_files(
     files: List[str],
     to_folder: str,
 ) -> None:
     """Move files."""
@@ -264,15 +265,15 @@
                 continue
             try:
                 os.rename(file, os.path.join(to_folder, os.path.basename(file)))
                 logger.debug(f"Moved {file} to {to_folder}.")
             except Exception as e:
                 logger.error(f"Failed to move `{file}`: {str(e)}")
 
-    await asyncio.shield(asyncio.to_thread(_move_files))
+    await asyncio.shield(to_thread(_move_files))
 
 
 async def cleanup_upload_data_folder(upload_data_path: str) -> None:
     """Clean up the upload data folder.
 
     List all files in the upload data folder, check if there is a JSON file (e.g., the upload request instructions) for each file.
     If no associated JSON file is found, remove all other files.
@@ -298,15 +299,15 @@
     """
     for filename in os.listdir(folder):
         file_path = os.path.join(folder, filename)
         try:
             if os.path.isfile(file_path) or os.path.islink(file_path):
                 os.unlink(file_path)
             elif os.path.isdir(file_path):
-                await asyncio.shield(asyncio.to_thread(shutil.rmtree, file_path))
+                await asyncio.shield(to_thread(shutil.rmtree, file_path))
         except Exception as e:
             logger.error(f"Failed to delete {file_path}: {e}")
 
 
 def flatten_dict(d: Union[Dict[Any, Any], MutableMapping[Any, Any]], parent_key: str = "", sep: str = "_") -> Dict[Any, Any]:
     """Flatten dictionary.
```

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/grpc/clients/robot_interface_client.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/grpc/clients/robot_interface_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         await self.robot_interface_client.RobotRegistration(request, metadata=self._metadata)
 
     async def robot_connectivity(self) -> None:
         """Set up a stream to send connectivity status to cloud and send connected messages."""
         if not self.initialized_channel:
             await self._refresh_channel()
             self.initialized_channel = True
-        queue: asyncio.Queue[connectivity_pb2.Pong] = asyncio.Queue()
+        queue: "asyncio.Queue[connectivity_pb2.Pong]" = asyncio.Queue()
 
         async def _generate_pong() -> AsyncGenerator[object, None]:
             connect_message = Connect()
             pong = connectivity_pb2.Pong()
             pong.connect.CopyFrom(connect_message)
             yield pong
             while not self.stop_tasks_trigger.is_set():
@@ -126,15 +126,15 @@
             AsyncGenerator[UserControlCommand, None]: UserControlCommand
 
         """
         if not self.initialized_channel:
             await self._refresh_channel()
             self.initialized_channel = True
 
-        queue: asyncio.Queue[ControlEvent] = asyncio.Queue()
+        queue: "asyncio.Queue[ControlEvent]" = asyncio.Queue()
 
         async def _generate_control_events() -> AsyncGenerator[ControlEvent, None]:
             connect_message = Connect()
             control_event = ControlEvent()
             control_event.connect.CopyFrom(connect_message)
             yield control_event
             while not self.stop_tasks_trigger.is_set():
```

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/grpc/clients/web_interface_client.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/grpc/clients/web_interface_client.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/grpc/helpers/bearer_token_auth.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/grpc/helpers/bearer_token_auth.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/grpc/helpers/channel.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/grpc/helpers/channel.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/grpc/helpers/messages.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/grpc/helpers/messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """Helper functions to create gRPC messages."""
 
 
-from typing import List
+from typing import List, Optional
 
 from cognite_robotics.protos.messages.geometry_pb2 import BODY, MAP, Point, Quaternion, Transform
 from cognite_robotics.protos.messages.joint_state_pb2 import JointState, JointStates
 from cognite_robotics.protos.messages.mission_pb2 import RobotCapability
 from cognite_robotics.protos.messages.payloads_pb2 import AbsolutePTZ
 from cognite_robotics.protos.messages.robot_registration_pb2 import Metadata, RobotRegistrationRequest
 from cognite_robotics.protos.messages.robot_state_pb2 import (
@@ -29,15 +29,15 @@
 
 
 def robot_registration_request(
     robot_name: str,
     robot_description: str,
     robot_type: str,
     robot_capability_external_ids: List[str],
-    video_configuration: VideoConfiguration,
+    video_configuration: Optional[VideoConfiguration],
     has_estop: bool,
     has_power_on: bool,
 ) -> RobotRegistrationRequest:
     """Create a RobotRegistrationRequest.
 
     Args:
         robot_name (str): Name of the robot
@@ -55,16 +55,17 @@
         [RobotCapability(capability_external_id=capability_external_id) for capability_external_id in robot_capability_external_ids]
     )
     metadata = Metadata(
         three_d_model="",  # TODO: Deprecate this: https://cognitedata.atlassian.net/browse/RS-1133
         get_estop=has_estop,
         power_on=has_power_on,
     )
-    request.video_config.CopyFrom(video_configuration)
     request.metadata.CopyFrom(metadata)
+    if video_configuration:
+        request.video_config.CopyFrom(video_configuration)
     return request
 
 
 def video_configuration(
     description: str, stream_id: int, room_id: int, available_video_compositions: List[str], ptz_go_to: bool, navigate_to: bool
 ) -> VideoConfiguration:
     """Create a VideoConfiguration.
```

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/common_pb2.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/common_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/common_pb2.pyi` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/connectivity_pb2.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/connectivity_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/connectivity_pb2.pyi` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/connectivity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/control_authority_pb2.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/control_authority_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/control_authority_pb2.pyi` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/control_authority_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/data_pb2.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/data_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/data_pb2.pyi` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/geometry_pb2.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/geometry_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/geometry_pb2.pyi` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/geometry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/joint_state_pb2.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/joint_state_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/joint_state_pb2.pyi` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/joint_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_event_pb2.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_event_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_event_pb2.pyi` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_log_pb2.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_log_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_log_pb2.pyi` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_pb2.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/mission_pb2.pyi` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/mission_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/payloads_pb2.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/payloads_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/payloads_pb2.pyi` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/payloads_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_control_pb2.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_control_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_control_pb2.pyi` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_control_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_registration_pb2.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_registration_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_registration_pb2.pyi` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_registration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_state_pb2.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_state_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/robot_state_pb2.pyi` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/robot_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/video_pb2.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/video_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/video_pb2.pyi` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/video_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/web_pb2.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/web_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/messages/web_pb2.pyi` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/messages/web_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/services/robot_interface_pb2.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/services/robot_interface_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/services/robot_interface_pb2_grpc.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/services/robot_interface_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/services/web_interface_pb2.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/services/web_interface_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/protos/services/web_interface_pb2_grpc.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/protos/services/web_interface_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/rest/base_model.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/rest/base_model.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/rest/models.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/rest/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,20 +10,30 @@
 from pydantic import Extra, Field
 
 
 class RobotCapability(RoboticsBaseModel):
     class Config:
         allow_population_by_field_name = True
 
-    name: str = Field(..., description='RobotCapability name', example='ptz')
-    external_id: str = Field(..., alias='externalId', description='RobotCapability external id. Unique for the resource.', example='ptz')
+    name: str = Field(..., description='RobotCapability name', example='ptz', max_length=255, min_length=1)
+    external_id: str = Field(
+        ...,
+        alias='externalId',
+        description='RobotCapability external id. Unique for the resource.',
+        example='ptz',
+        max_length=255,
+        min_length=1,
+        regex='^[a-zA-Z]([a-zA-Z0-9_]{0,253}[a-zA-Z0-9])?$',
+    )
     method: str = Field(
         ...,
         description='RobotCapability method, must be unique. The method is used to call the right functionality on the robot.',
         example='ptz',
+        max_length=255,
+        min_length=1,
     )
     description: Optional[str] = Field(
         None, description='Description of the RobotCapability.', example='Pan, tilt, zoom camera for visual image capture'
     )
     input_schema: Any = Field(
         ...,
         alias='inputSchema',
@@ -53,29 +63,32 @@
     )
 
 
 class ExternalId(RoboticsBaseModel):
     class Config:
         allow_population_by_field_name = True
 
-    external_id: str = Field(..., alias='externalId')
+    external_id: str = Field(..., alias='externalId', max_length=255, min_length=1, regex='^[a-zA-Z]([a-zA-Z0-9_]{0,253}[a-zA-Z0-9])?$')
 
 
 class CreateAction(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
     external_id: Optional[str] = Field(
         None,
         alias='externalId',
         description='Action external id. Must be unique for the resource type. Will be set to a random value if not set in the request.',
         example='gaugeReading',
+        max_length=255,
+        min_length=1,
+        regex='^[a-zA-Z]([a-zA-Z0-9_]{0,253}[a-zA-Z0-9])?$',
     )
-    name: Optional[str] = Field(None, description='The name of the action.', example='Action name')
+    name: Optional[str] = Field(None, description='The name of the action.', example='Action name', max_length=255, min_length=1)
     robot_capability_external_id: str = Field(
         ..., alias='robotCapabilityExternalId', description='Id of the robot capability the action is created from.', example='ptz'
     )
     robot_capability_input: str = Field(
         ...,
         alias='robotCapabilityInput',
         description='Input to the robot capability. The input are values that configure the action, e.g pan, tilt and zoom values. The format of the input is defined by the input_schema of the robot capability.    #[schemars(example = "example_input")]',
@@ -130,15 +143,15 @@
     unknown = 'UNKNOWN'
 
 
 class CreateRobot(RoboticsBaseModel):
     class Config:
         allow_population_by_field_name = True
 
-    name: str = Field(..., description='Robot name.', example='Robot 1')
+    name: str = Field(..., description='Robot name.', example='Robot 1', max_length=255, min_length=1)
     description: Optional[str] = Field(None, description='A brief description of the robot.', example='Legged inspection robot 1')
     metadata: Optional[Dict[str, str]] = Field(
         None, description='Custom, application specific metadata. String key -> String value.', example={'key1': 'value1', 'key2': 'value2'}
     )
     robot_type: RobotType = Field(..., alias='robotType', description='Type of robot.', example='UNKNOWN')
     data_set_id: int = Field(..., alias='dataSetId', description='The id of the data set this asset belongs to.', example=9007199254740991)
     location_external_id: Optional[str] = Field(
@@ -170,28 +183,38 @@
 
 
 class ItemsForRobotCapability(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[RobotCapability]
+    items: List[RobotCapability] = Field(..., max_items=10000, min_items=1)
 
 
 class CreateRobotCapability(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    name: str = Field(..., description='RobotCapability name', example='ptz')
+    name: str = Field(..., description='RobotCapability name', example='ptz', max_length=255, min_length=1)
     external_id: Optional[str] = Field(
-        None, alias='externalId', description='RobotCapability external id. Must be unique for the resource type.', example='ptz'
+        None,
+        alias='externalId',
+        description='RobotCapability external id. Must be unique for the resource type.',
+        example='ptz',
+        max_length=255,
+        min_length=1,
+        regex='^[a-zA-Z]([a-zA-Z0-9_]{0,253}[a-zA-Z0-9])?$',
     )
     method: str = Field(
-        ..., description='RobotCapability method. The method is used to call the right functionality on the robot.', example='ptz'
+        ...,
+        description='RobotCapability method. The method is used to call the right functionality on the robot.',
+        example='ptz',
+        max_length=255,
+        min_length=1,
     )
     description: Optional[str] = Field(
         None,
         description='Description of RobotCapability. Textual description of the RobotCapability.',
         example='Pan, tilt, zoom camera for visual image capture',
     )
     input_schema: Optional[Any] = Field(
@@ -255,33 +278,42 @@
 
 
 class Transform(RoboticsBaseModel):
     class Config:
         allow_population_by_field_name = True
 
     parent_frame_external_id: str = Field(
-        ..., alias='parentFrameExternalId', description='Parent frame external id', example='rootCoordinateFrame'
+        ...,
+        alias='parentFrameExternalId',
+        description='Parent frame external id',
+        example='rootCoordinateFrame',
+        max_length=255,
+        min_length=1,
+        regex='^[a-zA-Z]([a-zA-Z0-9_]{0,253}[a-zA-Z0-9])?$',
     )
-    translation: Point3 = Field(..., description='Transform translation (x,y,z)', example={'x': 0.0, 'y': 0.0, 'z': 0.0})
+    translation: Point3 = Field(..., description='Transform translation (Point3)', example={'x': 0.0, 'y': 0.0, 'z': 0.0})
     orientation: Quaternion = Field(
-        ..., description='Transform orientation as quaternion (x,y,z,w)', example={'w': 1.0, 'x': 0.0, 'y': 0.0, 'z': 0.0}
+        ..., description='Transform orientation as quaternion (Quaternion)', example={'w': 1.0, 'x': 0.0, 'y': 0.0, 'z': 0.0}
     )
 
 
 class CreateFrame(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    name: str = Field(..., description='Frame name', example='Root coordinate frame of a location')
+    name: str = Field(..., description='Frame name', example='Root coordinate frame of a location', max_length=255, min_length=1)
     external_id: Optional[str] = Field(
         None,
         alias='externalId',
         description='Frame external id. Must be unique for the resource type. Will be set to a random value if not set in the request.',
         example='rootCoordinateFrame',
+        max_length=255,
+        min_length=1,
+        regex='^[a-zA-Z]([a-zA-Z0-9_]{0,253}[a-zA-Z0-9])?$',
     )
     transform: Optional[Transform] = Field(
         None,
         description='Transform of the parent frame to the current frame.',
         example={
             'orientation': {'w': 1.0, 'x': 0.0, 'y': 0.0, 'z': 0.0},
             'parentFrameExternalId': 'rootCoordinateFrame',
@@ -305,30 +337,38 @@
     pointcloud = 'POINTCLOUD'
 
 
 class CreateMap(RoboticsBaseModel):
     class Config:
         allow_population_by_field_name = True
 
-    name: str = Field(..., description='Map name.', example='Robot navigation map')
+    name: str = Field(..., description='Map name.', example='Robot navigation map', max_length=255, min_length=1)
     external_id: Optional[str] = Field(
         None,
         alias='externalId',
         description='Map external id. Must be unique for the resource type. Will be set to a random value if not set in the request.',
         example='robotMap',
+        max_length=255,
+        min_length=1,
+        regex='^[a-zA-Z]([a-zA-Z0-9_]{0,253}[a-zA-Z0-9])?$',
     )
-    description: Optional[str] = Field(None, description='Map description.', example='Robot navigation map')
+    description: Optional[str] = Field(None, description='Map description.', example='Robot navigation map', max_length=255, min_length=1)
     map_type: MapType = Field(
         ...,
         alias='mapType',
         description="Map type. Available robot types are 'WAYPOINTMAP', 'THREEDMODEL', 'TWODMAP', 'POINTCLOUD'.",
         example='WAYPOINTMAP',
     )
     frame_external_id: Optional[str] = Field(
-        None, alias='frameExternalId', description="External id of the map's reference frame.", example='rootCoordinateFrame'
+        None,
+        alias='frameExternalId',
+        description="External id of the map's reference frame.",
+        example='rootCoordinateFrame',
+        max_length=255,
+        min_length=1,
     )
     data: Optional[Any] = Field(None, description='Map-specific  data.', example='{"fileId": 1234567891012131}')
     location_external_id: Optional[str] = Field(
         None, alias='locationExternalId', description="External id of the map's location.", example='waterTreatmentPlant1'
     )
     scale: Optional[float] = Field(
         None, description='Uniform scaling factor, for example for map unit conversion (centimeter to meter)', example=1.0
@@ -345,15 +385,21 @@
 
 class Location(RoboticsBaseModel):
     class Config:
         allow_population_by_field_name = True
 
     name: str = Field(..., description='Location name', example='Water treatment plant')
     external_id: str = Field(
-        ..., alias='externalId', description='Location external id. Must be unique for the resource type.', example='waterTreatmentPlant1'
+        ...,
+        alias='externalId',
+        description='Location external id. Must be unique for the resource type.',
+        example='waterTreatmentPlant1',
+        max_length=255,
+        min_length=1,
+        regex='^[a-zA-Z]([a-zA-Z0-9_]{0,253}[a-zA-Z0-9])?$',
     )
     description: Optional[str] = Field(None, description='Location description', example='Water treatment plant')
     created_time: int = Field(
         ...,
         alias='createdTime',
         description='The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.',
         example=1649059819000,
@@ -367,80 +413,100 @@
 
 
 class CreateLocation(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    name: str = Field(..., description='Location name.', example='Water treatment plant')
+    name: str = Field(..., description='Location name.', example='Water treatment plant', max_length=255, min_length=1)
     external_id: Optional[str] = Field(
         None,
         alias='externalId',
         description='Location external id. Must be unique for the resource type. Will be set to a random value if not set in the request.',
         example='waterTreatmentPlant1',
+        max_length=255,
+        min_length=1,
+        regex='^[a-zA-Z]([a-zA-Z0-9_]{0,253}[a-zA-Z0-9])?$',
     )
     description: Optional[str] = Field(None, description='Textual description of the location.', example='Water treatment plant')
 
 
 class UpdateLocation(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    name: Optional[ValueUpdateForString] = Field(None, description='New location name.')
-    description: Optional[ValueUpdateForString] = Field(None, description='New location description.')
+    name: Optional[ValueUpdateForString] = Field(None, description='Update location name.', example='Water treatment plant')
+    description: Optional[ValueUpdateForString] = Field(None, description='Update location description', example='Water treatment plant')
 
 
 class DataPostprocessing(RoboticsBaseModel):
     class Config:
         allow_population_by_field_name = True
 
-    name: str = Field(..., description='DataPostprocessing name', example='Read dial gauge')
+    name: str = Field(..., description='DataPostprocessing name', example='Read dial gauge', max_length=255, min_length=1)
     external_id: str = Field(
-        ..., alias='externalId', description='DataPostprocessing external id. Unique for the resource.', example='read_dial_gauge'
+        ...,
+        alias='externalId',
+        description='DataPostprocessing external id. Unique for the resource.',
+        example='read_dial_gauge',
+        max_length=255,
+        min_length=1,
+        regex='^[a-zA-Z]([a-zA-Z0-9_]{0,253}[a-zA-Z0-9])?$',
     )
     method: str = Field(
         ...,
         description='DataPostprocessing method. The method is used to call the right functionality on the robot.',
         example='read_dial_gauge',
+        max_length=255,
+        min_length=1,
     )
     description: Optional[str] = Field(
         None,
         description='Description of the data postprocessing.',
         example='Read dial gauge from an image using Cognite Vision gauge reader',
+        max_length=255,
+        min_length=1,
     )
     input_schema: Any = Field(
         ...,
         alias='inputSchema',
         description='Schema that defines what inputs are needed for the data postprocessing. The input are values that configure the data postprocessing, e.g max and min values for a gauge.',
         example='{\n        "$schema": "http://json-schema.org/draft-07/schema#",\n        "id": "robotics/schemas/0.1.0/data_postprocessing/read_dial_gauge",\n        "title": "Read dial gauge postprocessing input",\n        "type": "object",\n        "properties": {\n            "image": {\n                "type": "object",\n                "properties": {\n                    "method": {\n                        "type": "string"\n                    },\n                    "parameters": {\n                        "type": "object",\n                        "properties": {\n                            "unit": {\n                                "type": "string"\n                            },\n                            "deadAngle": {\n                                "type": "number"\n                            },\n                            "minLevel": {\n                                "type": "number"\n                            },\n                            "maxLevel": {\n                                "type": "number"\n                            }\n                        }\n                    }\n                },\n                "required": [\n                    "method",\n                    "parameters"\n                ],\n                "additionalProperties": false\n            }\n        },\n        "additionalProperties": false\n    }',
     )
 
 
 class CreateDataPostprocessing(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    name: str = Field(..., description='DataPostprocessing name', example='Read dial gauge')
+    name: str = Field(..., description='DataPostprocessing name', example='Read dial gauge', max_length=255, min_length=1)
     external_id: Optional[str] = Field(
         None,
         alias='externalId',
         description='DataPostprocessing external id. Must be unique for the resource type.',
         example='read_dial_gauge',
+        max_length=255,
+        min_length=1,
+        regex='^[a-zA-Z]([a-zA-Z0-9_]{0,253}[a-zA-Z0-9])?$',
     )
     method: str = Field(
         ...,
         description='DataPostprocessing method. The method is used to call the right functionality on the robot.',
         example='read_dial_gauge',
+        max_length=255,
+        min_length=1,
     )
     description: Optional[str] = Field(
         None,
         description='Description of data_postprocessing. Textual description of the data_postprocessing.',
         example='Read dial gauge from an image using Cognite Vision gauge reader',
+        max_length=255,
+        min_length=1,
     )
     input_schema: Optional[Any] = Field(
         None,
         alias='inputSchema',
         description='Schema that defines what inputs are needed for the data postprocessing. The input are values that configure the data postprocessing, e.g max and min values for a gauge.',
         example='{\n        "$schema": "http://json-schema.org/draft-07/schema#",\n        "id": "robotics/schemas/0.1.0/data_postprocessing/read_dial_gauge",\n        "title": "Read dial gauge postprocessing input",\n        "type": "object",\n        "properties": {\n            "image": {\n                "type": "object",\n                "properties": {\n                    "method": {\n                        "type": "string"\n                    },\n                    "parameters": {\n                        "type": "object",\n                        "properties": {\n                            "unit": {\n                                "type": "string"\n                            },\n                            "deadAngle": {\n                                "type": "number"\n                            },\n                            "minLevel": {\n                                "type": "number"\n                            },\n                            "maxLevel": {\n                                "type": "number"\n                            }\n                        }\n                    }\n                },\n                "required": [\n                    "method",\n                    "parameters"\n                ],\n                "additionalProperties": false\n            }\n        },\n        "additionalProperties": false\n    }',
     )
@@ -458,17 +524,23 @@
 
 
 class Action(RoboticsBaseModel):
     class Config:
         allow_population_by_field_name = True
 
     external_id: str = Field(
-        ..., alias='externalId', description='Action external id. Must be unique for the resource type..', example='gaugeReading'
+        ...,
+        alias='externalId',
+        description='Action external id. Must be unique for the resource type..',
+        example='gaugeReading',
+        max_length=255,
+        min_length=1,
+        regex='^[a-zA-Z]([a-zA-Z0-9_]{0,253}[a-zA-Z0-9])?$',
     )
-    name: Optional[str] = Field(None, description='The name of the action.', example='Action name')
+    name: Optional[str] = Field(None, description='The name of the action.', example='Action name', max_length=255, min_length=1)
     action_number: int = Field(
         ...,
         alias='actionNumber',
         description='Action number. Defines the ascending chronological order in which actions should be executed.',
         example=1,
     )
     robot_capability: RobotCapability = Field(
@@ -501,31 +573,40 @@
 
 
 class ItemsForExternalId(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[ExternalId]
+    items: List[ExternalId] = Field(..., max_items=10000, min_items=1)
 
 
 class CreateMission(RoboticsBaseModel):
     class Config:
         allow_population_by_field_name = True
 
-    name: str = Field(..., description='Mission name.', example='Inspection mission 1')
+    name: str = Field(..., description='Mission name.', example='Inspection mission 1', max_length=255, min_length=1)
     external_id: Optional[str] = Field(
         None,
         alias='externalId',
         description='Mission external id. Must be unique for the resource type. Will be set to a random value if not set in the request.',
         example='inspectionMission1',
+        max_length=255,
+        min_length=1,
+        regex='^[a-zA-Z]([a-zA-Z0-9_]{0,253}[a-zA-Z0-9])?$',
+    )
+    map_external_id: str = Field(
+        ..., alias='mapExternalId', description='Id of the map the mission is defined in.', example='robotMap', max_length=255, min_length=1
     )
-    map_external_id: str = Field(..., alias='mapExternalId', description='Id of the map the mission is defined in.', example='robotMap')
     description: Optional[str] = Field(
-        None, description='Textual description of the mission.', example='Visual robot inspection of the water treatment plant'
+        None,
+        description='Textual description of the mission.',
+        example='Visual robot inspection of the water treatment plant',
+        max_length=255,
+        min_length=1,
     )
     actions: List[CreateAction] = Field(
         ..., description='Actions to be executed in the mission. The order of the actions in the list defines the execution order.'
     )
 
 
 class UpdateMission(RoboticsBaseModel):
@@ -540,15 +621,15 @@
     )
 
 
 class Robot(RoboticsBaseModel):
     class Config:
         allow_population_by_field_name = True
 
-    name: str = Field(..., description='Robot name', example='Robot 1')
+    name: str = Field(..., description='Robot name', example='Robot 1', max_length=255, min_length=1)
     description: Optional[str] = Field(None, description='A brief description of the robot', example='Legged inspection robot 1')
     capabilities: List[str] = Field(..., description='List of externalIds of the capabilities the robot can perform.')
     metadata: Optional[Dict[str, str]] = Field(
         None, description='Custom, application specific metadata. String key -> String value.', example={'key1': 'value1', 'key2': 'value2'}
     )
     robot_type: RobotType = Field(..., alias='robotType', description='Type of robot.', example='UNKNOWN')
     data_set_id: int = Field(..., alias='dataSetId', description='The id of the data set this asset belongs to.', example=9007199254740991)
@@ -570,23 +651,23 @@
 
 
 class ItemsForCreateRobot(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[CreateRobot]
+    items: List[CreateRobot] = Field(..., max_items=10000, min_items=1)
 
 
 class ItemsForDatasetId(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[DatasetId]
+    items: List[DatasetId] = Field(..., max_items=10000, min_items=1)
 
 
 class UpdateRobot(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
@@ -602,15 +683,15 @@
 
 
 class ItemsForCreateRobotCapability(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[CreateRobotCapability]
+    items: List[CreateRobotCapability] = Field(..., max_items=10000, min_items=1)
 
 
 class UpdateRobotCapability(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
@@ -623,15 +704,20 @@
 
 class Waypoint(RoboticsBaseModel):
     class Config:
         allow_population_by_field_name = True
 
     external_id: str = Field(..., alias='externalId', description='Waypoint external id', example='waypoint1')
     map_external_id: str = Field(
-        ..., alias='mapExternalId', description='External id of the map the waypoint is defined in', example='robotMap'
+        ...,
+        alias='mapExternalId',
+        description='External id of the map the waypoint is defined in',
+        example='robotMap',
+        max_length=255,
+        min_length=1,
     )
     position: Point3 = Field(
         ...,
         description='Coordinates of waypoint in the frame of the map defined by map_external_id',
         example={'x': 0.0, 'y': 0.0, 'z': 0.0},
     )
     orientation: Quaternion = Field(
@@ -642,23 +728,31 @@
 
 
 class ItemsForCreateWaypoint(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[CreateWaypoint]
+    items: List[CreateWaypoint] = Field(..., max_items=10000, min_items=1)
 
 
 class Frame(RoboticsBaseModel):
     class Config:
         allow_population_by_field_name = True
 
-    name: str = Field(..., description='Frame name', example='Root coordinate frame of a location')
-    external_id: str = Field(..., alias='externalId', description='Frame external id', example='rootCoordinateFrame')
+    name: str = Field(..., description='Frame name', example='Root coordinate frame of a location', max_length=255, min_length=1)
+    external_id: str = Field(
+        ...,
+        alias='externalId',
+        description='Frame external id',
+        example='rootCoordinateFrame',
+        max_length=255,
+        min_length=1,
+        regex='^[a-zA-Z]([a-zA-Z0-9_]{0,253}[a-zA-Z0-9])?$',
+    )
     created_time: int = Field(
         ...,
         alias='createdTime',
         description='Created time in the number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.',
         example=1649059819000,
     )
     updated_time: int = Field(
@@ -679,104 +773,129 @@
 
 
 class ItemsForCreateFrame(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[CreateFrame]
+    items: List[CreateFrame] = Field(..., max_items=10000, min_items=1)
 
 
 class UpdateFrame(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    name: Optional[ValueUpdateForString] = Field(None, description='new frame name')
-    transform: Optional[ValueUpdateForTransform] = Field(None, description='update transform')
+    name: Optional[ValueUpdateForString] = Field(None, description='Update frame name', example='Root coordinate frame of a location')
+    transform: Optional[ValueUpdateForTransform] = Field(
+        None,
+        description='Update transform',
+        example={
+            'orientation': {'w': 1.0, 'x': 0.0, 'y': 0.0, 'z': 0.0},
+            'parentFrameExternalId': 'rootCoordinateFrame',
+            'translation': {'x': 0.0, 'y': 0.0, 'z': 0.0},
+        },
+    )
 
 
 class MapInfo(RoboticsBaseModel):
     class Config:
         allow_population_by_field_name = True
 
-    external_id: str = Field(..., alias='externalId', description='Map external id.', example='robotMap')
+    external_id: str = Field(
+        ...,
+        alias='externalId',
+        description='Map external id.',
+        example='robotMap',
+        max_length=255,
+        min_length=1,
+        regex='^[a-zA-Z]([a-zA-Z0-9_]{0,253}[a-zA-Z0-9])?$',
+    )
     created_time: int = Field(
         ...,
         alias='createdTime',
         description='The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.',
         example=1649059819000,
     )
     updated_time: int = Field(
         ...,
         alias='updatedTime',
         description='The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.',
         example=1649059819000,
     )
-    name: str = Field(..., description='Map name.', example='Robot navigation map')
-    description: Optional[str] = Field(None, description='Map description.', example='Robot navigation map')
+    name: str = Field(..., description='Map name.', example='Robot navigation map', max_length=255, min_length=1)
+    description: Optional[str] = Field(None, description='Map description.', example='Robot navigation map', max_length=255, min_length=1)
     map_type: MapType = Field(
         ...,
         alias='mapType',
         description="Map type. Available robot types are 'WAYPOINTMAP', 'THREEDMODEL', 'TWODMAP', 'POINTCLOUD'.",
         example='WAYPOINTMAP',
     )
     frame_external_id: Optional[str] = Field(
         None, alias='frameExternalId', description="External id of the map's reference frame.", example='rootCoordinateFrame'
     )
     data: Optional[Any] = Field(None, description='Map-specific data.', example='{"fileId": 1234567891012131}')
     location_external_id: Optional[str] = Field(
-        None, alias='locationExternalId', description="External id of the map's location.", example='waterTreatmentPlant1'
+        None,
+        alias='locationExternalId',
+        description="External id of the map's location.",
+        example='waterTreatmentPlant1',
+        max_length=255,
+        min_length=1,
     )
     scale: float = Field(..., description='Uniform scaling factor, for example for map unit conversion (centimeter to meter)', example=1.0)
     base_waypoint_external_id: Optional[str] = Field(
         None, alias='baseWaypointExternalId', description='Base waypoint point id.', example='waypoint1'
     )
 
 
 class ItemsForCreateMap(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[CreateMap]
+    items: List[CreateMap] = Field(..., max_items=10000, min_items=1)
 
 
 class UpdateMap(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    name: Optional[ValueUpdateForString] = Field(None, description='New map name.')
-    description: Optional[ValueUpdateForString] = Field(None, description='New map description.')
-    frame_external_id: Optional[ValueUpdateForString] = Field(None, alias='frameExternalId', description='New frame external id.')
-    data: Optional[ValueUpdateForAnyValue] = Field(None, description='Map data fields to set.')
+    name: Optional[ValueUpdateForString] = Field(None, description='New map name.', example='Robot navigation map')
+    description: Optional[ValueUpdateForString] = Field(None, description='New map description.', example='Robot navigation map')
+    frame_external_id: Optional[ValueUpdateForString] = Field(
+        None, alias='frameExternalId', description='New frame external id.', example='rootCoordinateFrame'
+    )
+    data: Optional[ValueUpdateForAnyValue] = Field(None, description='Map data fields to set.', example='{"fileId": 1234567891012131}')
     location_external_id: Optional[ValueUpdateForString] = Field(
-        None, alias='locationExternalId', description="External id of the map's location."
+        None, alias='locationExternalId', description="External id of the map's location.", example='waterTreatmentPlant1'
     )
     scale: Optional[ValueUpdateForDouble] = Field(
-        None, description='Uniform scaling factor, for example for map unit conversion (centimeter to meter)'
+        None, description='Uniform scaling factor, for example for map unit conversion (centimeter to meter)', example=1.0
+    )
+    base_waypoint_external_id: Optional[ValueUpdateForString] = Field(
+        None, alias='baseWaypointExternalId', description='Base waypoint id.', example='waypoint1'
     )
-    base_waypoint_external_id: Optional[ValueUpdateForString] = Field(None, alias='baseWaypointExternalId', description='Base waypoint id.')
 
 
 class ItemsForLocation(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[Location]
+    items: List[Location] = Field(..., max_items=10000, min_items=1)
 
 
 class ItemsForCreateLocation(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[CreateLocation]
+    items: List[CreateLocation] = Field(..., max_items=10000, min_items=1)
 
 
 class ResourceUpdateForUpdateLocation(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
@@ -785,23 +904,23 @@
 
 
 class ItemsForDataPostprocessing(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[DataPostprocessing]
+    items: List[DataPostprocessing] = Field(..., max_items=10000, min_items=1)
 
 
 class ItemsForCreateDataPostprocessing(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[CreateDataPostprocessing]
+    items: List[CreateDataPostprocessing] = Field(..., max_items=10000, min_items=1)
 
 
 class ResourceUpdateForUpdateDataPostprocessing(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
@@ -809,41 +928,51 @@
     update: UpdateDataPostprocessing = Field(..., description='Update.')
 
 
 class Mission(RoboticsBaseModel):
     class Config:
         allow_population_by_field_name = True
 
-    name: str = Field(..., description='Mission name.', example='Inspection mission 1')
+    name: str = Field(..., description='Mission name.', example='Inspection mission 1', max_length=255, min_length=1)
     external_id: str = Field(
-        ..., alias='externalId', description='Mission external id. Must be unique for the resource type.', example='inspectionMission1'
+        ...,
+        alias='externalId',
+        description='Mission external id. Must be unique for the resource type.',
+        example='inspectionMission1',
+        max_length=255,
+        min_length=1,
+        regex='^[a-zA-Z]([a-zA-Z0-9_]{0,253}[a-zA-Z0-9])?$',
+    )
+    map_external_id: str = Field(
+        ..., alias='mapExternalId', description='Id of the map the mission is defined in.', example='robotMap', max_length=255, min_length=1
     )
-    map_external_id: str = Field(..., alias='mapExternalId', description='Id of the map the mission is defined in.', example='robotMap')
     description: Optional[str] = Field(
         None, description='Textual description of the mission.', example='Visual robot inspection of the water treatment plant'
     )
     actions: List[Action] = Field(..., description='List of actions in the mission.')
     created_time: int = Field(
         ...,
         alias='createdTime',
         description='The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.',
+        example=1649059819000,
     )
     updated_time: int = Field(
         ...,
         alias='updatedTime',
         description='The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.',
+        example=1649059819000,
     )
 
 
 class ItemsForCreateMission(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[CreateMission]
+    items: List[CreateMission] = Field(..., max_items=10000, min_items=1)
 
 
 class ResourceUpdateForUpdateMission(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
@@ -852,15 +981,15 @@
 
 
 class ItemsForRobot(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[Robot]
+    items: List[Robot] = Field(..., max_items=10000, min_items=1)
 
 
 class RobotResourceUpdateForUpdateRobot(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
@@ -878,23 +1007,23 @@
 
 
 class ItemsForWaypoint(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[Waypoint]
+    items: List[Waypoint] = Field(..., max_items=10000, min_items=1)
 
 
 class ItemsForFrame(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[Frame]
+    items: List[Frame] = Field(..., max_items=10000, min_items=1)
 
 
 class ResourceUpdateForUpdateFrame(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
@@ -903,15 +1032,15 @@
 
 
 class ItemsForMapInfo(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[MapInfo]
+    items: List[MapInfo] = Field(..., max_items=10000, min_items=1)
 
 
 class ResourceUpdateForUpdateMap(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
@@ -920,64 +1049,64 @@
 
 
 class ItemsForResourceUpdateForUpdateLocation(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[ResourceUpdateForUpdateLocation]
+    items: List[ResourceUpdateForUpdateLocation] = Field(..., max_items=10000, min_items=1)
 
 
 class ItemsForResourceUpdateForUpdateDataPostprocessing(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[ResourceUpdateForUpdateDataPostprocessing]
+    items: List[ResourceUpdateForUpdateDataPostprocessing] = Field(..., max_items=10000, min_items=1)
 
 
 class ItemsForMission(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[Mission]
+    items: List[Mission] = Field(..., max_items=10000, min_items=1)
 
 
 class ItemsForResourceUpdateForUpdateMission(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[ResourceUpdateForUpdateMission]
+    items: List[ResourceUpdateForUpdateMission] = Field(..., max_items=10000, min_items=1)
 
 
 class ItemsForRobotResourceUpdateForUpdateRobot(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[RobotResourceUpdateForUpdateRobot]
+    items: List[RobotResourceUpdateForUpdateRobot] = Field(..., max_items=10000, min_items=1)
 
 
 class ItemsForResourceUpdateForUpdateRobotCapability(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[ResourceUpdateForUpdateRobotCapability]
+    items: List[ResourceUpdateForUpdateRobotCapability] = Field(..., max_items=10000, min_items=1)
 
 
 class ItemsForResourceUpdateForUpdateFrame(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[ResourceUpdateForUpdateFrame]
+    items: List[ResourceUpdateForUpdateFrame] = Field(..., max_items=10000, min_items=1)
 
 
 class ItemsForResourceUpdateForUpdateMap(RoboticsBaseModel):
     class Config:
         extra = Extra.forbid
         allow_population_by_field_name = True
 
-    items: List[ResourceUpdateForUpdateMap]
+    items: List[ResourceUpdateForUpdateMap] = Field(..., max_items=10000, min_items=1)
```

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/utils/env_utils.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/utils/token.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/utils/token.py`

 * *Files identical despite different names*

### Comparing `cognite_robotics_sdk-0.1.5/cognite_robotics/utils/utils.py` & `cognite_robotics_sdk-0.1.6/cognite_robotics/utils/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # -*- coding: utf-8 -*-
 """Utils tests."""
 import asyncio
+import contextvars
+import functools
 import logging
-from typing import AsyncGenerator, List, Optional, TypeVar
+import typing
+from typing import Any, AsyncGenerator, List, Optional, TypeVar
 
 import grpc
 from cognite.client import CogniteClient
 from cognite.client.config import ClientConfig
 from cognite.client.credentials import OAuthClientCredentials
 
 from cognite_robotics.utils.env_utils import get_env
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
 
-async def yield_from_queue(queue: asyncio.Queue[T]) -> AsyncGenerator[T, None]:
+async def yield_from_queue(queue: "asyncio.Queue[T]") -> AsyncGenerator[T, None]:
     """Yield items from a queue.
 
     Args:
         queue (asyncio.Queue[T]): queue to yield items from
     Returns:
         AsyncGenerator[T, None]: generator of items from the queue
     """
@@ -75,7 +78,16 @@
     token_url = f"https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/token"
     client_id = get_env("COGNITE_CLIENT_ID")
     token_scopes = [f"{base_url}/.default"]
 
     creds = OAuthClientCredentials(token_url=token_url, client_id=client_id, client_secret=client_secret, scopes=token_scopes)
     cnf = ClientConfig(client_name=client_name, base_url=base_url, project=str(project), credentials=creds)
     return CogniteClient(cnf)
+
+
+@typing.no_type_check
+async def to_thread(func, /, *args, **kwargs) -> Any:
+    """Asyncio thread implementation for Python 3.8."""
+    loop = asyncio.get_running_loop()
+    ctx = contextvars.copy_context()
+    func_call = functools.partial(ctx.run, func, *args, **kwargs)
+    return await loop.run_in_executor(None, func_call)
```

### Comparing `cognite_robotics_sdk-0.1.5/pyproject.toml` & `cognite_robotics_sdk-0.1.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 description = "Cognite Robotics SDK"
 name = "cognite-robotics-sdk"
 packages = [
     { include = "cognite_robotics", from = "." },
     { include = "protos", from = "cognite_robotics" },
 ]
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
-aiofiles = "23.1.0"
-cognite-sdk = "6.0.1"
-grpcio = "1.54.0"
-protobuf = "4.22.3"
+aiofiles = ">=23.1.0"
+cognite-sdk = ">=6.0.0"
+grpcio = ">=1.54.0"
+protobuf = ">=4.22.3"
 pydantic = "1.10.7"
-python = "^3.9"
+python = "^3.8"
 python-dotenv = "0.21.1"
 
 [tool.poetry.dev-dependencies]
 black = "23.3.0"
 datamodel-code-generator = "0.18.0"
 mypy = "1.2.0"
-pre-commit = "3.2.2"
+pre-commit = "3.3.1"
 pytest = "7.3.1"
 pytest-asyncio = "0.21.0"
 types-aiofiles = "23.1.0.1"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `cognite_robotics_sdk-0.1.5/PKG-INFO` & `cognite_robotics_sdk-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: cognite-robotics-sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: Cognite Robotics SDK
 Author: Cognite Robotics
 Author-email: robotics-team@cognite.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiofiles (==23.1.0)
-Requires-Dist: cognite-sdk (==6.0.1)
-Requires-Dist: grpcio (==1.54.0)
-Requires-Dist: protobuf (==4.22.3)
+Requires-Dist: aiofiles (>=23.1.0)
+Requires-Dist: cognite-sdk (>=6.0.0)
+Requires-Dist: grpcio (>=1.54.0)
+Requires-Dist: protobuf (>=4.22.3)
 Requires-Dist: pydantic (==1.10.7)
 Requires-Dist: python-dotenv (==0.21.1)
 Description-Content-Type: text/markdown
 
 # Cognite Robotics SDK
 
 [![PyPI version](https://badge.fury.io/py/cognite-robotics-sdk.svg)](https://pypi.org/project/cognite-robotics-sdk/)
```

