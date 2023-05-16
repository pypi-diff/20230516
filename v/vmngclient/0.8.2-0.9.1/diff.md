# Comparing `tmp/vmngclient-0.8.2.tar.gz` & `tmp/vmngclient-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmngclient-0.8.2.tar", max compression
+gzip compressed data, was "vmngclient-0.9.1.tar", max compression
```

## Comparing `vmngclient-0.8.2.tar` & `vmngclient-0.9.1.tar`

### file list

```diff
@@ -1,96 +1,107 @@
--rw-r--r--   0        0        0     2748 2023-04-13 09:36:23.756716 vmngclient-0.8.2/README.md
--rw-r--r--   0        0        0      807 2023-04-13 09:36:23.756716 vmngclient-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     2259 2023-04-13 09:36:23.756716 vmngclient-0.8.2/vmngclient/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 09:36:23.756716 vmngclient-0.8.2/vmngclient/api/__init__.py
--rw-r--r--   0        0        0     6010 2023-04-13 09:36:23.756716 vmngclient-0.8.2/vmngclient/api/admin_tech_api.py
--rw-r--r--   0        0        0     8671 2023-04-13 09:36:23.756716 vmngclient-0.8.2/vmngclient/api/administration.py
--rw-r--r--   0        0        0     6253 2023-04-13 09:36:23.756716 vmngclient-0.8.2/vmngclient/api/alarms_api.py
--rw-r--r--   0        0        0     1829 2023-04-13 09:36:23.756716 vmngclient-0.8.2/vmngclient/api/api_containter.py
--rw-r--r--   0        0        0    11371 2023-04-13 09:36:23.756716 vmngclient-0.8.2/vmngclient/api/basic_api.py
--rw-r--r--   0        0        0     2742 2023-04-13 09:36:23.756716 vmngclient-0.8.2/vmngclient/api/dashboard_api.py
--rw-r--r--   0        0        0     6508 2023-04-13 09:36:23.756716 vmngclient-0.8.2/vmngclient/api/device_action_api.py
--rw-r--r--   0        0        0     1651 2023-04-13 09:36:23.756716 vmngclient-0.8.2/vmngclient/api/logs_api.py
--rw-r--r--   0        0        0     5881 2023-04-13 09:36:23.756716 vmngclient-0.8.2/vmngclient/api/mtt_aaa_api.py
--rw-r--r--   0        0        0     4040 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/omp_api.py
--rw-r--r--   0        0        0     5432 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/packet_capture_api.py
--rw-r--r--   0        0        0     4945 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/partition_manager_api.py
--rw-r--r--   0        0        0     2041 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/resource_pool_api.py
--rw-r--r--   0        0        0     7330 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/software_action_api.py
--rw-r--r--   0        0        0     5412 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/speedtest_api.py
--rw-r--r--   0        0        0     9546 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/task_status_api.py
--rw-r--r--   0        0        0    21616 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/template_api.py
--rw-r--r--   0        0        0     1476 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/__init__.py
--rw-r--r--   0        0        0     7176 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/cli_template.py
--rw-r--r--   0        0        0     2109 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/device_template/device_template.py
--rw-r--r--   0        0        0      476 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/device_template/device_template_payload.json.j2
--rw-r--r--   0        0        0     1224 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/feature_template.py
--rw-r--r--   0        0        0     3118 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/feature_template_field.py
--rw-r--r--   0        0        0      615 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/feature_template_payload.py
--rw-r--r--   0        0        0     2441 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/models/cisco_aaa_model.py
--rw-r--r--   0        0        0     2160 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/aaa_model.py
--rw-r--r--   0        0        0    11178 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/feature/aaa.json.j2
--rw-r--r--   0        0        0     1041 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/feature/accounting.json.j2
--rw-r--r--   0        0        0     4264 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/feature/radius.json.j2
--rw-r--r--   0        0        0     3735 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/feature/tacacs.json.j2
--rw-r--r--   0        0        0     1999 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/feature/user.json.j2
--rw-r--r--   0        0        0      419 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_system/cisco_system_model.py
--rw-r--r--   0        0        0     6752 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_system/feature/cisco_system.json.j2
--rw-r--r--   0        0        0     2430 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
--rw-r--r--   0        0        0     4529 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
--rw-r--r--   0        0        0     1843 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/feature/dns.json.j2
--rw-r--r--   0        0        0     2123 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
--rw-r--r--   0        0        0     2098 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
--rw-r--r--   0        0        0      627 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
--rw-r--r--   0        0        0     2665 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/cisco_vpn_interface_ethernet_model.py
--rw-r--r--   0        0        0     8179 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/cisco_vpn_interface_ethernet.json.j2
--rw-r--r--   0        0        0     9926 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/tunnel.json.j2
--rw-r--r--   0        0        0     7057 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/tenant/tenant.json.j2
--rw-r--r--   0        0        0     1701 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/templates/payloads/tenant/tenant_model.py
--rw-r--r--   0        0        0     1119 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/tenant_api.py
--rw-r--r--   0        0        0     4953 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/tenant_backup_restore_api.py
--rw-r--r--   0        0        0    10790 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/api/versions_utils.py
--rw-r--r--   0        0        0    19969 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/dataclasses.py
--rw-r--r--   0        0        0     1634 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/exceptions.py
--rw-r--r--   0        0        0      672 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/logging.conf
--rw-r--r--   0        0        0     5615 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/response.py
--rw-r--r--   0        0        0    11671 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/session.py
--rw-r--r--   0        0        0     7877 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/tests/test_admin_tech_api.py
--rw-r--r--   0        0        0    12255 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/tests/test_administration.py
--rw-r--r--   0        0        0    11034 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/tests/test_alarms_api.py
--rw-r--r--   0        0        0     8053 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/tests/test_cli_template.py
--rw-r--r--   0        0        0     4460 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/tests/test_creation_tools.py
--rw-r--r--   0        0        0     3878 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/tests/test_device_action_api.py
--rw-r--r--   0        0        0    25969 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/tests/test_devices_api.py
--rw-r--r--   0        0        0      836 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/tests/test_feature_template_field.py
--rw-r--r--   0        0        0     1485 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/tests/test_logs_api.py
--rw-r--r--   0        0        0    11146 2023-04-13 09:36:23.760716 vmngclient-0.8.2/vmngclient/tests/test_mtt_aaa_api.py
--rw-r--r--   0        0        0    16398 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_omp_api.py
--rw-r--r--   0        0        0     5153 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_packet_capture.py
--rw-r--r--   0        0        0     4967 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_partition_manager_api.py
--rw-r--r--   0        0        0     2947 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_response.py
--rw-r--r--   0        0        0     4753 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_session.py
--rw-r--r--   0        0        0     3774 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_software_action_api.py
--rw-r--r--   0        0        0     6005 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_speed_test_api.py
--rw-r--r--   0        0        0     5042 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_task_status_api.py
--rw-r--r--   0        0        0     8686 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_templates.py
--rw-r--r--   0        0        0     3625 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_tenant_backup_restore_api.py
--rw-r--r--   0        0        0     8432 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_typed_list.py
--rw-r--r--   0        0        0     5170 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_version_utils.py
--rw-r--r--   0        0        0     3132 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/tests/test_vmanage_auth.py
--rw-r--r--   0        0        0     7357 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/typed_list.py
--rw-r--r--   0        0        0        0 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/__init__.py
--rw-r--r--   0        0        0      190 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/alarm_status.py
--rw-r--r--   0        0        0      196 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/certificate_status.py
--rw-r--r--   0        0        0       97 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/config_status.py
--rw-r--r--   0        0        0     4677 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/creation_tools.py
--rw-r--r--   0        0        0     1233 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/dashboard.py
--rw-r--r--   0        0        0     2261 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/device_model.py
--rw-r--r--   0        0        0      472 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/operation_status.py
--rw-r--r--   0        0        0      139 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/personality.py
--rw-r--r--   0        0        0      115 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/reachability.py
--rw-r--r--   0        0        0       92 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/template_type.py
--rw-r--r--   0        0        0     1944 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/upgrades_helper.py
--rw-r--r--   0        0        0      102 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/utils/validate_status.py
--rw-r--r--   0        0        0     4977 2023-04-13 09:36:23.764716 vmngclient-0.8.2/vmngclient/vmanage_auth.py
--rw-r--r--   0        0        0     4543 1970-01-01 00:00:00.000000 vmngclient-0.8.2/setup.py
--rw-r--r--   0        0        0     3894 1970-01-01 00:00:00.000000 vmngclient-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     3612 2023-05-16 11:41:29.006771 vmngclient-0.9.1/README.md
+-rw-r--r--   0        0        0      827 2023-05-16 11:41:29.010772 vmngclient-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     2259 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/__init__.py
+-rw-r--r--   0        0        0     6090 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/admin_tech_api.py
+-rw-r--r--   0        0        0     8709 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/administration.py
+-rw-r--r--   0        0        0     6253 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/alarms_api.py
+-rw-r--r--   0        0        0     1919 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/api_containter.py
+-rw-r--r--   0        0        0    11322 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/basic_api.py
+-rw-r--r--   0        0        0     7051 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/dashboard_api.py
+-rw-r--r--   0        0        0     6508 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/device_action_api.py
+-rw-r--r--   0        0        0     1651 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/logs_api.py
+-rw-r--r--   0        0        0     5971 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/mtt_aaa_api.py
+-rw-r--r--   0        0        0     4040 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/omp_api.py
+-rw-r--r--   0        0        0     5631 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/packet_capture_api.py
+-rw-r--r--   0        0        0     4945 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/partition_manager_api.py
+-rw-r--r--   0        0        0     2041 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/resource_pool_api.py
+-rw-r--r--   0        0        0     7330 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/software_action_api.py
+-rw-r--r--   0        0        0     5412 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/speedtest_api.py
+-rw-r--r--   0        0        0     8577 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/task_status_api.py
+-rw-r--r--   0        0        0    24650 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/template_api.py
+-rw-r--r--   0        0        0     3194 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/templates/README.md
+-rw-r--r--   0        0        0     1476 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/templates/__init__.py
+-rw-r--r--   0        0        0     7232 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/templates/cli_template.py
+-rw-r--r--   0        0        0     2093 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/templates/device_template/device_template.py
+-rw-r--r--   0        0        0      476 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/templates/device_template/device_template_payload.json.j2
+-rw-r--r--   0        0        0     1306 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/templates/feature_template.py
+-rw-r--r--   0        0        0     3101 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/templates/feature_template_field.py
+-rw-r--r--   0        0        0      599 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/templates/feature_template_payload.py
+-rw-r--r--   0        0        0     2425 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/templates/models/cisco_aaa_model.py
+-rw-r--r--   0        0        0     1159 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/templates/models/omp_vsmart_model.py
+-rw-r--r--   0        0        0      656 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/templates/models/security_vsmart_model.py
+-rw-r--r--   0        0        0     2199 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/templates/payloads/aaa/aaa_model.py
+-rw-r--r--   0        0        0    11178 2023-05-16 11:41:29.010772 vmngclient-0.9.1/vmngclient/api/templates/payloads/aaa/feature/aaa.json.j2
+-rw-r--r--   0        0        0     1041 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/api/templates/payloads/aaa/feature/accounting.json.j2
+-rw-r--r--   0        0        0     4264 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/api/templates/payloads/aaa/feature/radius.json.j2
+-rw-r--r--   0        0        0     3735 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/api/templates/payloads/aaa/feature/tacacs.json.j2
+-rw-r--r--   0        0        0     1999 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/api/templates/payloads/aaa/feature/user.json.j2
+-rw-r--r--   0        0        0      476 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/api/templates/payloads/cisco_system/cisco_system_model.py
+-rw-r--r--   0        0        0     6752 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/api/templates/payloads/cisco_system/feature/cisco_system.json.j2
+-rw-r--r--   0        0        0     2465 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
+-rw-r--r--   0        0        0     4529 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
+-rw-r--r--   0        0        0     1843 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/api/templates/payloads/cisco_vpn/feature/dns.json.j2
+-rw-r--r--   0        0        0     2123 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
+-rw-r--r--   0        0        0     2098 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
+-rw-r--r--   0        0        0      627 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
+-rw-r--r--   0        0        0     2745 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/cisco_vpn_interface_ethernet_model.py
+-rw-r--r--   0        0        0     8179 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/cisco_vpn_interface_ethernet.json.j2
+-rw-r--r--   0        0        0     9926 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/tunnel.json.j2
+-rw-r--r--   0        0        0     7057 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/api/templates/payloads/tenant/tenant.json.j2
+-rw-r--r--   0        0        0     1730 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/api/templates/payloads/tenant/tenant_model.py
+-rw-r--r--   0        0        0     1119 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/api/tenant_api.py
+-rw-r--r--   0        0        0     4953 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/api/tenant_backup_restore_api.py
+-rw-r--r--   0        0        0    10790 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/api/versions_utils.py
+-rw-r--r--   0        0        0    20283 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/dataclasses.py
+-rw-r--r--   0        0        0     2974 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/exceptions.py
+-rw-r--r--   0        0        0      672 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/logging.conf
+-rw-r--r--   0        0        0     5727 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/primitives/__init__.py
+-rw-r--r--   0        0        0     2299 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/primitives/client.py
+-rw-r--r--   0        0        0      780 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/primitives/primitive_container.py
+-rw-r--r--   0        0        0      832 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/primitives/tenant_backup_restore.py
+-rw-r--r--   0        0        0     6568 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/primitives/tenant_management.py
+-rw-r--r--   0        0        0      669 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/primitives/tenant_migration.py
+-rw-r--r--   0        0        0     6987 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/response.py
+-rw-r--r--   0        0        0    14291 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/session.py
+-rw-r--r--   0        0        0     7877 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_admin_tech_api.py
+-rw-r--r--   0        0        0    11881 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_administration.py
+-rw-r--r--   0        0        0    11034 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_alarms_api.py
+-rw-r--r--   0        0        0     8053 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_cli_template.py
+-rw-r--r--   0        0        0     4460 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_creation_tools.py
+-rw-r--r--   0        0        0     3878 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_device_action_api.py
+-rw-r--r--   0        0        0    25969 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_devices_api.py
+-rw-r--r--   0        0        0      836 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_feature_template_field.py
+-rw-r--r--   0        0        0     1485 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_logs_api.py
+-rw-r--r--   0        0        0    10911 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_mtt_aaa_api.py
+-rw-r--r--   0        0        0    16398 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_omp_api.py
+-rw-r--r--   0        0        0     5153 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_packet_capture.py
+-rw-r--r--   0        0        0     4967 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_partition_manager_api.py
+-rw-r--r--   0        0        0     7454 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_primitives.py
+-rw-r--r--   0        0        0     5724 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_response.py
+-rw-r--r--   0        0        0     4753 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_session.py
+-rw-r--r--   0        0        0     3774 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_software_action_api.py
+-rw-r--r--   0        0        0     6005 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_speed_test_api.py
+-rw-r--r--   0        0        0     3862 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_task_status_api.py
+-rw-r--r--   0        0        0     8686 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_templates.py
+-rw-r--r--   0        0        0     3625 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_tenant_backup_restore_api.py
+-rw-r--r--   0        0        0     8432 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_typed_list.py
+-rw-r--r--   0        0        0     5170 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_version_utils.py
+-rw-r--r--   0        0        0     3132 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/tests/test_vmanage_auth.py
+-rw-r--r--   0        0        0     7341 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/typed_list.py
+-rw-r--r--   0        0        0        0 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/utils/__init__.py
+-rw-r--r--   0        0        0      190 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/utils/alarm_status.py
+-rw-r--r--   0        0        0      196 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/utils/certificate_status.py
+-rw-r--r--   0        0        0       97 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/utils/config_status.py
+-rw-r--r--   0        0        0     4677 2023-05-16 11:41:29.014772 vmngclient-0.9.1/vmngclient/utils/creation_tools.py
+-rw-r--r--   0        0        0     7219 2023-05-16 11:41:29.018772 vmngclient-0.9.1/vmngclient/utils/dashboard.py
+-rw-r--r--   0        0        0     2321 2023-05-16 11:41:29.018772 vmngclient-0.9.1/vmngclient/utils/device_model.py
+-rw-r--r--   0        0        0      472 2023-05-16 11:41:29.018772 vmngclient-0.9.1/vmngclient/utils/operation_status.py
+-rw-r--r--   0        0        0      139 2023-05-16 11:41:29.018772 vmngclient-0.9.1/vmngclient/utils/personality.py
+-rw-r--r--   0        0        0      115 2023-05-16 11:41:29.018772 vmngclient-0.9.1/vmngclient/utils/reachability.py
+-rw-r--r--   0        0        0      278 2023-05-16 11:41:29.018772 vmngclient-0.9.1/vmngclient/utils/session_type.py
+-rw-r--r--   0        0        0       92 2023-05-16 11:41:29.018772 vmngclient-0.9.1/vmngclient/utils/template_type.py
+-rw-r--r--   0        0        0     1944 2023-05-16 11:41:29.018772 vmngclient-0.9.1/vmngclient/utils/upgrades_helper.py
+-rw-r--r--   0        0        0      102 2023-05-16 11:41:29.018772 vmngclient-0.9.1/vmngclient/utils/validate_status.py
+-rw-r--r--   0        0        0     5039 2023-05-16 11:41:29.018772 vmngclient-0.9.1/vmngclient/vmanage_auth.py
+-rw-r--r--   0        0        0     5500 1970-01-01 00:00:00.000000 vmngclient-0.9.1/setup.py
+-rw-r--r--   0        0        0     4798 1970-01-01 00:00:00.000000 vmngclient-0.9.1/PKG-INFO
```

### Comparing `vmngclient-0.8.2/README.md` & `vmngclient-0.9.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 </details>
 
 <details>
     <summary> <b>Admin Tech</b> <i>(click to expand)</i></summary>
 
 ```Python
 admin_tech_file = session.api.admin_tech.generate("172.16.255.11")
-admintech.download(admin_tech_file)
-admintech.delete(admin_tech_file)
+session.api.admin_tech.download(admin_tech_file)
+session.api.admin_tech.delete(admin_tech_file)
 ```
 </details>
 
 <details>
     <summary> <b>Speed test</b> <i>(click to expand)</i></summary>
 
 ```python
@@ -79,19 +79,51 @@
 
 ```python
 alarms = session.api.alarms.get()
 ```
 
 </details>
 
+<details>
+    <summary> <b>User operations</b> <i>(click to expand)</i></summary>
+
+```python
+from vmngclient.api.administration import User, UsersAPI
+
+# Get all users
+all_users = UsersAPI(session).get_all_users()
+
+# Create a user
+new_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")
+status = UsersAPI(session).create_user(new_user)
+
+# Delete a user
+status = UsersAPI(session).delete_user(username="new_user")
+```
+
+</details>
+
 ### Note:
-To remove `InsecureRequestWarning`, you can include in your scripts:
+To remove `InsecureRequestWarning`, you can include in your scripts (warning is suppressed when `VMNGCLIENT_DEVEL` environment variable is set):
 ```Python
 import urllib3
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 ```
 
+## Catching Exceptions
+```python
+try:
+	session.api.users.delete_user("XYZ")
+except vManageBadRequestError as error:
+	# Process an error.
+	logger.error(error.info.details)
+
+# message = 'Delete users request failed' 
+# details = 'No user with name XYZ was found' 
+# code = 'USER0006'
+```
+
 ## [Contributing, bug reporting and feature requests](https://github.com/CiscoDevNet/vManage-client/blob/main/CONTRIBUTING.md)
 
 ## Seeking support
 
 You can contact us by submitting [issues](https://github.com/CiscoDevNet/vManage-client/issues), or directly via mail on vmngclient@cisco.com.
```

