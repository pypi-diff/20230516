# Comparing `tmp/qwak_core-0.0.60.tar.gz` & `tmp/qwak_core-0.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.60.tar", max compression
+gzip compressed data, was "qwak_core-0.0.61.tar", max compression
```

## Comparing `qwak_core-0.0.60.tar` & `qwak_core-0.0.61.tar`

### file list

```diff
@@ -1,570 +1,573 @@
--rw-r--r--   0        0        0      264 2023-05-15 12:22:28.684237 qwak_core-0.0.60/README.md
--rw-r--r--   0        0        0        0 2023-05-15 12:24:09.141068 qwak_core-0.0.60/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-15 12:24:09.165068 qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-15 12:23:48.052897 qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.165068 qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-15 12:24:09.161069 qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-15 12:23:47.688894 qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.161069 qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-15 12:24:09.165068 qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-15 12:23:47.868895 qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.165068 qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-15 12:24:09.153068 qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-15 12:23:47.144890 qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-15 12:24:09.157069 qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-15 12:24:09.157069 qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-15 12:23:47.324891 qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.157069 qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-05-15 12:24:09.161069 qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-05-15 12:23:47.508893 qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.161069 qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-15 12:24:09.141068 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-15 12:23:46.960888 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-15 12:24:09.141068 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-05-15 12:24:09.145069 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-05-15 12:23:48.236899 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.145069 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-15 12:24:09.149068 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-15 12:23:48.600901 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.149068 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-15 12:24:09.149068 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-15 12:23:48.784903 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-15 12:24:09.153068 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-15 12:24:09.145069 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-15 12:23:48.416900 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.149068 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-15 12:24:09.153068 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-15 12:23:48.972905 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.153068 qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-15 12:24:09.197069 qwak_core-0.0.60/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-15 12:23:51.756927 qwak_core-0.0.60/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.197069 qwak_core-0.0.60/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-15 12:24:09.197069 qwak_core-0.0.60/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-15 12:23:51.980929 qwak_core-0.0.60/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-15 12:24:09.197069 qwak_core-0.0.60/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-15 12:24:09.337070 qwak_core-0.0.60/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-15 12:23:57.520974 qwak_core-0.0.60/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.337070 qwak_core-0.0.60/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-15 12:24:09.337070 qwak_core-0.0.60/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-15 12:23:57.708976 qwak_core-0.0.60/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-15 12:24:09.337070 qwak_core-0.0.60/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-15 12:24:09.341070 qwak_core-0.0.60/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-15 12:23:58.648984 qwak_core-0.0.60/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-15 12:24:09.345070 qwak_core-0.0.60/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-15 12:24:09.341070 qwak_core-0.0.60/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-15 12:23:58.460982 qwak_core-0.0.60/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.341070 qwak_core-0.0.60/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5497 2023-05-15 12:24:09.345070 qwak_core-0.0.60/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7820 2023-05-15 12:23:58.836985 qwak_core-0.0.60/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.345070 qwak_core-0.0.60/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-15 12:24:09.345070 qwak_core-0.0.60/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-15 12:23:59.020987 qwak_core-0.0.60/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-15 12:24:09.349070 qwak_core-0.0.60/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    12352 2023-05-15 12:24:09.433071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    18970 2023-05-15 12:24:06.681048 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.433071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5494 2023-05-15 12:24:09.429071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7776 2023-05-15 12:24:06.305045 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.429071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-15 12:24:09.433071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-15 12:24:06.489047 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.433071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-15 12:24:09.425071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-15 12:24:05.925042 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-15 12:24:09.425071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-15 12:24:09.429071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-15 12:24:06.117044 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.429071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-15 12:24:09.441071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-15 12:24:07.237053 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.441071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-15 12:24:09.437071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-15 12:24:07.053052 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.441071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-15 12:24:09.437071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-15 12:24:06.869050 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.437071 qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-15 12:24:09.421071 qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-15 12:24:05.729041 qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.425071 qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-15 12:24:09.417071 qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-15 12:24:05.341038 qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.421071 qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    42145 2023-05-15 12:24:09.421071 qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    55993 2023-05-15 12:24:05.541039 qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-15 12:24:09.421071 qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    18658 2023-05-15 12:24:09.373070 qwak_core-0.0.60/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    15525 2023-05-15 12:24:00.937002 qwak_core-0.0.60/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    18652 2023-05-15 12:24:09.373070 qwak_core-0.0.60/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-15 12:24:09.369070 qwak_core-0.0.60/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-15 12:24:00.749001 qwak_core-0.0.60/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.373070 qwak_core-0.0.60/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-05-15 12:24:09.361070 qwak_core-0.0.60/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-05-15 12:24:00.364997 qwak_core-0.0.60/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.361070 qwak_core-0.0.60/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-15 12:24:09.365070 qwak_core-0.0.60/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-15 12:24:00.552999 qwak_core-0.0.60/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.365070 qwak_core-0.0.60/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-15 12:24:09.365070 qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-15 12:24:01.129004 qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-15 12:24:09.369070 qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-05-15 12:24:09.369070 qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-05-15 12:24:01.537007 qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-15 12:24:09.369070 qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-15 12:24:09.381070 qwak_core-0.0.60/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-15 12:24:01.925010 qwak_core-0.0.60/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.381070 qwak_core-0.0.60/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-15 12:24:09.381070 qwak_core-0.0.60/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-15 12:24:02.109012 qwak_core-0.0.60/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-15 12:24:09.381070 qwak_core-0.0.60/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-15 12:24:09.357070 qwak_core-0.0.60/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-15 12:23:59.796993 qwak_core-0.0.60/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.357070 qwak_core-0.0.60/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-15 12:24:09.357070 qwak_core-0.0.60/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-15 12:23:59.980995 qwak_core-0.0.60/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-15 12:24:09.357070 qwak_core-0.0.60/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-15 12:24:09.349070 qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-15 12:23:59.408990 qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.353070 qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    43712 2023-05-15 12:24:09.349070 qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    63341 2023-05-15 12:23:59.220988 qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.349070 qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-15 12:24:09.353070 qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-15 12:23:59.608991 qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-15 12:24:09.353070 qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-15 12:24:09.185069 qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-15 12:23:50.724919 qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.185069 qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-15 12:24:09.189069 qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-15 12:23:50.932921 qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.189069 qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-15 12:24:09.189069 qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-15 12:23:51.140922 qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-15 12:24:09.189069 qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-15 12:24:09.317070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-15 12:23:56.412965 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.317070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-15 12:24:09.313070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-15 12:23:56.228964 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-15 12:24:09.317070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0     9535 2023-05-15 12:24:09.297070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    10460 2023-05-15 12:23:54.540950 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.297070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5268 2023-05-15 12:24:09.293070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8525 2023-05-15 12:23:54.352949 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.293070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-15 12:24:09.285070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-15 12:23:53.764944 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.289070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    27847 2023-05-15 12:24:09.289070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20073 2023-05-15 12:23:54.164947 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    33080 2023-05-15 12:24:09.293070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-15 12:24:09.297070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-15 12:23:54.728952 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.297070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-15 12:24:09.301070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-15 12:23:54.916953 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-15 12:24:09.301070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25213 2023-05-15 12:24:09.289070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37366 2023-05-15 12:23:53.960945 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.289070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-15 12:24:09.301070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-15 12:23:55.100955 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.301070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0     5958 2023-05-15 12:24:09.305070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.py
--rw-r--r--   0        0        0     6232 2023-05-15 12:23:55.288956 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.305070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-15 12:24:09.317070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-15 12:24:08.565064 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.321070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-15 12:24:09.321070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-15 12:24:08.781066 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-15 12:24:09.321070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-15 12:24:09.325070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-15 12:23:56.964970 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.325070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-15 12:24:09.325070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-15 12:23:57.152972 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-15 12:24:09.325070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-15 12:24:09.329070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-15 12:23:57.336973 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.329070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-15 12:24:09.333070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-15 12:23:58.088979 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.333070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-15 12:24:09.329070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-15 12:23:57.896978 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-15 12:24:09.329070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-15 12:24:09.333070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-15 12:23:58.276981 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.333070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-15 12:24:09.305070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-15 12:23:55.480958 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.305070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-15 12:24:09.309070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-15 12:23:55.672959 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.309070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-15 12:24:09.309070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-15 12:23:55.860961 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-15 12:24:09.313070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-15 12:24:09.313070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-15 12:23:56.044963 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.313070 qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-15 12:24:09.441071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-15 12:24:07.417055 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.445071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-15 12:24:09.445071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-15 12:24:07.601056 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-15 12:24:09.445071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-15 12:24:09.445071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-15 12:24:07.785057 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.449071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-15 12:24:09.449071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-15 12:24:07.981059 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-15 12:24:09.449071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-15 12:24:09.449071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-15 12:24:08.173061 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-15 12:24:09.453071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-15 12:24:09.453071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-15 12:24:08.361062 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.453071 qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-15 12:24:09.385070 qwak_core-0.0.60/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-15 12:24:02.297013 qwak_core-0.0.60/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.385070 qwak_core-0.0.60/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-15 12:24:09.385070 qwak_core-0.0.60/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-15 12:24:02.481015 qwak_core-0.0.60/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-15 12:24:09.385070 qwak_core-0.0.60/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-15 12:24:09.213069 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-15 12:23:52.924937 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.221069 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-15 12:24:09.233069 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-15 12:23:53.144939 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.241069 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-15 12:24:09.253069 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-15 12:23:53.356940 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-15 12:24:09.261069 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-15 12:24:09.277069 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-15 12:23:53.568942 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.285070 qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-15 12:24:09.361070 qwak_core-0.0.60/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-15 12:24:00.172996 qwak_core-0.0.60/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-15 12:24:09.361070 qwak_core-0.0.60/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-15 12:24:09.397071 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-15 12:24:03.621024 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.401070 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-15 12:24:09.401070 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-15 12:24:03.809025 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.401070 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-15 12:24:09.401070 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-15 12:24:04.001027 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.405070 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-15 12:24:09.405070 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-15 12:24:04.193029 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.405070 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-15 12:24:09.409071 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-15 12:24:04.389030 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.409071 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-15 12:24:09.409071 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-15 12:24:04.597032 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-15 12:24:09.409071 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-15 12:24:09.413071 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-15 12:24:04.785033 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.413071 qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-15 12:24:09.389070 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-15 12:24:02.853018 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.393070 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-15 12:24:09.397071 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-15 12:24:03.433022 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.397071 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-15 12:24:09.393070 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-15 12:24:03.041019 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-15 12:24:09.393070 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0     9322 2023-05-15 12:24:09.393070 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    13291 2023-05-15 12:24:03.249021 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.397071 qwak_core-0.0.60/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-15 12:24:09.377070 qwak_core-0.0.60/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-15 12:24:01.741009 qwak_core-0.0.60/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-15 12:24:09.377070 qwak_core-0.0.60/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-15 12:24:09.181069 qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-15 12:23:52.440933 qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-15 12:24:09.181069 qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-15 12:24:09.177069 qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-15 12:23:52.204931 qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.181069 qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-15 12:24:09.181069 qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-15 12:23:52.708935 qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-15 12:24:09.185069 qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-15 12:24:09.373070 qwak_core-0.0.60/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-15 12:24:01.329005 qwak_core-0.0.60/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-15 12:24:09.377070 qwak_core-0.0.60/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-15 12:24:09.389070 qwak_core-0.0.60/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-15 12:24:02.669016 qwak_core-0.0.60/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-15 12:24:09.389070 qwak_core-0.0.60/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-15 12:24:09.177069 qwak_core-0.0.60/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-15 12:23:49.900912 qwak_core-0.0.60/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.177069 qwak_core-0.0.60/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-15 12:24:09.173069 qwak_core-0.0.60/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-15 12:23:49.716911 qwak_core-0.0.60/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-15 12:24:09.177069 qwak_core-0.0.60/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-15 12:24:09.169069 qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-15 12:23:49.152906 qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.169069 qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-15 12:24:09.169069 qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-15 12:23:49.336907 qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.169069 qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-15 12:24:09.173069 qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-15 12:23:49.524909 qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-15 12:24:09.173069 qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-15 12:24:09.417071 qwak_core-0.0.60/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-15 12:24:05.157036 qwak_core-0.0.60/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-15 12:24:09.417071 qwak_core-0.0.60/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-15 12:24:09.413071 qwak_core-0.0.60/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-15 12:24:04.969035 qwak_core-0.0.60/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.417071 qwak_core-0.0.60/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-15 12:24:09.193069 qwak_core-0.0.60/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    15881 2023-05-15 12:23:51.348924 qwak_core-0.0.60/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.193069 qwak_core-0.0.60/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     2993 2023-05-15 12:24:09.193069 qwak_core-0.0.60/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2568 2023-05-15 12:23:51.552926 qwak_core-0.0.60/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-15 12:24:09.193069 qwak_core-0.0.60/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-05-15 12:24:14.013108 qwak_core-0.0.60/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-15 12:24:14.013108 qwak_core-0.0.60/qwak/__init__.py
--rw-r--r--   0        0        0     1204 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    32539 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/automations/automations.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.684237 qwak_core-0.0.60/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    17275 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14950 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0       41 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9261 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/const.py
--rw-r--r--   0        0        0     1377 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6083 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-15 12:22:28.688237 qwak_core-0.0.60/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12145 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     2696 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     3995 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13054 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-15 12:22:28.692237 qwak_core-0.0.60/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 qwak_core-0.0.60/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.60/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-16 14:33:43.315659 qwak_core-0.0.61/README.md
+-rw-r--r--   0        0        0        0 2023-05-16 14:35:36.216402 qwak_core-0.0.61/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-16 14:35:36.244402 qwak_core-0.0.61/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-16 14:35:14.392259 qwak_core-0.0.61/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.244402 qwak_core-0.0.61/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-16 14:35:36.240402 qwak_core-0.0.61/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-16 14:35:13.996257 qwak_core-0.0.61/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.240402 qwak_core-0.0.61/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-16 14:35:36.240402 qwak_core-0.0.61/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-16 14:35:14.192258 qwak_core-0.0.61/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.244402 qwak_core-0.0.61/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-16 14:35:36.232402 qwak_core-0.0.61/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-16 14:35:13.404253 qwak_core-0.0.61/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-16 14:35:36.232402 qwak_core-0.0.61/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-16 14:35:36.236402 qwak_core-0.0.61/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-16 14:35:13.600254 qwak_core-0.0.61/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.236402 qwak_core-0.0.61/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-05-16 14:35:36.236402 qwak_core-0.0.61/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-05-16 14:35:13.800256 qwak_core-0.0.61/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.236402 qwak_core-0.0.61/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-16 14:35:36.220402 qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-16 14:35:13.208252 qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-16 14:35:36.220402 qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-05-16 14:35:36.220402 qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-05-16 14:35:14.596261 qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.224402 qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-16 14:35:36.224402 qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-16 14:35:15.000263 qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.228402 qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-16 14:35:36.228402 qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-16 14:35:15.204264 qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-16 14:35:36.228402 qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-16 14:35:36.224402 qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-16 14:35:14.804262 qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.224402 qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-16 14:35:36.228402 qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-16 14:35:15.404266 qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.232402 qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-16 14:35:36.276402 qwak_core-0.0.61/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-16 14:35:18.216284 qwak_core-0.0.61/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.276402 qwak_core-0.0.61/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-16 14:35:36.276402 qwak_core-0.0.61/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-16 14:35:18.420286 qwak_core-0.0.61/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-16 14:35:36.280402 qwak_core-0.0.61/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-16 14:35:36.352403 qwak_core-0.0.61/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-16 14:35:24.036323 qwak_core-0.0.61/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.352403 qwak_core-0.0.61/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-16 14:35:36.352403 qwak_core-0.0.61/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-16 14:35:24.228324 qwak_core-0.0.61/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-16 14:35:36.356403 qwak_core-0.0.61/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-16 14:35:36.360403 qwak_core-0.0.61/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-16 14:35:25.196331 qwak_core-0.0.61/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-16 14:35:36.360403 qwak_core-0.0.61/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-16 14:35:36.356403 qwak_core-0.0.61/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-16 14:35:25.004329 qwak_core-0.0.61/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.356403 qwak_core-0.0.61/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5497 2023-05-16 14:35:36.360403 qwak_core-0.0.61/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7820 2023-05-16 14:35:25.388332 qwak_core-0.0.61/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.360403 qwak_core-0.0.61/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-16 14:35:36.364403 qwak_core-0.0.61/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-16 14:35:25.584333 qwak_core-0.0.61/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-16 14:35:36.364403 qwak_core-0.0.61/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12352 2023-05-16 14:35:36.456404 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    18970 2023-05-16 14:35:33.708386 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.456404 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5494 2023-05-16 14:35:36.452403 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7776 2023-05-16 14:35:33.280383 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.452403 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-16 14:35:36.452403 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-16 14:35:33.500385 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.456404 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-16 14:35:36.448403 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-16 14:35:32.872381 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-16 14:35:36.448403 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-16 14:35:36.448403 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-16 14:35:33.080382 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.448403 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-16 14:35:36.464403 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-16 14:35:34.296390 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.464403 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-16 14:35:36.460404 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-16 14:35:34.100389 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.460404 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-16 14:35:36.456404 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-16 14:35:33.904387 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.460404 qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-16 14:35:36.444404 qwak_core-0.0.61/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-16 14:35:32.652380 qwak_core-0.0.61/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.444404 qwak_core-0.0.61/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-16 14:35:36.440403 qwak_core-0.0.61/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-16 14:35:32.216377 qwak_core-0.0.61/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.440403 qwak_core-0.0.61/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    42145 2023-05-16 14:35:36.440403 qwak_core-0.0.61/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    55993 2023-05-16 14:35:32.448378 qwak_core-0.0.61/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-16 14:35:36.444404 qwak_core-0.0.61/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    18658 2023-05-16 14:35:36.392403 qwak_core-0.0.61/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    15525 2023-05-16 14:35:27.580346 qwak_core-0.0.61/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    18652 2023-05-16 14:35:36.392403 qwak_core-0.0.61/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-16 14:35:36.388403 qwak_core-0.0.61/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-16 14:35:27.376345 qwak_core-0.0.61/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.388403 qwak_core-0.0.61/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-05-16 14:35:36.380403 qwak_core-0.0.61/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-05-16 14:35:26.976342 qwak_core-0.0.61/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.380403 qwak_core-0.0.61/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-16 14:35:36.380403 qwak_core-0.0.61/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-16 14:35:27.172344 qwak_core-0.0.61/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.384403 qwak_core-0.0.61/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-16 14:35:36.384403 qwak_core-0.0.61/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-16 14:35:27.772348 qwak_core-0.0.61/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-16 14:35:36.384403 qwak_core-0.0.61/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-05-16 14:35:36.388403 qwak_core-0.0.61/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-05-16 14:35:28.200350 qwak_core-0.0.61/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-16 14:35:36.388403 qwak_core-0.0.61/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-16 14:35:36.396403 qwak_core-0.0.61/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-16 14:35:28.616353 qwak_core-0.0.61/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.400403 qwak_core-0.0.61/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-16 14:35:36.400403 qwak_core-0.0.61/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-16 14:35:28.808354 qwak_core-0.0.61/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-16 14:35:36.400403 qwak_core-0.0.61/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-16 14:35:36.372403 qwak_core-0.0.61/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-16 14:35:26.392338 qwak_core-0.0.61/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.372403 qwak_core-0.0.61/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-16 14:35:36.376403 qwak_core-0.0.61/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-16 14:35:26.580340 qwak_core-0.0.61/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-16 14:35:36.376403 qwak_core-0.0.61/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-16 14:35:36.368403 qwak_core-0.0.61/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-16 14:35:26.004336 qwak_core-0.0.61/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.368403 qwak_core-0.0.61/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    43712 2023-05-16 14:35:36.364403 qwak_core-0.0.61/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    63341 2023-05-16 14:35:25.808335 qwak_core-0.0.61/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.368403 qwak_core-0.0.61/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-16 14:35:36.372403 qwak_core-0.0.61/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-16 14:35:26.204337 qwak_core-0.0.61/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-16 14:35:36.372403 qwak_core-0.0.61/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-16 14:35:36.264402 qwak_core-0.0.61/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-16 14:35:17.204278 qwak_core-0.0.61/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.264402 qwak_core-0.0.61/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-16 14:35:36.268402 qwak_core-0.0.61/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-16 14:35:17.408279 qwak_core-0.0.61/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.268402 qwak_core-0.0.61/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-16 14:35:36.268402 qwak_core-0.0.61/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-16 14:35:17.608281 qwak_core-0.0.61/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-16 14:35:36.272402 qwak_core-0.0.61/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-16 14:35:36.328403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-16 14:35:22.892315 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.332403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-16 14:35:36.328403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-16 14:35:22.704314 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-16 14:35:36.328403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9535 2023-05-16 14:35:36.304402 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    10460 2023-05-16 14:35:20.912302 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.308403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5268 2023-05-16 14:35:36.304402 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8525 2023-05-16 14:35:20.720301 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.304402 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-16 14:35:36.296403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-16 14:35:20.056297 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.296403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    27847 2023-05-16 14:35:36.300402 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20073 2023-05-16 14:35:20.524300 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    33080 2023-05-16 14:35:36.304402 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-16 14:35:36.308403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-16 14:35:21.112304 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.308403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-16 14:35:36.312403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-16 14:35:21.308305 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-16 14:35:36.312403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25213 2023-05-16 14:35:36.300402 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37366 2023-05-16 14:35:20.276298 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.300402 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-16 14:35:36.312403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-16 14:35:21.508306 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.316403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0     5958 2023-05-16 14:35:36.316403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.py
+-rw-r--r--   0        0        0     6232 2023-05-16 14:35:21.704307 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.316403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-16 14:35:36.332403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-16 14:35:35.720399 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.332403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-16 14:35:36.332403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-16 14:35:35.924400 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-16 14:35:36.336403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-16 14:35:36.336403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-16 14:35:23.464319 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.336403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-16 14:35:36.340403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-16 14:35:23.652320 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-16 14:35:36.340403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-16 14:35:36.340403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-16 14:35:23.848322 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.344403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-16 14:35:36.344403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-16 14:35:24.612327 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.348403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-16 14:35:36.344403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-16 14:35:24.416325 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-16 14:35:36.344403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-16 14:35:36.348403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-16 14:35:24.812328 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.348403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-16 14:35:36.316403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-16 14:35:21.908309 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.320403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-16 14:35:36.320403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-16 14:35:22.112310 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.320403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-16 14:35:36.324403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-16 14:35:22.308312 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-16 14:35:36.324403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-16 14:35:36.324403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-16 14:35:22.500313 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.324403 qwak_core-0.0.61/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-16 14:35:36.464403 qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-16 14:35:34.496391 qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.464403 qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-16 14:35:36.468404 qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-16 14:35:34.692392 qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-16 14:35:36.468404 qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-16 14:35:36.468404 qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-16 14:35:34.892394 qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.472404 qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-16 14:35:36.472404 qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-16 14:35:35.100395 qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-16 14:35:36.472404 qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-16 14:35:36.472404 qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-16 14:35:35.308396 qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-16 14:35:36.476404 qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-16 14:35:36.476404 qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-16 14:35:35.512398 qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.476404 qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-16 14:35:36.404403 qwak_core-0.0.61/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-16 14:35:29.016356 qwak_core-0.0.61/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.404403 qwak_core-0.0.61/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-16 14:35:36.404403 qwak_core-0.0.61/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-16 14:35:29.212357 qwak_core-0.0.61/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-16 14:35:36.404403 qwak_core-0.0.61/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-16 14:35:36.280402 qwak_core-0.0.61/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-16 14:35:19.232291 qwak_core-0.0.61/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.284402 qwak_core-0.0.61/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-16 14:35:36.284402 qwak_core-0.0.61/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-16 14:35:19.428292 qwak_core-0.0.61/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.288402 qwak_core-0.0.61/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-16 14:35:36.288402 qwak_core-0.0.61/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-16 14:35:19.636294 qwak_core-0.0.61/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-16 14:35:36.292402 qwak_core-0.0.61/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-16 14:35:36.292402 qwak_core-0.0.61/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-16 14:35:19.836295 qwak_core-0.0.61/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.296403 qwak_core-0.0.61/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-16 14:35:36.376403 qwak_core-0.0.61/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-16 14:35:26.776341 qwak_core-0.0.61/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-16 14:35:36.380403 qwak_core-0.0.61/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-16 14:35:36.420403 qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-16 14:35:30.416365 qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.420403 qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-16 14:35:36.420403 qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-16 14:35:30.616366 qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.424403 qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-16 14:35:36.424403 qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-16 14:35:30.820368 qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.424403 qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-16 14:35:36.424403 qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-16 14:35:31.016369 qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.428403 qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-16 14:35:36.428403 qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-16 14:35:31.224370 qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.428403 qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-16 14:35:36.432403 qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-16 14:35:31.440372 qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-16 14:35:36.432403 qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-16 14:35:36.432403 qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-16 14:35:31.632373 qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.432403 qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-16 14:35:36.408403 qwak_core-0.0.61/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-16 14:35:29.612360 qwak_core-0.0.61/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.412403 qwak_core-0.0.61/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-16 14:35:36.416403 qwak_core-0.0.61/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-16 14:35:30.208364 qwak_core-0.0.61/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.416403 qwak_core-0.0.61/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-16 14:35:36.412403 qwak_core-0.0.61/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-16 14:35:29.812361 qwak_core-0.0.61/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-16 14:35:36.412403 qwak_core-0.0.61/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9322 2023-05-16 14:35:36.412403 qwak_core-0.0.61/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    13291 2023-05-16 14:35:30.008362 qwak_core-0.0.61/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.416403 qwak_core-0.0.61/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-16 14:35:36.396403 qwak_core-0.0.61/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-16 14:35:28.412352 qwak_core-0.0.61/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-16 14:35:36.396403 qwak_core-0.0.61/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-16 14:35:36.260402 qwak_core-0.0.61/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-16 14:35:18.832289 qwak_core-0.0.61/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-16 14:35:36.260402 qwak_core-0.0.61/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-16 14:35:36.256402 qwak_core-0.0.61/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-16 14:35:18.624287 qwak_core-0.0.61/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.260402 qwak_core-0.0.61/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-16 14:35:36.264402 qwak_core-0.0.61/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-16 14:35:19.028290 qwak_core-0.0.61/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-16 14:35:36.264402 qwak_core-0.0.61/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-16 14:35:36.392403 qwak_core-0.0.61/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-16 14:35:27.984349 qwak_core-0.0.61/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-16 14:35:36.396403 qwak_core-0.0.61/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-16 14:35:36.408403 qwak_core-0.0.61/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-16 14:35:29.412358 qwak_core-0.0.61/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-16 14:35:36.408403 qwak_core-0.0.61/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-16 14:35:36.256402 qwak_core-0.0.61/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-16 14:35:16.404272 qwak_core-0.0.61/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.256402 qwak_core-0.0.61/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-16 14:35:36.252402 qwak_core-0.0.61/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-16 14:35:16.204271 qwak_core-0.0.61/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-16 14:35:36.252402 qwak_core-0.0.61/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-16 14:35:36.244402 qwak_core-0.0.61/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-16 14:35:15.616267 qwak_core-0.0.61/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.248402 qwak_core-0.0.61/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-16 14:35:36.248402 qwak_core-0.0.61/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-16 14:35:15.808268 qwak_core-0.0.61/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.248402 qwak_core-0.0.61/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-16 14:35:36.252402 qwak_core-0.0.61/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-16 14:35:16.008270 qwak_core-0.0.61/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-16 14:35:36.252402 qwak_core-0.0.61/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-16 14:35:36.436403 qwak_core-0.0.61/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-16 14:35:32.024376 qwak_core-0.0.61/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-16 14:35:36.440403 qwak_core-0.0.61/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-16 14:35:36.436403 qwak_core-0.0.61/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-16 14:35:31.832374 qwak_core-0.0.61/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.436403 qwak_core-0.0.61/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-16 14:35:36.272402 qwak_core-0.0.61/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    15881 2023-05-16 14:35:17.812282 qwak_core-0.0.61/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.272402 qwak_core-0.0.61/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     2993 2023-05-16 14:35:36.272402 qwak_core-0.0.61/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2568 2023-05-16 14:35:18.016283 qwak_core-0.0.61/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 14:35:36.276402 qwak_core-0.0.61/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-05-16 14:35:37.944413 qwak_core-0.0.61/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-16 14:35:37.944413 qwak_core-0.0.61/qwak/__init__.py
+-rw-r--r--   0        0        0     1501 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12899 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/automations/automations.py
+-rw-r--r--   0        0        0     9638 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    18744 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     1697 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    17275 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14950 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0       41 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.315659 qwak_core-0.0.61/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/inner/const.py
+-rw-r--r--   0        0        0     1377 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-05-16 14:33:43.319659 qwak_core-0.0.61/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12145 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     2696 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     3995 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13054 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-16 14:33:43.323659 qwak_core-0.0.61/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 qwak_core-0.0.61/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.61/PKG-INFO
```

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/features/real_time_feature_set_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.61/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.61/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.61/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/pyproject.toml` & `qwak_core-0.0.61/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.60"
+version = "0.0.61"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.60/qwak/automations/__init__.py` & `qwak_core-0.0.61/qwak/automations/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 from qwak.automations.automations import (
     Action,
-    AggregationType,
     Automation,
     AutomationAudit,
+    CustomWebhook,
+    Metric,
+    MetricBasedTrigger,
+    NoneTrigger,
+    Notification,
+    ScheduledTrigger,
+    SlackNotification,
+    SqlMetric,
+    ThresholdDirection,
+    Trigger,
+)
+from qwak.automations.batch_execution_action import (
+    BatchExecution,
+    BatchJobDataSpecifications,
+    BatchJobExecutionSpecifications,
+)
+from qwak.automations.build_and_deploy_action import (
+    AggregationType,
     AutoScaleQuerySpec,
     AutoScaleTrigger,
     AutoScalingConfig,
     AutoScalingPrometheusTrigger,
     BuildMetric,
     BuildSpecifications,
     CpuResources,
-    CustomWebhook,
     DeploymentCondition,
     DeploymentSpecifications,
     GpuResources,
-    Metric,
-    MetricBasedTrigger,
     MetricType,
-    NoneTrigger,
-    Notification,
     QwakBuildDeploy,
     Resources,
-    ScheduledTrigger,
-    SlackNotification,
-    SqlMetric,
-    ThresholdDirection,
-    Trigger,
 )
 
 __all__ = [
     "Action",
     "AggregationType",
     "Automation",
     "AutomationAudit",
@@ -52,8 +59,11 @@
     "QwakBuildDeploy",
     "Resources",
     "ScheduledTrigger",
     "SlackNotification",
     "SqlMetric",
     "ThresholdDirection",
     "Trigger",
+    "BatchExecution",
+    "BatchJobDataSpecifications",
+    "BatchJobExecutionSpecifications",
 ]
```

