# Comparing `tmp/qwak_core-0.0.53.tar.gz` & `tmp/qwak_core-0.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.53.tar", max compression
+gzip compressed data, was "qwak_core-0.0.54.tar", max compression
```

## Comparing `qwak_core-0.0.53.tar` & `qwak_core-0.0.54.tar`

### file list

```diff
@@ -1,570 +1,570 @@
--rw-r--r--   0        0        0      264 2023-05-08 09:17:44.147743 qwak_core-0.0.53/README.md
--rw-r--r--   0        0        0        0 2023-05-08 09:19:32.672442 qwak_core-0.0.53/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-08 09:19:32.700442 qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-08 09:19:10.208298 qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.700442 qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-08 09:19:32.696442 qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-08 09:19:09.812295 qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.696442 qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-08 09:19:32.700442 qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-08 09:19:10.008296 qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.700442 qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-08 09:19:32.688442 qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-08 09:19:09.220291 qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-08 09:19:32.692442 qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-08 09:19:32.692442 qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-08 09:19:09.416292 qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.692442 qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-05-08 09:19:32.692442 qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-05-08 09:19:09.620294 qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.696442 qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-08 09:19:32.676442 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-08 09:19:09.020290 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-08 09:19:32.676442 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-05-08 09:19:32.676442 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-05-08 09:19:10.408299 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.680441 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-08 09:19:32.684442 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-08 09:19:10.792301 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.684442 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-08 09:19:32.684442 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-08 09:19:11.004303 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-08 09:19:32.684442 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-08 09:19:32.680441 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-08 09:19:10.600300 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.680441 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-08 09:19:32.688442 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-08 09:19:11.212304 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.688442 qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-08 09:19:32.732442 qwak_core-0.0.53/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-08 09:19:14.240323 qwak_core-0.0.53/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.732442 qwak_core-0.0.53/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-08 09:19:32.736442 qwak_core-0.0.53/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-08 09:19:14.488325 qwak_core-0.0.53/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-08 09:19:32.736442 qwak_core-0.0.53/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-08 09:19:32.812442 qwak_core-0.0.53/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-08 09:19:20.324362 qwak_core-0.0.53/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.812442 qwak_core-0.0.53/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-08 09:19:32.812442 qwak_core-0.0.53/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-08 09:19:20.536364 qwak_core-0.0.53/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-08 09:19:32.816442 qwak_core-0.0.53/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-08 09:19:32.816442 qwak_core-0.0.53/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-08 09:19:21.560370 qwak_core-0.0.53/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-08 09:19:32.820443 qwak_core-0.0.53/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-08 09:19:32.816442 qwak_core-0.0.53/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-08 09:19:21.364369 qwak_core-0.0.53/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.816442 qwak_core-0.0.53/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5497 2023-05-08 09:19:32.820443 qwak_core-0.0.53/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7820 2023-05-08 09:19:21.752372 qwak_core-0.0.53/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.820443 qwak_core-0.0.53/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-08 09:19:32.824442 qwak_core-0.0.53/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-08 09:19:21.948373 qwak_core-0.0.53/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-08 09:19:32.824442 qwak_core-0.0.53/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    11441 2023-05-08 09:19:32.892443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    17892 2023-05-08 09:19:27.712410 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.896443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5494 2023-05-08 09:19:32.888443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7776 2023-05-08 09:19:27.296407 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.888443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-08 09:19:32.892443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-08 09:19:27.512408 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.892443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-08 09:19:32.884443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-08 09:19:26.884405 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-08 09:19:32.884443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-08 09:19:32.888443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-08 09:19:27.092406 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.888443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-08 09:19:32.900443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-08 09:19:28.316413 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.900443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-08 09:19:32.896443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-08 09:19:28.120412 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.900443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-08 09:19:32.896443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-08 09:19:27.916411 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.896443 qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-08 09:19:32.940443 qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-08 09:19:31.920437 qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.944443 qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-08 09:19:32.936443 qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-08 09:19:31.528434 qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.940443 qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    37419 2023-05-08 09:19:32.940443 qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    48027 2023-05-08 09:19:31.728435 qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-08 09:19:32.940443 qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    18658 2023-05-08 09:19:32.856443 qwak_core-0.0.53/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    15525 2023-05-08 09:19:24.000386 qwak_core-0.0.53/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    18652 2023-05-08 09:19:32.856443 qwak_core-0.0.53/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-08 09:19:32.852443 qwak_core-0.0.53/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-08 09:19:23.800385 qwak_core-0.0.53/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.852443 qwak_core-0.0.53/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-05-08 09:19:32.840443 qwak_core-0.0.53/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-05-08 09:19:23.412382 qwak_core-0.0.53/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.840443 qwak_core-0.0.53/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-08 09:19:32.840443 qwak_core-0.0.53/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-08 09:19:23.604383 qwak_core-0.0.53/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.844443 qwak_core-0.0.53/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-08 09:19:32.844443 qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-08 09:19:24.208387 qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-08 09:19:32.844443 qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-05-08 09:19:32.848443 qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-05-08 09:19:24.640390 qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-08 09:19:32.852443 qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-08 09:19:32.864443 qwak_core-0.0.53/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-08 09:19:25.068393 qwak_core-0.0.53/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.864443 qwak_core-0.0.53/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-08 09:19:32.864443 qwak_core-0.0.53/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-08 09:19:25.272394 qwak_core-0.0.53/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-08 09:19:32.868443 qwak_core-0.0.53/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-08 09:19:32.832443 qwak_core-0.0.53/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-08 09:19:22.776378 qwak_core-0.0.53/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.832443 qwak_core-0.0.53/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-08 09:19:32.836443 qwak_core-0.0.53/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-08 09:19:22.980379 qwak_core-0.0.53/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-08 09:19:32.836443 qwak_core-0.0.53/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-08 09:19:32.828442 qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-08 09:19:22.352375 qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.828442 qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    42956 2023-05-08 09:19:32.824442 qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    62847 2023-05-08 09:19:22.156374 qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.828442 qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-08 09:19:32.828442 qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-08 09:19:22.572377 qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-08 09:19:32.832443 qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-08 09:19:32.720442 qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-08 09:19:13.100316 qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.724442 qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-08 09:19:32.724442 qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-08 09:19:13.328317 qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.724442 qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-08 09:19:32.724442 qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-08 09:19:13.580319 qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-08 09:19:32.728442 qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-08 09:19:32.792442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-08 09:19:19.120355 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.792442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-08 09:19:32.788442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-08 09:19:18.920354 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-08 09:19:32.788442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0     9535 2023-05-08 09:19:32.768442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    10460 2023-05-08 09:19:17.140342 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.768442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5268 2023-05-08 09:19:32.764442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8525 2023-05-08 09:19:16.940341 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.768442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-08 09:19:32.756442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-08 09:19:16.308337 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.760442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    27847 2023-05-08 09:19:32.764442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20073 2023-05-08 09:19:16.744340 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    33080 2023-05-08 09:19:32.764442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-08 09:19:32.768442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-08 09:19:17.336343 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.772442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-08 09:19:32.772442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-08 09:19:17.528344 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-08 09:19:32.772442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25213 2023-05-08 09:19:32.760442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37366 2023-05-08 09:19:16.528338 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.760442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-08 09:19:32.776442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-08 09:19:17.724346 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.776442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0     5958 2023-05-08 09:19:32.776442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.py
--rw-r--r--   0        0        0     6232 2023-05-08 09:19:17.932347 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.776442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-08 09:19:32.792442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-08 09:19:32.120438 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.792442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-08 09:19:32.796442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-08 09:19:32.316439 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-08 09:19:32.796442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-08 09:19:32.796442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-08 09:19:19.732359 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.800442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-08 09:19:32.800442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-08 09:19:19.932360 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-08 09:19:32.800442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-08 09:19:32.800442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-08 09:19:20.132361 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.804442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-08 09:19:32.808442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-08 09:19:20.960367 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.808442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-08 09:19:32.804442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-08 09:19:20.748365 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-08 09:19:32.804442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-08 09:19:32.808442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-08 09:19:21.160368 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.808442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-08 09:19:32.780442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-08 09:19:18.144348 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.780442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-08 09:19:32.780442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-08 09:19:18.336350 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.784442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-08 09:19:32.784442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-08 09:19:18.528351 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-08 09:19:32.784442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-08 09:19:32.784442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-08 09:19:18.720352 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.788442 qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-08 09:19:32.904443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-08 09:19:28.524415 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.904443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-08 09:19:32.904443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-08 09:19:28.720416 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-08 09:19:32.908443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-08 09:19:32.908443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-08 09:19:28.932417 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.908443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-08 09:19:32.908443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-08 09:19:29.140419 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-08 09:19:32.912443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-08 09:19:32.912443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-08 09:19:29.356420 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-08 09:19:32.912443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-08 09:19:32.916443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-08 09:19:29.552421 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.916443 qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-08 09:19:32.868443 qwak_core-0.0.53/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-08 09:19:25.472396 qwak_core-0.0.53/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.868443 qwak_core-0.0.53/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-08 09:19:32.868443 qwak_core-0.0.53/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-08 09:19:25.668397 qwak_core-0.0.53/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-08 09:19:32.872443 qwak_core-0.0.53/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-08 09:19:32.740442 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-08 09:19:15.432331 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.740442 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-08 09:19:32.740442 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-08 09:19:15.660333 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.744442 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-08 09:19:32.744442 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-08 09:19:15.872334 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-08 09:19:32.752442 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-08 09:19:32.756442 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-08 09:19:16.084335 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.756442 qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-08 09:19:32.836443 qwak_core-0.0.53/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-08 09:19:23.188381 qwak_core-0.0.53/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-08 09:19:32.836443 qwak_core-0.0.53/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-08 09:19:32.916443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-08 09:19:29.752423 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.916443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-08 09:19:32.920443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-08 09:19:29.948424 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.920443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-08 09:19:32.920443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-08 09:19:30.152425 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.920443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-08 09:19:32.924443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-08 09:19:30.348427 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.924443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-08 09:19:32.924443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-08 09:19:30.548428 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.928443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-08 09:19:32.928443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-08 09:19:30.756429 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-08 09:19:32.928443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-08 09:19:32.932443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-08 09:19:30.944430 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.932443 qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-08 09:19:32.876443 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-08 09:19:26.092399 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.876443 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-08 09:19:32.880443 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-08 09:19:26.688403 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.884443 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-08 09:19:32.876443 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-08 09:19:26.292401 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-08 09:19:32.880443 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0     9322 2023-05-08 09:19:32.880443 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    13291 2023-05-08 09:19:26.488402 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.880443 qwak_core-0.0.53/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-08 09:19:32.860443 qwak_core-0.0.53/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-08 09:19:24.864391 qwak_core-0.0.53/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-08 09:19:32.860443 qwak_core-0.0.53/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-08 09:19:32.716442 qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-08 09:19:14.932328 qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-08 09:19:32.716442 qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-08 09:19:32.716442 qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-08 09:19:14.708326 qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.716442 qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-08 09:19:32.720442 qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-08 09:19:15.156329 qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-08 09:19:32.720442 qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-08 09:19:32.856443 qwak_core-0.0.53/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-08 09:19:24.424389 qwak_core-0.0.53/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-08 09:19:32.860443 qwak_core-0.0.53/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-08 09:19:32.872443 qwak_core-0.0.53/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-08 09:19:25.872398 qwak_core-0.0.53/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-08 09:19:32.872443 qwak_core-0.0.53/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-08 09:19:32.712442 qwak_core-0.0.53/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-08 09:19:12.220310 qwak_core-0.0.53/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.712442 qwak_core-0.0.53/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-08 09:19:32.708442 qwak_core-0.0.53/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-08 09:19:12.024309 qwak_core-0.0.53/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-08 09:19:32.712442 qwak_core-0.0.53/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-08 09:19:32.704442 qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-08 09:19:11.416305 qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.704442 qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-08 09:19:32.704442 qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-08 09:19:11.616307 qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.708442 qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-08 09:19:32.708442 qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-08 09:19:11.816308 qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-08 09:19:32.708442 qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-08 09:19:32.936443 qwak_core-0.0.53/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-08 09:19:31.336433 qwak_core-0.0.53/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-08 09:19:32.936443 qwak_core-0.0.53/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-08 09:19:32.932443 qwak_core-0.0.53/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-08 09:19:31.144432 qwak_core-0.0.53/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.932443 qwak_core-0.0.53/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0     4083 2023-05-08 09:19:32.728442 qwak_core-0.0.53/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0     4036 2023-05-08 09:19:13.796321 qwak_core-0.0.53/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.728442 qwak_core-0.0.53/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     2993 2023-05-08 09:19:32.732442 qwak_core-0.0.53/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2568 2023-05-08 09:19:14.020322 qwak_core-0.0.53/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-08 09:19:32.732442 qwak_core-0.0.53/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-05-08 09:19:34.404453 qwak_core-0.0.53/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-08 09:19:34.404453 qwak_core-0.0.53/qwak/__init__.py
--rw-r--r--   0        0        0     1204 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    32539 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/automations/automations.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-05-08 09:17:44.147743 qwak_core-0.0.53/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    17275 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14950 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0       41 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9261 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/inner/const.py
--rw-r--r--   0        0        0     1377 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-08 09:17:44.151743 qwak_core-0.0.53/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6083 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12145 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-08 09:17:44.155743 qwak_core-0.0.53/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     2696 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     3995 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13054 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-08 09:17:44.159743 qwak_core-0.0.53/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 qwak_core-0.0.53/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.53/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-10 07:16:05.193148 qwak_core-0.0.54/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 07:17:40.133087 qwak_core-0.0.54/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-10 07:17:40.153087 qwak_core-0.0.54/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-10 07:17:21.845101 qwak_core-0.0.54/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.153087 qwak_core-0.0.54/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-10 07:17:40.149087 qwak_core-0.0.54/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-10 07:17:21.517102 qwak_core-0.0.54/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.149087 qwak_core-0.0.54/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-10 07:17:40.153087 qwak_core-0.0.54/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-10 07:17:21.681102 qwak_core-0.0.54/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.153087 qwak_core-0.0.54/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-10 07:17:40.145087 qwak_core-0.0.54/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-10 07:17:21.025102 qwak_core-0.0.54/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-10 07:17:40.145087 qwak_core-0.0.54/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-10 07:17:40.145087 qwak_core-0.0.54/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-10 07:17:21.189102 qwak_core-0.0.54/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.145087 qwak_core-0.0.54/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-05-10 07:17:40.149087 qwak_core-0.0.54/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-05-10 07:17:21.353102 qwak_core-0.0.54/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.149087 qwak_core-0.0.54/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-10 07:17:40.133087 qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-10 07:17:20.857102 qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-10 07:17:40.133087 qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-05-10 07:17:40.133087 qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-05-10 07:17:22.009101 qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.137087 qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-10 07:17:40.137087 qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-10 07:17:22.349101 qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.141087 qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-10 07:17:40.141087 qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-10 07:17:22.517101 qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-10 07:17:40.141087 qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-10 07:17:40.137087 qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-10 07:17:22.173101 qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.137087 qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-10 07:17:40.141087 qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-10 07:17:22.681101 qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.141087 qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-10 07:17:40.181087 qwak_core-0.0.54/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-10 07:17:25.009099 qwak_core-0.0.54/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.181087 qwak_core-0.0.54/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-10 07:17:40.181087 qwak_core-0.0.54/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-10 07:17:25.177099 qwak_core-0.0.54/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-10 07:17:40.181087 qwak_core-0.0.54/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-10 07:17:40.293087 qwak_core-0.0.54/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-10 07:17:29.905095 qwak_core-0.0.54/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.293087 qwak_core-0.0.54/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-10 07:17:40.297087 qwak_core-0.0.54/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-10 07:17:30.069095 qwak_core-0.0.54/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-10 07:17:40.297087 qwak_core-0.0.54/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-10 07:17:40.301087 qwak_core-0.0.54/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-10 07:17:30.901095 qwak_core-0.0.54/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-10 07:17:40.301087 qwak_core-0.0.54/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-10 07:17:40.297087 qwak_core-0.0.54/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-10 07:17:30.737095 qwak_core-0.0.54/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.297087 qwak_core-0.0.54/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5497 2023-05-10 07:17:40.301087 qwak_core-0.0.54/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7820 2023-05-10 07:17:31.065095 qwak_core-0.0.54/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.301087 qwak_core-0.0.54/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-10 07:17:40.305087 qwak_core-0.0.54/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-10 07:17:31.229094 qwak_core-0.0.54/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-10 07:17:40.305087 qwak_core-0.0.54/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11441 2023-05-10 07:17:40.357087 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    17892 2023-05-10 07:17:35.957091 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.357087 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5494 2023-05-10 07:17:40.353087 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7776 2023-05-10 07:17:35.625091 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.353087 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-10 07:17:40.353087 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-10 07:17:35.789091 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.357087 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-10 07:17:40.349087 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-10 07:17:35.285091 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-10 07:17:40.349087 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-10 07:17:40.349087 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-10 07:17:35.457091 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.353087 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-10 07:17:40.361087 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-10 07:17:36.449090 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.361087 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-10 07:17:40.361087 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-10 07:17:36.285090 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.361087 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-10 07:17:40.357087 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-10 07:17:36.121091 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.357087 qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-10 07:17:40.397087 qwak_core-0.0.54/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-10 07:17:39.485088 qwak_core-0.0.54/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.397087 qwak_core-0.0.54/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-10 07:17:40.393087 qwak_core-0.0.54/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-10 07:17:39.133088 qwak_core-0.0.54/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.393087 qwak_core-0.0.54/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    42145 2023-05-10 07:17:40.393087 qwak_core-0.0.54/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    55993 2023-05-10 07:17:39.313088 qwak_core-0.0.54/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-10 07:17:40.393087 qwak_core-0.0.54/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    18658 2023-05-10 07:17:40.325087 qwak_core-0.0.54/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    15525 2023-05-10 07:17:32.921093 qwak_core-0.0.54/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    18652 2023-05-10 07:17:40.329087 qwak_core-0.0.54/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-10 07:17:40.325087 qwak_core-0.0.54/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-10 07:17:32.753093 qwak_core-0.0.54/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.325087 qwak_core-0.0.54/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-05-10 07:17:40.317087 qwak_core-0.0.54/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-05-10 07:17:32.413094 qwak_core-0.0.54/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.317087 qwak_core-0.0.54/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-10 07:17:40.317087 qwak_core-0.0.54/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-10 07:17:32.577093 qwak_core-0.0.54/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.321087 qwak_core-0.0.54/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-10 07:17:40.321087 qwak_core-0.0.54/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-10 07:17:33.089093 qwak_core-0.0.54/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-10 07:17:40.321087 qwak_core-0.0.54/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-05-10 07:17:40.321087 qwak_core-0.0.54/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-05-10 07:17:33.449093 qwak_core-0.0.54/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-10 07:17:40.325087 qwak_core-0.0.54/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-10 07:17:40.333087 qwak_core-0.0.54/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-10 07:17:33.801092 qwak_core-0.0.54/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.333087 qwak_core-0.0.54/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-10 07:17:40.333087 qwak_core-0.0.54/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-10 07:17:33.961092 qwak_core-0.0.54/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-10 07:17:40.333087 qwak_core-0.0.54/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-10 07:17:40.309087 qwak_core-0.0.54/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-10 07:17:31.913094 qwak_core-0.0.54/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.313087 qwak_core-0.0.54/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-10 07:17:40.313087 qwak_core-0.0.54/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-10 07:17:32.077094 qwak_core-0.0.54/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-10 07:17:40.313087 qwak_core-0.0.54/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-10 07:17:40.305087 qwak_core-0.0.54/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-10 07:17:31.573094 qwak_core-0.0.54/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.309087 qwak_core-0.0.54/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    42956 2023-05-10 07:17:40.305087 qwak_core-0.0.54/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    62847 2023-05-10 07:17:31.405094 qwak_core-0.0.54/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.305087 qwak_core-0.0.54/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-10 07:17:40.309087 qwak_core-0.0.54/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-10 07:17:31.749094 qwak_core-0.0.54/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-10 07:17:40.309087 qwak_core-0.0.54/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-10 07:17:40.169087 qwak_core-0.0.54/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-10 07:17:24.177100 qwak_core-0.0.54/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.169087 qwak_core-0.0.54/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-10 07:17:40.173087 qwak_core-0.0.54/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-10 07:17:24.345100 qwak_core-0.0.54/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.173087 qwak_core-0.0.54/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-10 07:17:40.173087 qwak_core-0.0.54/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-10 07:17:24.513100 qwak_core-0.0.54/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-10 07:17:40.173087 qwak_core-0.0.54/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-10 07:17:40.277087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-10 07:17:28.905096 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.277087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-10 07:17:40.273087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-10 07:17:28.741096 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-10 07:17:40.277087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9535 2023-05-10 07:17:40.257087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    10460 2023-05-10 07:17:27.237097 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.257087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5268 2023-05-10 07:17:40.257087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8525 2023-05-10 07:17:27.073098 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.257087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-10 07:17:40.249087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-10 07:17:26.557098 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.249087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    27847 2023-05-10 07:17:40.253087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20073 2023-05-10 07:17:26.905098 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    33080 2023-05-10 07:17:40.253087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-10 07:17:40.261087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-10 07:17:27.405097 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.261087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-10 07:17:40.261087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-10 07:17:27.569097 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-10 07:17:40.261087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25213 2023-05-10 07:17:40.253087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37366 2023-05-10 07:17:26.733098 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.253087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-10 07:17:40.265087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-10 07:17:27.733097 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.265087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0     5958 2023-05-10 07:17:40.265087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.py
+-rw-r--r--   0        0        0     6232 2023-05-10 07:17:27.901097 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.265087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-10 07:17:40.277087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-10 07:17:39.665088 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.281087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-10 07:17:40.281087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-10 07:17:39.849088 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-10 07:17:40.281087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-10 07:17:40.281087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-10 07:17:29.409096 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.285087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-10 07:17:40.285087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-10 07:17:29.577096 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-10 07:17:40.285087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-10 07:17:40.285087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-10 07:17:29.741096 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.285087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-10 07:17:40.289087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-10 07:17:30.405095 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.289087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-10 07:17:40.289087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-10 07:17:30.237095 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-10 07:17:40.289087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-10 07:17:40.293087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-10 07:17:30.569095 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.293087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-10 07:17:40.269087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-10 07:17:28.069097 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.269087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-10 07:17:40.269087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-10 07:17:28.237097 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.269087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-10 07:17:40.269087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-10 07:17:28.401097 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-10 07:17:40.273087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-10 07:17:40.273087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-10 07:17:28.569096 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.273087 qwak_core-0.0.54/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-10 07:17:40.365087 qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-10 07:17:36.617090 qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.365087 qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-10 07:17:40.365087 qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-10 07:17:36.781090 qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-10 07:17:40.365087 qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-10 07:17:40.369087 qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-10 07:17:36.945090 qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.369087 qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-10 07:17:40.369087 qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-10 07:17:37.121090 qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-10 07:17:40.369087 qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-10 07:17:40.369087 qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-10 07:17:37.293089 qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-10 07:17:40.373087 qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-10 07:17:40.373087 qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-10 07:17:37.457090 qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.373087 qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-10 07:17:40.337087 qwak_core-0.0.54/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-10 07:17:34.125092 qwak_core-0.0.54/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.337087 qwak_core-0.0.54/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-10 07:17:40.337087 qwak_core-0.0.54/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-10 07:17:34.289092 qwak_core-0.0.54/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-10 07:17:40.337087 qwak_core-0.0.54/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-10 07:17:40.197087 qwak_core-0.0.54/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-10 07:17:25.885099 qwak_core-0.0.54/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.201087 qwak_core-0.0.54/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-10 07:17:40.209087 qwak_core-0.0.54/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-10 07:17:26.053098 qwak_core-0.0.54/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.217087 qwak_core-0.0.54/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-10 07:17:40.229087 qwak_core-0.0.54/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-10 07:17:26.217098 qwak_core-0.0.54/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-10 07:17:40.237087 qwak_core-0.0.54/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-10 07:17:40.245087 qwak_core-0.0.54/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-10 07:17:26.385098 qwak_core-0.0.54/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.249087 qwak_core-0.0.54/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-10 07:17:40.313087 qwak_core-0.0.54/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-10 07:17:32.245094 qwak_core-0.0.54/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-10 07:17:40.317087 qwak_core-0.0.54/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-10 07:17:40.373087 qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-10 07:17:37.621089 qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.377087 qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-10 07:17:40.377087 qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-10 07:17:37.785089 qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.377087 qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-10 07:17:40.377087 qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-10 07:17:37.957089 qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.381087 qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-10 07:17:40.381087 qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-10 07:17:38.121089 qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.381087 qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-10 07:17:40.381087 qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-10 07:17:38.297089 qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.381087 qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-10 07:17:40.385087 qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-10 07:17:38.477089 qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-10 07:17:40.385087 qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-10 07:17:40.385087 qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-10 07:17:38.641089 qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.389087 qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-10 07:17:40.341087 qwak_core-0.0.54/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-10 07:17:34.617092 qwak_core-0.0.54/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.341087 qwak_core-0.0.54/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-10 07:17:40.345087 qwak_core-0.0.54/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-10 07:17:35.117091 qwak_core-0.0.54/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.349087 qwak_core-0.0.54/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-10 07:17:40.341087 qwak_core-0.0.54/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-10 07:17:34.785092 qwak_core-0.0.54/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-10 07:17:40.345087 qwak_core-0.0.54/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9322 2023-05-10 07:17:40.345087 qwak_core-0.0.54/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    13291 2023-05-10 07:17:34.949092 qwak_core-0.0.54/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.345087 qwak_core-0.0.54/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-10 07:17:40.329087 qwak_core-0.0.54/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-10 07:17:33.633092 qwak_core-0.0.54/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-10 07:17:40.333087 qwak_core-0.0.54/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-10 07:17:40.165087 qwak_core-0.0.54/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-10 07:17:25.553099 qwak_core-0.0.54/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-10 07:17:40.169087 qwak_core-0.0.54/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-10 07:17:40.165087 qwak_core-0.0.54/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-10 07:17:25.345099 qwak_core-0.0.54/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.165087 qwak_core-0.0.54/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-10 07:17:40.169087 qwak_core-0.0.54/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-10 07:17:25.721099 qwak_core-0.0.54/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-10 07:17:40.169087 qwak_core-0.0.54/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-10 07:17:40.329087 qwak_core-0.0.54/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-10 07:17:33.265093 qwak_core-0.0.54/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-10 07:17:40.329087 qwak_core-0.0.54/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-10 07:17:40.341087 qwak_core-0.0.54/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-10 07:17:34.453092 qwak_core-0.0.54/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-10 07:17:40.341087 qwak_core-0.0.54/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-10 07:17:40.161087 qwak_core-0.0.54/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-10 07:17:23.513100 qwak_core-0.0.54/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.165087 qwak_core-0.0.54/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-10 07:17:40.161087 qwak_core-0.0.54/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-10 07:17:23.345100 qwak_core-0.0.54/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-10 07:17:40.161087 qwak_core-0.0.54/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-10 07:17:40.153087 qwak_core-0.0.54/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-10 07:17:22.849101 qwak_core-0.0.54/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.157087 qwak_core-0.0.54/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-10 07:17:40.157087 qwak_core-0.0.54/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-10 07:17:23.013101 qwak_core-0.0.54/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.157087 qwak_core-0.0.54/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-10 07:17:40.157087 qwak_core-0.0.54/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-10 07:17:23.177101 qwak_core-0.0.54/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-10 07:17:40.161087 qwak_core-0.0.54/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-10 07:17:40.389087 qwak_core-0.0.54/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-10 07:17:38.969088 qwak_core-0.0.54/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-10 07:17:40.389087 qwak_core-0.0.54/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-10 07:17:40.389087 qwak_core-0.0.54/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-10 07:17:38.805088 qwak_core-0.0.54/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.389087 qwak_core-0.0.54/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0     4083 2023-05-10 07:17:40.177087 qwak_core-0.0.54/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0     4036 2023-05-10 07:17:24.677099 qwak_core-0.0.54/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.177087 qwak_core-0.0.54/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     2993 2023-05-10 07:17:40.177087 qwak_core-0.0.54/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2568 2023-05-10 07:17:24.845099 qwak_core-0.0.54/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-10 07:17:40.177087 qwak_core-0.0.54/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-05-10 07:17:41.433086 qwak_core-0.0.54/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-10 07:17:41.437086 qwak_core-0.0.54/qwak/__init__.py
+-rw-r--r--   0        0        0     1204 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    32539 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/automations/automations.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    17275 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14950 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0       41 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.193148 qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/inner/const.py
+-rw-r--r--   0        0        0     1377 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12145 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-10 07:16:05.197148 qwak_core-0.0.54/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     2696 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     3995 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13054 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-10 07:16:05.201148 qwak_core-0.0.54/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 qwak_core-0.0.54/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.54/PKG-INFO
```

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from _qwak_proto.qwak.user_application.common.v0 import resources_pb2 as qwak_dot_user__application_dot_common_dot_v0_dot_resources__pb2
 from _qwak_proto.qwak.batch_job.v1 import batch_job_events_pb2 as qwak_dot_batch__job_dot_v1_dot_batch__job__events__pb2
 from _qwak_proto.qwak.administration.authenticated_user.v1 import credentials_pb2 as qwak_dot_administration_dot_authenticated__user_dot_v1_dot_credentials__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)qwak/batch_job/v1/batch_job_service.proto\x12\rqwak.batchjob\x1a\x1fgoogle/protobuf/timestamp.proto\x1a/qwak/user_application/common/v0/resources.proto\x1a(qwak/batch_job/v1/batch_job_events.proto\x1a;qwak/administration/authenticated_user/v1/credentials.proto\"\xb4\x01\n\x15StartWarmupJobRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x05 \x01(\t\x12\x16\n\x0ewarmup_timeout\x18\x03 \x01(\x05\x12H\n\x19\x62\x61tch_job_deployment_size\x18\x04 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\"B\n\x16StartWarmupJobResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\"S\n\x16\x43\x61ncelWarmupJobRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\"C\n\x17\x43\x61ncelWarmupJobResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\"\xce\x04\n\x14StartBatchJobRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x0f \x01(\t\x12\x15\n\rsource_bucket\x18\x03 \x01(\t\x12\x1a\n\x12\x64\x65stination_bucket\x18\x04 \x01(\t\x12\x15\n\rsource_folder\x18\x05 \x01(\t\x12\x1a\n\x12\x64\x65stination_folder\x18\x06 \x01(\t\x12H\n\x19\x62\x61tch_job_deployment_size\x18\x07 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12\x13\n\x0bjob_timeout\x18\x08 \x01(\x05\x12\x14\n\x0ctask_timeout\x18\t \x01(\x05\x12\x35\n\x0finput_file_type\x18\n \x01(\x0e\x32\x1c.qwak.batchjob.InputFileType\x12\x37\n\x10output_file_type\x18\x0b \x01(\x0e\x32\x1d.qwak.batchjob.OutputFileType\x12\x14\n\x0ctoken_secret\x18\x0c \x01(\t\x12\x15\n\rsecret_secret\x18\r \x01(\t\x12M\n\x1b\x61\x64vanced_deployment_options\x18\x0e \x01(\x0b\x32(.qwak.batchjob.AdvancedDeploymentOptions\x12\x34\n\nparameters\x18\x10 \x03(\x0b\x32 .qwak.batchjob.BatchJobParameter\"/\n\x11\x42\x61tchJobParameter\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"S\n\x15StartBatchJobResponse\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\")\n\x15\x43\x61ncelBatchJobRequest\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\"B\n\x16\x43\x61ncelBatchJobResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\",\n\x18GetBatchJobStatusRequest\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\"\xac\x01\n\x19GetBatchJobStatusResponse\x12\x38\n\njob_status\x18\x01 \x01(\x0e\x32$.qwak.batchjob.BatchJobStatusMessage\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\x12\x16\n\x0e\x66inished_files\x18\x04 \x01(\x05\x12\x13\n\x0btotal_files\x18\x05 \x01(\x05\",\n\x18GetBatchJobReportRequest\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\"a\n\x19GetBatchJobReportResponse\x12\x12\n\nsuccessful\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\x12\x17\n\x0freport_messages\x18\x03 \x03(\t\"`\n\x1dUpdateBatchTasksStatusRequest\x12?\n\x11\x62\x61tch_task_events\x18\x01 \x03(\x0b\x32$.qwak.batchjob.BatchTaskEventMessage\"I\n\x1dUpdateBatchTaskStatusResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\"Q\n\x19\x41\x64vancedDeploymentOptions\x12\x1b\n\x13\x63ustom_iam_role_arn\x18\x01 \x01(\t\x12\x17\n\x0fpurchase_option\x18\x02 \x01(\t\"\x8f\x02\n\x16\x42\x61tchJobDeploymentSize\x12\x16\n\x0enumber_of_pods\x18\x01 \x01(\x05\x12\x0b\n\x03\x63pu\x18\x02 \x01(\x02\x12\x15\n\rmemory_amount\x18\x03 \x01(\x05\x12\x46\n\x0cmemory_units\x18\x04 \x01(\x0e\x32\x30.qwak.batchjob.BatchJobDeploymentSize.MemoryUnit\x12\x44\n\rgpu_resources\x18\x05 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResources\"+\n\nMemoryUnit\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02\"?\n\x14ListBatchJobsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\"K\n\x15ListBatchJobsResponse\x12\x32\n\nbatch_jobs\x18\x01 \x03(\x0b\x32\x1e.qwak.batchjob.BatchJobDetails\"\x9d\x02\n\x0f\x42\x61tchJobDetails\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x0e\n\x06job_id\x18\x02 \x01(\t\x12\x38\n\njob_status\x18\x03 \x01(\x0e\x32$.qwak.batchjob.BatchJobStatusMessage\x12.\n\nstart_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0f\x66\x61ilure_message\x18\x06 \x01(\t\x12\x37\n\x08job_size\x18\x07 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\"+\n\x19GetBatchJobDetailsRequest\x12\x0e\n\x06job_id\x18\x01 \x01(\t\"y\n\x1aGetBatchJobDetailsResponse\x12\x31\n\tbatch_job\x18\x01 \x01(\x0b\x32\x1e.qwak.batchjob.BatchJobMessage\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\"\x84\x04\n\x0f\x42\x61tchJobMessage\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x15\n\tbranch_id\x18\x03 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x04 \x01(\t\x12.\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\njob_status\x18\x07 \x01(\x0e\x32$.qwak.batchjob.BatchJobStatusMessage\x12\x15\n\rtotal_records\x18\x08 \x01(\x05\x12\x37\n\x08job_size\x18\t \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12;\n\x0freport_messages\x18\n \x03(\x0b\x32\".qwak.batchjob.ExecutionReportLine\x12\x43\n\x16\x65xecution_file_details\x18\x0b \x01(\x0b\x32#.qwak.batchjob.ExecutionFileDetails\x12<\n\x0ftask_executions\x18\x0c \x03(\x0b\x32#.qwak.batchjob.TaskExecutionDetails\"M\n\x13\x45xecutionReportLine\x12(\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04line\x18\x02 \x01(\t\"\x95\x02\n\x14\x45xecutionFileDetails\x12\x15\n\rsource_bucket\x18\x01 \x01(\t\x12\x1a\n\x12\x64\x65stination_bucket\x18\x02 \x01(\t\x12\x13\n\x0bsource_path\x18\x03 \x01(\t\x12\x18\n\x10\x64\x65stination_path\x18\x04 \x01(\t\x12\x35\n\x0finput_file_type\x18\x05 \x01(\x0e\x32\x1c.qwak.batchjob.InputFileType\x12\x37\n\x10output_file_type\x18\x06 \x01(\x0e\x32\x1d.qwak.batchjob.OutputFileType\x12\x16\n\x0e\x66inished_files\x18\x07 \x01(\x05\x12\x13\n\x0btotal_files\x18\x08 \x01(\x05\"\xe6\x01\n\x14TaskExecutionDetails\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x35\n\x06status\x18\x02 \x01(\x0e\x32%.qwak.batchjob.BatchTaskStatusMessage\x12.\n\nstart_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0enum_of_records\x18\x05 \x01(\x05\x12\x10\n\x08\x66ilename\x18\x06 \x01(\t\"d\n$GetBatchJobPreSignedUploadUrlRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x17\n\x0fnumber_of_files\x18\x02 \x01(\x05\x12\x11\n\tfile_type\x18\x03 \x01(\t\"\x98\x01\n%GetBatchJobPreSignedUploadUrlResponse\x12\x12\n\ninput_path\x18\x01 \x01(\t\x12\x13\n\x0boutput_path\x18\x02 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x03 \x01(\t\x12\x0c\n\x04urls\x18\x04 \x03(\t\x12\x0f\n\x07success\x18\x05 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x06 \x01(\t\"8\n&GetBatchJobPreSignedDownloadUrlRequest\x12\x0e\n\x06job_id\x18\x01 \x01(\t\"a\n\'GetBatchJobPreSignedDownloadUrlResponse\x12\x0c\n\x04urls\x18\x01 \x03(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\"3\n\x1fGetBatchJobUploadDetailsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\"\xb4\x01\n GetBatchJobUploadDetailsResponse\x12\x12\n\ninput_path\x18\x01 \x01(\t\x12\x13\n\x0boutput_path\x18\x02 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x03 \x01(\t\x12W\n\x0b\x63redentials\x18\x04 \x01(\x0b\x32\x42.qwak.administration.authenticated_user.v1.AwsTemporaryCredentials\"3\n!GetBatchJobDownloadDetailsRequest\x12\x0e\n\x06job_id\x18\x01 \x01(\t\"\x9b\x01\n\"GetBatchJobDownloadDetailsResponse\x12\x0e\n\x06\x62ucket\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\t\x12W\n\x0b\x63redentials\x18\x03 \x01(\x0b\x32\x42.qwak.administration.authenticated_user.v1.AwsTemporaryCredentials\"\xd7\x01\n\x1aUpdateDefaultParamsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x10\n\x08\x62uild_id\x18\x02 \x01(\t\x12\x46\n\x17\x64\x65\x66\x61ult_deployment_size\x18\x03 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12M\n\x1b\x61\x64vanced_deployment_options\x18\x04 \x01(\x0b\x32(.qwak.batchjob.AdvancedDeploymentOptions\"\x1d\n\x1bUpdateDefaultParamsResponse\".\n\x1a\x44\x65leteDefaultParamsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\"\x1d\n\x1b\x44\x65leteDefaultParamsResponse*\x81\x01\n\rInputFileType\x12\x1d\n\x19UNDEFINED_INPUT_FILE_TYPE\x10\x00\x12\x17\n\x13\x43SV_INPUT_FILE_TYPE\x10\x01\x12\x1b\n\x17\x46\x45\x41THER_INPUT_FILE_TYPE\x10\x02\x12\x1b\n\x17PARQUET_INPUT_FILE_TYPE\x10\x03*\x86\x01\n\x0eOutputFileType\x12\x1e\n\x1aUNDEFINED_OUTPUT_FILE_TYPE\x10\x00\x12\x18\n\x14\x43SV_OUTPUT_FILE_TYPE\x10\x01\x12\x1c\n\x18\x46\x45\x41THER_OUTPUT_FILE_TYPE\x10\x02\x12\x1c\n\x18PARQUET_OUTPUT_FILE_TYPE\x10\x03*\x8d\x02\n\x15\x42\x61tchJobStatusMessage\x12\x1e\n\x1aUNDEFINED_BATCH_JOB_STATUS\x10\x00\x12\x1e\n\x1a\x42\x41TCH_JOB_COMMITTED_STATUS\x10\x01\x12\x1c\n\x18\x42\x41TCH_JOB_PENDING_STATUS\x10\x02\x12\x1c\n\x18\x42\x41TCH_JOB_RUNNING_STATUS\x10\x03\x12\x1d\n\x19\x42\x41TCH_JOB_FINISHED_STATUS\x10\x04\x12\x1b\n\x17\x42\x41TCH_JOB_FAILED_STATUS\x10\x05\x12\x1e\n\x1a\x42\x41TCH_JOB_CANCELLED_STATUS\x10\x06\x12\x1c\n\x18\x42\x41TCH_JOB_TIMEOUT_STATUS\x10\x07*\x9c\x02\n\x16\x42\x61tchTaskStatusMessage\x12\x1f\n\x1bUNDEFINED_BATCH_TASK_STATUS\x10\x00\x12\x1f\n\x1b\x42\x41TCH_TASK_COMMITTED_STATUS\x10\x01\x12#\n\x1f\x42\x41TCH_TASK_PENDING_START_STATUS\x10\x02\x12\x1d\n\x19\x42\x41TCH_TASK_RUNNING_STATUS\x10\x03\x12\x1e\n\x1a\x42\x41TCH_TASK_FINISHED_STATUS\x10\x04\x12\x1c\n\x18\x42\x41TCH_TASK_FAILED_STATUS\x10\x05\x12\x1f\n\x1b\x42\x41TCH_TASK_CANCELLED_STATUS\x10\x06\x12\x1d\n\x19\x42\x41TCH_TASK_TIMEOUT_STATUS\x10\x07\x32\xa1\r\n\x19\x42\x61tchJobManagementService\x12Z\n\rStartBatchJob\x12#.qwak.batchjob.StartBatchJobRequest\x1a$.qwak.batchjob.StartBatchJobResponse\x12]\n\x0e\x43\x61ncelBatchJob\x12$.qwak.batchjob.CancelBatchJobRequest\x1a%.qwak.batchjob.CancelBatchJobResponse\x12]\n\x0eStartWarmupJob\x12$.qwak.batchjob.StartWarmupJobRequest\x1a%.qwak.batchjob.StartWarmupJobResponse\x12`\n\x0f\x43\x61ncelWarmupJob\x12%.qwak.batchjob.CancelWarmupJobRequest\x1a&.qwak.batchjob.CancelWarmupJobResponse\x12\x66\n\x11GetBatchJobStatus\x12\'.qwak.batchjob.GetBatchJobStatusRequest\x1a(.qwak.batchjob.GetBatchJobStatusResponse\x12\x66\n\x11GetBatchJobReport\x12\'.qwak.batchjob.GetBatchJobReportRequest\x1a(.qwak.batchjob.GetBatchJobReportResponse\x12t\n\x16UpdateBatchTasksStatus\x12,.qwak.batchjob.UpdateBatchTasksStatusRequest\x1a,.qwak.batchjob.UpdateBatchTaskStatusResponse\x12Z\n\rListBatchJobs\x12#.qwak.batchjob.ListBatchJobsRequest\x1a$.qwak.batchjob.ListBatchJobsResponse\x12i\n\x12GetBatchJobDetails\x12(.qwak.batchjob.GetBatchJobDetailsRequest\x1a).qwak.batchjob.GetBatchJobDetailsResponse\x12\x8a\x01\n\x1dGetBatchJobPreSignedUploadUrl\x12\x33.qwak.batchjob.GetBatchJobPreSignedUploadUrlRequest\x1a\x34.qwak.batchjob.GetBatchJobPreSignedUploadUrlResponse\x12\x90\x01\n\x1fGetBatchJobPreSignedDownloadUrl\x12\x35.qwak.batchjob.GetBatchJobPreSignedDownloadUrlRequest\x1a\x36.qwak.batchjob.GetBatchJobPreSignedDownloadUrlResponse\x12{\n\x18GetBatchJobUploadDetails\x12..qwak.batchjob.GetBatchJobUploadDetailsRequest\x1a/.qwak.batchjob.GetBatchJobUploadDetailsResponse\x12\x81\x01\n\x1aGetBatchJobDownloadDetails\x12\x30.qwak.batchjob.GetBatchJobDownloadDetailsRequest\x1a\x31.qwak.batchjob.GetBatchJobDownloadDetailsResponse\x12l\n\x13UpdateDefaultParams\x12).qwak.batchjob.UpdateDefaultParamsRequest\x1a*.qwak.batchjob.UpdateDefaultParamsResponse\x12l\n\x13\x44\x65leteDefaultParams\x12).qwak.batchjob.DeleteDefaultParamsRequest\x1a*.qwak.batchjob.DeleteDefaultParamsResponseB.\n\x19\x63om.qwak.ai.batch.job.apiP\x01Z\x0f./;inferencejobb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)qwak/batch_job/v1/batch_job_service.proto\x12\rqwak.batchjob\x1a\x1fgoogle/protobuf/timestamp.proto\x1a/qwak/user_application/common/v0/resources.proto\x1a(qwak/batch_job/v1/batch_job_events.proto\x1a;qwak/administration/authenticated_user/v1/credentials.proto\"\xb4\x01\n\x15StartWarmupJobRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x05 \x01(\t\x12\x16\n\x0ewarmup_timeout\x18\x03 \x01(\x05\x12H\n\x19\x62\x61tch_job_deployment_size\x18\x04 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\"B\n\x16StartWarmupJobResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\"S\n\x16\x43\x61ncelWarmupJobRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x03 \x01(\t\"C\n\x17\x43\x61ncelWarmupJobResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\"\x89\x05\n\x14StartBatchJobRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x0f \x01(\t\x12\x15\n\rsource_bucket\x18\x03 \x01(\t\x12\x1a\n\x12\x64\x65stination_bucket\x18\x04 \x01(\t\x12\x15\n\rsource_folder\x18\x05 \x01(\t\x12\x1a\n\x12\x64\x65stination_folder\x18\x06 \x01(\t\x12H\n\x19\x62\x61tch_job_deployment_size\x18\x07 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12\x13\n\x0bjob_timeout\x18\x08 \x01(\x05\x12\x14\n\x0ctask_timeout\x18\t \x01(\x05\x12\x35\n\x0finput_file_type\x18\n \x01(\x0e\x32\x1c.qwak.batchjob.InputFileType\x12\x37\n\x10output_file_type\x18\x0b \x01(\x0e\x32\x1d.qwak.batchjob.OutputFileType\x12\x14\n\x0ctoken_secret\x18\x0c \x01(\t\x12\x15\n\rsecret_secret\x18\r \x01(\t\x12M\n\x1b\x61\x64vanced_deployment_options\x18\x0e \x01(\x0b\x32(.qwak.batchjob.AdvancedDeploymentOptions\x12\x34\n\nparameters\x18\x10 \x03(\x0b\x32 .qwak.batchjob.BatchJobParameter\x12\x39\n\x11\x62\x61tch_job_request\x18\x11 \x01(\x0b\x32\x1e.qwak.batchjob.BatchJobRequest\"\xcb\x01\n\x0f\x42\x61tchJobRequest\x12:\n\rmodel_details\x18\x01 \x01(\x0b\x32#.qwak.batchjob.BatchJobModelDetails\x12\x38\n\x0c\x64\x61ta_details\x18\x02 \x01(\x0b\x32\".qwak.batchjob.BatchJobDataDetails\x12\x42\n\x11\x65xecution_details\x18\x04 \x01(\x0b\x32\'.qwak.batchjob.BatchJobExecutionDetails\":\n\x14\x42\x61tchJobModelDetails\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x10\n\x08\x62uild_id\x18\x0f \x01(\t\"\xbc\x01\n\x13\x42\x61tchJobDataDetails\x12\x36\n\x0bsource_path\x18\x01 \x01(\x0b\x32!.qwak.batchjob.BatchJobSourcePath\x12@\n\x10\x64\x65stination_path\x18\x02 \x01(\x0b\x32&.qwak.batchjob.BatchJobDestinationPath\x12\x14\n\x0ctoken_secret\x18\x0c \x01(\t\x12\x15\n\rsecret_secret\x18\r \x01(\t\"y\n\x12\x42\x61tchJobSourcePath\x12\x15\n\rsource_bucket\x18\x01 \x01(\t\x12\x15\n\rsource_folder\x18\x02 \x01(\t\x12\x35\n\x0finput_file_type\x18\x03 \x01(\x0e\x32\x1c.qwak.batchjob.InputFileType\"\x8a\x01\n\x17\x42\x61tchJobDestinationPath\x12\x1a\n\x12\x64\x65stination_bucket\x18\x01 \x01(\t\x12\x1a\n\x12\x64\x65stination_folder\x18\x02 \x01(\t\x12\x37\n\x10output_file_type\x18\x03 \x01(\x0e\x32\x1d.qwak.batchjob.OutputFileType\"\x94\x02\n\x18\x42\x61tchJobExecutionDetails\x12\x13\n\x0bjob_timeout\x18\x01 \x01(\x05\x12\x14\n\x0ctask_timeout\x18\x02 \x01(\x05\x12H\n\x19\x62\x61tch_job_deployment_size\x18\x03 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12M\n\x1b\x61\x64vanced_deployment_options\x18\x04 \x01(\x0b\x32(.qwak.batchjob.AdvancedDeploymentOptions\x12\x34\n\nparameters\x18\x05 \x03(\x0b\x32 .qwak.batchjob.BatchJobParameter\"/\n\x11\x42\x61tchJobParameter\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"S\n\x15StartBatchJobResponse\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\")\n\x15\x43\x61ncelBatchJobRequest\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\"B\n\x16\x43\x61ncelBatchJobResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\",\n\x18GetBatchJobStatusRequest\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\"\xac\x01\n\x19GetBatchJobStatusResponse\x12\x38\n\njob_status\x18\x01 \x01(\x0e\x32$.qwak.batchjob.BatchJobStatusMessage\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\x12\x16\n\x0e\x66inished_files\x18\x04 \x01(\x05\x12\x13\n\x0btotal_files\x18\x05 \x01(\x05\",\n\x18GetBatchJobReportRequest\x12\x10\n\x08\x62\x61tch_id\x18\x01 \x01(\t\"a\n\x19GetBatchJobReportResponse\x12\x12\n\nsuccessful\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\x12\x17\n\x0freport_messages\x18\x03 \x03(\t\"`\n\x1dUpdateBatchTasksStatusRequest\x12?\n\x11\x62\x61tch_task_events\x18\x01 \x03(\x0b\x32$.qwak.batchjob.BatchTaskEventMessage\"I\n\x1dUpdateBatchTaskStatusResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x02 \x01(\t\"Q\n\x19\x41\x64vancedDeploymentOptions\x12\x1b\n\x13\x63ustom_iam_role_arn\x18\x01 \x01(\t\x12\x17\n\x0fpurchase_option\x18\x02 \x01(\t\"\x8f\x02\n\x16\x42\x61tchJobDeploymentSize\x12\x16\n\x0enumber_of_pods\x18\x01 \x01(\x05\x12\x0b\n\x03\x63pu\x18\x02 \x01(\x02\x12\x15\n\rmemory_amount\x18\x03 \x01(\x05\x12\x46\n\x0cmemory_units\x18\x04 \x01(\x0e\x32\x30.qwak.batchjob.BatchJobDeploymentSize.MemoryUnit\x12\x44\n\rgpu_resources\x18\x05 \x01(\x0b\x32-.qwak.user_application.common.v0.GpuResources\"+\n\nMemoryUnit\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03MIB\x10\x01\x12\x07\n\x03GIB\x10\x02\"?\n\x14ListBatchJobsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x15\n\tbranch_id\x18\x02 \x01(\tB\x02\x18\x01\"K\n\x15ListBatchJobsResponse\x12\x32\n\nbatch_jobs\x18\x01 \x03(\x0b\x32\x1e.qwak.batchjob.BatchJobDetails\"\x9d\x02\n\x0f\x42\x61tchJobDetails\x12\x10\n\x08\x62uild_id\x18\x01 \x01(\t\x12\x0e\n\x06job_id\x18\x02 \x01(\t\x12\x38\n\njob_status\x18\x03 \x01(\x0e\x32$.qwak.batchjob.BatchJobStatusMessage\x12.\n\nstart_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0f\x66\x61ilure_message\x18\x06 \x01(\t\x12\x37\n\x08job_size\x18\x07 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\"+\n\x19GetBatchJobDetailsRequest\x12\x0e\n\x06job_id\x18\x01 \x01(\t\"y\n\x1aGetBatchJobDetailsResponse\x12\x31\n\tbatch_job\x18\x01 \x01(\x0b\x32\x1e.qwak.batchjob.BatchJobMessage\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\"\x84\x04\n\x0f\x42\x61tchJobMessage\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x10\n\x08model_id\x18\x02 \x01(\t\x12\x15\n\tbranch_id\x18\x03 \x01(\tB\x02\x18\x01\x12\x10\n\x08\x62uild_id\x18\x04 \x01(\t\x12.\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\njob_status\x18\x07 \x01(\x0e\x32$.qwak.batchjob.BatchJobStatusMessage\x12\x15\n\rtotal_records\x18\x08 \x01(\x05\x12\x37\n\x08job_size\x18\t \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12;\n\x0freport_messages\x18\n \x03(\x0b\x32\".qwak.batchjob.ExecutionReportLine\x12\x43\n\x16\x65xecution_file_details\x18\x0b \x01(\x0b\x32#.qwak.batchjob.ExecutionFileDetails\x12<\n\x0ftask_executions\x18\x0c \x03(\x0b\x32#.qwak.batchjob.TaskExecutionDetails\"M\n\x13\x45xecutionReportLine\x12(\n\x04time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04line\x18\x02 \x01(\t\"\x95\x02\n\x14\x45xecutionFileDetails\x12\x15\n\rsource_bucket\x18\x01 \x01(\t\x12\x1a\n\x12\x64\x65stination_bucket\x18\x02 \x01(\t\x12\x13\n\x0bsource_path\x18\x03 \x01(\t\x12\x18\n\x10\x64\x65stination_path\x18\x04 \x01(\t\x12\x35\n\x0finput_file_type\x18\x05 \x01(\x0e\x32\x1c.qwak.batchjob.InputFileType\x12\x37\n\x10output_file_type\x18\x06 \x01(\x0e\x32\x1d.qwak.batchjob.OutputFileType\x12\x16\n\x0e\x66inished_files\x18\x07 \x01(\x05\x12\x13\n\x0btotal_files\x18\x08 \x01(\x05\"\xe6\x01\n\x14TaskExecutionDetails\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x35\n\x06status\x18\x02 \x01(\x0e\x32%.qwak.batchjob.BatchTaskStatusMessage\x12.\n\nstart_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0enum_of_records\x18\x05 \x01(\x05\x12\x10\n\x08\x66ilename\x18\x06 \x01(\t\"d\n$GetBatchJobPreSignedUploadUrlRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x17\n\x0fnumber_of_files\x18\x02 \x01(\x05\x12\x11\n\tfile_type\x18\x03 \x01(\t\"\x98\x01\n%GetBatchJobPreSignedUploadUrlResponse\x12\x12\n\ninput_path\x18\x01 \x01(\t\x12\x13\n\x0boutput_path\x18\x02 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x03 \x01(\t\x12\x0c\n\x04urls\x18\x04 \x03(\t\x12\x0f\n\x07success\x18\x05 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x06 \x01(\t\"8\n&GetBatchJobPreSignedDownloadUrlRequest\x12\x0e\n\x06job_id\x18\x01 \x01(\t\"a\n\'GetBatchJobPreSignedDownloadUrlResponse\x12\x0c\n\x04urls\x18\x01 \x03(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x17\n\x0f\x66\x61ilure_message\x18\x03 \x01(\t\"3\n\x1fGetBatchJobUploadDetailsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\"\xb4\x01\n GetBatchJobUploadDetailsResponse\x12\x12\n\ninput_path\x18\x01 \x01(\t\x12\x13\n\x0boutput_path\x18\x02 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x03 \x01(\t\x12W\n\x0b\x63redentials\x18\x04 \x01(\x0b\x32\x42.qwak.administration.authenticated_user.v1.AwsTemporaryCredentials\"3\n!GetBatchJobDownloadDetailsRequest\x12\x0e\n\x06job_id\x18\x01 \x01(\t\"\x9b\x01\n\"GetBatchJobDownloadDetailsResponse\x12\x0e\n\x06\x62ucket\x18\x01 \x01(\t\x12\x0c\n\x04keys\x18\x02 \x03(\t\x12W\n\x0b\x63redentials\x18\x03 \x01(\x0b\x32\x42.qwak.administration.authenticated_user.v1.AwsTemporaryCredentials\"\xd7\x01\n\x1aUpdateDefaultParamsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\x12\x10\n\x08\x62uild_id\x18\x02 \x01(\t\x12\x46\n\x17\x64\x65\x66\x61ult_deployment_size\x18\x03 \x01(\x0b\x32%.qwak.batchjob.BatchJobDeploymentSize\x12M\n\x1b\x61\x64vanced_deployment_options\x18\x04 \x01(\x0b\x32(.qwak.batchjob.AdvancedDeploymentOptions\"\x1d\n\x1bUpdateDefaultParamsResponse\".\n\x1a\x44\x65leteDefaultParamsRequest\x12\x10\n\x08model_id\x18\x01 \x01(\t\"\x1d\n\x1b\x44\x65leteDefaultParamsResponse*\x81\x01\n\rInputFileType\x12\x1d\n\x19UNDEFINED_INPUT_FILE_TYPE\x10\x00\x12\x17\n\x13\x43SV_INPUT_FILE_TYPE\x10\x01\x12\x1b\n\x17\x46\x45\x41THER_INPUT_FILE_TYPE\x10\x02\x12\x1b\n\x17PARQUET_INPUT_FILE_TYPE\x10\x03*\x86\x01\n\x0eOutputFileType\x12\x1e\n\x1aUNDEFINED_OUTPUT_FILE_TYPE\x10\x00\x12\x18\n\x14\x43SV_OUTPUT_FILE_TYPE\x10\x01\x12\x1c\n\x18\x46\x45\x41THER_OUTPUT_FILE_TYPE\x10\x02\x12\x1c\n\x18PARQUET_OUTPUT_FILE_TYPE\x10\x03*\x8d\x02\n\x15\x42\x61tchJobStatusMessage\x12\x1e\n\x1aUNDEFINED_BATCH_JOB_STATUS\x10\x00\x12\x1e\n\x1a\x42\x41TCH_JOB_COMMITTED_STATUS\x10\x01\x12\x1c\n\x18\x42\x41TCH_JOB_PENDING_STATUS\x10\x02\x12\x1c\n\x18\x42\x41TCH_JOB_RUNNING_STATUS\x10\x03\x12\x1d\n\x19\x42\x41TCH_JOB_FINISHED_STATUS\x10\x04\x12\x1b\n\x17\x42\x41TCH_JOB_FAILED_STATUS\x10\x05\x12\x1e\n\x1a\x42\x41TCH_JOB_CANCELLED_STATUS\x10\x06\x12\x1c\n\x18\x42\x41TCH_JOB_TIMEOUT_STATUS\x10\x07*\x9c\x02\n\x16\x42\x61tchTaskStatusMessage\x12\x1f\n\x1bUNDEFINED_BATCH_TASK_STATUS\x10\x00\x12\x1f\n\x1b\x42\x41TCH_TASK_COMMITTED_STATUS\x10\x01\x12#\n\x1f\x42\x41TCH_TASK_PENDING_START_STATUS\x10\x02\x12\x1d\n\x19\x42\x41TCH_TASK_RUNNING_STATUS\x10\x03\x12\x1e\n\x1a\x42\x41TCH_TASK_FINISHED_STATUS\x10\x04\x12\x1c\n\x18\x42\x41TCH_TASK_FAILED_STATUS\x10\x05\x12\x1f\n\x1b\x42\x41TCH_TASK_CANCELLED_STATUS\x10\x06\x12\x1d\n\x19\x42\x41TCH_TASK_TIMEOUT_STATUS\x10\x07\x32\xa1\r\n\x19\x42\x61tchJobManagementService\x12Z\n\rStartBatchJob\x12#.qwak.batchjob.StartBatchJobRequest\x1a$.qwak.batchjob.StartBatchJobResponse\x12]\n\x0e\x43\x61ncelBatchJob\x12$.qwak.batchjob.CancelBatchJobRequest\x1a%.qwak.batchjob.CancelBatchJobResponse\x12]\n\x0eStartWarmupJob\x12$.qwak.batchjob.StartWarmupJobRequest\x1a%.qwak.batchjob.StartWarmupJobResponse\x12`\n\x0f\x43\x61ncelWarmupJob\x12%.qwak.batchjob.CancelWarmupJobRequest\x1a&.qwak.batchjob.CancelWarmupJobResponse\x12\x66\n\x11GetBatchJobStatus\x12\'.qwak.batchjob.GetBatchJobStatusRequest\x1a(.qwak.batchjob.GetBatchJobStatusResponse\x12\x66\n\x11GetBatchJobReport\x12\'.qwak.batchjob.GetBatchJobReportRequest\x1a(.qwak.batchjob.GetBatchJobReportResponse\x12t\n\x16UpdateBatchTasksStatus\x12,.qwak.batchjob.UpdateBatchTasksStatusRequest\x1a,.qwak.batchjob.UpdateBatchTaskStatusResponse\x12Z\n\rListBatchJobs\x12#.qwak.batchjob.ListBatchJobsRequest\x1a$.qwak.batchjob.ListBatchJobsResponse\x12i\n\x12GetBatchJobDetails\x12(.qwak.batchjob.GetBatchJobDetailsRequest\x1a).qwak.batchjob.GetBatchJobDetailsResponse\x12\x8a\x01\n\x1dGetBatchJobPreSignedUploadUrl\x12\x33.qwak.batchjob.GetBatchJobPreSignedUploadUrlRequest\x1a\x34.qwak.batchjob.GetBatchJobPreSignedUploadUrlResponse\x12\x90\x01\n\x1fGetBatchJobPreSignedDownloadUrl\x12\x35.qwak.batchjob.GetBatchJobPreSignedDownloadUrlRequest\x1a\x36.qwak.batchjob.GetBatchJobPreSignedDownloadUrlResponse\x12{\n\x18GetBatchJobUploadDetails\x12..qwak.batchjob.GetBatchJobUploadDetailsRequest\x1a/.qwak.batchjob.GetBatchJobUploadDetailsResponse\x12\x81\x01\n\x1aGetBatchJobDownloadDetails\x12\x30.qwak.batchjob.GetBatchJobDownloadDetailsRequest\x1a\x31.qwak.batchjob.GetBatchJobDownloadDetailsResponse\x12l\n\x13UpdateDefaultParams\x12).qwak.batchjob.UpdateDefaultParamsRequest\x1a*.qwak.batchjob.UpdateDefaultParamsResponse\x12l\n\x13\x44\x65leteDefaultParams\x12).qwak.batchjob.DeleteDefaultParamsRequest\x1a*.qwak.batchjob.DeleteDefaultParamsResponseB.\n\x19\x63om.qwak.ai.batch.job.apiP\x01Z\x0f./;inferencejobb\x06proto3')
 
 _INPUTFILETYPE = DESCRIPTOR.enum_types_by_name['InputFileType']
 InputFileType = enum_type_wrapper.EnumTypeWrapper(_INPUTFILETYPE)
 _OUTPUTFILETYPE = DESCRIPTOR.enum_types_by_name['OutputFileType']
 OutputFileType = enum_type_wrapper.EnumTypeWrapper(_OUTPUTFILETYPE)
 _BATCHJOBSTATUSMESSAGE = DESCRIPTOR.enum_types_by_name['BatchJobStatusMessage']
 BatchJobStatusMessage = enum_type_wrapper.EnumTypeWrapper(_BATCHJOBSTATUSMESSAGE)
@@ -56,14 +56,20 @@
 
 
 _STARTWARMUPJOBREQUEST = DESCRIPTOR.message_types_by_name['StartWarmupJobRequest']
 _STARTWARMUPJOBRESPONSE = DESCRIPTOR.message_types_by_name['StartWarmupJobResponse']
 _CANCELWARMUPJOBREQUEST = DESCRIPTOR.message_types_by_name['CancelWarmupJobRequest']
 _CANCELWARMUPJOBRESPONSE = DESCRIPTOR.message_types_by_name['CancelWarmupJobResponse']
 _STARTBATCHJOBREQUEST = DESCRIPTOR.message_types_by_name['StartBatchJobRequest']
+_BATCHJOBREQUEST = DESCRIPTOR.message_types_by_name['BatchJobRequest']
+_BATCHJOBMODELDETAILS = DESCRIPTOR.message_types_by_name['BatchJobModelDetails']
+_BATCHJOBDATADETAILS = DESCRIPTOR.message_types_by_name['BatchJobDataDetails']
+_BATCHJOBSOURCEPATH = DESCRIPTOR.message_types_by_name['BatchJobSourcePath']
+_BATCHJOBDESTINATIONPATH = DESCRIPTOR.message_types_by_name['BatchJobDestinationPath']
+_BATCHJOBEXECUTIONDETAILS = DESCRIPTOR.message_types_by_name['BatchJobExecutionDetails']
 _BATCHJOBPARAMETER = DESCRIPTOR.message_types_by_name['BatchJobParameter']
 _STARTBATCHJOBRESPONSE = DESCRIPTOR.message_types_by_name['StartBatchJobResponse']
 _CANCELBATCHJOBREQUEST = DESCRIPTOR.message_types_by_name['CancelBatchJobRequest']
 _CANCELBATCHJOBRESPONSE = DESCRIPTOR.message_types_by_name['CancelBatchJobResponse']
 _GETBATCHJOBSTATUSREQUEST = DESCRIPTOR.message_types_by_name['GetBatchJobStatusRequest']
 _GETBATCHJOBSTATUSRESPONSE = DESCRIPTOR.message_types_by_name['GetBatchJobStatusResponse']
 _GETBATCHJOBREPORTREQUEST = DESCRIPTOR.message_types_by_name['GetBatchJobReportRequest']
@@ -125,14 +131,56 @@
 StartBatchJobRequest = _reflection.GeneratedProtocolMessageType('StartBatchJobRequest', (_message.Message,), {
   'DESCRIPTOR' : _STARTBATCHJOBREQUEST,
   '__module__' : 'qwak.batch_job.v1.batch_job_service_pb2'
   # @@protoc_insertion_point(class_scope:qwak.batchjob.StartBatchJobRequest)
   })
 _sym_db.RegisterMessage(StartBatchJobRequest)
 
+BatchJobRequest = _reflection.GeneratedProtocolMessageType('BatchJobRequest', (_message.Message,), {
+  'DESCRIPTOR' : _BATCHJOBREQUEST,
+  '__module__' : 'qwak.batch_job.v1.batch_job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.batchjob.BatchJobRequest)
+  })
+_sym_db.RegisterMessage(BatchJobRequest)
+
+BatchJobModelDetails = _reflection.GeneratedProtocolMessageType('BatchJobModelDetails', (_message.Message,), {
+  'DESCRIPTOR' : _BATCHJOBMODELDETAILS,
+  '__module__' : 'qwak.batch_job.v1.batch_job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.batchjob.BatchJobModelDetails)
+  })
+_sym_db.RegisterMessage(BatchJobModelDetails)
+
+BatchJobDataDetails = _reflection.GeneratedProtocolMessageType('BatchJobDataDetails', (_message.Message,), {
+  'DESCRIPTOR' : _BATCHJOBDATADETAILS,
+  '__module__' : 'qwak.batch_job.v1.batch_job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.batchjob.BatchJobDataDetails)
+  })
+_sym_db.RegisterMessage(BatchJobDataDetails)
+
+BatchJobSourcePath = _reflection.GeneratedProtocolMessageType('BatchJobSourcePath', (_message.Message,), {
+  'DESCRIPTOR' : _BATCHJOBSOURCEPATH,
+  '__module__' : 'qwak.batch_job.v1.batch_job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.batchjob.BatchJobSourcePath)
+  })
+_sym_db.RegisterMessage(BatchJobSourcePath)
+
+BatchJobDestinationPath = _reflection.GeneratedProtocolMessageType('BatchJobDestinationPath', (_message.Message,), {
+  'DESCRIPTOR' : _BATCHJOBDESTINATIONPATH,
+  '__module__' : 'qwak.batch_job.v1.batch_job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.batchjob.BatchJobDestinationPath)
+  })
+_sym_db.RegisterMessage(BatchJobDestinationPath)
+
+BatchJobExecutionDetails = _reflection.GeneratedProtocolMessageType('BatchJobExecutionDetails', (_message.Message,), {
+  'DESCRIPTOR' : _BATCHJOBEXECUTIONDETAILS,
+  '__module__' : 'qwak.batch_job.v1.batch_job_service_pb2'
+  # @@protoc_insertion_point(class_scope:qwak.batchjob.BatchJobExecutionDetails)
+  })
+_sym_db.RegisterMessage(BatchJobExecutionDetails)
+
 BatchJobParameter = _reflection.GeneratedProtocolMessageType('BatchJobParameter', (_message.Message,), {
   'DESCRIPTOR' : _BATCHJOBPARAMETER,
   '__module__' : 'qwak.batch_job.v1.batch_job_service_pb2'
   # @@protoc_insertion_point(class_scope:qwak.batchjob.BatchJobParameter)
   })
 _sym_db.RegisterMessage(BatchJobParameter)
 
@@ -371,96 +419,108 @@
   _CANCELWARMUPJOBREQUEST.fields_by_name['branch_id']._serialized_options = b'\030\001'
   _STARTBATCHJOBREQUEST.fields_by_name['branch_id']._options = None
   _STARTBATCHJOBREQUEST.fields_by_name['branch_id']._serialized_options = b'\030\001'
   _LISTBATCHJOBSREQUEST.fields_by_name['branch_id']._options = None
   _LISTBATCHJOBSREQUEST.fields_by_name['branch_id']._serialized_options = b'\030\001'
   _BATCHJOBMESSAGE.fields_by_name['branch_id']._options = None
   _BATCHJOBMESSAGE.fields_by_name['branch_id']._serialized_options = b'\030\001'
-  _INPUTFILETYPE._serialized_start=5283
-  _INPUTFILETYPE._serialized_end=5412
-  _OUTPUTFILETYPE._serialized_start=5415
-  _OUTPUTFILETYPE._serialized_end=5549
-  _BATCHJOBSTATUSMESSAGE._serialized_start=5552
-  _BATCHJOBSTATUSMESSAGE._serialized_end=5821
-  _BATCHTASKSTATUSMESSAGE._serialized_start=5824
-  _BATCHTASKSTATUSMESSAGE._serialized_end=6108
+  _INPUTFILETYPE._serialized_start=6342
+  _INPUTFILETYPE._serialized_end=6471
+  _OUTPUTFILETYPE._serialized_start=6474
+  _OUTPUTFILETYPE._serialized_end=6608
+  _BATCHJOBSTATUSMESSAGE._serialized_start=6611
+  _BATCHJOBSTATUSMESSAGE._serialized_end=6880
+  _BATCHTASKSTATUSMESSAGE._serialized_start=6883
+  _BATCHTASKSTATUSMESSAGE._serialized_end=7167
   _STARTWARMUPJOBREQUEST._serialized_start=246
   _STARTWARMUPJOBREQUEST._serialized_end=426
   _STARTWARMUPJOBRESPONSE._serialized_start=428
   _STARTWARMUPJOBRESPONSE._serialized_end=494
   _CANCELWARMUPJOBREQUEST._serialized_start=496
   _CANCELWARMUPJOBREQUEST._serialized_end=579
   _CANCELWARMUPJOBRESPONSE._serialized_start=581
   _CANCELWARMUPJOBRESPONSE._serialized_end=648
   _STARTBATCHJOBREQUEST._serialized_start=651
-  _STARTBATCHJOBREQUEST._serialized_end=1241
-  _BATCHJOBPARAMETER._serialized_start=1243
-  _BATCHJOBPARAMETER._serialized_end=1290
-  _STARTBATCHJOBRESPONSE._serialized_start=1292
-  _STARTBATCHJOBRESPONSE._serialized_end=1375
-  _CANCELBATCHJOBREQUEST._serialized_start=1377
-  _CANCELBATCHJOBREQUEST._serialized_end=1418
-  _CANCELBATCHJOBRESPONSE._serialized_start=1420
-  _CANCELBATCHJOBRESPONSE._serialized_end=1486
-  _GETBATCHJOBSTATUSREQUEST._serialized_start=1488
-  _GETBATCHJOBSTATUSREQUEST._serialized_end=1532
-  _GETBATCHJOBSTATUSRESPONSE._serialized_start=1535
-  _GETBATCHJOBSTATUSRESPONSE._serialized_end=1707
-  _GETBATCHJOBREPORTREQUEST._serialized_start=1709
-  _GETBATCHJOBREPORTREQUEST._serialized_end=1753
-  _GETBATCHJOBREPORTRESPONSE._serialized_start=1755
-  _GETBATCHJOBREPORTRESPONSE._serialized_end=1852
-  _UPDATEBATCHTASKSSTATUSREQUEST._serialized_start=1854
-  _UPDATEBATCHTASKSSTATUSREQUEST._serialized_end=1950
-  _UPDATEBATCHTASKSTATUSRESPONSE._serialized_start=1952
-  _UPDATEBATCHTASKSTATUSRESPONSE._serialized_end=2025
-  _ADVANCEDDEPLOYMENTOPTIONS._serialized_start=2027
-  _ADVANCEDDEPLOYMENTOPTIONS._serialized_end=2108
-  _BATCHJOBDEPLOYMENTSIZE._serialized_start=2111
-  _BATCHJOBDEPLOYMENTSIZE._serialized_end=2382
-  _BATCHJOBDEPLOYMENTSIZE_MEMORYUNIT._serialized_start=2339
-  _BATCHJOBDEPLOYMENTSIZE_MEMORYUNIT._serialized_end=2382
-  _LISTBATCHJOBSREQUEST._serialized_start=2384
-  _LISTBATCHJOBSREQUEST._serialized_end=2447
-  _LISTBATCHJOBSRESPONSE._serialized_start=2449
-  _LISTBATCHJOBSRESPONSE._serialized_end=2524
-  _BATCHJOBDETAILS._serialized_start=2527
-  _BATCHJOBDETAILS._serialized_end=2812
-  _GETBATCHJOBDETAILSREQUEST._serialized_start=2814
-  _GETBATCHJOBDETAILSREQUEST._serialized_end=2857
-  _GETBATCHJOBDETAILSRESPONSE._serialized_start=2859
-  _GETBATCHJOBDETAILSRESPONSE._serialized_end=2980
-  _BATCHJOBMESSAGE._serialized_start=2983
-  _BATCHJOBMESSAGE._serialized_end=3499
-  _EXECUTIONREPORTLINE._serialized_start=3501
-  _EXECUTIONREPORTLINE._serialized_end=3578
-  _EXECUTIONFILEDETAILS._serialized_start=3581
-  _EXECUTIONFILEDETAILS._serialized_end=3858
-  _TASKEXECUTIONDETAILS._serialized_start=3861
-  _TASKEXECUTIONDETAILS._serialized_end=4091
-  _GETBATCHJOBPRESIGNEDUPLOADURLREQUEST._serialized_start=4093
-  _GETBATCHJOBPRESIGNEDUPLOADURLREQUEST._serialized_end=4193
-  _GETBATCHJOBPRESIGNEDUPLOADURLRESPONSE._serialized_start=4196
-  _GETBATCHJOBPRESIGNEDUPLOADURLRESPONSE._serialized_end=4348
-  _GETBATCHJOBPRESIGNEDDOWNLOADURLREQUEST._serialized_start=4350
-  _GETBATCHJOBPRESIGNEDDOWNLOADURLREQUEST._serialized_end=4406
-  _GETBATCHJOBPRESIGNEDDOWNLOADURLRESPONSE._serialized_start=4408
-  _GETBATCHJOBPRESIGNEDDOWNLOADURLRESPONSE._serialized_end=4505
-  _GETBATCHJOBUPLOADDETAILSREQUEST._serialized_start=4507
-  _GETBATCHJOBUPLOADDETAILSREQUEST._serialized_end=4558
-  _GETBATCHJOBUPLOADDETAILSRESPONSE._serialized_start=4561
-  _GETBATCHJOBUPLOADDETAILSRESPONSE._serialized_end=4741
-  _GETBATCHJOBDOWNLOADDETAILSREQUEST._serialized_start=4743
-  _GETBATCHJOBDOWNLOADDETAILSREQUEST._serialized_end=4794
-  _GETBATCHJOBDOWNLOADDETAILSRESPONSE._serialized_start=4797
-  _GETBATCHJOBDOWNLOADDETAILSRESPONSE._serialized_end=4952
-  _UPDATEDEFAULTPARAMSREQUEST._serialized_start=4955
-  _UPDATEDEFAULTPARAMSREQUEST._serialized_end=5170
-  _UPDATEDEFAULTPARAMSRESPONSE._serialized_start=5172
-  _UPDATEDEFAULTPARAMSRESPONSE._serialized_end=5201
-  _DELETEDEFAULTPARAMSREQUEST._serialized_start=5203
-  _DELETEDEFAULTPARAMSREQUEST._serialized_end=5249
-  _DELETEDEFAULTPARAMSRESPONSE._serialized_start=5251
-  _DELETEDEFAULTPARAMSRESPONSE._serialized_end=5280
-  _BATCHJOBMANAGEMENTSERVICE._serialized_start=6111
-  _BATCHJOBMANAGEMENTSERVICE._serialized_end=7808
+  _STARTBATCHJOBREQUEST._serialized_end=1300
+  _BATCHJOBREQUEST._serialized_start=1303
+  _BATCHJOBREQUEST._serialized_end=1506
+  _BATCHJOBMODELDETAILS._serialized_start=1508
+  _BATCHJOBMODELDETAILS._serialized_end=1566
+  _BATCHJOBDATADETAILS._serialized_start=1569
+  _BATCHJOBDATADETAILS._serialized_end=1757
+  _BATCHJOBSOURCEPATH._serialized_start=1759
+  _BATCHJOBSOURCEPATH._serialized_end=1880
+  _BATCHJOBDESTINATIONPATH._serialized_start=1883
+  _BATCHJOBDESTINATIONPATH._serialized_end=2021
+  _BATCHJOBEXECUTIONDETAILS._serialized_start=2024
+  _BATCHJOBEXECUTIONDETAILS._serialized_end=2300
+  _BATCHJOBPARAMETER._serialized_start=2302
+  _BATCHJOBPARAMETER._serialized_end=2349
+  _STARTBATCHJOBRESPONSE._serialized_start=2351
+  _STARTBATCHJOBRESPONSE._serialized_end=2434
+  _CANCELBATCHJOBREQUEST._serialized_start=2436
+  _CANCELBATCHJOBREQUEST._serialized_end=2477
+  _CANCELBATCHJOBRESPONSE._serialized_start=2479
+  _CANCELBATCHJOBRESPONSE._serialized_end=2545
+  _GETBATCHJOBSTATUSREQUEST._serialized_start=2547
+  _GETBATCHJOBSTATUSREQUEST._serialized_end=2591
+  _GETBATCHJOBSTATUSRESPONSE._serialized_start=2594
+  _GETBATCHJOBSTATUSRESPONSE._serialized_end=2766
+  _GETBATCHJOBREPORTREQUEST._serialized_start=2768
+  _GETBATCHJOBREPORTREQUEST._serialized_end=2812
+  _GETBATCHJOBREPORTRESPONSE._serialized_start=2814
+  _GETBATCHJOBREPORTRESPONSE._serialized_end=2911
+  _UPDATEBATCHTASKSSTATUSREQUEST._serialized_start=2913
+  _UPDATEBATCHTASKSSTATUSREQUEST._serialized_end=3009
+  _UPDATEBATCHTASKSTATUSRESPONSE._serialized_start=3011
+  _UPDATEBATCHTASKSTATUSRESPONSE._serialized_end=3084
+  _ADVANCEDDEPLOYMENTOPTIONS._serialized_start=3086
+  _ADVANCEDDEPLOYMENTOPTIONS._serialized_end=3167
+  _BATCHJOBDEPLOYMENTSIZE._serialized_start=3170
+  _BATCHJOBDEPLOYMENTSIZE._serialized_end=3441
+  _BATCHJOBDEPLOYMENTSIZE_MEMORYUNIT._serialized_start=3398
+  _BATCHJOBDEPLOYMENTSIZE_MEMORYUNIT._serialized_end=3441
+  _LISTBATCHJOBSREQUEST._serialized_start=3443
+  _LISTBATCHJOBSREQUEST._serialized_end=3506
+  _LISTBATCHJOBSRESPONSE._serialized_start=3508
+  _LISTBATCHJOBSRESPONSE._serialized_end=3583
+  _BATCHJOBDETAILS._serialized_start=3586
+  _BATCHJOBDETAILS._serialized_end=3871
+  _GETBATCHJOBDETAILSREQUEST._serialized_start=3873
+  _GETBATCHJOBDETAILSREQUEST._serialized_end=3916
+  _GETBATCHJOBDETAILSRESPONSE._serialized_start=3918
+  _GETBATCHJOBDETAILSRESPONSE._serialized_end=4039
+  _BATCHJOBMESSAGE._serialized_start=4042
+  _BATCHJOBMESSAGE._serialized_end=4558
+  _EXECUTIONREPORTLINE._serialized_start=4560
+  _EXECUTIONREPORTLINE._serialized_end=4637
+  _EXECUTIONFILEDETAILS._serialized_start=4640
+  _EXECUTIONFILEDETAILS._serialized_end=4917
+  _TASKEXECUTIONDETAILS._serialized_start=4920
+  _TASKEXECUTIONDETAILS._serialized_end=5150
+  _GETBATCHJOBPRESIGNEDUPLOADURLREQUEST._serialized_start=5152
+  _GETBATCHJOBPRESIGNEDUPLOADURLREQUEST._serialized_end=5252
+  _GETBATCHJOBPRESIGNEDUPLOADURLRESPONSE._serialized_start=5255
+  _GETBATCHJOBPRESIGNEDUPLOADURLRESPONSE._serialized_end=5407
+  _GETBATCHJOBPRESIGNEDDOWNLOADURLREQUEST._serialized_start=5409
+  _GETBATCHJOBPRESIGNEDDOWNLOADURLREQUEST._serialized_end=5465
+  _GETBATCHJOBPRESIGNEDDOWNLOADURLRESPONSE._serialized_start=5467
+  _GETBATCHJOBPRESIGNEDDOWNLOADURLRESPONSE._serialized_end=5564
+  _GETBATCHJOBUPLOADDETAILSREQUEST._serialized_start=5566
+  _GETBATCHJOBUPLOADDETAILSREQUEST._serialized_end=5617
+  _GETBATCHJOBUPLOADDETAILSRESPONSE._serialized_start=5620
+  _GETBATCHJOBUPLOADDETAILSRESPONSE._serialized_end=5800
+  _GETBATCHJOBDOWNLOADDETAILSREQUEST._serialized_start=5802
+  _GETBATCHJOBDOWNLOADDETAILSREQUEST._serialized_end=5853
+  _GETBATCHJOBDOWNLOADDETAILSRESPONSE._serialized_start=5856
+  _GETBATCHJOBDOWNLOADDETAILSRESPONSE._serialized_end=6011
+  _UPDATEDEFAULTPARAMSREQUEST._serialized_start=6014
+  _UPDATEDEFAULTPARAMSREQUEST._serialized_end=6229
+  _UPDATEDEFAULTPARAMSRESPONSE._serialized_start=6231
+  _UPDATEDEFAULTPARAMSRESPONSE._serialized_end=6260
+  _DELETEDEFAULTPARAMSREQUEST._serialized_start=6262
+  _DELETEDEFAULTPARAMSREQUEST._serialized_end=6308
+  _DELETEDEFAULTPARAMSRESPONSE._serialized_start=6310
+  _DELETEDEFAULTPARAMSRESPONSE._serialized_end=6339
+  _BATCHJOBMANAGEMENTSERVICE._serialized_start=7170
+  _BATCHJOBMANAGEMENTSERVICE._serialized_end=8867
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -228,14 +228,15 @@
     TASK_TIMEOUT_FIELD_NUMBER: builtins.int
     INPUT_FILE_TYPE_FIELD_NUMBER: builtins.int
     OUTPUT_FILE_TYPE_FIELD_NUMBER: builtins.int
     TOKEN_SECRET_FIELD_NUMBER: builtins.int
     SECRET_SECRET_FIELD_NUMBER: builtins.int
     ADVANCED_DEPLOYMENT_OPTIONS_FIELD_NUMBER: builtins.int
     PARAMETERS_FIELD_NUMBER: builtins.int
+    BATCH_JOB_REQUEST_FIELD_NUMBER: builtins.int
     model_id: builtins.str
     """The model ID to start the job on"""
     branch_id: builtins.str
     """The branch ID of the model"""
     build_id: builtins.str
     """Specific build ID the invocation will be executed upon. If empty - deployed build ID will be the default"""
     source_bucket: builtins.str
@@ -263,14 +264,19 @@
     """The access secret's secret name in secret service"""
     @property
     def advanced_deployment_options(self) -> global___AdvancedDeploymentOptions:
         """Advanced deployment options"""
     @property
     def parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___BatchJobParameter]:
         """User provided parameters which will be passed to the batch execution job as environment variables"""