### Comparing `vmngclient-0.8.2/pyproject.toml` & `vmngclient-0.9.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vmngclient"
-version = "0.8.2"
+version = "0.9.1"
 description = "Universal vManage API"
 authors = ["kagorski <kagorski@cisco.com>"]
 readme = "README.md"
 repository = "https://github.com/CiscoDevNet/vManage-client"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -12,19 +12,20 @@
 python-dateutil = "^2.8.2"
 attrs = "^21.4.0"
 aiohttp = "^3.8.1"
 ciscoconfparse = "^1.6.40"
 tenacity = "^8.1.0"
 parameterized = "^0.8.1"
 cattrs = "^22.2.0"
-pydantic = "^1.10.4"
 Jinja2 = "^3.1.2"
 flake8-quotes = "^3.3.1"
 clint = "^0.5.1"
 requests-toolbelt = "^0.10.1"
+packaging = "^23.0"
+pydantic = "^1.10.7"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-mock = "^3.7.0"
 isort = "^5.10.1"
 pre-commit = "^2.19.0"
```

### Comparing `vmngclient-0.8.2/vmngclient/__init__.py` & `vmngclient-0.9.1/vmngclient/__init__.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/admin_tech_api.py` & `vmngclient-0.9.1/vmngclient/api/admin_tech_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,31 +8,32 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, List, Optional
 
 from requests import Response
 from requests.exceptions import HTTPError
 
 from vmngclient.dataclasses import AdminTech, DeviceAdminTech
+from vmngclient.exceptions import vManageClientError
 from vmngclient.utils.creation_tools import create_dataclass
 
 if TYPE_CHECKING:
     from vmngclient.session import vManageSession
 
 logger = logging.getLogger(__name__)
 
 
-class GenerateAdminTechLogError(Exception):
+class GenerateAdminTechLogError(vManageClientError):
     pass
 
 
-class DownloadAdminTechLogError(Exception):
+class DownloadAdminTechLogError(vManageClientError):
     pass
 
 
-class RequestTokenIdNotFound(Exception):
+class RequestTokenIdNotFound(vManageClientError):
     pass
 
 
 class AdminTechAPI:
     """Class for handling admintech logs for a device.
 
     Attributes:
```

### Comparing `vmngclient-0.8.2/vmngclient/api/administration.py` & `vmngclient-0.9.1/vmngclient/api/administration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,71 +1,70 @@
 from __future__ import annotations
 
 import logging
 from http import HTTPStatus
 from typing import TYPE_CHECKING, List, Union, cast, overload
 
-from requests import Response
+from requests import HTTPError, Response
 
 from vmngclient.dataclasses import (
     Certificate,
     CloudConnectorData,
     CloudServicesSettings,
     Organization,
     Password,
     ServiceConfigurationData,
     SoftwareInstallTimeout,
     User,
     Vbond,
 )
-from vmngclient.exceptions import InvalidOperationError
+from vmngclient.exceptions import AlreadyExistsError, InvalidOperationError
+from vmngclient.typed_list import DataSequence
 from vmngclient.utils.creation_tools import asdict, create_dataclass
 
 if TYPE_CHECKING:
     from vmngclient.session import vManageSession
 
 logger = logging.getLogger(__name__)
 
 
-class UserAlreadyExistsError(Exception):
-    pass
-
-
-class UserDoesNotExists(Exception):
-    pass
-
-
 class UsersAPI:
     def __init__(self, session: vManageSession) -> None:
         self.session = session
 
+    def get(self) -> DataSequence[User]:
+        endpoint = "/dataservice/admin/user"
+        users = self.session.get(endpoint)
+
+        return users.dataseq(User)
+
     def get_all_users(self) -> List[User]:
         url_path = "/dataservice/admin/user"
         users = self.session.get_data(url_path)
         logger.debug(f"List of users: {users}")
         return [create_dataclass(User, user) for user in users]
 
     def exists(self, username: str) -> bool:
         return username in [user.username for user in self.get_all_users()]
 
-    def create_user(self, user: User) -> bool:
+    def create(self, user: User) -> bool:
         if self.exists(user.username):
-            raise UserAlreadyExistsError(f"{user.username} already exists.")
+            raise AlreadyExistsError(f"User {user.username} already exists.")
         url_path = "/dataservice/admin/user"
         data = asdict(user)  # type: ignore
 
-        response = self.session.post(url=url_path, json=data)
-        logger.info(response)
+        try:
+            response = self.session.post(url=url_path, json=data)
+        except HTTPError:
+            logger.error(response.json)
+
         return True if response.status_code == 200 else False
 
     def delete_user(self, username: str) -> bool:
-        if not self.exists(username):
-            raise UserDoesNotExists(f"{username} does not exists.")
         url_path = f"/dataservice/admin/user/{username}"
-        logger.debug(f"Deleting user {username}.")
         response = self.session.delete(url_path)
         return True if response.status_code == 200 else False
 
 
 class ClusterManagementAPI:
     """Covers clusterManagement API calls.