### Comparing `qwak_core-0.0.60/qwak/automations/automation_executions.py` & `qwak_core-0.0.61/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/automations/automations.py` & `qwak_core-0.0.61/qwak/automations/build_and_deploy_action.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import re
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
-from datetime import datetime
 from enum import Enum
 from typing import Dict, List
 
 from _qwak_proto.qwak.automation.v1.action_pb2 import Action as ActionProto
 from _qwak_proto.qwak.automation.v1.action_pb2 import (
     AdvancedDeploymentOptions,
     BuildAndDeployAction,
@@ -17,17 +16,16 @@
     DeploymentCondition as DeploymentConditionProto,
 )
 from _qwak_proto.qwak.automation.v1.action_pb2 import (
     DeploymentSize,
     DeploymentSpec,
     GitModelSource,
 )
-from _qwak_proto.qwak.automation.v1.action_pb2 import GpuResources
 from _qwak_proto.qwak.automation.v1.action_pb2 import GpuResources as GpuResourceProto
-from _qwak_proto.qwak.automation.v1.action_pb2 import GpuType, MemoryUnit
+from _qwak_proto.qwak.automation.v1.action_pb2 import GpuType
 from _qwak_proto.qwak.automation.v1.action_pb2 import Resources as ResourceProto
 from _qwak_proto.qwak.automation.v1.auto_scaling_pb2 import (
     AGGREGATION_TYPE_AVERAGE,
     AGGREGATION_TYPE_MAX,
     AGGREGATION_TYPE_MIN,
     AGGREGATION_TYPE_SUM,
     METRIC_TYPE_CPU,
@@ -41,327 +39,22 @@
     AutoScalingPrometheusTrigger as AutoScalingPrometheusTriggerProto,
 )
 from _qwak_proto.qwak.automation.v1.auto_scaling_pb2 import QuerySpec
 from _qwak_proto.qwak.automation.v1.auto_scaling_pb2 import (
     ScaleTrigger as ScaleTriggerProto,
 )
 from _qwak_proto.qwak.automation.v1.auto_scaling_pb2 import Triggers as TriggersProto