+    @property
+    def batch_job_request(self) -> global___BatchJobRequest:
+        """The request message reorganized
+        We will migrate to this massage.
+        """
     def __init__(
         self,
         *,
         model_id: builtins.str = ...,
         branch_id: builtins.str = ...,
         build_id: builtins.str = ...,
         source_bucket: builtins.str = ...,
@@ -282,20 +288,178 @@
         task_timeout: builtins.int = ...,
         input_file_type: global___InputFileType.ValueType = ...,
         output_file_type: global___OutputFileType.ValueType = ...,
         token_secret: builtins.str = ...,
         secret_secret: builtins.str = ...,
         advanced_deployment_options: global___AdvancedDeploymentOptions | None = ...,
         parameters: collections.abc.Iterable[global___BatchJobParameter] | None = ...,
+        batch_job_request: global___BatchJobRequest | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["advanced_deployment_options", b"advanced_deployment_options", "batch_job_deployment_size", b"batch_job_deployment_size"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["advanced_deployment_options", b"advanced_deployment_options", "batch_job_deployment_size", b"batch_job_deployment_size", "branch_id", b"branch_id", "build_id", b"build_id", "destination_bucket", b"destination_bucket", "destination_folder", b"destination_folder", "input_file_type", b"input_file_type", "job_timeout", b"job_timeout", "model_id", b"model_id", "output_file_type", b"output_file_type", "parameters", b"parameters", "secret_secret", b"secret_secret", "source_bucket", b"source_bucket", "source_folder", b"source_folder", "task_timeout", b"task_timeout", "token_secret", b"token_secret"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["advanced_deployment_options", b"advanced_deployment_options", "batch_job_deployment_size", b"batch_job_deployment_size", "batch_job_request", b"batch_job_request"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["advanced_deployment_options", b"advanced_deployment_options", "batch_job_deployment_size", b"batch_job_deployment_size", "batch_job_request", b"batch_job_request", "branch_id", b"branch_id", "build_id", b"build_id", "destination_bucket", b"destination_bucket", "destination_folder", b"destination_folder", "input_file_type", b"input_file_type", "job_timeout", b"job_timeout", "model_id", b"model_id", "output_file_type", b"output_file_type", "parameters", b"parameters", "secret_secret", b"secret_secret", "source_bucket", b"source_bucket", "source_folder", b"source_folder", "task_timeout", b"task_timeout", "token_secret", b"token_secret"]) -> None: ...
 
 global___StartBatchJobRequest = StartBatchJobRequest
 
+class BatchJobRequest(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    MODEL_DETAILS_FIELD_NUMBER: builtins.int
+    DATA_DETAILS_FIELD_NUMBER: builtins.int
+    EXECUTION_DETAILS_FIELD_NUMBER: builtins.int
+    @property
+    def model_details(self) -> global___BatchJobModelDetails:
+        """Data about the model to do batch prediction on"""
+    @property
+    def data_details(self) -> global___BatchJobDataDetails:
+        """The params for the data that the prediction executed on"""
+    @property
+    def execution_details(self) -> global___BatchJobExecutionDetails:
+        """How to execute the job"""
+    def __init__(
+        self,
+        *,
+        model_details: global___BatchJobModelDetails | None = ...,
+        data_details: global___BatchJobDataDetails | None = ...,
+        execution_details: global___BatchJobExecutionDetails | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["data_details", b"data_details", "execution_details", b"execution_details", "model_details", b"model_details"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["data_details", b"data_details", "execution_details", b"execution_details", "model_details", b"model_details"]) -> None: ...
+
+global___BatchJobRequest = BatchJobRequest
+
+class BatchJobModelDetails(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    MODEL_ID_FIELD_NUMBER: builtins.int
+    BUILD_ID_FIELD_NUMBER: builtins.int
+    model_id: builtins.str
+    """The model ID to start the job on"""
+    build_id: builtins.str
+    """Specific build ID the invocation will be executed upon. If empty - deployed build ID will be the default"""
+    def __init__(
+        self,
+        *,
+        model_id: builtins.str = ...,
+        build_id: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["build_id", b"build_id", "model_id", b"model_id"]) -> None: ...
+
+global___BatchJobModelDetails = BatchJobModelDetails
+
+class BatchJobDataDetails(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    SOURCE_PATH_FIELD_NUMBER: builtins.int
+    DESTINATION_PATH_FIELD_NUMBER: builtins.int
+    TOKEN_SECRET_FIELD_NUMBER: builtins.int
+    SECRET_SECRET_FIELD_NUMBER: builtins.int
+    @property
+    def source_path(self) -> global___BatchJobSourcePath:
+        """The source data details"""
+    @property
+    def destination_path(self) -> global___BatchJobDestinationPath:
+        """The destination data details"""
+    token_secret: builtins.str
+    """The access token's secret name in secret service"""
+    secret_secret: builtins.str
+    """The access secret's secret name in secret service"""
+    def __init__(
+        self,
+        *,
+        source_path: global___BatchJobSourcePath | None = ...,
+        destination_path: global___BatchJobDestinationPath | None = ...,
+        token_secret: builtins.str = ...,
+        secret_secret: builtins.str = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["destination_path", b"destination_path", "source_path", b"source_path"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["destination_path", b"destination_path", "secret_secret", b"secret_secret", "source_path", b"source_path", "token_secret", b"token_secret"]) -> None: ...
+
+global___BatchJobDataDetails = BatchJobDataDetails
+
+class BatchJobSourcePath(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    SOURCE_BUCKET_FIELD_NUMBER: builtins.int
+    SOURCE_FOLDER_FIELD_NUMBER: builtins.int
+    INPUT_FILE_TYPE_FIELD_NUMBER: builtins.int
+    source_bucket: builtins.str
+    """The source bucket from which the files will be read"""
+    source_folder: builtins.str
+    """The source folder from which the files will be read on the source bucket"""
+    input_file_type: global___InputFileType.ValueType
+    """The file type for the input files"""
+    def __init__(
+        self,
+        *,
+        source_bucket: builtins.str = ...,
+        source_folder: builtins.str = ...,
+        input_file_type: global___InputFileType.ValueType = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["input_file_type", b"input_file_type", "source_bucket", b"source_bucket", "source_folder", b"source_folder"]) -> None: ...
+
+global___BatchJobSourcePath = BatchJobSourcePath
+
+class BatchJobDestinationPath(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    DESTINATION_BUCKET_FIELD_NUMBER: builtins.int
+    DESTINATION_FOLDER_FIELD_NUMBER: builtins.int
+    OUTPUT_FILE_TYPE_FIELD_NUMBER: builtins.int
+    destination_bucket: builtins.str
+    """The destination bucket to which the files will be written"""
+    destination_folder: builtins.str
+    """The destination folder to which the files will be written on the destination bucket"""
+    output_file_type: global___OutputFileType.ValueType
+    """The file type for the output files"""
+    def __init__(
+        self,
+        *,
+        destination_bucket: builtins.str = ...,
+        destination_folder: builtins.str = ...,
+        output_file_type: global___OutputFileType.ValueType = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["destination_bucket", b"destination_bucket", "destination_folder", b"destination_folder", "output_file_type", b"output_file_type"]) -> None: ...
+
+global___BatchJobDestinationPath = BatchJobDestinationPath
+
+class BatchJobExecutionDetails(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    JOB_TIMEOUT_FIELD_NUMBER: builtins.int
+    TASK_TIMEOUT_FIELD_NUMBER: builtins.int
+    BATCH_JOB_DEPLOYMENT_SIZE_FIELD_NUMBER: builtins.int
+    ADVANCED_DEPLOYMENT_OPTIONS_FIELD_NUMBER: builtins.int
+    PARAMETERS_FIELD_NUMBER: builtins.int
+    job_timeout: builtins.int
+    """The total batch job timeout in seconds"""
+    task_timeout: builtins.int
+    """The single task timeout in seconds"""
+    @property
+    def batch_job_deployment_size(self) -> global___BatchJobDeploymentSize:
+        """The batch job size"""
+    @property
+    def advanced_deployment_options(self) -> global___AdvancedDeploymentOptions:
+        """Advanced deployment options"""
+    @property
+    def parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___BatchJobParameter]:
+        """User provided parameters which will be passed to the batch execution job as environment variables"""
+    def __init__(
+        self,
+        *,
+        job_timeout: builtins.int = ...,
+        task_timeout: builtins.int = ...,
+        batch_job_deployment_size: global___BatchJobDeploymentSize | None = ...,
+        advanced_deployment_options: global___AdvancedDeploymentOptions | None = ...,
+        parameters: collections.abc.Iterable[global___BatchJobParameter] | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["advanced_deployment_options", b"advanced_deployment_options", "batch_job_deployment_size", b"batch_job_deployment_size"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["advanced_deployment_options", b"advanced_deployment_options", "batch_job_deployment_size", b"batch_job_deployment_size", "job_timeout", b"job_timeout", "parameters", b"parameters", "task_timeout", b"task_timeout"]) -> None: ...
+
+global___BatchJobExecutionDetails = BatchJobExecutionDetails
+
 class BatchJobParameter(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     KEY_FIELD_NUMBER: builtins.int
     VALUE_FIELD_NUMBER: builtins.int
     key: builtins.str
     value: builtins.str
```

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.54/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.54/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.54/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/pyproject.toml` & `qwak_core-0.0.54/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.53"
+version = "0.0.54"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.53/qwak/automations/__init__.py` & `qwak_core-0.0.54/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/automations/automation_executions.py` & `qwak_core-0.0.54/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/automations/automations.py` & `qwak_core-0.0.54/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.54/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.54/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.54/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.54/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.54/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/alert_management/client.py` & `qwak_core-0.0.54/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/analytics/client.py` & `qwak_core-0.0.54/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/audience/client.py` & `qwak_core-0.0.54/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/automation_management/client.py` & `qwak_core-0.0.54/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.54/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.54/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.54/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.54/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/build_management/client.py` & `qwak_core-0.0.54/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.54/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.54/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/deployment/client.py` & `qwak_core-0.0.54/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.54/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.54/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.54/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.54/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.54/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/logging_client/client.py` & `qwak_core-0.0.54/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/model_management/client.py` & `qwak_core-0.0.54/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/project/client.py` & `qwak_core-0.0.54/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/secret_service/client.py` & `qwak_core-0.0.54/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.54/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.54/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.54/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.54/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.54/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.54/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.54/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.54/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.54/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.54/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.54/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.54/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.54/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.54/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.54/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.54/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/offline/client.py` & `qwak_core-0.0.54/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/feature_store/online/client.py` & `qwak_core-0.0.54/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/inner/const.py` & `qwak_core-0.0.54/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.54/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.54/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.54/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.54/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/inner/singleton_meta.py` & `qwak_core-0.0.54/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/inner/tool/auth.py` & `qwak_core-0.0.54/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.54/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.54/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.54/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.54/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/adapters/__init__.py` & `qwak_core-0.0.54/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.54/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.54/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.54/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.54/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.54/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/base.py` & `qwak_core-0.0.54/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/decorators/api.py` & `qwak_core-0.0.54/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.54/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/experiment_tracking.py` & `qwak_core-0.0.54/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/schema.py` & `qwak_core-0.0.54/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/schema_entities.py` & `qwak_core-0.0.54/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.54/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.54/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.54/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.54/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.54/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.54/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.54/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.54/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.54/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.54/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.54/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.54/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.54/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.54/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.54/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.54/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.54/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.54/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.54/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/qwak_client/client.py` & `qwak_core-0.0.54/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.54/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/qwak_client/models/model.py` & `qwak_core-0.0.54/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.54/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.54/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/tools/logger/logger.py` & `qwak_core-0.0.54/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak/tools/logger/logging.yml` & `qwak_core-0.0.54/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.54/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/qwak_services_mock/services_mock.py` & `qwak_core-0.0.54/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.53/setup.py` & `qwak_core-0.0.54/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.53',
+    'version': '0.0.54',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.53/PKG-INFO` & `qwak_core-0.0.54/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.53
+Version: 0.0.54
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