```

### Comparing `vmngclient-0.8.2/vmngclient/api/alarms_api.py` & `vmngclient-0.9.1/vmngclient/api/alarms_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/api_containter.py` & `vmngclient-0.9.1/vmngclient/api/api_containter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from vmngclient.api.admin_tech_api import AdminTechAPI
+from vmngclient.api.administration import UsersAPI
 from vmngclient.api.alarms_api import AlarmsAPI
 from vmngclient.api.basic_api import DevicesAPI, DeviceStateAPI
 from vmngclient.api.dashboard_api import DashboardAPI
 from vmngclient.api.logs_api import LogsAPI
 from vmngclient.api.omp_api import OmpAPI
 from vmngclient.api.packet_capture_api import PacketCaptureAPI
 from vmngclient.api.partition_manager_api import PartitionManagerAPI
@@ -36,7 +37,8 @@
         self.speedtest = SpeedtestAPI(session)
         self.templates = TemplatesAPI(session)
         self.tenant_backup = TenantBackupRestoreAPI(session)
         self.repository = RepositoryAPI(session)
         self.resource_pool = ResourcePoolAPI(session)
         self.software = SoftwareActionAPI(session)
         self.partition = PartitionManagerAPI(session)
+        self.users = UsersAPI(session)
```

### Comparing `vmngclient-0.8.2/vmngclient/api/basic_api.py` & `vmngclient-0.9.1/vmngclient/api/basic_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,18 +17,14 @@
 if TYPE_CHECKING:
     from vmngclient.session import vManageSession
 
 
 logger = logging.getLogger(__name__)
 
 
-class DeviceNotFoundError(Exception):
-    pass
-
-
 class DevicesAPI:
     """API methods of vManage for getting devices and controllers.
 
     Attributes:
         session: logged in API client session
     """
```

### Comparing `vmngclient-0.8.2/vmngclient/api/device_action_api.py` & `vmngclient-0.9.1/vmngclient/api/device_action_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/logs_api.py` & `vmngclient-0.9.1/vmngclient/api/logs_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/mtt_aaa_api.py` & `vmngclient-0.9.1/vmngclient/api/mtt_aaa_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 
 from vmngclient.dataclasses import TenantAAA, TenantRadiusServer, TenantTacacsServer
+from vmngclient.exceptions import vManageClientError
 from vmngclient.utils.creation_tools import asdict, create_dataclass
 
 if TYPE_CHECKING:
     from vmngclient.session import vManageSession
 
 logger = logging.getLogger(__name__)
 
 
-class AAAConfigNotPresent(Exception):
+class AAAConfigNotPresent(vManageClientError):
     pass
 
 
 def status_ok(func):
     def wrapper(*args, **kwargs):
         response = func(*args, **kwargs)
         return True if response.status_code in [200, 204] else False
@@ -62,14 +63,15 @@
         """
         Returns the Tenant AAA
         :param aaa:
         :return:
         """
         logger.debug(f"AAA config {self.tenant_id}.")
         tenant_aaa = self.session.get_data(self.url_path)
+        # return tenant_aaa
         return create_dataclass(TenantAAA, tenant_aaa)
 
     @status_ok
     def del_aaa(self):
         """
         Delete aaa works only for tenants
         :return:
```

### Comparing `vmngclient-0.8.2/vmngclient/api/omp_api.py` & `vmngclient-0.9.1/vmngclient/api/omp_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/packet_capture_api.py` & `vmngclient-0.9.1/vmngclient/api/packet_capture_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,9 @@
 from __future__ import annotations
 
-""" Methods for setting up packet capture session,
-   and download .pcap session file.
-
-    Returns:
-        status: Status
-"""
-
-
 import logging
 import time
 from contextlib import contextmanager
 from enum import Enum
 from pathlib import Path
 from typing import TYPE_CHECKING, Iterator, Optional
 
@@ -28,28 +20,38 @@
 class DownloadStatus(Enum):
     COMPLETED = "COMPLETED"
     IMPOSSIBLE = "IMPOSSIBLE"
     FILESIZE = None
 
 
 class PacketCaptureAPI:
+    """Methods for setting up packet capture session, and download .pcap session file.
+
+    Args:
+        session:
+        vpn: Defaults to 0.
+        interface: Defaults to ge0/1.
+
+    Examples:
+        >>> edge_device = session.api.devices.get().filter(personality=Personality.EDGE)[0]
+        >>> packet_capture = session.api.packet_capture.get_packets(edge_device)
+    """
+
     def __init__(
         self,
         session: vManageSession,
         vpn: str = "0",
         interface: str = "ge0/1",
-        status=None,
     ) -> None:
         self.session = session
         self.vpn = vpn
         self.interface = interface
-        self.status = status
 
     def get_packets(self, device: Device, duration_seconds=120) -> Status:
-        """Initate packet capture process.
+        """Initiate packet capture process.
 
         Args:
             device (Device): Device class object
             duration_seconds (int, optional): Duration od packet capturing . Defaults to 20.
 
         Returns:
             Status
@@ -92,15 +94,15 @@
             url_path = r"/dataservice/stream/device/capture"
             packet_setup = self.session.post(url=url_path, json=query).json()
             logger.debug(f"Packet capture session for device {device.uuid} has been opened")
             self.packet_channel = create_dataclass(PacketSetup, packet_setup)
             if self.packet_channel.is_new_session is True:
                 yield self.packet_channel
             else:
-                self.status = None
+                self.status = None  # type: ignore
                 raise PermissionError("Can't start new session, another is already open")
         finally:
             for _ in range(3):
                 time.sleep(10)
                 self.status = self.get_status(self.packet_channel)
                 if self.status.file_download_status == DownloadStatus.COMPLETED.value:
                     self.download_capture_session(self.packet_channel, device)
@@ -140,10 +142,10 @@
             file_path = f"{Path(__file__).parents[0]}/{device.uuid}.pcap"
         url = f"/dataservice/stream/device/capture/download/{packet.session_id}"
         self.session.get_file(url, file_path)  # type: ignore
         return True
 
     def get_status(self, packet_channel: PacketSetup) -> Status:
         url_path = f"/dataservice/stream/device/capture/status/{packet_channel.session_id}"
-        self.status = dict(self.session.get_json(url_path))
-        self.status = create_dataclass(Status, self.status)
+        status = self.session.get_json(url_path)
+        self.status = create_dataclass(Status, status)
         return self.status
```

### Comparing `vmngclient-0.8.2/vmngclient/api/partition_manager_api.py` & `vmngclient-0.9.1/vmngclient/api/partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/resource_pool_api.py` & `vmngclient-0.9.1/vmngclient/api/resource_pool_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/software_action_api.py` & `vmngclient-0.9.1/vmngclient/api/software_action_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/speedtest_api.py` & `vmngclient-0.9.1/vmngclient/api/speedtest_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/task_status_api.py` & `vmngclient-0.9.1/vmngclient/api/task_status_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 from __future__ import annotations
 
 import logging
-from time import sleep
-from typing import TYPE_CHECKING, List, cast
+from typing import TYPE_CHECKING, List, Optional, cast
 
 from tenacity import retry, retry_if_result, stop_after_attempt, wait_fixed  # type: ignore
 
 if TYPE_CHECKING:
     from vmngclient.session import vManageSession
 
-from pydantic import BaseModel, Field  # type: ignore
+from pydantic import BaseModel, Field
 
-from vmngclient.exceptions import EmptyTaskResponseError, TaskNotRegisteredError
 from vmngclient.utils.operation_status import OperationStatus, OperationStatusId
 
 logger = logging.getLogger(__name__)
 
 
 class SubTaskData(BaseModel):
     status: str
     status_id: str = Field(alias="statusId")
     action: str
     activity: List[str]
     current_activity: str = Field(alias="currentActivity")
-    action_config: str = Field(alias="actionConfig")
-    order: int
-    uuid: str
-    hostname: str = Field(alias="host-name")
-    site_id: str = Field(alias="site-id")
+    action_config: Optional[str] = Field(alias="actionConfig")
+    order: Optional[int]
+    uuid: Optional[str]
+    hostname: Optional[str] = Field(alias="host-name")
+    site_id: Optional[str] = Field(alias="site-id")
 
 
 class TaskResult(BaseModel):
     result: bool
     sub_tasks_data: List[SubTaskData]
 
 
@@ -74,44 +72,28 @@
         Returns:
         TasksData: Data about all tasks in vmanage
         """
         url = "dataservice/device/action/status/tasks"
         json = self.session.get_json(url)
         return TasksData.parse_obj(json)
 
-    def get_task_data(self, delay_seconds: int = 5) -> List[SubTaskData]:
+    def get_task_data(self) -> List[SubTaskData]:
         """
         Get data about all sub-tasks in task
 
         Args:
             delay_seconds (int, optional): If vmanage doesn't get data about task, after this time will asks again.
             Defaults to 5.
 
         Returns:
             List[SubTaskData]: List of all sub-tusks
         """
-        self.__check_if_data_is_available(delay_seconds)
         task_data = self.session.get_data(self.url)
         return [SubTaskData.parse_obj(subtask_data) for subtask_data in task_data]
 
-    def __check_if_data_is_available(self, delay_seconds):
-        task_data = self.session.get_data(self.url)
-        if not task_data:
-            all_tasks_ids = [task.process_id for task in self.get_all_tasks().running_tasks]
-            if self.task_id in all_tasks_ids:
-                sleep(delay_seconds)
-                task_data = self.session.get_data(self.url)
-                if not task_data:
-                    raise EmptyTaskResponseError(
-                        f"Task id {self.task_id} registered by vManage in all tasks list, "
-                        f"but response about it's status didn't contain any information."
-                    )
-            else:
-                raise TaskNotRegisteredError(f"Task id {self.task_id} is not registered by vManage.")
-
 
 class Task:
     """
     API class for getting data about task/sub-tasks
     """
 
     def __init__(self, session: vManageSession, task_id: str):