-from _qwak_proto.qwak.automation.v1.automation_pb2 import Automation as AutomationProto
-from _qwak_proto.qwak.automation.v1.automation_pb2 import (
-    AutomationAudit as AutomationAuditProto,
+from qwak.automations.common import (
+    Action,
+    ThresholdDirection,
+    map_memory_units,
+    map_memory_units_proto,
+    map_proto_threshold_to_direction,
+    map_threshold_direction_to_proto,
 )
-from _qwak_proto.qwak.automation.v1.automation_pb2 import (
-    AutomationSpec as AutomationSpecProto,
-)
-from _qwak_proto.qwak.automation.v1.common_pb2 import Metric as MetricProto
-from _qwak_proto.qwak.automation.v1.common_pb2 import MetricThresholdDirection
-from _qwak_proto.qwak.automation.v1.common_pb2 import SqlMetric as SqlMetricProto
-from _qwak_proto.qwak.automation.v1.notification_pb2 import (
-    CustomWebhook as CustomWebhookProto,
-)
-from _qwak_proto.qwak.automation.v1.notification_pb2 import (
-    HttpMethodType as HttpMethodTypeProto,
-)
-from _qwak_proto.qwak.automation.v1.notification_pb2 import (
-    Notification as NotificationProto,
-)
-from _qwak_proto.qwak.automation.v1.notification_pb2 import (
-    PostSlackNotification as PostSlackNotificationProto,
-)
-from _qwak_proto.qwak.automation.v1.trigger_pb2 import (
-    MetricBasedTrigger as MetricBasedTriggerProto,
-)
-from _qwak_proto.qwak.automation.v1.trigger_pb2 import NoneTrigger as NoneTriggerProto
-from _qwak_proto.qwak.automation.v1.trigger_pb2 import (
-    OnBoardingTrigger as OnBoardingTriggerProto,
-)
-from _qwak_proto.qwak.automation.v1.trigger_pb2 import (
-    ScheduledTrigger as ScheduledTriggerProto,
-)
-from _qwak_proto.qwak.automation.v1.trigger_pb2 import Trigger as TriggerProto
-from google.protobuf.timestamp_pb2 import Timestamp
-
-
-class ThresholdDirection(Enum):
-    ABOVE = 1
-    BELOW = 2
-
-
-threshold_to_proto_mapping = {
-    ThresholdDirection.ABOVE: MetricThresholdDirection.ABOVE,
-    ThresholdDirection.BELOW: MetricThresholdDirection.BELOW,
-}
-
-proto_threshold_to_threshold = {v: k for k, v in threshold_to_proto_mapping.items()}
-
-
-def map_threshold_direction_to_proto(
-    direction: ThresholdDirection,
-) -> MetricThresholdDirection:
-    return threshold_to_proto_mapping.get(
-        direction, MetricThresholdDirection.INVALID_METRIC_DIRECTION
-    )
-
-
-def map_proto_threshold_to_direction(
-    direction: MetricThresholdDirection,
-) -> ThresholdDirection:
-    return proto_threshold_to_threshold.get(direction)
-
-
-def map_memory_units(memory):
-    memory_unit = re.sub(r"\d+", "", memory)
-    if memory_unit == "Gi":
-        return MemoryUnit.GIB
-    elif memory_unit == "Mib":
-        return MemoryUnit.MIB
-    else:
-        return MemoryUnit.UNKNOWN
-
-
-def map_memory_units_proto(memory_unit: MemoryUnit):
-    if memory_unit == MemoryUnit.MIB:
-        return "Mib"
-    elif memory_unit == MemoryUnit.GIB:
-        return "Gi"
-    else:
-        return ""
-
-
-@dataclass
-class Trigger(ABC):
-    def to_proto(self):
-        # abstract method
-        pass
-
-    @staticmethod
-    @abstractmethod
-    def from_proto(message: TriggerProto):
-        # abstract method
-        pass
-
-
-@dataclass
-class Metric(ABC):
-    @abstractmethod
-    def to_proto(self):
-        # abstract method
-        pass
-
-    @staticmethod
-    @abstractmethod
-    def from_proto(message: MetricProto):
-        # abstract method
-        pass
-
-
-@dataclass
-class ScheduledTrigger(Trigger):
-    cron: str = field(default="")
-    interval: str = field(default="")
-
-    def to_proto(self):
-        return (
-            TriggerProto(
-                scheduled_trigger=ScheduledTriggerProto(interval=self.interval)
-            )
-            if self.interval
-            else TriggerProto(scheduled_trigger=ScheduledTriggerProto(cron=self.cron))
-        )
-
-    @staticmethod
-    def from_proto(message: TriggerProto):
-        return ScheduledTrigger(
-            cron=message.scheduled_trigger.cron,
-            interval=message.scheduled_trigger.interval,
-        )
-
-
-@dataclass
-class MetricBasedTrigger(Trigger):
-    name: str = field(default="")
-    metric: Metric = field(default="")
-    direction: ThresholdDirection = field(default=ThresholdDirection.ABOVE)
-    threshold: str = field(default="")
-    override_cron: str = field(default="")
-
-    def to_proto(self):
-        return TriggerProto(
-            metric_based_trigger=MetricBasedTriggerProto(
-                name=self.name,
-                threshold=self.threshold,
-                metric=self.metric.to_proto(),
-                threshold_direction=map_threshold_direction_to_proto(self.direction),
-                override_cron=self.override_cron,
-            )
-        )
-
-    @staticmethod
-    def from_proto(message: TriggerProto):
-        metric = map_metric_name_to_class(
-            message.metric_based_trigger.metric.WhichOneof("metric")
-        )
-        return MetricBasedTrigger(
-            name=message.metric_based_trigger.name,
-            metric=metric.from_proto(message.metric_based_trigger.metric)
-            if metric
-            else None,
-            threshold=message.metric_based_trigger.threshold,
-            direction=map_proto_threshold_to_direction(
-                message.metric_based_trigger.threshold_direction
-            ),
-            override_cron=message.metric_based_trigger.override_cron,
-        )
-
-
-@dataclass
-class NoneTrigger(Trigger):
-    def to_proto(self):
-        return TriggerProto(none_trigger=NoneTriggerProto())
-
-    @staticmethod
-    def from_proto(message: TriggerProto):
-        return NoneTrigger()
-
-
-@dataclass
-class OnBoardingTrigger(Trigger):
-    def to_proto(self):
-        return TriggerProto(on_boarding_trigger=OnBoardingTriggerProto())
-
-    @staticmethod
-    def from_proto(message: TriggerProto):
-        return OnBoardingTrigger()
-
-
-@dataclass
-class SqlMetric(Metric):
-    sql_query: str = field(default="")
-
-    def to_proto(self):
-        return MetricProto(sql_metric=SqlMetricProto(sql_query=self.sql_query))
-
-    @staticmethod
-    def from_proto(message: MetricProto):
-        return SqlMetric(sql_query=message.sql_metric.sql_query)
-
-
-@dataclass
-class Notification(ABC):
-    def to_proto(self):
-        # abstract method
-        pass
-
-    @staticmethod
-    @abstractmethod
-    def from_proto(message: TriggerProto):
-        # abstract method
-        pass
-
-
-@dataclass
-class SlackNotification(Notification):
-    webhook: str = field(default="")
-
-    def to_proto(self):
-        return NotificationProto(
-            post_slack_notification=PostSlackNotificationProto(
-                webhook=self.webhook,
-            )
-        )
-
-    @staticmethod
-    def from_proto(message: NotificationProto):
-        return SlackNotification(
-            webhook=message.post_slack_notification.webhook,
-        )
-
-    def __str__(self):
-        return f"Slack Notification:\n webhook:{self.webhook}\n"
-
-
-@dataclass
-class CustomWebhook(Notification):
-    url: str = field(default="")
-    http_method: str = field(default="GET")
-    headers: Dict[str, str] = field(default_factory=dict)
-    data: Dict[str, str] = field(default_factory=dict)
-
-    _HTTP_NAME_TO_STATUS_MAPPING = {
-        "GET": HttpMethodTypeProto.HTTP_METHOD_TYPE_GET,
-        "POST": HttpMethodTypeProto.HTTP_METHOD_TYPE_POST,
-        "PUT": HttpMethodTypeProto.HTTP_METHOD_TYPE_PUT,
-        "PATCH": HttpMethodTypeProto.HTTP_METHOD_TYPE_PATCH,
-        "DELETE": HttpMethodTypeProto.HTTP_METHOD_TYPE_DELETE,
-        "HEAD": HttpMethodTypeProto.HTTP_METHOD_TYPE_HEAD,
-    }
-
-    _HTTP_STATUS_TO_NAME_MAPPING = {
-        v: k for k, v in _HTTP_NAME_TO_STATUS_MAPPING.items()
-    }
-
-    def __post_init__(self):
-        if self.http_method.upper() not in self._HTTP_NAME_TO_STATUS_MAPPING.keys():
-            raise ValueError(
-                f"HTTP method {self.http_method} is not a valid method. Available options are "
-                f"{list(self._HTTP_NAME_TO_STATUS_MAPPING.keys())}"
-            )
-
-    def to_proto(self):
-        return NotificationProto(
-            custom_webhook=CustomWebhookProto(
-                url=self.url,
-                http_method=self._HTTP_NAME_TO_STATUS_MAPPING.get(
-                    self.http_method.upper()
-                ),
-                headers=self.headers,
-                data=self.data,
-            )
-        )
-
-    @staticmethod
-    def from_proto(message: NotificationProto):
-        return CustomWebhook(
-            url=message.custom_webhook.url,
-            data=message.custom_webhook.data,
-            headers=message.custom_webhook.headers,
-            http_method=CustomWebhook._HTTP_STATUS_TO_NAME_MAPPING.get(
-                message.custom_webhook.http_method
-            ),
-        )
-
-    def __str__(self):
-        return f"Custom webhook:\n url:{self.url}\n data:{self.data}\n headers:{self.headers}\n http method:{self.http_method}\n"
-
-
-class MetricType(Enum):
-    cpu = METRIC_TYPE_CPU
-    latency = METRIC_TYPE_LATENCY
-    memory = METRIC_TYPE_MEMORY
-
-
-class AggregationType(Enum):
-    avg = AGGREGATION_TYPE_AVERAGE
-    max = AGGREGATION_TYPE_MAX
-    min = AGGREGATION_TYPE_MIN
-    sum = AGGREGATION_TYPE_SUM
-
-
-@dataclass
-class Action(ABC):
-    @abstractmethod
-    def to_proto(self):
-        # abstract method
-        pass
-
-    @staticmethod
-    @abstractmethod
-    def from_proto(message: ActionProto):
-        # abstract method
-        pass
 
 
 @dataclass
 class DeploymentCondition(ABC):
     @abstractmethod
     def to_proto(self):
         # abstract method
@@ -486,45 +179,25 @@
     def from_proto(message: ResourceProto):
         return GpuResources(
             gpu_type=GpuType.Name(message.gpu_resources.gpu_type),
             gpu_amount=str(message.gpu_resources.gpu_amount),
         )
 
     @staticmethod
-    def from_gpu_proto(message: GpuResources):
+    def from_gpu_proto(message: GpuResourceProto):
         return GpuResources(
             gpu_type=GpuType.Name(message.gpu_type),
             gpu_amount=str(message.gpu_amount),
         )
 
     def __str__(self):
         return f"GPU Type: {self.gpu_type}, GPU Amount: {self.gpu_amount}"
 
 
 @dataclass
-class AutomationAudit(ABC):
-    date: datetime = field(default=datetime.now())
-    user_id: str = field(default="")
-
-    def to_proto(self):
-        timestamp = Timestamp()
-        timestamp.FromDatetime(self.date)
-        return AutomationAuditProto(user_id=self.user_id, date=timestamp)
-
-    @staticmethod
-    def from_proto(message: AutomationAuditProto):
-        return AutomationAudit(
-            user_id=message.user_id,
-            date=datetime.fromtimestamp(
-                message.date.seconds + message.date.nanos / 1e9
-            ),
-        )
-
-
-@dataclass
 class BuildSpecifications:
     parameters: Dict[str, str] = field(default_factory=dict)
     git_uri: str = field(default=None)
     tags: List[str] = field(default_factory=list)
     git_access_token_secret: str = field(default=None)
     git_branch: str = field(default="main")
     main_dir: str = field(default="main")
@@ -586,14 +259,27 @@
         )
         result += f"Base Image:\t{self.base_image}\n" if self.base_image else ""
         result += f"Resources:\n{self.resources}\n" if self.resources else ""
         result += f"Environment Variables:\n{self.env_vars}\n" if self.env_vars else ""
         return result
 
 
+class MetricType(Enum):
+    cpu = METRIC_TYPE_CPU
+    latency = METRIC_TYPE_LATENCY
+    memory = METRIC_TYPE_MEMORY
+
+
+class AggregationType(Enum):
+    avg = AGGREGATION_TYPE_AVERAGE
+    max = AGGREGATION_TYPE_MAX
+    min = AGGREGATION_TYPE_MIN
+    sum = AGGREGATION_TYPE_SUM
+
+
 @dataclass
 class AutoScalingConfig:
     min_replica_count: int = field(default=None)
     max_replica_count: int = field(default=None)
     polling_interval: int = field(default=None)
     cool_down_period: int = field(default=None)
     triggers: List[AutoScaleTrigger] = field(default_factory=list)
@@ -809,146 +495,24 @@
             ),
         )
 
     def __str__(self):
         return f"threshold: {self.threshold} \t {self.query_spec}"
 
 
-@dataclass
-class Automation:
-    id: str = field(default="")
-    name: str = field(default="")
-    model_id: str = field(default="")
-    execute_immediately: bool = field(default=False)
-    trigger: Trigger = field(default_factory=Trigger)
-    action: Action = field(default_factory=Action)
-    description: str = field(default="")
-    environment: str = field(default="")
-    is_enabled: bool = field(default=True)
-    is_deleted: bool = field(default=False)
-    is_sdk_v1: bool = field(default=False)
-    create_audit: AutomationAudit = field(default_factory=AutomationAudit)
-    on_error: Notification = field(default=None)
-    on_success: Notification = field(default=None)
-
-    def to_proto(self):
-        return AutomationProto(
-            automation_id=self.id,
-            automation_spec=AutomationSpecProto(
-                automation_name=self.name,
-                is_enabled=self.is_enabled,
-                is_sdk_v1=self.is_sdk_v1,
-                execute_immediately=self.execute_immediately,
-                model_id=self.model_id,
-                action=self.action.to_proto(),
-                trigger=self.trigger.to_proto() if self.trigger is not None else None,
-                on_error=self.on_error.to_proto()
-                if self.on_error is not None
-                else None,
-                on_success=self.on_success.to_proto()
-                if self.on_success is not None
-                else None,
-            ),
-            qwak_environment_id=self.environment,
-            create_audit=self.create_audit.to_proto(),
-            is_deleted=self.is_deleted,
-        )
-
-    @staticmethod
-    def from_proto(message: AutomationProto):
-        action = map_action_name_to_class(
-            message.automation_spec.action.WhichOneof("action")
-        )
-        trigger = map_trigger_name_to_class(
-            message.automation_spec.trigger.WhichOneof("trigger")
-        )
-        on_error_notification = map_notification_name_to_class(
-            message.automation_spec.on_error.WhichOneof("notification")
-        )
-        on_success_notification = map_notification_name_to_class(
-            message.automation_spec.on_success.WhichOneof("notification")
-        )
-
-        return Automation(
-            id=message.automation_id,
-            name=message.automation_spec.automation_name,
-            description=message.automation_spec.automation_description,
-            execute_immediately=message.automation_spec.execute_immediately,
-            model_id=message.automation_spec.model_id,
-            is_enabled=message.automation_spec.is_enabled,
-            is_sdk_v1=message.automation_spec.is_sdk_v1,
-            is_deleted=message.is_deleted,
-            action=action.from_proto(message.automation_spec.action)
-            if action
-            else None,
-            trigger=trigger.from_proto(message.automation_spec.trigger)
-            if trigger
-            else None,
-            environment=message.qwak_environment_id,
-            create_audit=AutomationAudit.from_proto(message.create_audit),
-            on_error=on_error_notification.from_proto(message.automation_spec.on_error)
-            if on_error_notification
-            else None,
-            on_success=on_success_notification.from_proto(
-                message.automation_spec.on_success
-            )
-            if on_success_notification
-            else None,
-        )
-
-    def __str__(self):
-        on_error = f"\nOn Error: {self.on_error}" if self.on_error else ""
-        on_success = f"\nOn Success: {self.on_success}" if self.on_success else ""
-        return f"Id: {self.id}\tName: {self.name}\tModel: {self.model_id}\nDescription: {self.description}\nAction: {self.action}\nTrigger: {self.trigger}{on_error}{on_success}"
-
-
-def map_notification_name_to_class(notification_name: str):
-    mapping = {
-        "post_slack_notification": SlackNotification,
-        "custom_webhook": CustomWebhook,
-    }
-    return mapping.get(notification_name)
-
-
-def map_action_name_to_class(action_name: str):
-    mapping = {"build_deploy": QwakBuildDeploy}
-    return mapping.get(action_name)
-
-
-def map_autoscaling_trigger_name_to_class(auto_scaling_trigger_name: str):
-    mapping = {"prometheus_trigger": AutoScalingPrometheusTrigger}
-    return mapping.get(auto_scaling_trigger_name)
-
-
-def map_trigger_name_to_class(trigger_name: str):
-    mapping = {
-        "scheduled_trigger": ScheduledTrigger,
-        "metric_based_trigger": MetricBasedTrigger,
-        "none_trigger": NoneTrigger,
-        "on_boarding_trigger": OnBoardingTrigger,
-    }
-
-    return mapping.get(trigger_name)
-
-
 def map_resources_name_to_class(resource_name: str):
     mapping = {"cpu_resources": CpuResources, "gpu_resources": GpuResources}
     return mapping.get(resource_name)
 
 
 def map_deployment_condition_name_to_class(deployment_condition_name: str):
     mapping = {"build_metric": BuildMetric}
     return mapping.get(deployment_condition_name)
 
 