@@ -120,15 +102,14 @@
         self.url = f"/dataservice/device/action/status/{self.task_id}"
         self.task_data: List[SubTaskData]
 
     def wait_for_completed(
         self,
         timeout_seconds: int = 300,
         interval_seconds: int = 5,
-        delay_seconds: int = 10,
         success_statuses: List[OperationStatus] = [
             OperationStatus.SUCCESS,
         ],
         failure_statuses: List[OperationStatus] = [
             OperationStatus.FAILURE,
         ],
         success_statuses_ids: List[OperationStatusId] = [
@@ -224,15 +205,15 @@
             Keep asking for task status, status_id,
             activity(optional), untill check_status is True
 
             Returns:
                 List[SubTaskData]
             """
 
-            self.task_data = TasksAPI(self.session, self.task_id).get_task_data(delay_seconds)
+            self.task_data = TasksAPI(self.session, self.task_id).get_task_data()
             sub_task_statuses = [task.status for task in self.task_data]
             sub_task_statuses_id = [task.status_id for task in self.task_data]
             sub_task_activities = [task.activity for task in self.task_data]
             logger.info(
                 f"Sub-tasks data for task {self.task_id}: \n "
                 f"statuses: {sub_task_statuses}, status_ids: {sub_task_statuses_id}, activities: {sub_task_activities}."
             )
```

### Comparing `vmngclient-0.8.2/vmngclient/api/template_api.py` & `vmngclient-0.9.1/vmngclient/api/template_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,37 @@
     DeviceTemplate,
     GeneralTemplate,
 )
 from vmngclient.api.templates.feature_template import FeatureTemplate
 from vmngclient.api.templates.feature_template_field import FeatureTemplateField, get_path_dict
 from vmngclient.api.templates.feature_template_payload import FeatureTemplatePayload
 from vmngclient.api.templates.models.cisco_aaa_model import CiscoAAAModel
-from vmngclient.dataclasses import Device, DeviceTemplateInfo, FeatureTemplateInfo, TemplateInfo
+from vmngclient.api.templates.models.omp_vsmart_model import OMPvSmart
+from vmngclient.api.templates.models.security_vsmart_model import SecurityvSmart
+from vmngclient.dataclasses import Device, DeviceTemplateInfo, FeatureTemplateInfo, FeatureTemplatesTypes, TemplateInfo
 from vmngclient.exceptions import AlreadyExistsError, AttachedError, TemplateNotFoundError
+from vmngclient.response import vManageResponse
 from vmngclient.typed_list import DataSequence
+from vmngclient.utils.device_model import DeviceModel
 from vmngclient.utils.template_type import TemplateType
 
 if TYPE_CHECKING:
     from vmngclient.session import vManageSession
 
 logger = logging.getLogger(__name__)
 
 
+class DeviceModelError(Exception):
+    """Used when unsupported device model used in template."""
+
+    def __init__(self, template, device_models):
+        self.message = f"Provided template type '{template.type}' not available for device models: {device_models}"
+        super().__init__(self.message)
+
+
 class DeviceTemplateFeature(Enum):
     LAWFUL_INTERCEPTION = "lawful-interception"
     CLOUD_DOCK = "cloud-dock"
     NETWORK_DESIGN = "network-design"
     VMANAGE_DEFAULT = "vmanage-default"
     ALL = "all"
 
@@ -314,14 +326,43 @@
                 logger.info(f"Template with name: {name} - deleted.")
                 return response.ok
             logger.warning(f"Template: {template} is attached to device - cannot be deleted.")
             raise AttachedError(template.name)
         return True
 
     @overload
+    def edit(self, template: FeatureTemplate) -> Any:
+        ...
+
+    @overload
+    def edit(self, template: CLITemplate) -> Any:
+        ...
+
+    def edit(self, template):
+        template_info = self.get(template).filter(name=template.name).single_or_default()
+        if not template_info:
+            raise TemplateNotFoundError(f"Template with name [{template.name}] does not exists.")
+
+        if isinstance(template, FeatureTemplate):
+            return self._edit_feature_template(template, template_info)
+
+        raise NotImplementedError()
+
+    def _edit_feature_template(self, template: FeatureTemplate, data: FeatureTemplateInfo) -> vManageResponse:
+        if self.is_created_by_generator(template):
+            debug = False
+            schema = self.get_feature_template_schema(template, debug)
+            payload = self.generate_feature_template_payload(template, schema, debug).dict(by_alias=True)
+        else:
+            payload = json.loads(template.generate_payload(self.session))
+
+        response = self.session.put(f"/dataservice/template/feature/{data.id}", json=payload)
+        return response
+
+    @overload
     def create(self, template: FeatureTemplate) -> str:
         ...
 
     @overload
     def create(self, template: DeviceTemplate) -> str:
         ...
 
@@ -365,15 +406,14 @@
         payload = template.generate_payload(self.session)
         response = self.session.post("/dataservice/template/feature", json=json.loads(payload))
         template_id = response.json()["templateId"]
 
         return template_id
 
     def _create_cli_template(self, template: CLITemplate) -> str:
-
         payload = template.generate_payload()
         response = self.session.post("/dataservice/template/device/cli/", json=payload)
         template_id = response.json()["templateId"]
 
         return template_id
 
     def _create_device_template(self, device_template: DeviceTemplate) -> str:
@@ -414,15 +454,19 @@
         return response.text
 
     def is_created_by_generator(self, template: FeatureTemplate) -> bool:
         """Checks if template is created by generator
 
         Method will be deleted if every template's payload will be generated dynamically.
         """
-        ported_templates = (CiscoAAAModel,)
+        ported_templates = (
+            CiscoAAAModel,
+            OMPvSmart,
+            SecurityvSmart,
+        )
 
         return isinstance(template, ported_templates)
 
     def get_feature_template_schema(self, template: FeatureTemplate, debug: bool = False) -> Any:
         endpoint = f"/dataservice/template/feature/types/definition/{template.type}/15.0.0"
         schema = self.session.get(url=endpoint).json()
 
@@ -433,28 +477,28 @@
         return schema
 
     def create_by_generator(self, template: FeatureTemplate, debug: bool) -> str:
         schema = self.get_feature_template_schema(template, debug)
         payload = self.generate_feature_template_payload(template, schema, debug)
 
         endpoint = "/dataservice/template/feature"
-        response = self.session.post(endpoint, json=payload.dict(by_alias=True))
+        response = self.session.post(endpoint, json=payload.dict(by_alias=True, exclude_none=True))
 
         return response.json()["templateId"]
 
     def generate_feature_template_payload(
         self, template: FeatureTemplate, schema: Any, debug: bool = False
     ) -> FeatureTemplatePayload:
         payload = FeatureTemplatePayload(
             name=template.name,
             description=template.description,
             template_type=template.type,
-            device_types=["vedge-C8000V"],  # TODO
+            device_types=["omp-vsmart"],  # TODO
             definition={},
-        )
+        )  # type: ignore
 
         fr_template_fields = [FeatureTemplateField(**field) for field in schema["fields"]]  # TODO
         payload.definition.update(get_path_dict([field.dataPath for field in fr_template_fields]))
 
         for field in fr_template_fields:
             payload.definition.update(field.data_path(output={}))
 
@@ -471,14 +515,39 @@
 
         if debug:
             with open(f"payload_{template.type}.json", "w") as f:
                 f.write(json.dumps(payload.dict(by_alias=True), indent=4))
 
         return payload
 
+    def validate_device_model(self, template: FeatureTemplate) -> bool:
+        """Verify if selected template can be used with provided device model"""
+
+        template_type = self._get_feature_template_types().filter(name=template.type).single_or_default()
+
+        available_devices_for_template = [device["name"] for device in template_type.device_models]
+
+        provided_device_models = [
+            dev_mod.value if type(dev_mod) is DeviceModel else dev_mod for dev_mod in template.device_models
+        ]
+
+        if not all(dev in available_devices_for_template for dev in provided_device_models):
+            logger.debug(f"Available devices for template '{template.type}': {available_devices_for_template}")
+            raise DeviceModelError(template, provided_device_models)
+        return True
+
+    def _get_feature_template_types(self, type: str = "all") -> DataSequence[FeatureTemplatesTypes]:
+        """Gets list off all templates and devices associated with these templates"""
+
+        endpoint = "/dataservice/template/feature/types"
+        params = {"type": type}
+        response = self.session.get(endpoint, params=params)
+
+        return response.dataseq(FeatureTemplatesTypes)
+
     def template_validation(self, id: str, device: Device) -> str:
         """Checking the template of the configuration on the machine.
 
         Args:
             id (str): template id to check.
             device (Device): The device on which the configuration is to be validate.
```

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/__init__.py` & `vmngclient-0.9.1/vmngclient/api/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/cli_template.py` & `vmngclient-0.9.1/vmngclient/api/templates/cli_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,16 @@
         Args:
             session: logged in API client session
             device: The device from which load config.
 
         Returns:
             CiscoConfParse: A working configuration on the machine.
         """
-        endpoint = f"/dataservice/template/config/running/{device.uuid}"
+        encoded_uuid = device.uuid.replace("/", "%2F")
+        endpoint = f"/dataservice/template/config/running/{encoded_uuid}"
         config = session.get_json(endpoint)
         self.config = CiscoConfParse(config["config"].splitlines())
         logger.debug(f"Template loaded from {device.hostname}.")
         return self.config
 
     def generate_payload(self) -> dict:
         config_str = "\n".join(self.config.ioscfg)
```

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/device_template/device_template.py` & `vmngclient-0.9.1/vmngclient/api/templates/device_template/device_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import logging
 from pathlib import Path
 from typing import Final, List
 
 from jinja2 import DebugUndefined, Environment, FileSystemLoader, meta  # type: ignore
-from pydantic import BaseModel, validator  # type: ignore
+from pydantic import BaseModel, validator
 
 logger = logging.getLogger(__name__)
 
 
 class GeneralTemplate(BaseModel):
     class Config:
         arbitrary_types_allowed = True
```

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/feature_template.py` & `vmngclient-0.9.1/vmngclient/api/templates/feature_template.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, List
 
 from jinja2 import DebugUndefined, Environment, FileSystemLoader, meta  # type: ignore
-from pydantic import BaseModel  # type: ignore
+from pydantic import BaseModel
+
+from vmngclient.utils.device_model import DeviceModel
 
 if TYPE_CHECKING:
     from vmngclient.session import vManageSession
 
 
 class FeatureTemplate(BaseModel, ABC):
     name: str
     description: str
+    device_models: List[DeviceModel]
 
     def generate_payload(self, session: vManageSession) -> str:
         env = Environment(
             loader=FileSystemLoader(self.payload_path.parent),
             trim_blocks=True,
             lstrip_blocks=True,
             undefined=DebugUndefined,
```

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/feature_template_field.py` & `vmngclient-0.9.1/vmngclient/api/templates/feature_template_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from enum import Enum
 from typing import Any, Dict, List
 
-from pydantic import BaseModel  # type: ignore
+from pydantic import BaseModel
 
 
 class FeatureTemplateOptionType(Enum):
     CONSTANT = "constant"
     VARIABLE = "variable"
     IGNORE = "ignore"
     NOT_IGNORE = "notIgnore"
@@ -52,15 +52,14 @@
     dataPath: List[str] = []
     objectType: FeatureTemplateObjectType
     dataType: dict = {}
     primaryKeys: List[str] = []
     children: List[FeatureTemplateField] = []
 
     def data_path(self, output):
-
         for child in self.children:
             child.data_path(output)
         output.update(get_path_dict([t.dataPath for t in self.children]))
 
         return output
 
     # value must be JSON serializable, return JSON serializable dict
```

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/feature_template_payload.py` & `vmngclient-0.9.1/vmngclient/api/templates/feature_template_payload.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from pydantic import BaseModel, Field  # type: ignore
+from pydantic import BaseModel, Field
 
 
 class FeatureTemplatePayload(BaseModel):
     class Config:
         allow_population_by_field_name = True
 
     name: str = Field(alias="templateName")
```

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/models/cisco_aaa_model.py` & `vmngclient-0.9.1/vmngclient/api/templates/models/cisco_aaa_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 from pathlib import Path
 from typing import ClassVar, List, Optional
 
-from pydantic import BaseModel, Field  # type: ignore
+from pydantic import BaseModel, Field
 
 from vmngclient.api.templates.feature_template import FeatureTemplate
 
 
 class User(BaseModel):
     name: str
     password: str
```

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/aaa_model.py` & `vmngclient-0.9.1/vmngclient/api/templates/payloads/aaa/aaa_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 
 
 class AAAModel(FeatureTemplate):
     class Config:
         arbitrary_types_allowed = True
 
     payload_path: ClassVar[Path] = Path(__file__).parent / "feature" / "aaa.json.j2"
+    type: ClassVar[str] = "aaa"  # AAA
 
     auth_order: List[AuthenticationOrder]
     auth_fallback: bool
     auth_disable_audit_logs: bool
     auth_admin_order: bool
     auth_disable_netconf_logs: bool
     auth_radius_servers: List[str] = []
```

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/feature/aaa.json.j2` & `vmngclient-0.9.1/vmngclient/api/templates/payloads/aaa/feature/aaa.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/feature/accounting.json.j2` & `vmngclient-0.9.1/vmngclient/api/templates/payloads/aaa/feature/accounting.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/feature/radius.json.j2` & `vmngclient-0.9.1/vmngclient/api/templates/payloads/aaa/feature/radius.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/feature/tacacs.json.j2` & `vmngclient-0.9.1/vmngclient/api/templates/payloads/aaa/feature/tacacs.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/payloads/aaa/feature/user.json.j2` & `vmngclient-0.9.1/vmngclient/api/templates/payloads/aaa/feature/user.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_system/feature/cisco_system.json.j2` & `vmngclient-0.9.1/vmngclient/api/templates/payloads/cisco_system/feature/cisco_system.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/cisco_vpn_model.py` & `vmngclient-0.9.1/vmngclient/api/templates/payloads/cisco_vpn/cisco_vpn_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 from enum import Enum
 from pathlib import Path
 from typing import TYPE_CHECKING, ClassVar, List, Optional
 
 from attr import define, field  # type: ignore
-from pydantic import validator  # type: ignore
+from pydantic import validator
 
 from vmngclient.api.templates.feature_template import FeatureTemplate
 from vmngclient.api.templates.payloads.aaa.aaa_model import VpnType
 
 if TYPE_CHECKING:
     from vmngclient.session import vManageSession
 
@@ -54,14 +54,15 @@
 class IPv6Route:
     prefixv6: str
     next_hopv6: list[NextHop]
     gatewayv6: GatewayType = field(default=GatewayType.NEXT_HOP)
 
 
 class CiscoVPNModel(FeatureTemplate):
+    type: ClassVar[str] = "cisco_vpn"  # Cisco VPN
     payload_path: ClassVar[Path] = Path(__file__).parent / "feature/cisco_vpn.json.j2"
     tenant_vpn: Optional[int]
     tenant_org_name: Optional[str]
     vpn_id: int
     dns: Optional[DNS] = None
     mapping: List[Mapping] = []
     ipv4route: List[IPv4Route] = []
```

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2` & `vmngclient-0.9.1/vmngclient/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/feature/dns.json.j2` & `vmngclient-0.9.1/vmngclient/api/templates/payloads/cisco_vpn/feature/dns.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2` & `vmngclient-0.9.1/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2` & `vmngclient-0.9.1/vmngclient/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn/feature/mapping.json.j2` & `vmngclient-0.9.1/vmngclient/api/templates/payloads/cisco_vpn/feature/mapping.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/cisco_vpn_interface_ethernet_model.py` & `vmngclient-0.9.1/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/cisco_vpn_interface_ethernet_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,14 +90,15 @@
     stun: Optional[bool] = None
     https: Optional[bool] = None
     snmp: Optional[bool] = None
     encapsulation: list[Encapsulation] = []
 
 
 class CiscoVpnInterfaceEthernetModel(FeatureTemplate):
+    type: ClassVar[str] = "cisco_vpn_interface"  # Cisco VPN Interface Ethernet
     payload_path: ClassVar[Path] = Path(__file__).parent / "feature/cisco_vpn_interface_ethernet.json.j2"
     interface_name: InterfaceName
     shutdown: Optional[bool]
     type_address: TypeAddress = TypeAddress.STATIC
     ip: Optional[str]
     tunnel: Optional[Tunnel]
     mtu: Optional[int]
```

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/cisco_vpn_interface_ethernet.json.j2` & `vmngclient-0.9.1/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/cisco_vpn_interface_ethernet.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/tunnel.json.j2` & `vmngclient-0.9.1/vmngclient/api/templates/payloads/cisco_vpn_interface_ethernet/feature/tunnel.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/payloads/tenant/tenant.json.j2` & `vmngclient-0.9.1/vmngclient/api/templates/payloads/tenant/tenant.json.j2`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/templates/payloads/tenant/tenant_model.py` & `vmngclient-0.9.1/vmngclient/api/templates/payloads/tenant/tenant_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from functools import lru_cache
 from pathlib import Path
 from typing import TYPE_CHECKING, ClassVar, List
 
-from pydantic import BaseModel  # type: ignore
+from pydantic import BaseModel
 
 from vmngclient.api.templates.feature_template import FeatureTemplate
 from vmngclient.api.tenant_api import TenantsAPI
 from vmngclient.dataclasses import TenantInfo, TierInfo
 
 if TYPE_CHECKING:
     from vmngclient.session import vManageSession
@@ -35,14 +35,15 @@
     tier_name: str
 
 
 class TenantModel(FeatureTemplate):
     class Config:
         arbitrary_types_allowed = True
 
+    type: ClassVar[str] = "tenant"  # Tenant
     payload_path: ClassVar[Path] = Path(__file__).parent / "tenant.json.j2"
 
     tenants: List[Tenant] = []
 
     def generate_payload(self, session: vManageSession) -> str:
         tenants_api = TenantsAPI(session)
```

### Comparing `vmngclient-0.8.2/vmngclient/api/tenant_api.py` & `vmngclient-0.9.1/vmngclient/api/tenant_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/tenant_backup_restore_api.py` & `vmngclient-0.9.1/vmngclient/api/tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/api/versions_utils.py` & `vmngclient-0.9.1/vmngclient/api/versions_utils.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/dataclasses.py` & `vmngclient-0.9.1/vmngclient/dataclasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import datetime as dt
 from typing import List, Optional
 
 from attr import define, field  # type: ignore
+from pydantic import BaseModel, Field
 
 from vmngclient.exceptions import RetrieveIntervalOutOfRange
 from vmngclient.utils.alarm_status import Severity
 from vmngclient.utils.certificate_status import ValidityPeriod
 from vmngclient.utils.creation_tools import FIELD_NAME, asdict, convert_attributes
 from vmngclient.utils.personality import Personality
 from vmngclient.utils.reachability import Reachability
@@ -40,15 +41,14 @@
     size: int
     state: str
     token_id: Optional[str] = field(default=None, metadata={FIELD_NAME: "requestTokenId"})
 
 
 @define(frozen=True, field_transformer=convert_attributes)
 class AlarmData(DataclassBase):
-
     component: Optional[str] = field(default=None)
     active: Optional[bool] = field(default=None)
     severity: Optional[Severity] = field(converter=Severity, default=None)
     name: Optional[str] = field(default=None, metadata={FIELD_NAME: "type"})
     system_ip: Optional[str] = field(default=None, metadata={FIELD_NAME: "system-ip"})
     hostname: Optional[str] = field(default=None, metadata={FIELD_NAME: "host-name"})
     site_id: Optional[str] = field(default=None, metadata={FIELD_NAME: "site-id"})
@@ -413,27 +413,25 @@
     """
 
     accounting: bool = field(metadata={FIELD_NAME: "accounting"})
     admin_auth_order: bool = field(metadata={FIELD_NAME: "adminAuthOrder"})
     audit_disable: bool = field(metadata={FIELD_NAME: "auditDisable"})
     auth_fallback: bool = field(metadata={FIELD_NAME: "authFallback"})
     auth_order: List[str] = field(metadata={FIELD_NAME: "authOrder"})
-    radius_servers: str = field(metadata={FIELD_NAME: "radiusServers"})
 
 
 @define(frozen=True)
 class RadiusServer(DataclassBase):
     """
     Provider-Tenant -> Tenant -> Administration -> Manage users -> Remote AAA -> RADIUS
     """
 
     address: str = field(metadata={FIELD_NAME: "address"})
     auth_port: int = field(metadata={FIELD_NAME: "authPort"})
     acct_port: int = field(metadata={FIELD_NAME: "acctPort"})
-    tag: str = field(metadata={FIELD_NAME: "tag"})
     vpn: int = field(metadata={FIELD_NAME: "vpn"})
     vpn_ip_subnet: str = field(metadata={FIELD_NAME: "vpnIpSubnet"})
     key: str = field(metadata={FIELD_NAME: "key"})
     secret_key: str = field(metadata={FIELD_NAME: "secretKey"})
     priority: int = field(metadata={FIELD_NAME: "priority"})
 
 
@@ -476,14 +474,27 @@
 
 @define
 class SoftwareInstallTimeout(DataclassBase):
     download_timeout_min: int = field(converter=str, metadata={FIELD_NAME: "downloadTimeoutInMin"})
     activate_timeout_min: int = field(converter=str, metadata={FIELD_NAME: "activateTimeoutInMin"})
 
 
+class FeatureTemplatesTypes(BaseModel):
+    parent: str
+    default: str
+    display_name: str = Field(alias="displayName")
+    name: str
+    type_class: str = Field(alias="typeClass")
+    description: str
+    write_permission: bool
+    read_permission: bool
+    helper_type: List[str] = Field(default=[], alias="helperType")
+    device_models: List[dict] = Field(default=[], alias="deviceModels")
+
+
 @define
 class ResourcePoolData(DataclassBase):
     """Endpoint: /resourcepool/resource/vpn"""
 
     tenant_id: str = field(metadata={FIELD_NAME: "tenantId"})
     tenant_vpn: int = field(metadata={FIELD_NAME: "tenantVpn"})
     device_vpn: Optional[int] = field(default=None, metadata={FIELD_NAME: "deviceVpn"})
```

### Comparing `vmngclient-0.8.2/vmngclient/logging.conf` & `vmngclient-0.9.1/vmngclient/logging.conf`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/response.py` & `vmngclient-0.9.1/vmngclient/response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from functools import wraps
 from pprint import pformat
 from typing import Any, Callable, Optional, Sequence, Type, TypeVar, Union, cast
 
-from attr import define  # type: ignore
+from pydantic import BaseModel
 from requests import PreparedRequest, Request, Response
 from requests.exceptions import JSONDecodeError
 
 from vmngclient import with_proc_info_header
-from vmngclient.dataclasses import DataclassBase
+from vmngclient.exceptions import CookieNotValidError
 from vmngclient.typed_list import DataSequence
 from vmngclient.utils.creation_tools import create_dataclass
 
 T = TypeVar("T")
 
 
-@define(frozen=True)
-class ErrorInfo(DataclassBase):
+class ErrorInfo(BaseModel):
     message: str
     details: str
     code: str
 
 
 def response_debug(response: Optional[Response], request: Union[Request, PreparedRequest, None]) -> str:
     """Returns human readable string containing Request-Response contents (helpful for debugging).
@@ -107,14 +106,16 @@
             self.headers = json.get("headers", None)
 
 
 class vManageResponse(Response):
     """Extends Response object with methods specific to vManage"""
 
     def __init__(self, response: Response):
+        if response.headers.get("set-cookie"):
+            raise CookieNotValidError("Session cookie is not valid.")
         self.__dict__.update(response.__dict__)
         try:
             self.payload = JsonPayload(response.json())
         except JSONDecodeError:
             self.payload = JsonPayload()
 
     def info(self, history: bool = False) -> str:
@@ -125,33 +126,63 @@
         Returns:
             str
         """
         if history:
             return response_history_debug(self, None)
         return response_debug(self, None)
 
-    def dataseq(self, cls: Type[T]) -> DataSequence[T]:
-        """Returns data contents from JSON payload deserialized to Sequence of Dataclass instances
+    def dataseq(self, cls: Type[T], sourcekey: Optional[str] = "data") -> DataSequence[T]:
+        """Returns data contents from JSON payload parsed as DataSequence of Dataclass/BaseModel instances
         Args:
-            cls: Dataclass subtype (eg. Devices)
+            cls: Dataclass/BaseModel subtype (eg. Devices)
+            sourcekey: name of the JSON key from response payload to be parsed. If None whole JSON payload will be used
 
         Returns:
-            DataSequence of given type,
+            DataSequence[T] of given type T which is subclassing from Dataclass/BaseModel,
             in case JSON payload was containing a single Object - sequence with one element is returned
         """
-        data = self.payload.data
+        if sourcekey is None:
+            data = self.payload.json
+        else:
+            data = self.payload.json.get(sourcekey)
+
         if isinstance(data, Sequence):
             sequence = data
         else:
             sequence = [cast(dict, data)]
+
+        if issubclass(cls, BaseModel):
+            return DataSequence(cls, [cls.parse_obj(item) for item in sequence])  # type: ignore
         return DataSequence(cls, [create_dataclass(cls, item) for item in sequence])
 
+    def dataobj(self, cls: Type[T], sourcekey: Optional[str] = "data") -> T:
+        """Returns data contents from JSON payload parsed as Dataclass/BaseModel instance
+        Args:
+            cls: Dataclass/BaseModel subtype (eg. Devices)
+            sourcekey: name of the JSON key from response payload to be parsed. If None whole JSON payload will be used
+
+        Returns:
+            Object of given type T which is subclassing from Dataclass/BaseModel,
+
+        """
+        if sourcekey is None:
+            data = self.payload.json
+        else:
+            data = self.payload.json.get(sourcekey)
+
+        if issubclass(cls, BaseModel):
+            return cls.parse_obj(data)  # type: ignore
+        return create_dataclass(cls, data)
+
     def get_error_info(self) -> ErrorInfo:
         """Returns error information from JSON payload"""
-        return create_dataclass(ErrorInfo, cast(dict, self.payload.error))
+
+        if self.payload.error is None:
+            raise TypeError("Payload error should not be None.")
+        return ErrorInfo(**self.payload.error)
 
 
 def with_vmanage_response(method: Callable[[Any], Response]) -> Callable[[Any], vManageResponse]:
     @wraps(method)
     def wrapper(*args, **kwargs) -> vManageResponse:
         return vManageResponse(method(*args, **kwargs))
```

### Comparing `vmngclient-0.8.2/vmngclient/session.py` & `vmngclient-0.9.1/vmngclient/session.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,52 @@
 from __future__ import annotations
 
 import logging
 import time
-from enum import Enum, auto
+from enum import Enum
 from pathlib import Path
 from typing import Any, Callable, ClassVar, Dict, List, Optional, Union
 from urllib.parse import urljoin
 
+from packaging.version import Version  # type: ignore
 from requests import PreparedRequest, Request, Response, Session, head
 from requests.auth import AuthBase
 from requests.exceptions import ConnectionError, HTTPError, RequestException
 from tenacity import retry, retry_if_exception_type, stop_after_attempt, wait_fixed  # type: ignore
 
 from vmngclient.api.api_containter import APIContainter
-from vmngclient.exceptions import InvalidOperationError
-from vmngclient.response import response_history_debug, vManageResponse
+from vmngclient.exceptions import (
+    AuthenticationError,
+    CookieNotValidError,
+    InvalidOperationError,
+    SessionNotCreatedError,
+    TenantSubdomainNotFound,
+    vManageClientError,
+)
+from vmngclient.primitives.client import AboutInfo, ServerInfo
+from vmngclient.primitives.primitive_container import APIPrimitiveContainter
+from vmngclient.response import ErrorInfo, response_history_debug, vManageResponse
+from vmngclient.utils.session_type import SessionType
 from vmngclient.vmanage_auth import vManageAuth
 
 JSON = Union[Dict[str, "JSON"], List["JSON"], str, int, float, bool, None]
 
 
-class SessionType(Enum):
-    PROVIDER = auto()
-    TENANT = auto()
-    PROVIDER_AS_TENANT = auto()
-    NOT_DEFINED = auto()
+class vManageBadRequestError(vManageClientError):
+    """Indicates that vManage returned HTTP status code 400.
+
+    A 400 Bad Request response status code indicates that the server
+    could not understand the request due to invalid syntax,
+    malformed request message, or missing request parameters.
+    """
+
+    def __init__(self, error_info: Optional[ErrorInfo], response: vManageResponse):
+        self.response = response
+        self.info = error_info
+        super().__init__(error_info)
 
 
 class UserMode(Enum):
     PROVIDER = "provider"
     TENANT = "tenant"
     NOT_RECOGNIZED = "not recognized"
     NOT_FOUND = "not found"
@@ -37,33 +55,29 @@
 class ViewMode(Enum):
     PROVIDER = "provider"
     TENANT = "tenant"
     NOT_RECOGNIZED = "not recognized"
     NOT_FOUND = "not found"
 
 
-class SessionNotCreatedError(Exception):
-    pass
-
-
 def create_vManageSession(
     url: str,
     username: str,
     password: str,
     port: Optional[int] = None,
     subdomain: Optional[str] = None,
     logger: Optional[logging.Logger] = None,
 ) -> vManageSession:
     """Factory function that creates session object based on provided arguments.
 
     Args:
         url (str): IP address or domain name
-        port (int): port
         username (str): username
         password (str): password
+        port (int): port
         subdomain: subdomain specifying to which view switch when creating provider as a tenant session,
             works only on provider user mode
         logger: logger for logging API requests
 
     Returns:
         Session object
 
@@ -78,30 +92,30 @@
         tenant_id = session.get_tenant_id()
         vsession_id = session.get_virtual_session_id(tenant_id)
         session.headers.update({"VSessionId": vsession_id})
 
     try:
         server_info = session.server()
     except InvalidOperationError:
-        server_info = {}
+        server_info = ServerInfo.parse_obj({})
 
-    session.server_name = server_info.get("server")
+    session.server_name = server_info.server
     session.on_session_create_hook()
 
     try:
-        user_mode = UserMode(server_info.get("userMode", "not found"))
+        user_mode = UserMode(server_info.user_mode or "not found")
     except ValueError:
         user_mode = UserMode.NOT_RECOGNIZED
-        session.logger.warning(f"Unrecognized user mode is: '{server_info.get('userMode')}'")
+        session.logger.warning(f"Unrecognized user mode is: '{server_info.user_mode}'")
 
     try:
-        view_mode = ViewMode(server_info.get("viewMode", "not found"))
+        view_mode = ViewMode(server_info.view_mode or "not found")
     except ValueError:
         view_mode = ViewMode.NOT_RECOGNIZED
-        session.logger.warning(f"Unrecognized user mode is: '{server_info.get('viewMode')}'")
+        session.logger.warning(f"Unrecognized user mode is: '{server_info.view_mode}'")
 
     if user_mode is UserMode.TENANT and not subdomain and view_mode is ViewMode.TENANT:
         session._session_type = SessionType.TENANT
     elif user_mode is UserMode.PROVIDER and not subdomain and view_mode is ViewMode.PROVIDER:
         session._session_type = SessionType.PROVIDER
     elif user_mode is UserMode.PROVIDER and view_mode is ViewMode.TENANT:
         session._session_type = SessionType.PROVIDER_AS_TENANT
@@ -110,15 +124,17 @@
             f"Session not created. Subdomain {subdomain} passed to tenant session, "
             "cannot switch to tenant from tenant user mode."
         )
     else:
         session._session_type = SessionType.NOT_DEFINED
         session.logger.warning(f"Session created with {user_mode} and {view_mode}.")
 
-    session.logger.info(f"Logged as {username}. The session type is {session.session_type}")
+    session.logger.info(
+        f"Logged to vManage({session.platform_version}) as {username}. The session type is {session.session_type}"
+    )
     return session
 
 
 class vManageResponseAdapter(Session):
     def request(self, method, url, *args, **kwargs) -> vManageResponse:
         return vManageResponse(super().request(method, url, *args, **kwargs))
 
@@ -141,14 +157,18 @@
     Defines methods and handles session connectivity available for provider, provider as tenant, and tenant.
 
     Args:
         url: IP address or domain name, i.e. '10.0.1.200' or 'example.com'
         port: port
         username: username
         password: password
+
+    Attributes:
+        enable_relogin (bool): defaults to True, in case that session is not properly logged-in, session will try to
+            relogin and try the same request again
     """
 
     on_session_create_hook: ClassVar[Callable[[vManageSession], Any]] = lambda *args: None
 
     def __init__(
         self,
         url: str,
@@ -163,43 +183,62 @@
         self.port = port
         self.base_url = self.__create_base_url()
         self.username = username
         self.password = password
         self.subdomain = subdomain
 
         self._session_type = SessionType.NOT_DEFINED
-        self.server_name = None
+        self.server_name: Optional[str] = None
         self.logger = logging.getLogger(__name__)
+        self.enable_relogin: bool = True
+        self.__second_relogin_try: bool = False
         self.response_trace: Callable[
             [Optional[Response], Union[Request, PreparedRequest, None]], str
         ] = response_history_debug
         super(vManageSession, self).__init__()
         self.__prepare_session(verify, auth)
 
         self.api = APIContainter(self)
+        self.primitives = APIPrimitiveContainter(self)
+        self._platform_version: Version
+        self._api_version: Version
 
     def request(self, method, url, *args, **kwargs) -> vManageResponse:
         full_url = self.get_full_url(url)
         try:
             response = super(vManageSession, self).request(method, full_url, *args, **kwargs)
             self.logger.debug(self.response_trace(response, None))
         except RequestException as exception:
             self.logger.debug(self.response_trace(exception.response, exception.request))
             self.logger.error(exception)
             raise
+        except CookieNotValidError as exception:
+            if self.enable_relogin and not self.__second_relogin_try:
+                self.logger.warning(f"Loging to session again. Reason: '{str(exception)}'")
+                self.auth = vManageAuth(self.base_url, self.username, self.password, verify=False)
+                self.__second_relogin_try = True
+                return self.request(method, url, *args, **kwargs)
+            elif self.enable_relogin and self.__second_relogin_try:
+                raise AuthenticationError("Session is not properly logged in and relogin failed.")
+            else:
+                raise AuthenticationError("Session is not properly logged in and relogin is not enabled.")
+
+        self.__second_relogin_try = False
 
         if response.request.url and "passwordReset.html" in response.request.url:
             raise InvalidOperationError("Password must be changed to use this session.")
 
         try:
             response.raise_for_status()
         except HTTPError as error:
             self.logger.debug(error)
             if response.status_code == 403:
                 self.logger.info(f"User {self.username} is unauthorized for method {method} {full_url}")
+            elif response.status_code == 400:
+                raise vManageBadRequestError(response.get_error_info(), response)
             else:
                 raise error
         return response
 
     def get_full_url(self, url_path: str) -> str:
         """Returns base API url plus given url path."""
         return urljoin(self.base_url, url_path)
@@ -210,19 +249,21 @@
         Returns:
             str: Base url shared for every request.
         """
         if self.port:
             return f"https://{self.url}:{self.port}"
         return f"https://{self.url}"
 
-    def about(self) -> Dict:
-        return self.get_data(url="/dataservice/client/about")
+    def about(self) -> AboutInfo:
+        return self.primitives.client.about()
 
-    def server(self) -> Dict:
-        return self.get_data(url="/dataservice/client/server")
+    def server(self) -> ServerInfo:
+        server_info = self.primitives.client.server()
+        self.platform_version = server_info.platform_version
+        return server_info
 
     def get_data(self, url: str) -> Any:
         return self.get_json(url)["data"]
 
     def get_json(self, url: str) -> Any:
         response = self.get(url)
         return response.json()
@@ -282,17 +323,21 @@
 
     def get_tenant_id(self) -> str:
         """Gets tenant UUID for its subdomain.
 
         Returns:
             Tenant UUID.
         """
-        tenants = self.get_data(url="/dataservice/tenant")
-        tenant_id = [tenant.get("tenantId", None) for tenant in tenants if tenant["subDomain"] == self.subdomain][0]
-        return tenant_id
+        tenants = self.primitives.tenant_management.get_all_tenants()
+        tenant = tenants.filter(sub_domain=self.subdomain).single_or_default()
+
+        if not tenant:
+            raise TenantSubdomainNotFound(f"Tenant with sub-domain: {self.subdomain} not found")
+
+        return tenant.tenant_id
 
     def get_virtual_session_id(self, tenant_id: str) -> str:
         """Get VSessionId for a specific tenant
 
         Note: In a multitenant vManage system, this API is only available in the Provider view.
 
         Args:
@@ -316,14 +361,27 @@
         else:
             return True
 
     @property
     def session_type(self) -> SessionType:
         return self._session_type
 
+    @property
+    def platform_version(self) -> Version:
+        return self._platform_version
+
+    @platform_version.setter
+    def platform_version(self, version: Version):
+        self._platform_version = version
+        self._api_version = Version(f"{version.major}.{version.minor}")
+
+    @property
+    def api_version(self) -> Version:
+        return self._api_version
+
     def __str__(self) -> str:
         return f"{self.username}@{self.base_url}"
 
     def __repr__(self):
         return (
             f"{self.__class__.__name__}('{self.url}', '{self.username}', '{self.password}', port={self.port}, "
             f"subdomain='{self.subdomain}')"
```

### Comparing `vmngclient-0.8.2/vmngclient/tests/test_admin_tech_api.py` & `vmngclient-0.9.1/vmngclient/tests/test_admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/tests/test_administration.py` & `vmngclient-0.9.1/vmngclient/tests/test_administration.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,30 @@
+# type: ignore
 import unittest
 from unittest.mock import patch
 
 from attr.exceptions import NotAnAttrsClassError
 from parameterized import parameterized  # type: ignore
 
-from vmngclient.api.administration import (
-    AdministrationSettingsAPI,
-    ClusterManagementAPI,
-    UserAlreadyExistsError,
-    UserDoesNotExists,
-    UsersAPI,
-)
+from vmngclient.api.administration import AdministrationSettingsAPI, ClusterManagementAPI, UsersAPI
 from vmngclient.dataclasses import (
     Certificate,
     CloudConnectorData,
     CloudServicesSettings,
     Organization,
     Password,
     ServiceConfigurationData,
     User,
     Vbond,
 )
-from vmngclient.exceptions import InvalidOperationError
+from vmngclient.exceptions import AlreadyExistsError, InvalidOperationError
 from vmngclient.utils.certificate_status import ValidityPeriod
 from vmngclient.utils.creation_tools import create_dataclass
 
-password_dataclass = Password("old_password_123", "new_password_123")
+password_dataclass = Password(old_password="old_password_123", new_password="new_password_123")
 certificate_dataclass = Certificate("cert", "Name", "Surname", "name@sur.name", ValidityPeriod.ONE_YEAR, 10)
 vbond_dataclass = Vbond("1.1.1.1", 1234)
 organization_dataclass = Organization("My org name", 1)
 
 
 class TestUsersAPI(unittest.TestCase):
     def setUp(self) -> None:
@@ -78,55 +73,43 @@
     @patch("requests.Response")
     def test_create_user(self, status_code, expected_outcome, mock_response, mock_session):
         # Arrange
         mock_session.get_data.return_value = [self.users[1]]
         mock_session.post.return_value = mock_response
         mock_response.status_code = status_code
         # Act
-        answer = UsersAPI(mock_session).create_user(self.user_dataclass[0])
+        answer = UsersAPI(mock_session).create(self.user_dataclass[0])
         # Assert
         self.assertEqual(answer, expected_outcome)
 
     @patch("vmngclient.session.vManageSession")
     def test_create_user_existing(self, mock_session):
         # Arrange
         mock_session.get_data.return_value = self.users
 
         # Act
         def answer():
-            UsersAPI(mock_session).create_user(self.user_dataclass[0])
+            UsersAPI(mock_session).create(self.user_dataclass[0])
 
         # Assert
-        self.assertRaises(UserAlreadyExistsError, answer)
+        self.assertRaises(AlreadyExistsError, answer)
 
     @parameterized.expand([[200, True], [400, False]])
     @patch("vmngclient.session.vManageSession")
     @patch("requests.Response")
     def test_delete_user(self, status_code, expected_outcome, mock_response, mock_session):
         # Arrange
         mock_session.get_data.return_value = self.users
         mock_session.delete.return_value = mock_response
         mock_response.status_code = status_code
         # Act
         answer = UsersAPI(mock_session).delete_user("admin")
         # Assert
         self.assertEqual(answer, expected_outcome)
 
-    @patch("vmngclient.session.vManageSession")
-    def test_delete_user_not_existing(self, mock_session):
-        # Arrange
-        mock_session.get_data.return_value = [self.users[1]]
-
-        # Act
-        def answer():
-            UsersAPI(mock_session).delete_user("no_user")
-
-        # Assert
-        self.assertRaises(UserDoesNotExists, answer)
-
 
 class TestClusterManagementAPI(unittest.TestCase):
     def setUp(self) -> None:
         self.service_configuration = {
             "vmanageID": "1.1.1.1",
             "deviceIP": "1.1.1.2",
             "services": "none",
```

### Comparing `vmngclient-0.8.2/vmngclient/tests/test_alarms_api.py` & `vmngclient-0.9.1/vmngclient/tests/test_alarms_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/tests/test_cli_template.py` & `vmngclient-0.9.1/vmngclient/tests/test_cli_template.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/tests/test_creation_tools.py` & `vmngclient-0.9.1/vmngclient/tests/test_creation_tools.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/tests/test_device_action_api.py` & `vmngclient-0.9.1/vmngclient/tests/test_device_action_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/tests/test_devices_api.py` & `vmngclient-0.9.1/vmngclient/tests/test_devices_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/tests/test_feature_template_field.py` & `vmngclient-0.9.1/vmngclient/tests/test_feature_template_field.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/tests/test_logs_api.py` & `vmngclient-0.9.1/vmngclient/tests/test_logs_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/tests/test_mtt_aaa_api.py` & `vmngclient-0.9.1/vmngclient/tests/test_mtt_aaa_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,21 @@
     def setUp(self) -> None:
         self.aaa = {
             "authOrder": ["radius", "tacacs", "local"],
             "authFallback": True,
             "adminAuthOrder": True,
             "auditDisable": False,
             "accounting": False,
-            "radiusServers": "server1",
         }
         self.p_aaa = {
             "authOrder": ["radius", "local"],
             "authFallback": True,
             "adminAuthOrder": True,
             "auditDisable": True,
             "accounting": True,
-            "radiusServers": "serverX",
         }
         self.aaa_dataclass = create_dataclass(TenantAAA, self.aaa)
         self.p_aaa_dataclass = create_dataclass(TenantAAA, self.p_aaa)
 
     @parameterized.expand([[200, True], [400, False]])
     @patch("vmngclient.session.Session")
     @patch("requests.Response")
@@ -39,16 +37,16 @@
         mock_response.status_code = status_code
         # Act
         answer = TenantAaaAPI(mock_session).del_aaa()
         # Assert
         self.assertEqual(answer, expected_outcome)
 
     @parameterized.expand([[200, True], [400, False]])
-    @patch("vmngclient.session.Session")
     @patch("requests.Response")
+    @patch("vmngclient.session.Session")
     def test_add_aaa(self, status_code, expected_outcome, mock_session, mock_response):
         # Arrange
         mock_session.get_data.return_value = self.aaa
         mock_session.post.return_value = mock_response
         mock_response.status_code = status_code
         # Act
         answer = TenantAaaAPI(mock_session).add_aaa(self.aaa_dataclass)
@@ -80,62 +78,57 @@
 class TestRadiusAPI(unittest.TestCase):
     def setUp(self) -> None:
         self.radius_server_list = [
             {
                 "address": "10.0.5.143",
                 "authPort": 1812,
                 "acctPort": 1813,
-                "tag": "test",
                 "vpn": 1,
                 "vpnIpSubnet": "192.168.1.0/24",
                 "key": "testing",
                 "secretKey": "cisco123",
                 "priority": 1,
             },
             {
                 "address": "10.0.5.144",
                 "authPort": 1812,
                 "acctPort": 1813,
-                "tag": "test",
                 "vpn": 1,
                 "vpnIpSubnet": "192.168.1.0/24",
                 "key": "testing",
                 "secretKey": "cisco123",
                 "priority": 1,
             },
             {
                 "address": "10.0.5.145",
                 "authPort": 1812,
                 "acctPort": 1813,
-                "tag": "test",
                 "vpn": 1,
                 "vpnIpSubnet": "192.168.1.0/24",
                 "key": "testing",
                 "secretKey": "cisco123",
                 "priority": 1,
             },
         ]
 
         self.p_radius_server_list = [
             {
                 "address": "10.0.5.143",
                 "authPort": 1812,
                 "acctPort": 1813,
-                "tag": "test",
                 "vpn": 1,
                 "vpnIpSubnet": "192.168.1.0/24",
                 "key": "testing",
                 "secretKey": "cisco123",
                 "priority": 1,
             },
             {
                 "address": "10.0.5.144",
                 "authPort": 1812,
                 "acctPort": 1813,
-                "tag": "test",
                 "vpn": 1,
                 "vpnIpSubnet": "192.168.1.0/24",
                 "key": "testing",
                 "secretKey": "cisco123",
                 "priority": 1,
             },
         ]
```

### Comparing `vmngclient-0.8.2/vmngclient/tests/test_omp_api.py` & `vmngclient-0.9.1/vmngclient/tests/test_omp_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/tests/test_packet_capture.py` & `vmngclient-0.9.1/vmngclient/tests/test_packet_capture.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/tests/test_partition_manager_api.py` & `vmngclient-0.9.1/vmngclient/tests/test_partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/tests/test_session.py` & `vmngclient-0.9.1/vmngclient/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/tests/test_software_action_api.py` & `vmngclient-0.9.1/vmngclient/tests/test_software_action_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/tests/test_speed_test_api.py` & `vmngclient-0.9.1/vmngclient/tests/test_speed_test_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/tests/test_task_status_api.py` & `vmngclient-0.9.1/vmngclient/tests/test_task_status_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import unittest
 from unittest.mock import patch
 
 from vmngclient.api.task_status_api import RunningTaskData, SubTaskData, Task, TaskResult, TasksAPI, TasksData
-from vmngclient.exceptions import EmptyTaskResponseError, TaskNotRegisteredError
 
 
 class TestTaskStatusApi(unittest.TestCase):
     def setUp(self):
         sub_tasks_data = SubTaskData.parse_obj(
             {
                 "status": "Success",
@@ -99,36 +98,14 @@
         # Prepare mock data
         mock_session.get_data.return_value = self.action_data_time_out
 
         # Assert
         answer = Task(mock_session, "mock_action_id").wait_for_completed(1, 1).result
         self.assertEqual(answer, False)
 
-    @patch("vmngclient.api.task_status_api.sleep")
-    @patch.object(TasksAPI, "get_all_tasks")
-    @patch("vmngclient.session.vManageSession")
-    def test_raise_error_actionid_in_tasks_ids_data_dosnt_exists(self, mock_session, mock_get_tasks, mock_sleep):
-        # Arrange
-        mock_session.get_data.return_value = []
-        mock_get_tasks.return_value = TasksData.parse_obj(self.running_task_data_json)
-        # Act&Assert
-        self.assertRaises(EmptyTaskResponseError, Task(mock_session, "processId_1").wait_for_completed, 1, 1)
-
-    @patch("vmngclient.api.task_status_api.sleep")
-    @patch.object(TasksAPI, "get_all_tasks")
-    @patch("vmngclient.session.vManageSession")
-    def test_raise_TaskNotRegistered_error(self, mock_session, mock_get_tasks, mock_sleep):
-        # Arrange
-        mock_session.get_data.return_value = []
-        mock_get_tasks.return_value = TasksData.parse_obj(self.running_task_data_json)
-        # Act&Assert
-        self.assertRaises(
-            TaskNotRegisteredError, Task(mock_session, "missing_id").wait_for_completed, mock_session, 1, 1
-        )
-
     @patch("vmngclient.session.vManageSession")
     def test_get_all_tasks(self, mock_session):
         # Arrange
         mock_session.get_json.return_value = self.running_task_data_json
 
         # Act
         answer = TasksAPI(mock_session, "").get_all_tasks()
```

### Comparing `vmngclient-0.8.2/vmngclient/tests/test_templates.py` & `vmngclient-0.9.1/vmngclient/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/tests/test_tenant_backup_restore_api.py` & `vmngclient-0.9.1/vmngclient/tests/test_tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/tests/test_typed_list.py` & `vmngclient-0.9.1/vmngclient/tests/test_typed_list.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/tests/test_version_utils.py` & `vmngclient-0.9.1/vmngclient/tests/test_version_utils.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/tests/test_vmanage_auth.py` & `vmngclient-0.9.1/vmngclient/tests/test_vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/typed_list.py` & `vmngclient-0.9.1/vmngclient/typed_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import Any, Generic, Iterable, MutableSequence, Type, TypeVar, overload
 
-from pydantic import BaseModel  # type: ignore
+from pydantic import BaseModel
 
 from vmngclient.exceptions import InvalidOperationError
 from vmngclient.utils.creation_tools import AttrsInstance
 
 T = TypeVar("T")
 D = TypeVar("D")
```

### Comparing `vmngclient-0.8.2/vmngclient/utils/creation_tools.py` & `vmngclient-0.9.1/vmngclient/utils/creation_tools.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/utils/device_model.py` & `vmngclient-0.9.1/vmngclient/utils/device_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from enum import Enum
 
 
 class DeviceModel(Enum):
-
     # controlers
     VSMART = "vsmart"
     VBOND = "vedge-cloud"
     VMANAGE = "vmanage"
 
     # vedges
     VEDGE_ISR1100_6G = "vedge-ISR1100-6G"
@@ -66,9 +65,12 @@
     VEDGE_C1116_4PLTEEA = "vedge-C1116-4PLTEEA"
     VEDGE_C1117_4P = "vedge-C1117-4P"
     VEDGE_C1117_4PM = "vedge-C1117-4PM"
     VEDGE_C1117_4PLTEEA = "vedge-C1117-4PLTEEA"
     VEDGE_C1111_8PLTELA = "vedge-C1111-8PLTELA"
     VEDGE_C1111_8PLTEEA = "vedge-C1111-8PLTEEA"
 
+    # C8300
+    VEDGE_C8300_2N2S_6T = "vedge-C8300-2N2S-6T"
+
     # ISRv
     VEDGE_ISRV = "vedge-ISRv"
```

### Comparing `vmngclient-0.8.2/vmngclient/utils/upgrades_helper.py` & `vmngclient-0.9.1/vmngclient/utils/upgrades_helper.py`

 * *Files identical despite different names*

### Comparing `vmngclient-0.8.2/vmngclient/vmanage_auth.py` & `vmngclient-0.9.1/vmngclient/vmanage_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 
 import requests
 from requests import PreparedRequest, Response
 from requests.auth import AuthBase
 from requests.cookies import RequestsCookieJar
 
 from vmngclient import with_proc_info_header
+from vmngclient.exceptions import vManageClientError
 
 
-class InvalidCredentialsError(Exception):
+class InvalidCredentialsError(vManageClientError):
     """Exception raised for invalid credentials.
 
     Attributes:
         username (str): vManage username.
         password (str): vManage password.
         message (str): precise error explanation.
     """
```

### Comparing `vmngclient-0.8.2/setup.py` & `vmngclient-0.9.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
  'vmngclient.api.templates.device_template',
  'vmngclient.api.templates.models',
  'vmngclient.api.templates.payloads.aaa',
  'vmngclient.api.templates.payloads.cisco_system',
  'vmngclient.api.templates.payloads.cisco_vpn',
  'vmngclient.api.templates.payloads.cisco_vpn_interface_ethernet',
  'vmngclient.api.templates.payloads.tenant',
+ 'vmngclient.primitives',
  'vmngclient.tests',
  'vmngclient.utils']
 
 package_data = \
 {'': ['*'],
  'vmngclient.api.templates.payloads.aaa': ['feature/*'],
  'vmngclient.api.templates.payloads.cisco_system': ['feature/*'],
@@ -26,26 +27,27 @@
 ['Jinja2>=3.1.2,<4.0.0',
  'aiohttp>=3.8.1,<4.0.0',
  'attrs>=21.4.0,<22.0.0',
  'cattrs>=22.2.0,<23.0.0',
  'ciscoconfparse>=1.6.40,<2.0.0',
  'clint>=0.5.1,<0.6.0',
  'flake8-quotes>=3.3.1,<4.0.0',
+ 'packaging>=23.0,<24.0',
  'parameterized>=0.8.1,<0.9.0',
- 'pydantic>=1.10.4,<2.0.0',
+ 'pydantic>=1.10.7,<2.0.0',
  'python-dateutil>=2.8.2,<3.0.0',
  'requests-toolbelt>=0.10.1,<0.11.0',
  'requests>=2.27.1,<3.0.0',
  'tenacity>=8.1.0,<9.0.0']
 
 setup_kwargs = {
     'name': 'vmngclient',
-    'version': '0.8.2',
+    'version': '0.9.1',
     'description': 'Universal vManage API',
-    'long_description': '# vManage-client\n[![Python3.8](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3.8)](https://www.python.org/)\n\nvManage client is a package for creating simple and parallel automatic requests via official vManageAPI. It is intended to serve as a multiple session handler (provider, provider as a tenant, tenant). The library is not dependent on environment which is being run in, you just need a connection to any vManage.\n\n## Installation\n```console\npip install vmngclient\n```\n\n## Session usage example\nOur session is an extension to `requests.Session` designed to make it easier to communicate via API calls with vManage. We provide ready to use authenticetion, you have to simply provide the vmanage url, username and password as as if you were doing it through a GUI. \n```python\nfrom vmngclient.session import create_vManageSession\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\nsession = create_vManageSession(url=url, username=username, password=password)\n\nsession.get("/dataservice/device")\n```\n\n## API usage examples\n\n<details>\n    <summary> <b>Get devices</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\n```\n\n</details>\n\n<details>\n    <summary> <b>Admin Tech</b> <i>(click to expand)</i></summary>\n\n```Python\nadmin_tech_file = session.api.admin_tech.generate("172.16.255.11")\nadmintech.download(admin_tech_file)\nadmintech.delete(admin_tech_file)\n```\n</details>\n\n<details>\n    <summary> <b>Speed test</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\nspeedtest = session.api.speedtest.speedtest(devices[0], devices[1])\n```\n\n</details>\n\n<details>\n    <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>\n\n```python\n# Prepare devices list\nvsmarts = session.api.devices.get().filter(personality = Personality.VSMART)\nimage = "viptela-20.7.2-x86_64.tar.gz"\n\n# Upload image\nsession.api.repository.upload_image(software_image)\n\n# Install software\n\ninstall_task = session.api.software.install(devices = vsmarts,\n    image= image)\n\n# Check action status\ninstall_task.wait_for_completed()\n```\n\n</details>\n\n<details>\n    <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>\n\n```python\nalarms = session.api.alarms.get()\n```\n\n</details>\n\n### Note:\nTo remove `InsecureRequestWarning`, you can include in your scripts:\n```Python\nimport urllib3\nurllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)\n```\n\n## [Contributing, bug reporting and feature requests](https://github.com/CiscoDevNet/vManage-client/blob/main/CONTRIBUTING.md)\n\n## Seeking support\n\nYou can contact us by submitting [issues](https://github.com/CiscoDevNet/vManage-client/issues), or directly via mail on vmngclient@cisco.com.\n',
+    'long_description': '# vManage-client\n[![Python3.8](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3.8)](https://www.python.org/)\n\nvManage client is a package for creating simple and parallel automatic requests via official vManageAPI. It is intended to serve as a multiple session handler (provider, provider as a tenant, tenant). The library is not dependent on environment which is being run in, you just need a connection to any vManage.\n\n## Installation\n```console\npip install vmngclient\n```\n\n## Session usage example\nOur session is an extension to `requests.Session` designed to make it easier to communicate via API calls with vManage. We provide ready to use authenticetion, you have to simply provide the vmanage url, username and password as as if you were doing it through a GUI. \n```python\nfrom vmngclient.session import create_vManageSession\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\nsession = create_vManageSession(url=url, username=username, password=password)\n\nsession.get("/dataservice/device")\n```\n\n## API usage examples\n\n<details>\n    <summary> <b>Get devices</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\n```\n\n</details>\n\n<details>\n    <summary> <b>Admin Tech</b> <i>(click to expand)</i></summary>\n\n```Python\nadmin_tech_file = session.api.admin_tech.generate("172.16.255.11")\nsession.api.admin_tech.download(admin_tech_file)\nsession.api.admin_tech.delete(admin_tech_file)\n```\n</details>\n\n<details>\n    <summary> <b>Speed test</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\nspeedtest = session.api.speedtest.speedtest(devices[0], devices[1])\n```\n\n</details>\n\n<details>\n    <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>\n\n```python\n# Prepare devices list\nvsmarts = session.api.devices.get().filter(personality = Personality.VSMART)\nimage = "viptela-20.7.2-x86_64.tar.gz"\n\n# Upload image\nsession.api.repository.upload_image(software_image)\n\n# Install software\n\ninstall_task = session.api.software.install(devices = vsmarts,\n    image= image)\n\n# Check action status\ninstall_task.wait_for_completed()\n```\n\n</details>\n\n<details>\n    <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>\n\n```python\nalarms = session.api.alarms.get()\n```\n\n</details>\n\n<details>\n    <summary> <b>User operations</b> <i>(click to expand)</i></summary>\n\n```python\nfrom vmngclient.api.administration import User, UsersAPI\n\n# Get all users\nall_users = UsersAPI(session).get_all_users()\n\n# Create a user\nnew_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")\nstatus = UsersAPI(session).create_user(new_user)\n\n# Delete a user\nstatus = UsersAPI(session).delete_user(username="new_user")\n```\n\n</details>\n\n### Note:\nTo remove `InsecureRequestWarning`, you can include in your scripts (warning is suppressed when `VMNGCLIENT_DEVEL` environment variable is set):\n```Python\nimport urllib3\nurllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)\n```\n\n## Catching Exceptions\n```python\ntry:\n\tsession.api.users.delete_user("XYZ")\nexcept vManageBadRequestError as error:\n\t# Process an error.\n\tlogger.error(error.info.details)\n\n# message = \'Delete users request failed\' \n# details = \'No user with name XYZ was found\' \n# code = \'USER0006\'\n```\n\n## [Contributing, bug reporting and feature requests](https://github.com/CiscoDevNet/vManage-client/blob/main/CONTRIBUTING.md)\n\n## Seeking support\n\nYou can contact us by submitting [issues](https://github.com/CiscoDevNet/vManage-client/issues), or directly via mail on vmngclient@cisco.com.\n',
     'author': 'kagorski',
     'author_email': 'kagorski@cisco.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/CiscoDevNet/vManage-client',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `vmngclient-0.8.2/PKG-INFO` & `vmngclient-0.9.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmngclient
-Version: 0.8.2
+Version: 0.9.1
 Summary: Universal vManage API
 Home-page: https://github.com/CiscoDevNet/vManage-client
 Author: kagorski
 Author-email: kagorski@cisco.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -14,16 +14,17 @@
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: attrs (>=21.4.0,<22.0.0)
 Requires-Dist: cattrs (>=22.2.0,<23.0.0)
 Requires-Dist: ciscoconfparse (>=1.6.40,<2.0.0)
 Requires-Dist: clint (>=0.5.1,<0.6.0)
 Requires-Dist: flake8-quotes (>=3.3.1,<4.0.0)
+Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: parameterized (>=0.8.1,<0.9.0)
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: requests-toolbelt (>=0.10.1,<0.11.0)
 Requires-Dist: tenacity (>=8.1.0,<9.0.0)
 Project-URL: Repository, https://github.com/CiscoDevNet/vManage-client
 Description-Content-Type: text/markdown
 
@@ -62,16 +63,16 @@
 </details>
 
 <details>
     <summary> <b>Admin Tech</b> <i>(click to expand)</i></summary>
 
 ```Python
 admin_tech_file = session.api.admin_tech.generate("172.16.255.11")
-admintech.download(admin_tech_file)
-admintech.delete(admin_tech_file)
+session.api.admin_tech.download(admin_tech_file)
+session.api.admin_tech.delete(admin_tech_file)
 ```
 </details>
 
 <details>
     <summary> <b>Speed test</b> <i>(click to expand)</i></summary>
 
 ```python
@@ -108,20 +109,52 @@
 
 ```python
 alarms = session.api.alarms.get()
 ```
 
 </details>
 
+<details>
+    <summary> <b>User operations</b> <i>(click to expand)</i></summary>
+
+```python
+from vmngclient.api.administration import User, UsersAPI
+
+# Get all users
+all_users = UsersAPI(session).get_all_users()
+
+# Create a user
+new_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")
+status = UsersAPI(session).create_user(new_user)
+
+# Delete a user
+status = UsersAPI(session).delete_user(username="new_user")
+```
+
+</details>
+
 ### Note:
-To remove `InsecureRequestWarning`, you can include in your scripts:
+To remove `InsecureRequestWarning`, you can include in your scripts (warning is suppressed when `VMNGCLIENT_DEVEL` environment variable is set):
 ```Python
 import urllib3
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 ```
 
+## Catching Exceptions
+```python
+try:
+	session.api.users.delete_user("XYZ")
+except vManageBadRequestError as error:
+	# Process an error.
+	logger.error(error.info.details)
+
+# message = 'Delete users request failed' 
+# details = 'No user with name XYZ was found' 
+# code = 'USER0006'
+```
+
 ## [Contributing, bug reporting and feature requests](https://github.com/CiscoDevNet/vManage-client/blob/main/CONTRIBUTING.md)
 
 ## Seeking support
 
 You can contact us by submitting [issues](https://github.com/CiscoDevNet/vManage-client/issues), or directly via mail on vmngclient@cisco.com.
```