-def map_metric_name_to_class(metric_name: str):
-    mapping = {"sql_metric": SqlMetric}
-    return mapping.get(metric_name)
-
-
 def map_auto_scaling_metric_type_proto_to_name(metric_type):
     mapping = {
         METRIC_TYPE_CPU: "cpu",
         METRIC_TYPE_LATENCY: "latency",
         METRIC_TYPE_MEMORY: "memory",
     }
     return mapping.get(metric_type)
@@ -958,7 +522,12 @@
     mapping = {
         AGGREGATION_TYPE_AVERAGE: "avg",
         AGGREGATION_TYPE_MAX: "max",
         AGGREGATION_TYPE_MIN: "min",
         AGGREGATION_TYPE_SUM: "sum",
     }
     return mapping.get(aggregation_type)
+
+
+def map_autoscaling_trigger_name_to_class(auto_scaling_trigger_name: str):
+    mapping = {"prometheus_trigger": AutoScalingPrometheusTrigger}
+    return mapping.get(auto_scaling_trigger_name)
```

### Comparing `qwak_core-0.0.60/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.61/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.61/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.61/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.61/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.61/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/alert_management/client.py` & `qwak_core-0.0.61/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/analytics/client.py` & `qwak_core-0.0.61/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/audience/client.py` & `qwak_core-0.0.61/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/automation_management/client.py` & `qwak_core-0.0.61/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.61/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.61/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.61/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.61/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/build_management/client.py` & `qwak_core-0.0.61/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.61/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.61/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/deployment/client.py` & `qwak_core-0.0.61/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.61/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.61/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.61/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.61/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.61/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/logging_client/client.py` & `qwak_core-0.0.61/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/model_management/client.py` & `qwak_core-0.0.61/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/project/client.py` & `qwak_core-0.0.61/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/secret_service/client.py` & `qwak_core-0.0.61/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.61/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.61/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.61/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.61/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.61/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.61/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.61/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.61/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.61/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.61/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.61/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.61/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.61/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.61/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.61/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.61/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/offline/client.py` & `qwak_core-0.0.61/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/feature_store/online/client.py` & `qwak_core-0.0.61/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/inner/const.py` & `qwak_core-0.0.61/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.61/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.61/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.61/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.61/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/inner/singleton_meta.py` & `qwak_core-0.0.61/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/inner/tool/auth.py` & `qwak_core-0.0.61/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.61/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.61/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.61/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.61/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/adapters/__init__.py` & `qwak_core-0.0.61/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.61/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.61/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.61/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.61/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.61/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/base.py` & `qwak_core-0.0.61/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/decorators/api.py` & `qwak_core-0.0.61/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.61/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/experiment_tracking.py` & `qwak_core-0.0.61/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/schema.py` & `qwak_core-0.0.61/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/schema_entities.py` & `qwak_core-0.0.61/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.61/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.61/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.61/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.61/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.61/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.61/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.61/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.61/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.61/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.61/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.61/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.61/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.61/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.61/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.61/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.61/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.61/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.61/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.61/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/qwak_client/client.py` & `qwak_core-0.0.61/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.61/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/qwak_client/models/model.py` & `qwak_core-0.0.61/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.61/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.61/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/tools/logger/logger.py` & `qwak_core-0.0.61/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak/tools/logger/logging.yml` & `qwak_core-0.0.61/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.61/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/qwak_services_mock/services_mock.py` & `qwak_core-0.0.61/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.60/setup.py` & `qwak_core-0.0.61/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.60',
+    'version': '0.0.61',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.60/PKG-INFO` & `qwak_core-0.0.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.60
+Version: 0.0.61
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

