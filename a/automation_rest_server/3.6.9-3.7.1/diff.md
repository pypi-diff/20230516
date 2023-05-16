# Comparing `tmp/automation_rest_server-3.6.9.tar.gz` & `tmp/automation_rest_server-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\automation_rest_server-3.6.9.tar", last modified: Thu May 11 08:02:54 2023, max compression
+gzip compressed data, was "dist\automation_rest_server-3.7.1.tar", last modified: Tue May 16 09:00:02 2023, max compression
```

## Comparing `automation_rest_server-3.6.9.tar` & `automation_rest_server-3.7.1.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/
--rw-rw-rw-   0        0        0     1098 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/LICENSE.txt
--rw-rw-rw-   0        0        0      687 2022-08-30 06:56:12.000000 automation_rest_server-3.6.9/MANIFEST.in
--rw-rw-rw-   0        0        0      551 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:53.000000 automation_rest_server-3.6.9/automation_rest_server/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/configuration/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/configuration/__init__.py
--rw-rw-rw-   0        0        0      581 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/configuration/config.yaml
--rw-rw-rw-   0        0        0     1099 2022-12-13 11:04:16.000000 automation_rest_server-3.6.9/automation_rest_server/configuration/firmware_build.yaml
--rw-rw-rw-   0        0        0  1333232 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/configuration/pci.ids
--rw-rw-rw-   0        0        0      157 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/configuration/version.yaml
--rw-rw-rw-   0        0        0       83 2022-08-25 03:13:17.000000 automation_rest_server-3.6.9/automation_rest_server/configuration/web_server.yaml
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/rest_client/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:18:57.000000 automation_rest_server-3.6.9/automation_rest_server/rest_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/rest_client/resource/
--rw-rw-rw-   0        0        0        0 2022-08-10 09:04:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_client/resource/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/rest_client/resource/models/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:20:01.000000 automation_rest_server-3.6.9/automation_rest_server/rest_client/resource/models/__init__.py
--rw-rw-rw-   0        0        0     4257 2023-05-10 02:20:31.000000 automation_rest_server-3.6.9/automation_rest_server/rest_client/resource/models/helper.py
--rw-rw-rw-   0        0        0     1944 2022-08-17 05:58:24.000000 automation_rest_server-3.6.9/automation_rest_server/rest_client/resource/node_resource.py
--rw-rw-rw-   0        0        0     1374 2022-08-30 04:43:20.000000 automation_rest_server-3.6.9/automation_rest_server/rest_client/resource/test_resource.py
--rw-rw-rw-   0        0        0      340 2022-08-25 03:00:40.000000 automation_rest_server-3.6.9/automation_rest_server/rest_client/resource/web_resource.py
--rw-rw-rw-   0        0        0     2536 2023-02-21 08:02:23.000000 automation_rest_server-3.6.9/automation_rest_server/rest_client/web_rest_client.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/__init__.py
--rw-rw-rw-   0        0        0     1678 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/reset_server.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/__init__.py
--rw-rw-rw-   0        0        0     2150 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/benchmark_resource.py
--rw-rw-rw-   0        0        0     1956 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/build_firmware_resource.py
--rw-rw-rw-   0        0        0      933 2022-12-12 01:57:01.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/git_resource.py
--rw-rw-rw-   0        0        0      850 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/models/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/models/__init__.py
--rw-rw-rw-   0        0        0     2044 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/models/ftp_server.py
--rw-rw-rw-   0        0        0     1732 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/models/helper.py
--rw-rw-rw-   0        0        0      958 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/oakgate_resource.py
--rw-rw-rw-   0        0        0      691 2022-08-11 02:31:16.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/operation_resource.py
--rw-rw-rw-   0        0        0     1641 2022-09-20 01:54:25.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/state_resource.py
--rw-rw-rw-   0        0        0     1085 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/stop_flag_resource.py
--rw-rw-rw-   0        0        0     6233 2022-12-03 07:36:31.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/test_resource.py
--rw-rw-rw-   0        0        0     1295 2023-05-10 02:20:31.000000 automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/upgrade_resource.py
--rw-rw-rw-   0        0        0     6063 2023-05-04 07:05:41.000000 automation_rest_server-3.6.9/automation_rest_server/run.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/__init__.py
--rw-rw-rw-   0        0        0     6679 2022-09-20 04:46:34.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/database.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/
--rw-rw-rw-   0        0        0        0 2021-11-12 08:10:50.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/__init__.py
--rw-rw-rw-   0        0        0     3082 2023-04-19 05:40:44.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/slot.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/sub_slot/
--rw-rw-rw-   0        0        0        0 2021-11-24 03:48:51.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/sub_slot/__init__.py
--rw-rw-rw-   0        0        0     1434 2022-09-15 07:43:45.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py
--rw-rw-rw-   0        0        0     3541 2023-04-17 06:49:22.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py
--rw-rw-rw-   0        0        0      901 2023-04-19 03:39:13.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py
--rw-rw-rw-   0        0        0     8894 2023-05-09 09:27:56.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/
--rw-rw-rw-   0        0        0      214 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/__init__.py
--rw-rw-rw-   0        0        0     2068 2023-04-25 07:50:43.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/nose_engine.py
--rw-rw-rw-   0        0        0     4926 2023-02-16 01:39:59.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/oakgate_engine.py
--rw-rw-rw-   0        0        0     4007 2023-03-02 06:19:25.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/perses_engine.py
--rw-rw-rw-   0        0        0     1489 2022-09-30 01:53:36.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py
--rw-rw-rw-   0        0        0      239 2023-04-07 02:04:12.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/special_parameter.py
--rw-rw-rw-   0        0        0     3562 2022-09-20 07:48:14.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/sse_engine.py
--rw-rw-rw-   0        0        0     4006 2023-04-25 07:48:48.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/venus_engine.py
--rw-rw-rw-   0        0        0     1517 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_build.py
--rw-rw-rw-   0        0        0     3049 2023-05-10 02:58:49.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_download.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/__init__.py
--rw-rw-rw-   0        0        0     7168 2022-12-13 11:05:02.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py
--rw-rw-rw-   0        0        0     6196 2023-05-11 07:52:03.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/logic_with_firmware_engine.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/oakgate/
--rw-rw-rw-   0        0        0        0 2023-04-11 02:31:20.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/oakgate/__init__.py
--rw-rw-rw-   0        0        0     2925 2023-04-11 02:43:50.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/oakgate/nvme_download.py
--rw-rw-rw-   0        0        0     2691 2023-04-17 07:35:59.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/oakgate/two_step_download.py
--rw-rw-rw-   0        0        0      671 2023-05-10 02:30:29.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py
--rw-rw-rw-   0        0        0     1996 2023-05-10 03:22:37.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py
--rw-rw-rw-   0        0        0     1585 2023-05-10 02:30:15.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py
--rw-rw-rw-   0        0        0     2344 2023-04-09 02:31:46.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py
--rw-rw-rw-   0        0        0     5139 2023-05-10 07:14:09.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/node_database.py
--rw-rw-rw-   0        0        0    10717 2023-04-19 03:38:41.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/performance_database.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/reboot_engine/
--rw-rw-rw-   0        0        0       50 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/reboot_engine/__init__.py
--rw-rw-rw-   0        0        0     2439 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py
--rw-rw-rw-   0        0        0     2055 2023-05-10 02:51:26.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/state.py
--rw-rw-rw-   0        0        0      672 2022-12-13 03:29:14.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/status_file.py
--rw-rw-rw-   0        0        0     5684 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/test_base.py
--rw-rw-rw-   0        0        0     1973 2023-02-14 08:06:21.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/test_benchmark.py
--rw-rw-rw-   0        0        0     3512 2023-02-07 07:54:27.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/test_benchmark_group.py
--rw-rw-rw-   0        0        0     1263 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/test_case.py
--rw-rw-rw-   0        0        0    22062 2023-05-10 02:21:32.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/test_pool.py
--rw-rw-rw-   0        0        0      892 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/test_reboot_handle.py
--rw-rw-rw-   0        0        0     4365 2022-12-03 07:44:06.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/test_result.py
--rw-rw-rw-   0        0        0     3757 2023-03-02 10:28:02.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/test_runner.py
--rw-rw-rw-   0        0        0     4717 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/test_framework/test_suite.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/tool/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/tool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/
--rw-rw-rw-   0        0        0        0 2021-11-12 06:54:04.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/dll/
--rw-rw-rw-   0        0        0        0 2021-10-23 02:17:43.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/dll/__init__.py
--rw-rw-rw-   0        0        0    24064 2021-10-23 02:17:43.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/dll/buf.dll
--rw-rw-rw-   0        0        0    12760 2021-10-23 02:17:43.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/dll/buf.so
--rw-rw-rw-   0        0        0      777 2021-10-23 02:17:43.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/dll/build.py
--rw-rw-rw-   0        0        0      861 2022-09-15 07:43:45.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/linux_nvme.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/
--rw-rw-rw-   0        0        0        0 2021-11-23 06:34:00.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/__init__.py
--rw-rw-rw-   0        0        0    14077 2021-11-23 06:29:25.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/buf.py
--rw-rw-rw-   0        0        0     4722 2021-11-23 06:25:09.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/ctype.py
--rw-rw-rw-   0        0        0    39204 2021-11-23 06:28:50.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/get_feature.py
--rw-rw-rw-   0        0        0    38547 2022-09-15 07:43:45.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/ioctl.py
--rw-rw-rw-   0        0        0    23303 2022-09-15 07:42:03.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/nvme.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/
--rw-rw-rw-   0        0        0      256 2021-11-23 06:21:15.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/__init__.py
--rw-rw-rw-   0        0        0    30449 2021-11-23 06:59:35.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/command.py
--rw-rw-rw-   0        0        0    15322 2021-11-23 06:59:35.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/features.py
--rw-rw-rw-   0        0        0     1104 2021-10-23 02:17:43.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/hmb.py
--rw-rw-rw-   0        0        0    16135 2021-11-23 07:31:19.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/identify.py
--rw-rw-rw-   0        0        0    13915 2021-11-23 06:59:59.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/log_page.py
--rw-rw-rw-   0        0        0     2361 2021-11-12 10:37:37.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/memory.py
--rw-rw-rw-   0        0        0    10510 2021-10-23 02:17:43.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/pcie.py
--rw-rw-rw-   0        0        0    35527 2021-10-23 02:17:43.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/registers.py
--rw-rw-rw-   0        0        0     9095 2021-11-24 06:24:21.000000 automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/utility_vu.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/tool/diskpart/
--rw-rw-rw-   0        0        0       56 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/tool/diskpart/__init__.py
--rw-rw-rw-   0        0        0      770 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/tool/diskpart/diskpart.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/tool/fio/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/tool/fio/__init__.py
--rw-rw-rw-   0        0        0    18967 2023-02-23 03:46:38.000000 automation_rest_server-3.6.9/automation_rest_server/tool/fio/fio.py
--rw-rw-rw-   0        0        0     5032 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/tool/fio/fio_linux.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/tool/fio/tool/
--rw-rw-rw-   0        0        0  4733892 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/tool/fio/tool/fio
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/tool/git/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/tool/git/__init__.py
--rw-rw-rw-   0        0        0     5645 2023-03-02 10:20:30.000000 automation_rest_server-3.6.9/automation_rest_server/tool/git/git_operator.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/tool/iometer/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/tool/iometer/__init__.py
--rw-rw-rw-   0        0        0     9223 2023-02-07 08:25:51.000000 automation_rest_server-3.6.9/automation_rest_server/tool/iometer/iometer.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/automation_rest_server/utils/
--rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/utils/__init__.py
--rw-rw-rw-   0        0        0    12385 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/utils/buf.py
--rw-rw-rw-   0        0        0     5636 2023-04-10 09:29:00.000000 automation_rest_server-3.6.9/automation_rest_server/utils/firmware_path.py
--rw-rw-rw-   0        0        0     3697 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/utils/log.py
--rw-rw-rw-   0        0        0      386 2023-02-23 02:34:33.000000 automation_rest_server-3.6.9/automation_rest_server/utils/message.py
--rw-rw-rw-   0        0        0     3532 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/utils/nose_xml.py
--rw-rw-rw-   0        0        0     1742 2022-09-20 07:22:33.000000 automation_rest_server-3.6.9/automation_rest_server/utils/pip_operation.py
--rw-rw-rw-   0        0        0     1823 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/utils/process.py
--rw-rw-rw-   0        0        0     3157 2023-05-11 07:32:58.000000 automation_rest_server-3.6.9/automation_rest_server/utils/serial_tool.py
--rw-rw-rw-   0        0        0     9222 2022-06-02 02:49:38.000000 automation_rest_server-3.6.9/automation_rest_server/utils/ssh.py
--rw-rw-rw-   0        0        0     5366 2022-12-22 01:47:58.000000 automation_rest_server-3.6.9/automation_rest_server/utils/system.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:02:53.000000 automation_rest_server-3.6.9/automation_rest_server.egg-info/
--rw-rw-rw-   0        0        0      551 2023-05-11 08:02:53.000000 automation_rest_server-3.6.9/automation_rest_server.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7047 2023-05-11 08:02:53.000000 automation_rest_server-3.6.9/automation_rest_server.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 08:02:53.000000 automation_rest_server-3.6.9/automation_rest_server.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-05-11 08:02:53.000000 automation_rest_server-3.6.9/automation_rest_server.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       98 2023-05-11 08:02:53.000000 automation_rest_server-3.6.9/automation_rest_server.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-05-11 08:02:53.000000 automation_rest_server-3.6.9/automation_rest_server.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       64 2023-05-11 08:02:54.000000 automation_rest_server-3.6.9/setup.cfg
--rw-rw-rw-   0        0        0     1211 2023-05-11 08:02:35.000000 automation_rest_server-3.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:02.000000 automation_rest_server-3.7.1/
+-rw-rw-rw-   0        0        0     1098 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      687 2022-08-30 06:56:12.000000 automation_rest_server-3.7.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      551 2023-05-16 09:00:02.000000 automation_rest_server-3.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:01.000000 automation_rest_server-3.7.1/automation_rest_server/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:01.000000 automation_rest_server-3.7.1/automation_rest_server/configuration/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/configuration/__init__.py
+-rw-rw-rw-   0        0        0      581 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/configuration/config.yaml
+-rw-rw-rw-   0        0        0     1099 2022-12-13 11:04:16.000000 automation_rest_server-3.7.1/automation_rest_server/configuration/firmware_build.yaml
+-rw-rw-rw-   0        0        0  1333232 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/configuration/pci.ids
+-rw-rw-rw-   0        0        0      157 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/configuration/version.yaml
+-rw-rw-rw-   0        0        0       83 2022-08-25 03:13:17.000000 automation_rest_server-3.7.1/automation_rest_server/configuration/web_server.yaml
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:01.000000 automation_rest_server-3.7.1/automation_rest_server/rest_client/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:18:57.000000 automation_rest_server-3.7.1/automation_rest_server/rest_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:01.000000 automation_rest_server-3.7.1/automation_rest_server/rest_client/resource/
+-rw-rw-rw-   0        0        0        0 2022-08-10 09:04:38.000000 automation_rest_server-3.7.1/automation_rest_server/rest_client/resource/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:01.000000 automation_rest_server-3.7.1/automation_rest_server/rest_client/resource/models/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:20:01.000000 automation_rest_server-3.7.1/automation_rest_server/rest_client/resource/models/__init__.py
+-rw-rw-rw-   0        0        0     4257 2023-05-10 02:20:31.000000 automation_rest_server-3.7.1/automation_rest_server/rest_client/resource/models/helper.py
+-rw-rw-rw-   0        0        0     1944 2022-08-17 05:58:24.000000 automation_rest_server-3.7.1/automation_rest_server/rest_client/resource/node_resource.py
+-rw-rw-rw-   0        0        0     1374 2022-08-30 04:43:20.000000 automation_rest_server-3.7.1/automation_rest_server/rest_client/resource/test_resource.py
+-rw-rw-rw-   0        0        0      340 2022-08-25 03:00:40.000000 automation_rest_server-3.7.1/automation_rest_server/rest_client/resource/web_resource.py
+-rw-rw-rw-   0        0        0     2536 2023-02-21 08:02:23.000000 automation_rest_server-3.7.1/automation_rest_server/rest_client/web_rest_client.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:01.000000 automation_rest_server-3.7.1/automation_rest_server/rest_server/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/rest_server/__init__.py
+-rw-rw-rw-   0        0        0     1678 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/rest_server/reset_server.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:01.000000 automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/__init__.py
+-rw-rw-rw-   0        0        0     2150 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/benchmark_resource.py
+-rw-rw-rw-   0        0        0     1956 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/build_firmware_resource.py
+-rw-rw-rw-   0        0        0      933 2022-12-12 01:57:01.000000 automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/git_resource.py
+-rw-rw-rw-   0        0        0      850 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:01.000000 automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/models/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/models/__init__.py
+-rw-rw-rw-   0        0        0     2044 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/models/ftp_server.py
+-rw-rw-rw-   0        0        0     1732 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/models/helper.py
+-rw-rw-rw-   0        0        0      958 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/oakgate_resource.py
+-rw-rw-rw-   0        0        0      691 2022-08-11 02:31:16.000000 automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/operation_resource.py
+-rw-rw-rw-   0        0        0     1641 2022-09-20 01:54:25.000000 automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/state_resource.py
+-rw-rw-rw-   0        0        0     1085 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/stop_flag_resource.py
+-rw-rw-rw-   0        0        0     6233 2022-12-03 07:36:31.000000 automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/test_resource.py
+-rw-rw-rw-   0        0        0     1295 2023-05-10 02:20:31.000000 automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/upgrade_resource.py
+-rw-rw-rw-   0        0        0     6063 2023-05-04 07:05:41.000000 automation_rest_server-3.7.1/automation_rest_server/run.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:01.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/__init__.py
+-rw-rw-rw-   0        0        0     6679 2022-09-20 04:46:34.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/database.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:01.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/dut/
+-rw-rw-rw-   0        0        0        0 2021-11-12 08:10:50.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/dut/__init__.py
+-rw-rw-rw-   0        0        0     3082 2023-04-19 05:40:44.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/dut/slot.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:01.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/dut/sub_slot/
+-rw-rw-rw-   0        0        0        0 2021-11-24 03:48:51.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/dut/sub_slot/__init__.py
+-rw-rw-rw-   0        0        0     1434 2022-09-15 07:43:45.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py
+-rw-rw-rw-   0        0        0     3541 2023-04-17 06:49:22.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py
+-rw-rw-rw-   0        0        0      901 2023-04-19 03:39:13.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py
+-rw-rw-rw-   0        0        0     8894 2023-05-09 09:27:56.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:02.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/engine/
+-rw-rw-rw-   0        0        0      214 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/engine/__init__.py
+-rw-rw-rw-   0        0        0     3076 2023-05-12 03:00:15.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/engine/nose_engine.py
+-rw-rw-rw-   0        0        0     4926 2023-02-16 01:39:59.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/engine/oakgate_engine.py
+-rw-rw-rw-   0        0        0     4007 2023-03-02 06:19:25.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/engine/perses_engine.py
+-rw-rw-rw-   0        0        0     1489 2022-09-30 01:53:36.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py
+-rw-rw-rw-   0        0        0      239 2023-04-07 02:04:12.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/engine/special_parameter.py
+-rw-rw-rw-   0        0        0     3562 2022-09-20 07:48:14.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/engine/sse_engine.py
+-rw-rw-rw-   0        0        0     3986 2023-05-12 01:47:10.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/engine/venus_engine.py
+-rw-rw-rw-   0        0        0     1517 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_build.py
+-rw-rw-rw-   0        0        0     3049 2023-05-10 02:58:49.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_download.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:02.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_engine/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_engine/__init__.py
+-rw-rw-rw-   0        0        0     7168 2022-12-13 11:05:02.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py
+-rw-rw-rw-   0        0        0     6204 2023-05-11 09:15:12.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_engine/logic_with_firmware_engine.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:02.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_engine/oakgate/
+-rw-rw-rw-   0        0        0        0 2023-04-11 02:31:20.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_engine/oakgate/__init__.py
+-rw-rw-rw-   0        0        0     2925 2023-04-11 02:43:50.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_engine/oakgate/nvme_download.py
+-rw-rw-rw-   0        0        0     2691 2023-04-17 07:35:59.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_engine/oakgate/two_step_download.py
+-rw-rw-rw-   0        0        0      671 2023-05-10 02:30:29.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py
+-rw-rw-rw-   0        0        0     1996 2023-05-10 03:22:37.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py
+-rw-rw-rw-   0        0        0     1585 2023-05-10 02:30:15.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py
+-rw-rw-rw-   0        0        0     2344 2023-04-09 02:31:46.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py
+-rw-rw-rw-   0        0        0     5139 2023-05-10 07:14:09.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/node_database.py
+-rw-rw-rw-   0        0        0    10717 2023-04-19 03:38:41.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/performance_database.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:02.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/reboot_engine/
+-rw-rw-rw-   0        0        0       50 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/reboot_engine/__init__.py
+-rw-rw-rw-   0        0        0     2439 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py
+-rw-rw-rw-   0        0        0     2055 2023-05-10 02:51:26.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/state.py
+-rw-rw-rw-   0        0        0      672 2022-12-13 03:29:14.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/status_file.py
+-rw-rw-rw-   0        0        0     5684 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/test_base.py
+-rw-rw-rw-   0        0        0     1973 2023-02-14 08:06:21.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/test_benchmark.py
+-rw-rw-rw-   0        0        0     3512 2023-02-07 07:54:27.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/test_benchmark_group.py
+-rw-rw-rw-   0        0        0     1263 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/test_case.py
+-rw-rw-rw-   0        0        0    22062 2023-05-10 02:21:32.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/test_pool.py
+-rw-rw-rw-   0        0        0      892 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/test_reboot_handle.py
+-rw-rw-rw-   0        0        0     4485 2023-05-12 02:37:27.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/test_result.py
+-rw-rw-rw-   0        0        0     3757 2023-03-02 10:28:02.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/test_runner.py
+-rw-rw-rw-   0        0        0     4717 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/test_framework/test_suite.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:02.000000 automation_rest_server-3.7.1/automation_rest_server/tool/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/tool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:02.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/
+-rw-rw-rw-   0        0        0        0 2021-11-12 06:54:04.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:02.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/dll/
+-rw-rw-rw-   0        0        0        0 2021-10-23 02:17:43.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/dll/__init__.py
+-rw-rw-rw-   0        0        0    24064 2021-10-23 02:17:43.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/dll/buf.dll
+-rw-rw-rw-   0        0        0    12760 2021-10-23 02:17:43.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/dll/buf.so
+-rw-rw-rw-   0        0        0      777 2021-10-23 02:17:43.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/dll/build.py
+-rw-rw-rw-   0        0        0      861 2022-09-15 07:43:45.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/linux_nvme.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:02.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/
+-rw-rw-rw-   0        0        0        0 2021-11-23 06:34:00.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/__init__.py
+-rw-rw-rw-   0        0        0    14077 2021-11-23 06:29:25.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/buf.py
+-rw-rw-rw-   0        0        0     4722 2021-11-23 06:25:09.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/ctype.py
+-rw-rw-rw-   0        0        0    39204 2021-11-23 06:28:50.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/get_feature.py
+-rw-rw-rw-   0        0        0    38547 2022-09-15 07:43:45.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/ioctl.py
+-rw-rw-rw-   0        0        0    23303 2022-09-15 07:42:03.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/nvme.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:02.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/struct/
+-rw-rw-rw-   0        0        0      256 2021-11-23 06:21:15.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/struct/__init__.py
+-rw-rw-rw-   0        0        0    30449 2021-11-23 06:59:35.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/struct/command.py
+-rw-rw-rw-   0        0        0    15322 2021-11-23 06:59:35.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/struct/features.py
+-rw-rw-rw-   0        0        0     1104 2021-10-23 02:17:43.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/struct/hmb.py
+-rw-rw-rw-   0        0        0    16135 2021-11-23 07:31:19.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/struct/identify.py
+-rw-rw-rw-   0        0        0    13915 2021-11-23 06:59:59.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/struct/log_page.py
+-rw-rw-rw-   0        0        0     2361 2021-11-12 10:37:37.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/struct/memory.py
+-rw-rw-rw-   0        0        0    10510 2021-10-23 02:17:43.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/struct/pcie.py
+-rw-rw-rw-   0        0        0    35527 2021-10-23 02:17:43.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/struct/registers.py
+-rw-rw-rw-   0        0        0     9095 2021-11-24 06:24:21.000000 automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/utility_vu.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:02.000000 automation_rest_server-3.7.1/automation_rest_server/tool/diskpart/
+-rw-rw-rw-   0        0        0       56 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/tool/diskpart/__init__.py
+-rw-rw-rw-   0        0        0      770 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/tool/diskpart/diskpart.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:02.000000 automation_rest_server-3.7.1/automation_rest_server/tool/fio/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/tool/fio/__init__.py
+-rw-rw-rw-   0        0        0    18967 2023-02-23 03:46:38.000000 automation_rest_server-3.7.1/automation_rest_server/tool/fio/fio.py
+-rw-rw-rw-   0        0        0     5032 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/tool/fio/fio_linux.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:02.000000 automation_rest_server-3.7.1/automation_rest_server/tool/fio/tool/
+-rw-rw-rw-   0        0        0  4733892 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/tool/fio/tool/fio
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:02.000000 automation_rest_server-3.7.1/automation_rest_server/tool/git/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/tool/git/__init__.py
+-rw-rw-rw-   0        0        0     5645 2023-03-02 10:20:30.000000 automation_rest_server-3.7.1/automation_rest_server/tool/git/git_operator.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:02.000000 automation_rest_server-3.7.1/automation_rest_server/tool/iometer/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/tool/iometer/__init__.py
+-rw-rw-rw-   0        0        0     9223 2023-02-07 08:25:51.000000 automation_rest_server-3.7.1/automation_rest_server/tool/iometer/iometer.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:02.000000 automation_rest_server-3.7.1/automation_rest_server/utils/
+-rw-rw-rw-   0        0        0        0 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/utils/__init__.py
+-rw-rw-rw-   0        0        0    12385 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/utils/buf.py
+-rw-rw-rw-   0        0        0     5636 2023-04-10 09:29:00.000000 automation_rest_server-3.7.1/automation_rest_server/utils/firmware_path.py
+-rw-rw-rw-   0        0        0     3697 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/utils/log.py
+-rw-rw-rw-   0        0        0      386 2023-02-23 02:34:33.000000 automation_rest_server-3.7.1/automation_rest_server/utils/message.py
+-rw-rw-rw-   0        0        0     3532 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/utils/nose_xml.py
+-rw-rw-rw-   0        0        0     1742 2022-09-20 07:22:33.000000 automation_rest_server-3.7.1/automation_rest_server/utils/pip_operation.py
+-rw-rw-rw-   0        0        0     1823 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/utils/process.py
+-rw-rw-rw-   0        0        0     3226 2023-05-11 09:28:31.000000 automation_rest_server-3.7.1/automation_rest_server/utils/serial_tool.py
+-rw-rw-rw-   0        0        0     9222 2022-06-02 02:49:38.000000 automation_rest_server-3.7.1/automation_rest_server/utils/ssh.py
+-rw-rw-rw-   0        0        0     5366 2022-12-22 01:47:58.000000 automation_rest_server-3.7.1/automation_rest_server/utils/system.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:00:01.000000 automation_rest_server-3.7.1/automation_rest_server.egg-info/
+-rw-rw-rw-   0        0        0      551 2023-05-16 09:00:00.000000 automation_rest_server-3.7.1/automation_rest_server.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7047 2023-05-16 09:00:01.000000 automation_rest_server-3.7.1/automation_rest_server.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 09:00:00.000000 automation_rest_server-3.7.1/automation_rest_server.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-05-16 09:00:00.000000 automation_rest_server-3.7.1/automation_rest_server.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      107 2023-05-16 09:00:00.000000 automation_rest_server-3.7.1/automation_rest_server.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-05-16 09:00:00.000000 automation_rest_server-3.7.1/automation_rest_server.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       64 2023-05-16 09:00:02.000000 automation_rest_server-3.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1248 2023-05-16 08:59:58.000000 automation_rest_server-3.7.1/setup.py
```

### Comparing `automation_rest_server-3.6.9/LICENSE.txt` & `automation_rest_server-3.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/MANIFEST.in` & `automation_rest_server-3.7.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/PKG-INFO` & `automation_rest_server-3.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: automation_rest_server
-Version: 3.6.9
+Version: 3.7.1
 Summary: NVMe production server
 Home-page: https://pypi.org/project/automation_rest_server
 Author: yuwen123441
 Author-email: yuwen123441@126.com
 License: MIT License
 Description: UNKNOWN
 Keywords: runner,server
```

### Comparing `automation_rest_server-3.6.9/automation_rest_server/configuration/config.yaml` & `automation_rest_server-3.7.1/automation_rest_server/configuration/config.yaml`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/configuration/firmware_build.yaml` & `automation_rest_server-3.7.1/automation_rest_server/configuration/firmware_build.yaml`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/configuration/pci.ids` & `automation_rest_server-3.7.1/automation_rest_server/configuration/pci.ids`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/rest_client/resource/models/helper.py` & `automation_rest_server-3.7.1/automation_rest_server/rest_client/resource/models/helper.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/rest_client/resource/node_resource.py` & `automation_rest_server-3.7.1/automation_rest_server/rest_client/resource/node_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/rest_client/resource/test_resource.py` & `automation_rest_server-3.7.1/automation_rest_server/rest_client/resource/test_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/rest_client/web_rest_client.py` & `automation_rest_server-3.7.1/automation_rest_server/rest_client/web_rest_client.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/rest_server/reset_server.py` & `automation_rest_server-3.7.1/automation_rest_server/rest_server/reset_server.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/benchmark_resource.py` & `automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/benchmark_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/build_firmware_resource.py` & `automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/build_firmware_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/git_resource.py` & `automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/git_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py` & `automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/iometer_benchmark_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/models/ftp_server.py` & `automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/models/ftp_server.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/models/helper.py` & `automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/models/helper.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/oakgate_resource.py` & `automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/oakgate_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/operation_resource.py` & `automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/operation_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/state_resource.py` & `automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/state_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/stop_flag_resource.py` & `automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/stop_flag_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/test_resource.py` & `automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/test_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/rest_server/resource/upgrade_resource.py` & `automation_rest_server-3.7.1/automation_rest_server/rest_server/resource/upgrade_resource.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/run.py` & `automation_rest_server-3.7.1/automation_rest_server/run.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/database.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/database.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/slot.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/dut/slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/dut/sub_slot/linux_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/dut/sub_slot/oakgate_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/dut/sub_slot/perses_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/dut/sub_slot/powercycle_slot.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/nose_engine.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/engine/nose_engine.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,78 @@
 import os
-from utils import log
 import time
 import subprocess
+import yaml
 from test_framework.state import State
+from utils import log
 
 
 class NoseEngine(object):
 
     def __init__(self):
+        self.prun_port = os.environ.get("prun_port", 5000)
         self.working_path = os.environ["working_path"]
         self.log_path = self.get_log_path()
 
     def get_log_path(self):
         log_path = os.path.join(self.working_path, "log")
         if os.path.exists(log_path) is False:
             os.mkdir(log_path)
         return log_path
 
-    @staticmethod
-    def get_msg(out, err):
-        msg = str()
-        if err is not None:
-            msg += err.decode('utf-8')
-        if out is not None:
-            msg += out.decode('utf-8')
-        return msg
+    def get_orig_logs(self):
+        self.orig_log_folders = os.path.join(self.log_path, "org_logs_{}.yaml".format(self.prun_port))
+        orig_log_folders = os.listdir(self.log_path)
+        with open(self.orig_log_folders, 'w') as f:
+            yaml.dump(orig_log_folders, f)
+
+    def get_new_log(self):
+        latest_log_folders = os.listdir(self.log_path)
+        orig_log_folders = self.read_orig_logs()
+        new_logs = []
+        for item in latest_log_folders:
+            if item not in orig_log_folders:
+                item_path = os.path.join(self.log_path, item)
+                if os.path.isdir(item_path):
+                    for temp_log in os.listdir(item_path):
+                        temp_log_path = os.path.join(item_path, temp_log)
+                        if os.path.isfile(temp_log_path):
+                            new_logs.append(temp_log_path)
+        return new_logs
+
+    def read_orig_logs(self):
+        with open(self.orig_log_folders) as f:
+            log_folders = yaml.load(f.read(), Loader=yaml.SafeLoader)
+        return log_folders
 
     def save_msg(self, msg, test_case):
         test_function = test_case.split(".")
         log_file = "{}_{}.log".format(test_function[-1], time.time())
         log_path = os.path.join(self.log_path, log_file)
         with open(log_path, "w") as file_:
             file_.write(msg)
         return log_path
 
     def command_run_test(self, test_case, test_path):
         test_function = test_case.split(".")
         xml_name = "nosetests_%s_%s.xml" % (test_function[-1], time.time())
         xml_path = os.path.join(self.log_path, xml_name)
-        command_line = "nosetests --exe --nocapture --with-printlog --with-xunit --xunit-file={} -x {}"\
+        command_line = "nosetests --exe --nocapture --with-printlog --with-xunit --xunit-file={} -x {}" \
             .format(xml_path, test_path)
         child1 = subprocess.Popen(command_line, shell=True)
         return_code = child1.wait()
         ret = True if return_code == 0 else False
         return ret, xml_path
 
     def run(self, test_case, test_path, parameters, queue):
-        ret,  xml_path = self.command_run_test(test_case, test_path)
+        self.get_orig_logs()
+        ret, xml_path = self.command_run_test(test_case, test_path)
+        logs = self.get_new_log()
         if ret is True:
             log.INFO("TestCase run succeed.%s", test_case)
             result = State.PASS
         else:
             log.ERR("TestCase run failed. %s", test_case)
             result = State.FAIL
-        result = {"name": test_case, "result": result, "log":xml_path, "xml_path": xml_path}
+        result = {"name": test_case, "result": result, "log": logs, "xml_path": xml_path}
         queue.put(result)
         return ret
```

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/oakgate_engine.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/engine/oakgate_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/perses_engine.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/engine/perses_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/engine/perses_power_cycle_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/sse_engine.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/engine/sse_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/engine/venus_engine.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/engine/venus_engine.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,47 +6,48 @@
 from test_framework.state import State
 from utils.firmware_path import FirmwareBinPath
 
 
 class VenusEngine(object):
 
     def __init__(self):
-        self.local_ip = get_ip_address()
         self.working_path = os.environ["working_path"]
         self.prun_port = os.environ["prun_port"]
         self.log_path = self.get_log_path()
         self.orig_log_folders = ""
         self.fw_path_manage = FirmwareBinPath()
 
     def get_log_path(self):
         log_path = os.path.join(self.working_path, "log")
         if os.path.exists(log_path) is False:
             os.mkdir(log_path)
-        if self.local_ip is not None:
-            log_path = os.path.join(log_path, self.local_ip)
         if os.path.exists(log_path) is False:
             os.mkdir(log_path)
         return log_path
 
     def get_new_log(self, test_case):
         test_name = test_case.split('.')[-1]
         latest_log_folders = os.listdir(self.log_path)
         orig_log_folders = self.read_orig_logs()
-        new_logs = list()
+        new_logs = []
         for item in latest_log_folders:
             if item not in orig_log_folders:
-                if os.path.isfile(os.path.join(self.log_path, item)):
-                    if test_name in item:
-                        new_logs.append(os.path.join(self.log_path, item))
+                item_path = os.path.join(self.log_path, item)
+                if os.path.isfile(item_path) and test_name in item:
+                    new_logs.append(item_path)
+                elif os.path.isdir(item_path):
+                    for temp_log in os.listdir(item_path):
+                        temp_log_path = os.path.join(item_path, temp_log)
+                        if os.path.isfile(temp_log_path):
+                            new_logs.append(temp_log_path)
         return new_logs
 
     def get_orig_logs(self):
         self.orig_log_folders = os.path.join(self.log_path, "org_logs_{}.yaml".format(self.prun_port))
         orig_log_folders = os.listdir(self.log_path)
-        orig_log_folders = [item for item in orig_log_folders if "test_" in item]
         with open(self.orig_log_folders, 'w') as f:
             yaml.dump(orig_log_folders, f)
 
     def read_orig_logs(self):
         with open(self.orig_log_folders) as f:
             log_folders = yaml.load(f.read(), Loader=yaml.SafeLoader)
         return log_folders
@@ -59,32 +60,30 @@
             if para_str == "":
                 para_str = temp
             else:
                 para_str = "{},{}".format(para_str, temp)
         return para_str
 
     def run_test(self, test_case, parameters):
-        log.INFO("Perses run_test")
         parameters = self.fw_path_manage.update_perses_fw_path(parameters)
-        print("perses para", parameters)
+        print("venus para", parameters)
         para_str = self.convert_para_2_string(parameters)
-        log.INFO("Perses para str {}".format(para_str))
+        log.INFO("venus para str {}".format(para_str))
         if para_str == "":
             command_line = "python run.py testcase -n {}".format(test_case)
         else:
             command_line = "python run.py testcase -n {} -v {}".format(test_case, para_str)
-        log.INFO("PersesEngine run command: {}".format(command_line))
+        log.INFO("Venus Engine run command: {}".format(command_line))
         child1 = subprocess.Popen(command_line, shell=True)
         return_code = child1.wait()
         return return_code
 
     def run(self, test_case, test_path, parameters, queue):
-        log.INFO("Perses run")
+        log.INFO("venus run")
         self.get_orig_logs()
-        log.INFO("Perses get_orig_logs")
         ret_code = self.run_test(test_case, parameters)
         logs = self.get_new_log(test_case)
         if ret_code == 0:
             test_result = State.PASS
         elif ret_code == 1:
             test_result = State.FAIL
         elif ret_code == 2:
```

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_build.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_build.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_download.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_download.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_engine/build_firmware_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/logic_with_firmware_engine.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_engine/logic_with_firmware_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,388 +1,388 @@
 00000000: 0d0a 696d 706f 7274 206f 730d 0a69 6d70  ..import os..imp
 00000010: 6f72 7420 7469 6d65 0d0a 696d 706f 7274  ort time..import
 00000020: 2073 6875 7469 6c0d 0a69 6d70 6f72 7420   shutil..import 
-00000030: 6674 706c 6962 0d0a 696d 706f 7274 2070  ftplib..import p
-00000040: 7937 7a72 0d0a 6672 6f6d 2074 6f6f 6c2e  y7zr..from tool.
-00000050: 6769 742e 6769 745f 6f70 6572 6174 6f72  git.git_operator
-00000060: 2069 6d70 6f72 7420 4769 744f 7065 7261   import GitOpera
-00000070: 746f 720d 0a66 726f 6d20 7574 696c 732e  tor..from utils.
-00000080: 7373 6820 696d 706f 7274 2053 5348 0d0a  ssh import SSH..
-00000090: 6672 6f6d 2075 7469 6c73 2e73 7973 7465  from utils.syste
-000000a0: 6d20 696d 706f 7274 2064 6563 6f72 6174  m import decorat
-000000b0: 655f 6578 6365 7074 696f 6e5f 7265 7375  e_exception_resu
-000000c0: 6c74 0d0a 6672 6f6d 2075 7469 6c73 2e73  lt..from utils.s
-000000d0: 6572 6961 6c5f 746f 6f6c 2069 6d70 6f72  erial_tool impor
-000000e0: 7420 436e 6578 5365 7269 616c 0d0a 6672  t CnexSerial..fr
-000000f0: 6f6d 2075 7469 6c73 2069 6d70 6f72 7420  om utils import 
-00000100: 6c6f 670d 0a0d 0a0d 0a63 6c61 7373 204c  log......class L
-00000110: 6f67 6963 4657 446f 776e 6c6f 6164 6572  ogicFWDownloader
-00000120: 286f 626a 6563 7429 3a0d 0a0d 0a20 2020  (object):....   
-00000130: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00000140: 6c66 293a 0d0a 2020 2020 2020 2020 7365  lf):..        se
-00000150: 6c66 2e69 635f 6674 7020 3d20 2231 3732  lf.ic_ftp = "172
-00000160: 2e32 392e 302e 3230 3822 0d0a 2020 2020  .29.0.208"..    
-00000170: 2020 2020 7365 6c66 2e69 635f 6674 705f      self.ic_ftp_
-00000180: 7573 6572 203d 2022 6c61 6222 0d0a 2020  user = "lab"..  
-00000190: 2020 2020 2020 7365 6c66 2e69 635f 6674        self.ic_ft
-000001a0: 705f 7077 6420 3d20 226c 6162 220d 0a20  p_pwd = "lab".. 
-000001b0: 2020 2020 2020 2073 656c 662e 6674 705f         self.ftp_
-000001c0: 7061 7474 656e 203d 2022 6670 6761 2e37  patten = "fpga.7
-000001d0: 7a22 0d0a 2020 2020 2020 2020 7365 6c66  z"..        self
-000001e0: 2e6c 6f63 616c 5f66 7470 5f70 6174 6820  .local_ftp_path 
-000001f0: 3d20 7222 433a 5c70 7275 6e22 0d0a 2020  = r"C:\prun"..  
-00000200: 2020 2020 2020 7365 6c66 2e6c 6f63 616c        self.local
-00000210: 5f66 7470 5f66 7067 615f 7061 7468 203d  _ftp_fpga_path =
-00000220: 206f 732e 7061 7468 2e6a 6f69 6e28 7365   os.path.join(se
-00000230: 6c66 2e6c 6f63 616c 5f66 7470 5f70 6174  lf.local_ftp_pat
-00000240: 682c 2022 6670 6761 2229 0d0a 2020 2020  h, "fpga")..    
-00000250: 2020 2020 7365 6c66 2e6c 6f63 616c 5f66      self.local_f
-00000260: 775f 7061 7468 203d 206f 732e 7061 7468  w_path = os.path
-00000270: 2e6a 6f69 6e28 7365 6c66 2e6c 6f63 616c  .join(self.local
-00000280: 5f66 7470 5f70 6174 682c 2022 6669 726d  _ftp_path, "firm
-00000290: 7761 7265 2229 0d0a 2020 2020 2020 2020  ware")..        
-000002a0: 7365 6c66 2e67 6974 5f75 726c 203d 2022  self.git_url = "
-000002b0: 6874 7470 733a 2f2f 6769 742e 636e 6578  https://git.cnex
-000002c0: 6c61 6273 2e63 6f6d 2f63 6e65 782d 6669  labs.com/cnex-fi
-000002d0: 726d 7761 7265 2f74 6168 6f65 5f66 772e  rmware/tahoe_fw.
-000002e0: 6769 7422 0d0a 2020 2020 2020 2020 7365  git"..        se
-000002f0: 6c66 2e6c 6f63 616c 5f66 775f 706a 5f70  lf.local_fw_pj_p
-00000300: 6174 6820 3d20 7365 6c66 2e67 6574 5f67  ath = self.get_g
-00000310: 6974 5f70 726f 6a65 6374 5f70 6174 6828  it_project_path(
-00000320: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00000330: 696e 6974 5f6c 6f63 616c 5f66 6f6c 6465  init_local_folde
-00000340: 7228 290d 0a0d 0a20 2020 2064 6566 2069  r()....    def i
-00000350: 6e69 745f 6c6f 6361 6c5f 666f 6c64 6572  nit_local_folder
-00000360: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00000370: 2069 6e69 745f 7061 7468 203d 205b 7365   init_path = [se
-00000380: 6c66 2e6c 6f63 616c 5f66 7470 5f70 6174  lf.local_ftp_pat
-00000390: 682c 2073 656c 662e 6c6f 6361 6c5f 6674  h, self.local_ft
-000003a0: 705f 6670 6761 5f70 6174 682c 2073 656c  p_fpga_path, sel
-000003b0: 662e 6c6f 6361 6c5f 6677 5f70 6174 685d  f.local_fw_path]
-000003c0: 0d0a 2020 2020 2020 2020 666f 7220 7465  ..        for te
-000003d0: 6d70 5f70 6174 6820 696e 2069 6e69 745f  mp_path in init_
-000003e0: 7061 7468 3a0d 0a20 2020 2020 2020 2020  path:..         
-000003f0: 2020 2069 6620 6e6f 7420 6f73 2e70 6174     if not os.pat
-00000400: 682e 6578 6973 7473 2874 656d 705f 7061  h.exists(temp_pa
-00000410: 7468 293a 0d0a 2020 2020 2020 2020 2020  th):..          
-00000420: 2020 2020 2020 6f73 2e6d 6b64 6972 2874        os.mkdir(t
-00000430: 656d 705f 7061 7468 290d 0a0d 0a20 2020  emp_path)....   
-00000440: 2040 7374 6174 6963 6d65 7468 6f64 0d0a   @staticmethod..
-00000450: 2020 2020 6465 6620 6973 5f64 6972 6563      def is_direc
-00000460: 746f 7279 2866 7470 2c20 7061 7468 293a  tory(ftp, path):
-00000470: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
-00000480: 2020 2020 2020 2020 2020 2020 6674 702e              ftp.
-00000490: 6377 6428 7061 7468 290d 0a20 2020 2020  cwd(path)..     
-000004a0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-000004b0: 7565 0d0a 2020 2020 2020 2020 6578 6365  ue..        exce
-000004c0: 7074 2066 7470 6c69 622e 6572 726f 725f  pt ftplib.error_
-000004d0: 7065 726d 3a0d 0a20 2020 2020 2020 2020  perm:..         
-000004e0: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
-000004f0: 0a0d 0a20 2020 2040 7374 6174 6963 6d65  ...    @staticme
-00000500: 7468 6f64 0d0a 2020 2020 6465 6620 756e  thod..    def un
-00000510: 7a69 705f 6670 6761 5f66 696c 6528 7a69  zip_fpga_file(zi
-00000520: 705f 7061 7468 293a 0d0a 2020 2020 2020  p_path):..      
-00000530: 2020 7769 7468 2070 7937 7a72 2e53 6576    with py7zr.Sev
-00000540: 656e 5a69 7046 696c 6528 7a69 705f 7061  enZipFile(zip_pa
-00000550: 7468 2c20 6d6f 6465 3d22 7222 2920 6173  th, mode="r") as
-00000560: 207a 3a0d 0a20 2020 2020 2020 2020 2020   z:..           
-00000570: 207a 2e65 7874 7261 6374 616c 6c28 7061   z.extractall(pa
-00000580: 7468 3d6f 732e 7061 7468 2e64 6972 6e61  th=os.path.dirna
-00000590: 6d65 287a 6970 5f70 6174 6829 290d 0a20  me(zip_path)).. 
-000005a0: 2020 2020 2020 2075 6e7a 6970 5f66 6f6c         unzip_fol
-000005b0: 6465 7220 3d20 6f73 2e70 6174 682e 7370  der = os.path.sp
-000005c0: 6c69 7465 7874 286f 732e 7061 7468 2e62  litext(os.path.b
-000005d0: 6173 656e 616d 6528 7a69 705f 7061 7468  asename(zip_path
-000005e0: 2929 5b30 5d0d 0a20 2020 2020 2020 2075  ))[0]..        u
-000005f0: 6e7a 6970 5f66 6f6c 6465 725f 7061 7468  nzip_folder_path
-00000600: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-00000610: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
-00000620: 7a69 705f 7061 7468 292c 2075 6e7a 6970  zip_path), unzip
-00000630: 5f66 6f6c 6465 7229 0d0a 2020 2020 2020  _folder)..      
-00000640: 2020 666f 7220 7465 6d70 2069 6e20 6f73    for temp in os
-00000650: 2e6c 6973 7464 6972 2875 6e7a 6970 5f66  .listdir(unzip_f
-00000660: 6f6c 6465 725f 7061 7468 293a 0d0a 2020  older_path):..  
-00000670: 2020 2020 2020 2020 2020 6966 2074 656d            if tem
-00000680: 702e 656e 6473 7769 7468 2822 2e73 6f66  p.endswith(".sof
-00000690: 2229 3a0d 0a20 2020 2020 2020 2020 2020  "):..           
-000006a0: 2020 2020 2072 6574 7572 6e20 6f73 2e70       return os.p
-000006b0: 6174 682e 6a6f 696e 2875 6e7a 6970 5f66  ath.join(unzip_f
-000006c0: 6f6c 6465 725f 7061 7468 2c20 7465 6d70  older_path, temp
-000006d0: 290d 0a0d 0a20 2020 2064 6566 2066 7470  )....    def ftp
-000006e0: 5f64 6f77 6e6c 6f61 645f 6669 6c65 2873  _download_file(s
-000006f0: 656c 662c 2066 7470 2c20 6670 6761 5f66  elf, ftp, fpga_f
-00000700: 6f6c 6465 722c 2066 7067 615f 6669 6c65  older, fpga_file
-00000710: 293a 0d0a 2020 2020 2020 2020 6c6f 6361  ):..        loca
-00000720: 6c5f 7061 7468 203d 206f 732e 7061 7468  l_path = os.path
-00000730: 2e6a 6f69 6e28 7365 6c66 2e6c 6f63 616c  .join(self.local
-00000740: 5f66 7470 5f66 7067 615f 7061 7468 2c20  _ftp_fpga_path, 
-00000750: 6670 6761 5f66 6f6c 6465 7229 0d0a 2020  fpga_folder)..  
-00000760: 2020 2020 2020 6966 206f 732e 7061 7468        if os.path
-00000770: 2e65 7869 7374 7328 6c6f 6361 6c5f 7061  .exists(local_pa
-00000780: 7468 293a 0d0a 2020 2020 2020 2020 2020  th):..          
-00000790: 2020 7368 7574 696c 2e72 6d74 7265 6528    shutil.rmtree(
-000007a0: 6c6f 6361 6c5f 7061 7468 290d 0a20 2020  local_path)..   
-000007b0: 2020 2020 206f 732e 6d6b 6469 7228 6c6f       os.mkdir(lo
-000007c0: 6361 6c5f 7061 7468 290d 0a20 2020 2020  cal_path)..     
-000007d0: 2020 206c 6f63 616c 5f66 7067 615f 6669     local_fpga_fi
-000007e0: 6c65 203d 206f 732e 7061 7468 2e6a 6f69  le = os.path.joi
-000007f0: 6e28 6c6f 6361 6c5f 7061 7468 2c20 6670  n(local_path, fp
-00000800: 6761 5f66 696c 6529 0d0a 2020 2020 2020  ga_file)..      
-00000810: 2020 7769 7468 206f 7065 6e28 6c6f 6361    with open(loca
-00000820: 6c5f 6670 6761 5f66 696c 652c 2027 7762  l_fpga_file, 'wb
-00000830: 2729 2061 7320 663a 0d0a 2020 2020 2020  ') as f:..      
-00000840: 2020 2020 2020 6674 702e 7265 7472 6269        ftp.retrbi
-00000850: 6e61 7279 2866 2752 4554 5220 7b66 7067  nary(f'RETR {fpg
-00000860: 615f 6669 6c65 7d27 2c20 662e 7772 6974  a_file}', f.writ
-00000870: 6529 0d0a 2020 2020 2020 2020 7265 7475  e)..        retu
-00000880: 726e 206c 6f63 616c 5f66 7067 615f 6669  rn local_fpga_fi
-00000890: 6c65 0d0a 0d0a 2020 2020 6465 6620 5f67  le....    def _g
-000008a0: 6574 5f66 696c 655f 6e61 6d65 2873 656c  et_file_name(sel
-000008b0: 662c 2066 7470 293a 0d0a 2020 2020 2020  f, ftp):..      
-000008c0: 2020 6670 6761 5f66 696c 6520 3d20 4e6f    fpga_file = No
-000008d0: 6e65 0d0a 2020 2020 2020 2020 6669 6c65  ne..        file
-000008e0: 6e61 6d65 7320 3d20 6674 702e 6e6c 7374  names = ftp.nlst
-000008f0: 2829 0d0a 2020 2020 2020 2020 666f 7220  ()..        for 
-00000900: 6669 6c65 5f20 696e 2066 696c 656e 616d  file_ in filenam
-00000910: 6573 3a0d 0a20 2020 2020 2020 2020 2020  es:..           
-00000920: 2069 6620 7365 6c66 2e66 7470 5f70 6174   if self.ftp_pat
-00000930: 7465 6e20 696e 2066 696c 655f 3a0d 0a20  ten in file_:.. 
-00000940: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00000950: 7067 615f 6669 6c65 203d 2066 696c 655f  pga_file = file_
-00000960: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000970: 2020 6272 6561 6b0d 0a20 2020 2020 2020    break..       
-00000980: 2072 6574 7572 6e20 6670 6761 5f66 696c   return fpga_fil
-00000990: 650d 0a0d 0a20 2020 2064 6566 2073 706c  e....    def spl
-000009a0: 6974 5f70 6174 685f 666f 6c64 6572 5f66  it_path_folder_f
-000009b0: 696c 6528 7365 6c66 2c20 6674 702c 2066  ile(self, ftp, f
-000009c0: 7470 5f70 6174 6829 3a0d 0a20 2020 2020  tp_path):..     
-000009d0: 2020 2066 7470 5f70 6174 6820 3d20 6674     ftp_path = ft
-000009e0: 705f 7061 7468 2e72 6570 6c61 6365 2866  p_path.replace(f
-000009f0: 2266 7470 3a2f 2f7b 7365 6c66 2e69 635f  "ftp://{self.ic_
-00000a00: 6674 707d 2f22 2c20 2222 290d 0a20 2020  ftp}/", "")..   
-00000a10: 2020 2020 2073 706c 6974 5f70 6174 6873       split_paths
-00000a20: 203d 2066 7470 5f70 6174 682e 7370 6c69   = ftp_path.spli
-00000a30: 7428 222f 2229 0d0a 2020 2020 2020 2020  t("/")..        
-00000a40: 6966 206e 6f74 2073 656c 662e 6973 5f64  if not self.is_d
-00000a50: 6972 6563 746f 7279 2866 7470 2c20 6674  irectory(ftp, ft
-00000a60: 705f 7061 7468 293a 0d0a 2020 2020 2020  p_path):..      
-00000a70: 2020 2020 2020 6670 6761 5f66 696c 6520        fpga_file 
-00000a80: 3d20 7370 6c69 745f 7061 7468 735b 2d31  = split_paths[-1
-00000a90: 5d0d 0a20 2020 2020 2020 2020 2020 2066  ]..            f
-00000aa0: 7067 615f 666f 6c64 6572 203d 2073 706c  pga_folder = spl
-00000ab0: 6974 5f70 6174 6873 5b2d 325d 0d0a 2020  it_paths[-2]..  
-00000ac0: 2020 2020 2020 2020 2020 6674 702e 6377            ftp.cw
-00000ad0: 6428 6f73 2e70 6174 682e 6469 726e 616d  d(os.path.dirnam
-00000ae0: 6528 6674 705f 7061 7468 2929 0d0a 2020  e(ftp_path))..  
-00000af0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00000b00: 2020 2020 2020 2020 2066 7067 615f 666f           fpga_fo
-00000b10: 6c64 6572 203d 2073 706c 6974 5f70 6174  lder = split_pat
-00000b20: 6873 5b2d 315d 2069 6620 7370 6c69 745f  hs[-1] if split_
-00000b30: 7061 7468 735b 2d31 5d20 213d 2022 2220  paths[-1] != "" 
-00000b40: 656c 7365 2073 706c 6974 5f70 6174 6873  else split_paths
-00000b50: 5b2d 325d 0d0a 2020 2020 2020 2020 2020  [-2]..          
-00000b60: 2020 6670 6761 5f66 696c 6520 3d20 7365    fpga_file = se
-00000b70: 6c66 2e5f 6765 745f 6669 6c65 5f6e 616d  lf._get_file_nam
-00000b80: 6528 6674 7029 0d0a 2020 2020 2020 2020  e(ftp)..        
-00000b90: 7265 7475 726e 2066 7067 615f 666f 6c64  return fpga_fold
-00000ba0: 6572 2c20 6670 6761 5f66 696c 650d 0a0d  er, fpga_file...
-00000bb0: 0a20 2020 2064 6566 2067 6574 5f66 7067  .    def get_fpg
-00000bc0: 615f 6672 6f6d 5f66 7470 2873 656c 662c  a_from_ftp(self,
-00000bd0: 2066 7470 5f70 6174 6829 3a0d 0a20 2020   ftp_path):..   
-00000be0: 2020 2020 206c 6f67 2e49 4e46 4f28 6622       log.INFO(f"
-00000bf0: 4265 6769 6e20 746f 2067 6574 2073 6f66  Begin to get sof
-00000c00: 2066 726f 6d20 7b66 7470 5f70 6174 687d   from {ftp_path}
-00000c10: 2229 0d0a 2020 2020 2020 2020 6674 7020  ")..        ftp 
-00000c20: 3d20 6674 706c 6962 2e46 5450 2873 656c  = ftplib.FTP(sel
-00000c30: 662e 6963 5f66 7470 2c20 7365 6c66 2e69  f.ic_ftp, self.i
-00000c40: 635f 6674 705f 7573 6572 2c20 7365 6c66  c_ftp_user, self
-00000c50: 2e69 635f 6674 705f 7077 6429 0d0a 2020  .ic_ftp_pwd)..  
-00000c60: 2020 2020 2020 6670 6761 5f66 6f6c 6465        fpga_folde
-00000c70: 722c 2066 7067 615f 6669 6c65 203d 2073  r, fpga_file = s
-00000c80: 656c 662e 7370 6c69 745f 7061 7468 5f66  elf.split_path_f
-00000c90: 6f6c 6465 725f 6669 6c65 2866 7470 2c20  older_file(ftp, 
-00000ca0: 6674 705f 7061 7468 290d 0a20 2020 2020  ftp_path)..     
-00000cb0: 2020 2064 6c5f 6670 6761 5f70 6174 6820     dl_fpga_path 
-00000cc0: 3d20 7365 6c66 2e66 7470 5f64 6f77 6e6c  = self.ftp_downl
-00000cd0: 6f61 645f 6669 6c65 2866 7470 2c20 6670  oad_file(ftp, fp
-00000ce0: 6761 5f66 6f6c 6465 722c 2066 7067 615f  ga_folder, fpga_
-00000cf0: 6669 6c65 290d 0a20 2020 2020 2020 2073  file)..        s
-00000d00: 6f66 5f66 696c 6520 3d20 7365 6c66 2e75  of_file = self.u
-00000d10: 6e7a 6970 5f66 7067 615f 6669 6c65 2864  nzip_fpga_file(d
-00000d20: 6c5f 6670 6761 5f70 6174 6829 0d0a 2020  l_fpga_path)..  
-00000d30: 2020 2020 2020 6c6f 672e 494e 464f 2866        log.INFO(f
-00000d40: 2247 6574 2073 6f66 207b 736f 665f 6669  "Get sof {sof_fi
-00000d50: 6c65 7d20 6672 6f6d 2066 7470 2229 0d0a  le} from ftp")..
-00000d60: 2020 2020 2020 2020 6674 702e 7175 6974          ftp.quit
-00000d70: 2829 0d0a 2020 2020 2020 2020 6966 2073  ()..        if s
-00000d80: 6f66 5f66 696c 6520 6973 204e 6f6e 653a  of_file is None:
-00000d90: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-00000da0: 6973 6520 5275 6e74 696d 6545 7272 6f72  ise RuntimeError
-00000db0: 2866 2273 6f66 5f66 696c 6520 6765 7420  (f"sof_file get 
-00000dc0: 6661 696c 6564 3a20 7b66 7470 5f70 6174  failed: {ftp_pat
-00000dd0: 687d 2229 0d0a 2020 2020 2020 2020 7265  h}")..        re
-00000de0: 7475 726e 2073 6f66 5f66 696c 650d 0a0d  turn sof_file...
-00000df0: 0a20 2020 2064 6566 2067 6574 5f67 6974  .    def get_git
-00000e00: 5f70 726f 6a65 6374 5f70 6174 6828 7365  _project_path(se
-00000e10: 6c66 293a 0d0a 2020 2020 2020 2020 6261  lf):..        ba
-00000e20: 7365 6e61 6d65 203d 206f 732e 7061 7468  sename = os.path
-00000e30: 2e62 6173 656e 616d 6528 7365 6c66 2e67  .basename(self.g
-00000e40: 6974 5f75 726c 290d 0a20 2020 2020 2020  it_url)..       
-00000e50: 2066 6f6c 6465 725f 6e61 6d65 203d 206f   folder_name = o
-00000e60: 732e 7061 7468 2e73 706c 6974 6578 7428  s.path.splitext(
-00000e70: 6261 7365 6e61 6d65 295b 305d 0d0a 2020  basename)[0]..  
-00000e80: 2020 2020 2020 7265 7475 726e 206f 732e        return os.
-00000e90: 7061 7468 2e6a 6f69 6e28 7365 6c66 2e6c  path.join(self.l
-00000ea0: 6f63 616c 5f66 775f 7061 7468 2c20 666f  ocal_fw_path, fo
-00000eb0: 6c64 6572 5f6e 616d 6529 0d0a 0d0a 2020  lder_name)....  
-00000ec0: 2020 6465 6620 7570 6461 7465 5f66 775f    def update_fw_
-00000ed0: 636f 6465 2873 656c 662c 2062 7261 6e63  code(self, branc
-00000ee0: 6829 3a0d 0a20 2020 2020 2020 206c 6f63  h):..        loc
-00000ef0: 616c 5f66 775f 7061 7468 203d 2073 656c  al_fw_path = sel
-00000f00: 662e 6c6f 6361 6c5f 6677 5f70 6a5f 7061  f.local_fw_pj_pa
-00000f10: 7468 2069 6620 6f73 2e70 6174 682e 6578  th if os.path.ex
-00000f20: 6973 7473 2873 656c 662e 6c6f 6361 6c5f  ists(self.local_
-00000f30: 6677 5f70 6a5f 7061 7468 2920 656c 7365  fw_pj_path) else
-00000f40: 2073 656c 662e 6c6f 6361 6c5f 6677 5f70   self.local_fw_p
-00000f50: 6174 680d 0a20 2020 2020 2020 2067 6974  ath..        git
-00000f60: 203d 2047 6974 4f70 6572 6174 6f72 2822   = GitOperator("
-00000f70: 7368 616f 6269 6e2e 7368 7522 2c20 2243  shaobin.shu", "C
-00000f80: 6e65 7821 3230 3234 222c 206c 6f63 616c  nex!2024", local
-00000f90: 5f66 775f 7061 7468 290d 0a20 2020 2020  _fw_path)..     
-00000fa0: 2020 2069 6620 6f73 2e70 6174 682e 6578     if os.path.ex
-00000fb0: 6973 7473 2873 656c 662e 6c6f 6361 6c5f  ists(self.local_
-00000fc0: 6677 5f70 6a5f 7061 7468 293a 0d0a 2020  fw_pj_path):..  
-00000fd0: 2020 2020 2020 2020 2020 6e65 775f 6d73            new_ms
-00000fe0: 672c 2072 6574 203d 2067 6974 2e75 7064  g, ret = git.upd
-00000ff0: 6174 655f 6c61 7465 7374 5f63 6f64 6528  ate_latest_code(
-00001000: 6622 6f72 6967 696e 2f7b 6272 616e 6368  f"origin/{branch
-00001010: 7d22 290d 0a20 2020 2020 2020 2020 2020  }")..           
-00001020: 2069 6620 7265 7420 213d 2030 3a0d 0a20   if ret != 0:.. 
-00001030: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00001040: 6169 7365 2052 756e 7469 6d65 4572 726f  aise RuntimeErro
-00001050: 7228 6622 4769 7420 7570 6461 7465 2066  r(f"Git update f
-00001060: 6169 6c65 642c 2075 726c 3a7b 7365 6c66  ailed, url:{self
-00001070: 2e67 6974 5f75 726c 7d20 6272 616e 6368  .git_url} branch
-00001080: 3a7b 6272 616e 6368 7d22 290d 0a20 2020  :{branch}")..   
-00001090: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-000010a0: 2020 2020 2020 2020 6966 2067 6974 2e63          if git.c
-000010b0: 6c6f 6e65 2873 656c 662e 6769 745f 7572  lone(self.git_ur
-000010c0: 6c2c 2066 226f 7269 6769 6e2f 7b62 7261  l, f"origin/{bra
-000010d0: 6e63 687d 2229 2021 3d20 303a 0d0a 2020  nch}") != 0:..  
-000010e0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-000010f0: 6973 6520 5275 6e74 696d 6545 7272 6f72  ise RuntimeError
-00001100: 2866 2247 6974 2063 6c6f 6e65 2066 6169  (f"Git clone fai
-00001110: 6c65 642c 2075 726c 3a7b 7365 6c66 2e67  led, url:{self.g
-00001120: 6974 5f75 726c 7d20 6272 616e 6368 3a7b  it_url} branch:{
-00001130: 6272 616e 6368 7d22 290d 0a0d 0a20 2020  branch}")....   
-00001140: 2064 6566 2063 6f70 795f 736f 665f 325f   def copy_sof_2_
-00001150: 6677 2873 656c 662c 2073 7263 5f73 6f66  fw(self, src_sof
-00001160: 293a 0d0a 2020 2020 2020 2020 6473 745f  ):..        dst_
-00001170: 736f 6620 3d20 6f73 2e70 6174 682e 6a6f  sof = os.path.jo
-00001180: 696e 2873 656c 662e 6c6f 6361 6c5f 6677  in(self.local_fw
-00001190: 5f70 6a5f 7061 7468 2c20 2274 6168 6f65  _pj_path, "tahoe
-000011a0: 2e73 6f66 2229 0d0a 2020 2020 2020 2020  .sof")..        
-000011b0: 6966 206f 732e 7061 7468 2e65 7869 7374  if os.path.exist
-000011c0: 7328 6473 745f 736f 6629 3a0d 0a20 2020  s(dst_sof):..   
-000011d0: 2020 2020 2020 2020 206f 732e 7265 6d6f           os.remo
-000011e0: 7665 2864 7374 5f73 6f66 290d 0a20 2020  ve(dst_sof)..   
-000011f0: 2020 2020 2073 6875 7469 6c2e 636f 7079       shutil.copy
-00001200: 2873 7263 5f73 6f66 2c20 6473 745f 736f  (src_sof, dst_so
-00001210: 6629 0d0a 0d0a 2020 2020 6465 6620 6c6f  f)....    def lo
-00001220: 6164 5f61 6c6c 2873 656c 6629 3a0d 0a20  ad_all(self):.. 
-00001230: 2020 2020 2020 2063 6d64 203d 2066 2263         cmd = f"c
-00001240: 6420 2f64 207b 7365 6c66 2e6c 6f63 616c  d /d {self.local
-00001250: 5f66 775f 706a 5f70 6174 687d 2026 2620  _fw_pj_path} && 
-00001260: 6c6f 6164 5f61 6c6c 2e62 6174 220d 0a20  load_all.bat".. 
-00001270: 2020 2020 2020 206c 6f67 2e49 4e46 4f28         log.INFO(
-00001280: 6622 7570 6772 6164 6520 6c6f 6769 6320  f"upgrade logic 
-00001290: 616e 6420 6669 726d 7761 7265 2077 6974  and firmware wit
-000012a0: 6820 636d 643a 207b 636d 647d 2229 0d0a  h cmd: {cmd}")..
-000012b0: 2020 2020 2020 2020 7265 7420 3d20 6f73          ret = os
-000012c0: 2e73 7973 7465 6d28 636d 6429 0d0a 2020  .system(cmd)..  
-000012d0: 2020 2020 2020 6966 2072 6574 2021 3d20        if ret != 
-000012e0: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
-000012f0: 7261 6973 6520 5275 6e74 696d 6545 7272  raise RuntimeErr
-00001300: 6f72 2822 6c6f 6164 5f61 6c6c 2066 6169  or("load_all fai
-00001310: 6c65 6422 290d 0a20 2020 2020 2020 2074  led")..        t
-00001320: 696d 652e 736c 6565 7028 3630 290d 0a0d  ime.sleep(60)...
-00001330: 0a20 2020 2064 6566 2069 6e73 6d6f 645f  .    def insmod_
-00001340: 6b6f 2873 656c 662c 2073 7368 2c20 7665  ko(self, ssh, ve
-00001350: 6e75 7329 3a0d 0a20 2020 2020 2020 206b  nus):..        k
-00001360: 6f5f 7061 7468 203d 2066 227b 7665 6e75  o_path = f"{venu
-00001370: 737d 2f62 696e 2f74 6168 6f65 2f71 615f  s}/bin/tahoe/qa_
-00001380: 6d6f 6465 220d 0a20 2020 2020 2020 2063  mode"..        c
-00001390: 6d64 203d 2066 2263 6420 7b6b 6f5f 7061  md = f"cd {ko_pa
-000013a0: 7468 7d20 2626 2069 6e73 6d6f 6420 6e65  th} && insmod ne
-000013b0: 7875 732e 6b6f 2026 2620 696e 736d 6f64  xus.ko && insmod
-000013c0: 206b 7465 7374 2e6b 6f22 0d0a 2020 2020   ktest.ko"..    
-000013d0: 2020 2020 7374 6174 7573 2c20 6f75 7470      status, outp
-000013e0: 7574 203d 2073 7368 2e63 6f6d 6d61 6e64  ut = ssh.command
-000013f0: 2863 6d64 290d 0a20 2020 2020 2020 2069  (cmd)..        i
-00001400: 6620 7374 6174 7573 2021 3d20 303a 0d0a  f status != 0:..
-00001410: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00001420: 6520 5275 6e74 696d 6545 7272 6f72 2866  e RuntimeError(f
-00001430: 2269 6e73 6d6f 6420 6661 696c 6564 2c20  "insmod failed, 
-00001440: 636d 643a 207b 636d 647d 2e20 4f75 7470  cmd: {cmd}. Outp
-00001450: 7574 3a7b 6f75 7470 7574 7d22 290d 0a0d  ut:{output}")...
-00001460: 0a20 2020 2064 6566 2072 6562 6f6f 745f  .    def reboot_
-00001470: 6c69 6e75 7828 7365 6c66 2c20 6c69 6e75  linux(self, linu
-00001480: 782c 2075 7365 722c 2070 7764 2c20 7665  x, user, pwd, ve
-00001490: 6e75 735f 7061 7468 293a 0d0a 2020 2020  nus_path):..    
-000014a0: 2020 2020 7373 6820 3d20 5353 4828 6c69      ssh = SSH(li
-000014b0: 6e75 782c 2075 7365 726e 616d 653d 7573  nux, username=us
-000014c0: 6572 2c20 7061 7373 776f 7264 3d70 7764  er, password=pwd
-000014d0: 290d 0a20 2020 2020 2020 2073 7368 2e6f  )..        ssh.o
-000014e0: 7065 6e28 290d 0a20 2020 2020 2020 2073  pen()..        s
-000014f0: 7368 2e63 6f6d 6d61 6e64 5f77 6974 686f  sh.command_witho
-00001500: 7574 5f72 6573 756c 7428 2272 6562 6f6f  ut_result("reboo
-00001510: 7420 2d6e 6622 2c20 7469 6d65 6f75 743d  t -nf", timeout=
-00001520: 3130 290d 0a20 2020 2020 2020 2074 696d  10)..        tim
-00001530: 652e 736c 6565 7028 3630 290d 0a20 2020  e.sleep(60)..   
-00001540: 2020 2020 2073 7368 2e6f 7065 6e28 290d       ssh.open().
-00001550: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
-00001560: 736d 6f64 5f6b 6f28 7373 682c 2076 656e  smod_ko(ssh, ven
-00001570: 7573 5f70 6174 6829 0d0a 0d0a 2020 2020  us_path)....    
-00001580: 4073 7461 7469 636d 6574 686f 640d 0a20  @staticmethod.. 
-00001590: 2020 2064 6566 2063 6c65 6172 5f75 6172     def clear_uar
-000015a0: 7428 636f 6d29 3a0d 0a20 2020 2020 2020  t(com):..       
-000015b0: 2073 6572 203d 2043 6e65 7853 6572 6961   ser = CnexSeria
-000015c0: 6c28 636f 6d29 0d0a 2020 2020 2020 2020  l(com)..        
-000015d0: 7365 722e 636c 6f73 655f 7474 6572 6d70  ser.close_ttermp
-000015e0: 726f 2829 0d0a 2020 2020 2020 2020 7469  ro()..        ti
-000015f0: 6d65 2e73 6c65 6570 2832 290d 0a20 2020  me.sleep(2)..   
-00001600: 2020 2020 2073 6572 2e63 6c65 6172 7370       ser.clearsp
-00001610: 6931 2829 0d0a 2020 2020 2020 2020 7469  i1()..        ti
-00001620: 6d65 2e73 6c65 6570 2832 290d 0a20 2020  me.sleep(2)..   
-00001630: 2020 2020 2073 6572 2e6f 7065 6e5f 7474       ser.open_tt
-00001640: 6572 6d70 726f 2829 0d0a 0d0a 2020 2020  ermpro()....    
-00001650: 4064 6563 6f72 6174 655f 6578 6365 7074  @decorate_except
-00001660: 696f 6e5f 7265 7375 6c74 0d0a 2020 2020  ion_result..    
-00001670: 6465 6620 7275 6e28 7365 6c66 2c20 7061  def run(self, pa
-00001680: 7261 293a 0d0a 2020 2020 2020 2020 6c6f  ra):..        lo
-00001690: 672e 494e 464f 2822 4265 6769 6e20 746f  g.INFO("Begin to
-000016a0: 2064 6f77 6e6c 6f61 6420 6c6f 6769 6320   download logic 
-000016b0: 616e 6420 6669 726d 7761 7265 2229 0d0a  and firmware")..
-000016c0: 2020 2020 2020 2020 7372 635f 736f 6620          src_sof 
-000016d0: 3d20 7365 6c66 2e67 6574 5f66 7067 615f  = self.get_fpga_
-000016e0: 6672 6f6d 5f66 7470 2870 6172 615b 2269  from_ftp(para["i
-000016f0: 635f 6c6f 6769 6322 5d29 0d0a 2020 2020  c_logic"])..    
-00001700: 2020 2020 7365 6c66 2e75 7064 6174 655f      self.update_
-00001710: 6677 5f63 6f64 6528 7061 7261 5b22 6963  fw_code(para["ic
-00001720: 5f66 775f 6272 616e 6368 225d 290d 0a20  _fw_branch"]).. 
-00001730: 2020 2020 2020 2073 656c 662e 636c 6561         self.clea
-00001740: 725f 7561 7274 2870 6172 615b 2263 6f6d  r_uart(para["com
-00001750: 225d 290d 0a20 2020 2020 2020 2073 656c  "])..        sel
-00001760: 662e 636f 7079 5f73 6f66 5f32 5f66 7728  f.copy_sof_2_fw(
-00001770: 7372 635f 736f 6629 0d0a 2020 2020 2020  src_sof)..      
-00001780: 2020 7365 6c66 2e6c 6f61 645f 616c 6c28    self.load_all(
-00001790: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000017a0: 7265 626f 6f74 5f6c 696e 7578 2870 6172  reboot_linux(par
-000017b0: 615b 2274 6172 6765 745f 6970 225d 2c20  a["target_ip"], 
-000017c0: 7061 7261 5b22 6c69 6e75 785f 7573 6572  para["linux_user
-000017d0: 225d 2c20 7061 7261 5b22 6c69 6e75 785f  "], para["linux_
-000017e0: 7077 6422 5d2c 2070 6172 615b 2277 6f72  pwd"], para["wor
-000017f0: 6b5f 7061 7468 225d 290d 0a20 2020 2020  k_path"])..     
-00001800: 2020 2072 6574 7572 6e20 302c 2022 646f     return 0, "do
-00001810: 776e 6c6f 6164 206c 6f67 6963 2061 6e64  wnload logic and
-00001820: 2066 6972 6d77 6172 6520 7375 6363 6565   firmware succee
-00001830: 6422 0d0a                                d"..
+00000030: 6674 706c 6962 0d0a 6672 6f6d 2074 6f6f  ftplib..from too
+00000040: 6c2e 6769 742e 6769 745f 6f70 6572 6174  l.git.git_operat
+00000050: 6f72 2069 6d70 6f72 7420 4769 744f 7065  or import GitOpe
+00000060: 7261 746f 720d 0a66 726f 6d20 7574 696c  rator..from util
+00000070: 732e 7373 6820 696d 706f 7274 2053 5348  s.ssh import SSH
+00000080: 0d0a 6672 6f6d 2075 7469 6c73 2e73 7973  ..from utils.sys
+00000090: 7465 6d20 696d 706f 7274 2064 6563 6f72  tem import decor
+000000a0: 6174 655f 6578 6365 7074 696f 6e5f 7265  ate_exception_re
+000000b0: 7375 6c74 0d0a 6672 6f6d 2075 7469 6c73  sult..from utils
+000000c0: 2e73 6572 6961 6c5f 746f 6f6c 2069 6d70  .serial_tool imp
+000000d0: 6f72 7420 436e 6578 5365 7269 616c 0d0a  ort CnexSerial..
+000000e0: 6672 6f6d 2075 7469 6c73 2069 6d70 6f72  from utils impor
+000000f0: 7420 6c6f 670d 0a0d 0a0d 0a63 6c61 7373  t log......class
+00000100: 204c 6f67 6963 4657 446f 776e 6c6f 6164   LogicFWDownload
+00000110: 6572 286f 626a 6563 7429 3a0d 0a0d 0a20  er(object):.... 
+00000120: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00000130: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00000140: 7365 6c66 2e69 635f 6674 7020 3d20 2231  self.ic_ftp = "1
+00000150: 3732 2e32 392e 302e 3230 3822 0d0a 2020  72.29.0.208"..  
+00000160: 2020 2020 2020 7365 6c66 2e69 635f 6674        self.ic_ft
+00000170: 705f 7573 6572 203d 2022 6c61 6222 0d0a  p_user = "lab"..
+00000180: 2020 2020 2020 2020 7365 6c66 2e69 635f          self.ic_
+00000190: 6674 705f 7077 6420 3d20 226c 6162 220d  ftp_pwd = "lab".
+000001a0: 0a20 2020 2020 2020 2073 656c 662e 6674  .        self.ft
+000001b0: 705f 7061 7474 656e 203d 2022 6670 6761  p_patten = "fpga
+000001c0: 2e37 7a22 0d0a 2020 2020 2020 2020 7365  .7z"..        se
+000001d0: 6c66 2e6c 6f63 616c 5f66 7470 5f70 6174  lf.local_ftp_pat
+000001e0: 6820 3d20 7222 433a 5c70 7275 6e22 0d0a  h = r"C:\prun"..
+000001f0: 2020 2020 2020 2020 7365 6c66 2e6c 6f63          self.loc
+00000200: 616c 5f66 7470 5f66 7067 615f 7061 7468  al_ftp_fpga_path
+00000210: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+00000220: 7365 6c66 2e6c 6f63 616c 5f66 7470 5f70  self.local_ftp_p
+00000230: 6174 682c 2022 6670 6761 2229 0d0a 2020  ath, "fpga")..  
+00000240: 2020 2020 2020 7365 6c66 2e6c 6f63 616c        self.local
+00000250: 5f66 775f 7061 7468 203d 206f 732e 7061  _fw_path = os.pa
+00000260: 7468 2e6a 6f69 6e28 7365 6c66 2e6c 6f63  th.join(self.loc
+00000270: 616c 5f66 7470 5f70 6174 682c 2022 6669  al_ftp_path, "fi
+00000280: 726d 7761 7265 2229 0d0a 2020 2020 2020  rmware")..      
+00000290: 2020 7365 6c66 2e67 6974 5f75 726c 203d    self.git_url =
+000002a0: 2022 6874 7470 733a 2f2f 6769 742e 636e   "https://git.cn
+000002b0: 6578 6c61 6273 2e63 6f6d 2f63 6e65 782d  exlabs.com/cnex-
+000002c0: 6669 726d 7761 7265 2f74 6168 6f65 5f66  firmware/tahoe_f
+000002d0: 772e 6769 7422 0d0a 2020 2020 2020 2020  w.git"..        
+000002e0: 7365 6c66 2e6c 6f63 616c 5f66 775f 706a  self.local_fw_pj
+000002f0: 5f70 6174 6820 3d20 7365 6c66 2e67 6574  _path = self.get
+00000300: 5f67 6974 5f70 726f 6a65 6374 5f70 6174  _git_project_pat
+00000310: 6828 290d 0a20 2020 2020 2020 2073 656c  h()..        sel
+00000320: 662e 696e 6974 5f6c 6f63 616c 5f66 6f6c  f.init_local_fol
+00000330: 6465 7228 290d 0a0d 0a20 2020 2064 6566  der()....    def
+00000340: 2069 6e69 745f 6c6f 6361 6c5f 666f 6c64   init_local_fold
+00000350: 6572 2873 656c 6629 3a0d 0a20 2020 2020  er(self):..     
+00000360: 2020 2069 6e69 745f 7061 7468 203d 205b     init_path = [
+00000370: 7365 6c66 2e6c 6f63 616c 5f66 7470 5f70  self.local_ftp_p
+00000380: 6174 682c 2073 656c 662e 6c6f 6361 6c5f  ath, self.local_
+00000390: 6674 705f 6670 6761 5f70 6174 682c 2073  ftp_fpga_path, s
+000003a0: 656c 662e 6c6f 6361 6c5f 6677 5f70 6174  elf.local_fw_pat
+000003b0: 685d 0d0a 2020 2020 2020 2020 666f 7220  h]..        for 
+000003c0: 7465 6d70 5f70 6174 6820 696e 2069 6e69  temp_path in ini
+000003d0: 745f 7061 7468 3a0d 0a20 2020 2020 2020  t_path:..       
+000003e0: 2020 2020 2069 6620 6e6f 7420 6f73 2e70       if not os.p
+000003f0: 6174 682e 6578 6973 7473 2874 656d 705f  ath.exists(temp_
+00000400: 7061 7468 293a 0d0a 2020 2020 2020 2020  path):..        
+00000410: 2020 2020 2020 2020 6f73 2e6d 6b64 6972          os.mkdir
+00000420: 2874 656d 705f 7061 7468 290d 0a0d 0a20  (temp_path).... 
+00000430: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+00000440: 0d0a 2020 2020 6465 6620 6973 5f64 6972  ..    def is_dir
+00000450: 6563 746f 7279 2866 7470 2c20 7061 7468  ectory(ftp, path
+00000460: 293a 0d0a 2020 2020 2020 2020 7472 793a  ):..        try:
+00000470: 0d0a 2020 2020 2020 2020 2020 2020 6674  ..            ft
+00000480: 702e 6377 6428 7061 7468 290d 0a20 2020  p.cwd(path)..   
+00000490: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000004a0: 5472 7565 0d0a 2020 2020 2020 2020 6578  True..        ex
+000004b0: 6365 7074 2066 7470 6c69 622e 6572 726f  cept ftplib.erro
+000004c0: 725f 7065 726d 3a0d 0a20 2020 2020 2020  r_perm:..       
+000004d0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+000004e0: 650d 0a0d 0a20 2020 2040 7374 6174 6963  e....    @static
+000004f0: 6d65 7468 6f64 0d0a 2020 2020 6465 6620  method..    def 
+00000500: 756e 7a69 705f 6670 6761 5f66 696c 6528  unzip_fpga_file(
+00000510: 7a69 705f 7061 7468 293a 0d0a 2020 2020  zip_path):..    
+00000520: 2020 2020 696d 706f 7274 2070 7937 7a72      import py7zr
+00000530: 0d0a 2020 2020 2020 2020 7769 7468 2070  ..        with p
+00000540: 7937 7a72 2e53 6576 656e 5a69 7046 696c  y7zr.SevenZipFil
+00000550: 6528 7a69 705f 7061 7468 2c20 6d6f 6465  e(zip_path, mode
+00000560: 3d22 7222 2920 6173 207a 3a0d 0a20 2020  ="r") as z:..   
+00000570: 2020 2020 2020 2020 207a 2e65 7874 7261           z.extra
+00000580: 6374 616c 6c28 7061 7468 3d6f 732e 7061  ctall(path=os.pa
+00000590: 7468 2e64 6972 6e61 6d65 287a 6970 5f70  th.dirname(zip_p
+000005a0: 6174 6829 290d 0a20 2020 2020 2020 2075  ath))..        u
+000005b0: 6e7a 6970 5f66 6f6c 6465 7220 3d20 6f73  nzip_folder = os
+000005c0: 2e70 6174 682e 7370 6c69 7465 7874 286f  .path.splitext(o
+000005d0: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
+000005e0: 7a69 705f 7061 7468 2929 5b30 5d0d 0a20  zip_path))[0].. 
+000005f0: 2020 2020 2020 2075 6e7a 6970 5f66 6f6c         unzip_fol
+00000600: 6465 725f 7061 7468 203d 206f 732e 7061  der_path = os.pa
+00000610: 7468 2e6a 6f69 6e28 6f73 2e70 6174 682e  th.join(os.path.
+00000620: 6469 726e 616d 6528 7a69 705f 7061 7468  dirname(zip_path
+00000630: 292c 2075 6e7a 6970 5f66 6f6c 6465 7229  ), unzip_folder)
+00000640: 0d0a 2020 2020 2020 2020 666f 7220 7465  ..        for te
+00000650: 6d70 2069 6e20 6f73 2e6c 6973 7464 6972  mp in os.listdir
+00000660: 2875 6e7a 6970 5f66 6f6c 6465 725f 7061  (unzip_folder_pa
+00000670: 7468 293a 0d0a 2020 2020 2020 2020 2020  th):..          
+00000680: 2020 6966 2074 656d 702e 656e 6473 7769    if temp.endswi
+00000690: 7468 2822 2e73 6f66 2229 3a0d 0a20 2020  th(".sof"):..   
+000006a0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000006b0: 7572 6e20 6f73 2e70 6174 682e 6a6f 696e  urn os.path.join
+000006c0: 2875 6e7a 6970 5f66 6f6c 6465 725f 7061  (unzip_folder_pa
+000006d0: 7468 2c20 7465 6d70 290d 0a0d 0a20 2020  th, temp)....   
+000006e0: 2064 6566 2066 7470 5f64 6f77 6e6c 6f61   def ftp_downloa
+000006f0: 645f 6669 6c65 2873 656c 662c 2066 7470  d_file(self, ftp
+00000700: 2c20 6670 6761 5f66 6f6c 6465 722c 2066  , fpga_folder, f
+00000710: 7067 615f 6669 6c65 293a 0d0a 2020 2020  pga_file):..    
+00000720: 2020 2020 6c6f 6361 6c5f 7061 7468 203d      local_path =
+00000730: 206f 732e 7061 7468 2e6a 6f69 6e28 7365   os.path.join(se
+00000740: 6c66 2e6c 6f63 616c 5f66 7470 5f66 7067  lf.local_ftp_fpg
+00000750: 615f 7061 7468 2c20 6670 6761 5f66 6f6c  a_path, fpga_fol
+00000760: 6465 7229 0d0a 2020 2020 2020 2020 6966  der)..        if
+00000770: 206f 732e 7061 7468 2e65 7869 7374 7328   os.path.exists(
+00000780: 6c6f 6361 6c5f 7061 7468 293a 0d0a 2020  local_path):..  
+00000790: 2020 2020 2020 2020 2020 7368 7574 696c            shutil
+000007a0: 2e72 6d74 7265 6528 6c6f 6361 6c5f 7061  .rmtree(local_pa
+000007b0: 7468 290d 0a20 2020 2020 2020 206f 732e  th)..        os.
+000007c0: 6d6b 6469 7228 6c6f 6361 6c5f 7061 7468  mkdir(local_path
+000007d0: 290d 0a20 2020 2020 2020 206c 6f63 616c  )..        local
+000007e0: 5f66 7067 615f 6669 6c65 203d 206f 732e  _fpga_file = os.
+000007f0: 7061 7468 2e6a 6f69 6e28 6c6f 6361 6c5f  path.join(local_
+00000800: 7061 7468 2c20 6670 6761 5f66 696c 6529  path, fpga_file)
+00000810: 0d0a 2020 2020 2020 2020 7769 7468 206f  ..        with o
+00000820: 7065 6e28 6c6f 6361 6c5f 6670 6761 5f66  pen(local_fpga_f
+00000830: 696c 652c 2027 7762 2729 2061 7320 663a  ile, 'wb') as f:
+00000840: 0d0a 2020 2020 2020 2020 2020 2020 6674  ..            ft
+00000850: 702e 7265 7472 6269 6e61 7279 2866 2752  p.retrbinary(f'R
+00000860: 4554 5220 7b66 7067 615f 6669 6c65 7d27  ETR {fpga_file}'
+00000870: 2c20 662e 7772 6974 6529 0d0a 2020 2020  , f.write)..    
+00000880: 2020 2020 7265 7475 726e 206c 6f63 616c      return local
+00000890: 5f66 7067 615f 6669 6c65 0d0a 0d0a 2020  _fpga_file....  
+000008a0: 2020 6465 6620 5f67 6574 5f66 696c 655f    def _get_file_
+000008b0: 6e61 6d65 2873 656c 662c 2066 7470 293a  name(self, ftp):
+000008c0: 0d0a 2020 2020 2020 2020 6670 6761 5f66  ..        fpga_f
+000008d0: 696c 6520 3d20 4e6f 6e65 0d0a 2020 2020  ile = None..    
+000008e0: 2020 2020 6669 6c65 6e61 6d65 7320 3d20      filenames = 
+000008f0: 6674 702e 6e6c 7374 2829 0d0a 2020 2020  ftp.nlst()..    
+00000900: 2020 2020 666f 7220 6669 6c65 5f20 696e      for file_ in
+00000910: 2066 696c 656e 616d 6573 3a0d 0a20 2020   filenames:..   
+00000920: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00000930: 2e66 7470 5f70 6174 7465 6e20 696e 2066  .ftp_patten in f
+00000940: 696c 655f 3a0d 0a20 2020 2020 2020 2020  ile_:..         
+00000950: 2020 2020 2020 2066 7067 615f 6669 6c65         fpga_file
+00000960: 203d 2066 696c 655f 0d0a 2020 2020 2020   = file_..      
+00000970: 2020 2020 2020 2020 2020 6272 6561 6b0d            break.
+00000980: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000990: 6670 6761 5f66 696c 650d 0a0d 0a20 2020  fpga_file....   
+000009a0: 2064 6566 2073 706c 6974 5f70 6174 685f   def split_path_
+000009b0: 666f 6c64 6572 5f66 696c 6528 7365 6c66  folder_file(self
+000009c0: 2c20 6674 702c 2066 7470 5f70 6174 6829  , ftp, ftp_path)
+000009d0: 3a0d 0a20 2020 2020 2020 2066 7470 5f70  :..        ftp_p
+000009e0: 6174 6820 3d20 6674 705f 7061 7468 2e72  ath = ftp_path.r
+000009f0: 6570 6c61 6365 2866 2266 7470 3a2f 2f7b  eplace(f"ftp://{
+00000a00: 7365 6c66 2e69 635f 6674 707d 2f22 2c20  self.ic_ftp}/", 
+00000a10: 2222 290d 0a20 2020 2020 2020 2073 706c  "")..        spl
+00000a20: 6974 5f70 6174 6873 203d 2066 7470 5f70  it_paths = ftp_p
+00000a30: 6174 682e 7370 6c69 7428 222f 2229 0d0a  ath.split("/")..
+00000a40: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+00000a50: 656c 662e 6973 5f64 6972 6563 746f 7279  elf.is_directory
+00000a60: 2866 7470 2c20 6674 705f 7061 7468 293a  (ftp, ftp_path):
+00000a70: 0d0a 2020 2020 2020 2020 2020 2020 6670  ..            fp
+00000a80: 6761 5f66 696c 6520 3d20 7370 6c69 745f  ga_file = split_
+00000a90: 7061 7468 735b 2d31 5d0d 0a20 2020 2020  paths[-1]..     
+00000aa0: 2020 2020 2020 2066 7067 615f 666f 6c64         fpga_fold
+00000ab0: 6572 203d 2073 706c 6974 5f70 6174 6873  er = split_paths
+00000ac0: 5b2d 325d 0d0a 2020 2020 2020 2020 2020  [-2]..          
+00000ad0: 2020 6674 702e 6377 6428 6f73 2e70 6174    ftp.cwd(os.pat
+00000ae0: 682e 6469 726e 616d 6528 6674 705f 7061  h.dirname(ftp_pa
+00000af0: 7468 2929 0d0a 2020 2020 2020 2020 656c  th))..        el
+00000b00: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00000b10: 2066 7067 615f 666f 6c64 6572 203d 2073   fpga_folder = s
+00000b20: 706c 6974 5f70 6174 6873 5b2d 315d 2069  plit_paths[-1] i
+00000b30: 6620 7370 6c69 745f 7061 7468 735b 2d31  f split_paths[-1
+00000b40: 5d20 213d 2022 2220 656c 7365 2073 706c  ] != "" else spl
+00000b50: 6974 5f70 6174 6873 5b2d 325d 0d0a 2020  it_paths[-2]..  
+00000b60: 2020 2020 2020 2020 2020 6670 6761 5f66            fpga_f
+00000b70: 696c 6520 3d20 7365 6c66 2e5f 6765 745f  ile = self._get_
+00000b80: 6669 6c65 5f6e 616d 6528 6674 7029 0d0a  file_name(ftp)..
+00000b90: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+00000ba0: 7067 615f 666f 6c64 6572 2c20 6670 6761  pga_folder, fpga
+00000bb0: 5f66 696c 650d 0a0d 0a20 2020 2064 6566  _file....    def
+00000bc0: 2067 6574 5f66 7067 615f 6672 6f6d 5f66   get_fpga_from_f
+00000bd0: 7470 2873 656c 662c 2066 7470 5f70 6174  tp(self, ftp_pat
+00000be0: 6829 3a0d 0a20 2020 2020 2020 206c 6f67  h):..        log
+00000bf0: 2e49 4e46 4f28 6622 4265 6769 6e20 746f  .INFO(f"Begin to
+00000c00: 2067 6574 2073 6f66 2066 726f 6d20 7b66   get sof from {f
+00000c10: 7470 5f70 6174 687d 2229 0d0a 2020 2020  tp_path}")..    
+00000c20: 2020 2020 6674 7020 3d20 6674 706c 6962      ftp = ftplib
+00000c30: 2e46 5450 2873 656c 662e 6963 5f66 7470  .FTP(self.ic_ftp
+00000c40: 2c20 7365 6c66 2e69 635f 6674 705f 7573  , self.ic_ftp_us
+00000c50: 6572 2c20 7365 6c66 2e69 635f 6674 705f  er, self.ic_ftp_
+00000c60: 7077 6429 0d0a 2020 2020 2020 2020 6670  pwd)..        fp
+00000c70: 6761 5f66 6f6c 6465 722c 2066 7067 615f  ga_folder, fpga_
+00000c80: 6669 6c65 203d 2073 656c 662e 7370 6c69  file = self.spli
+00000c90: 745f 7061 7468 5f66 6f6c 6465 725f 6669  t_path_folder_fi
+00000ca0: 6c65 2866 7470 2c20 6674 705f 7061 7468  le(ftp, ftp_path
+00000cb0: 290d 0a20 2020 2020 2020 2064 6c5f 6670  )..        dl_fp
+00000cc0: 6761 5f70 6174 6820 3d20 7365 6c66 2e66  ga_path = self.f
+00000cd0: 7470 5f64 6f77 6e6c 6f61 645f 6669 6c65  tp_download_file
+00000ce0: 2866 7470 2c20 6670 6761 5f66 6f6c 6465  (ftp, fpga_folde
+00000cf0: 722c 2066 7067 615f 6669 6c65 290d 0a20  r, fpga_file).. 
+00000d00: 2020 2020 2020 2073 6f66 5f66 696c 6520         sof_file 
+00000d10: 3d20 7365 6c66 2e75 6e7a 6970 5f66 7067  = self.unzip_fpg
+00000d20: 615f 6669 6c65 2864 6c5f 6670 6761 5f70  a_file(dl_fpga_p
+00000d30: 6174 6829 0d0a 2020 2020 2020 2020 6c6f  ath)..        lo
+00000d40: 672e 494e 464f 2866 2247 6574 2073 6f66  g.INFO(f"Get sof
+00000d50: 207b 736f 665f 6669 6c65 7d20 6672 6f6d   {sof_file} from
+00000d60: 2066 7470 2229 0d0a 2020 2020 2020 2020   ftp")..        
+00000d70: 6674 702e 7175 6974 2829 0d0a 2020 2020  ftp.quit()..    
+00000d80: 2020 2020 6966 2073 6f66 5f66 696c 6520      if sof_file 
+00000d90: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
+00000da0: 2020 2020 2020 7261 6973 6520 5275 6e74        raise Runt
+00000db0: 696d 6545 7272 6f72 2866 2273 6f66 5f66  imeError(f"sof_f
+00000dc0: 696c 6520 6765 7420 6661 696c 6564 3a20  ile get failed: 
+00000dd0: 7b66 7470 5f70 6174 687d 2229 0d0a 2020  {ftp_path}")..  
+00000de0: 2020 2020 2020 7265 7475 726e 2073 6f66        return sof
+00000df0: 5f66 696c 650d 0a0d 0a20 2020 2064 6566  _file....    def
+00000e00: 2067 6574 5f67 6974 5f70 726f 6a65 6374   get_git_project
+00000e10: 5f70 6174 6828 7365 6c66 293a 0d0a 2020  _path(self):..  
+00000e20: 2020 2020 2020 6261 7365 6e61 6d65 203d        basename =
+00000e30: 206f 732e 7061 7468 2e62 6173 656e 616d   os.path.basenam
+00000e40: 6528 7365 6c66 2e67 6974 5f75 726c 290d  e(self.git_url).
+00000e50: 0a20 2020 2020 2020 2066 6f6c 6465 725f  .        folder_
+00000e60: 6e61 6d65 203d 206f 732e 7061 7468 2e73  name = os.path.s
+00000e70: 706c 6974 6578 7428 6261 7365 6e61 6d65  plitext(basename
+00000e80: 295b 305d 0d0a 2020 2020 2020 2020 7265  )[0]..        re
+00000e90: 7475 726e 206f 732e 7061 7468 2e6a 6f69  turn os.path.joi
+00000ea0: 6e28 7365 6c66 2e6c 6f63 616c 5f66 775f  n(self.local_fw_
+00000eb0: 7061 7468 2c20 666f 6c64 6572 5f6e 616d  path, folder_nam
+00000ec0: 6529 0d0a 0d0a 2020 2020 6465 6620 7570  e)....    def up
+00000ed0: 6461 7465 5f66 775f 636f 6465 2873 656c  date_fw_code(sel
+00000ee0: 662c 2062 7261 6e63 6829 3a0d 0a20 2020  f, branch):..   
+00000ef0: 2020 2020 206c 6f63 616c 5f66 775f 7061       local_fw_pa
+00000f00: 7468 203d 2073 656c 662e 6c6f 6361 6c5f  th = self.local_
+00000f10: 6677 5f70 6a5f 7061 7468 2069 6620 6f73  fw_pj_path if os
+00000f20: 2e70 6174 682e 6578 6973 7473 2873 656c  .path.exists(sel
+00000f30: 662e 6c6f 6361 6c5f 6677 5f70 6a5f 7061  f.local_fw_pj_pa
+00000f40: 7468 2920 656c 7365 2073 656c 662e 6c6f  th) else self.lo
+00000f50: 6361 6c5f 6677 5f70 6174 680d 0a20 2020  cal_fw_path..   
+00000f60: 2020 2020 2067 6974 203d 2047 6974 4f70       git = GitOp
+00000f70: 6572 6174 6f72 2822 7368 616f 6269 6e2e  erator("shaobin.
+00000f80: 7368 7522 2c20 2243 6e65 7821 3230 3234  shu", "Cnex!2024
+00000f90: 222c 206c 6f63 616c 5f66 775f 7061 7468  ", local_fw_path
+00000fa0: 290d 0a20 2020 2020 2020 2069 6620 6f73  )..        if os
+00000fb0: 2e70 6174 682e 6578 6973 7473 2873 656c  .path.exists(sel
+00000fc0: 662e 6c6f 6361 6c5f 6677 5f70 6a5f 7061  f.local_fw_pj_pa
+00000fd0: 7468 293a 0d0a 2020 2020 2020 2020 2020  th):..          
+00000fe0: 2020 6e65 775f 6d73 672c 2072 6574 203d    new_msg, ret =
+00000ff0: 2067 6974 2e75 7064 6174 655f 6c61 7465   git.update_late
+00001000: 7374 5f63 6f64 6528 6622 6f72 6967 696e  st_code(f"origin
+00001010: 2f7b 6272 616e 6368 7d22 290d 0a20 2020  /{branch}")..   
+00001020: 2020 2020 2020 2020 2069 6620 7265 7420           if ret 
+00001030: 213d 2030 3a0d 0a20 2020 2020 2020 2020  != 0:..         
+00001040: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
+00001050: 7469 6d65 4572 726f 7228 6622 4769 7420  timeError(f"Git 
+00001060: 7570 6461 7465 2066 6169 6c65 642c 2075  update failed, u
+00001070: 726c 3a7b 7365 6c66 2e67 6974 5f75 726c  rl:{self.git_url
+00001080: 7d20 6272 616e 6368 3a7b 6272 616e 6368  } branch:{branch
+00001090: 7d22 290d 0a20 2020 2020 2020 2065 6c73  }")..        els
+000010a0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000010b0: 6966 2067 6974 2e63 6c6f 6e65 2873 656c  if git.clone(sel
+000010c0: 662e 6769 745f 7572 6c2c 2066 226f 7269  f.git_url, f"ori
+000010d0: 6769 6e2f 7b62 7261 6e63 687d 2229 2021  gin/{branch}") !
+000010e0: 3d20 303a 0d0a 2020 2020 2020 2020 2020  = 0:..          
+000010f0: 2020 2020 2020 7261 6973 6520 5275 6e74        raise Runt
+00001100: 696d 6545 7272 6f72 2866 2247 6974 2063  imeError(f"Git c
+00001110: 6c6f 6e65 2066 6169 6c65 642c 2075 726c  lone failed, url
+00001120: 3a7b 7365 6c66 2e67 6974 5f75 726c 7d20  :{self.git_url} 
+00001130: 6272 616e 6368 3a7b 6272 616e 6368 7d22  branch:{branch}"
+00001140: 290d 0a0d 0a20 2020 2064 6566 2063 6f70  )....    def cop
+00001150: 795f 736f 665f 325f 6677 2873 656c 662c  y_sof_2_fw(self,
+00001160: 2073 7263 5f73 6f66 293a 0d0a 2020 2020   src_sof):..    
+00001170: 2020 2020 6473 745f 736f 6620 3d20 6f73      dst_sof = os
+00001180: 2e70 6174 682e 6a6f 696e 2873 656c 662e  .path.join(self.
+00001190: 6c6f 6361 6c5f 6677 5f70 6a5f 7061 7468  local_fw_pj_path
+000011a0: 2c20 2274 6168 6f65 2e73 6f66 2229 0d0a  , "tahoe.sof")..
+000011b0: 2020 2020 2020 2020 6966 206f 732e 7061          if os.pa
+000011c0: 7468 2e65 7869 7374 7328 6473 745f 736f  th.exists(dst_so
+000011d0: 6629 3a0d 0a20 2020 2020 2020 2020 2020  f):..           
+000011e0: 206f 732e 7265 6d6f 7665 2864 7374 5f73   os.remove(dst_s
+000011f0: 6f66 290d 0a20 2020 2020 2020 2073 6875  of)..        shu
+00001200: 7469 6c2e 636f 7079 2873 7263 5f73 6f66  til.copy(src_sof
+00001210: 2c20 6473 745f 736f 6629 0d0a 0d0a 2020  , dst_sof)....  
+00001220: 2020 6465 6620 6c6f 6164 5f61 6c6c 2873    def load_all(s
+00001230: 656c 6629 3a0d 0a20 2020 2020 2020 2063  elf):..        c
+00001240: 6d64 203d 2066 2263 6420 2f64 207b 7365  md = f"cd /d {se
+00001250: 6c66 2e6c 6f63 616c 5f66 775f 706a 5f70  lf.local_fw_pj_p
+00001260: 6174 687d 2026 2620 6c6f 6164 5f61 6c6c  ath} && load_all
+00001270: 2e62 6174 220d 0a20 2020 2020 2020 206c  .bat"..        l
+00001280: 6f67 2e49 4e46 4f28 6622 7570 6772 6164  og.INFO(f"upgrad
+00001290: 6520 6c6f 6769 6320 616e 6420 6669 726d  e logic and firm
+000012a0: 7761 7265 2077 6974 6820 636d 643a 207b  ware with cmd: {
+000012b0: 636d 647d 2229 0d0a 2020 2020 2020 2020  cmd}")..        
+000012c0: 7265 7420 3d20 6f73 2e73 7973 7465 6d28  ret = os.system(
+000012d0: 636d 6429 0d0a 2020 2020 2020 2020 6966  cmd)..        if
+000012e0: 2072 6574 2021 3d20 303a 0d0a 2020 2020   ret != 0:..    
+000012f0: 2020 2020 2020 2020 7261 6973 6520 5275          raise Ru
+00001300: 6e74 696d 6545 7272 6f72 2822 6c6f 6164  ntimeError("load
+00001310: 5f61 6c6c 2066 6169 6c65 6422 290d 0a20  _all failed").. 
+00001320: 2020 2020 2020 2074 696d 652e 736c 6565         time.slee
+00001330: 7028 3630 290d 0a0d 0a20 2020 2064 6566  p(60)....    def
+00001340: 2069 6e73 6d6f 645f 6b6f 2873 656c 662c   insmod_ko(self,
+00001350: 2073 7368 2c20 7665 6e75 7329 3a0d 0a20   ssh, venus):.. 
+00001360: 2020 2020 2020 206b 6f5f 7061 7468 203d         ko_path =
+00001370: 2066 227b 7665 6e75 737d 2f62 696e 2f74   f"{venus}/bin/t
+00001380: 6168 6f65 2f71 615f 6d6f 6465 220d 0a20  ahoe/qa_mode".. 
+00001390: 2020 2020 2020 2063 6d64 203d 2066 2263         cmd = f"c
+000013a0: 6420 7b6b 6f5f 7061 7468 7d20 2626 2069  d {ko_path} && i
+000013b0: 6e73 6d6f 6420 6e65 7875 732e 6b6f 2026  nsmod nexus.ko &
+000013c0: 2620 696e 736d 6f64 206b 7465 7374 2e6b  & insmod ktest.k
+000013d0: 6f22 0d0a 2020 2020 2020 2020 7374 6174  o"..        stat
+000013e0: 7573 2c20 6f75 7470 7574 203d 2073 7368  us, output = ssh
+000013f0: 2e63 6f6d 6d61 6e64 2863 6d64 290d 0a20  .command(cmd).. 
+00001400: 2020 2020 2020 2069 6620 7374 6174 7573         if status
+00001410: 2021 3d20 303a 0d0a 2020 2020 2020 2020   != 0:..        
+00001420: 2020 2020 7261 6973 6520 5275 6e74 696d      raise Runtim
+00001430: 6545 7272 6f72 2866 2269 6e73 6d6f 6420  eError(f"insmod 
+00001440: 6661 696c 6564 2c20 636d 643a 207b 636d  failed, cmd: {cm
+00001450: 647d 2e20 4f75 7470 7574 3a7b 6f75 7470  d}. Output:{outp
+00001460: 7574 7d22 290d 0a0d 0a20 2020 2064 6566  ut}")....    def
+00001470: 2072 6562 6f6f 745f 6c69 6e75 7828 7365   reboot_linux(se
+00001480: 6c66 2c20 6c69 6e75 782c 2075 7365 722c  lf, linux, user,
+00001490: 2070 7764 2c20 7665 6e75 735f 7061 7468   pwd, venus_path
+000014a0: 293a 0d0a 2020 2020 2020 2020 7373 6820  ):..        ssh 
+000014b0: 3d20 5353 4828 6c69 6e75 782c 2075 7365  = SSH(linux, use
+000014c0: 726e 616d 653d 7573 6572 2c20 7061 7373  rname=user, pass
+000014d0: 776f 7264 3d70 7764 290d 0a20 2020 2020  word=pwd)..     
+000014e0: 2020 2073 7368 2e6f 7065 6e28 290d 0a20     ssh.open().. 
+000014f0: 2020 2020 2020 2073 7368 2e63 6f6d 6d61         ssh.comma
+00001500: 6e64 5f77 6974 686f 7574 5f72 6573 756c  nd_without_resul
+00001510: 7428 2272 6562 6f6f 7420 2d6e 6622 2c20  t("reboot -nf", 
+00001520: 7469 6d65 6f75 743d 3130 290d 0a20 2020  timeout=10)..   
+00001530: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
+00001540: 3630 290d 0a20 2020 2020 2020 2073 7368  60)..        ssh
+00001550: 2e6f 7065 6e28 290d 0a20 2020 2020 2020  .open()..       
+00001560: 2073 656c 662e 696e 736d 6f64 5f6b 6f28   self.insmod_ko(
+00001570: 7373 682c 2076 656e 7573 5f70 6174 6829  ssh, venus_path)
+00001580: 0d0a 0d0a 2020 2020 4073 7461 7469 636d  ....    @staticm
+00001590: 6574 686f 640d 0a20 2020 2064 6566 2063  ethod..    def c
+000015a0: 6c65 6172 5f75 6172 7428 636f 6d29 3a0d  lear_uart(com):.
+000015b0: 0a20 2020 2020 2020 2073 6572 203d 2043  .        ser = C
+000015c0: 6e65 7853 6572 6961 6c28 636f 6d29 0d0a  nexSerial(com)..
+000015d0: 2020 2020 2020 2020 7365 722e 636c 6f73          ser.clos
+000015e0: 655f 7474 6572 6d70 726f 2829 0d0a 2020  e_ttermpro()..  
+000015f0: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
+00001600: 2832 290d 0a20 2020 2020 2020 2073 6572  (2)..        ser
+00001610: 2e63 6c65 6172 7370 6931 2829 0d0a 2020  .clearspi1()..  
+00001620: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
+00001630: 2832 290d 0a20 2020 2020 2020 2073 6572  (2)..        ser
+00001640: 2e6f 7065 6e5f 7474 6572 6d70 726f 2829  .open_ttermpro()
+00001650: 0d0a 0d0a 2020 2020 4064 6563 6f72 6174  ....    @decorat
+00001660: 655f 6578 6365 7074 696f 6e5f 7265 7375  e_exception_resu
+00001670: 6c74 0d0a 2020 2020 6465 6620 7275 6e28  lt..    def run(
+00001680: 7365 6c66 2c20 7061 7261 293a 0d0a 2020  self, para):..  
+00001690: 2020 2020 2020 6c6f 672e 494e 464f 2822        log.INFO("
+000016a0: 4265 6769 6e20 746f 2064 6f77 6e6c 6f61  Begin to downloa
+000016b0: 6420 6c6f 6769 6320 616e 6420 6669 726d  d logic and firm
+000016c0: 7761 7265 2229 0d0a 2020 2020 2020 2020  ware")..        
+000016d0: 7372 635f 736f 6620 3d20 7365 6c66 2e67  src_sof = self.g
+000016e0: 6574 5f66 7067 615f 6672 6f6d 5f66 7470  et_fpga_from_ftp
+000016f0: 2870 6172 615b 2269 635f 6c6f 6769 6322  (para["ic_logic"
+00001700: 5d29 0d0a 2020 2020 2020 2020 7365 6c66  ])..        self
+00001710: 2e75 7064 6174 655f 6677 5f63 6f64 6528  .update_fw_code(
+00001720: 7061 7261 5b22 6963 5f66 775f 6272 616e  para["ic_fw_bran
+00001730: 6368 225d 290d 0a20 2020 2020 2020 2073  ch"])..        s
+00001740: 656c 662e 636c 6561 725f 7561 7274 2870  elf.clear_uart(p
+00001750: 6172 615b 2263 6f6d 225d 290d 0a20 2020  ara["com"])..   
+00001760: 2020 2020 2073 656c 662e 636f 7079 5f73       self.copy_s
+00001770: 6f66 5f32 5f66 7728 7372 635f 736f 6629  of_2_fw(src_sof)
+00001780: 0d0a 2020 2020 2020 2020 7365 6c66 2e6c  ..        self.l
+00001790: 6f61 645f 616c 6c28 290d 0a20 2020 2020  oad_all()..     
+000017a0: 2020 2073 656c 662e 7265 626f 6f74 5f6c     self.reboot_l
+000017b0: 696e 7578 2870 6172 615b 2274 6172 6765  inux(para["targe
+000017c0: 745f 6970 225d 2c20 7061 7261 5b22 6c69  t_ip"], para["li
+000017d0: 6e75 785f 7573 6572 225d 2c20 7061 7261  nux_user"], para
+000017e0: 5b22 6c69 6e75 785f 7077 6422 5d2c 2070  ["linux_pwd"], p
+000017f0: 6172 615b 2277 6f72 6b5f 7061 7468 225d  ara["work_path"]
+00001800: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00001810: 6e20 302c 2022 646f 776e 6c6f 6164 206c  n 0, "download l
+00001820: 6f67 6963 2061 6e64 2066 6972 6d77 6172  ogic and firmwar
+00001830: 6520 7375 6363 6565 6422 0d0a            e succeed"..
```

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/oakgate/nvme_download.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_engine/oakgate/nvme_download.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/oakgate/two_step_download.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_engine/oakgate/two_step_download.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_engine/oakgate_download_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_engine/perses_download_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_engine/perses_download_engine_old.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/firmware_engine/serial_download_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/node_database.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/node_database.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/performance_database.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/performance_database.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/reboot_engine/sse_reboot_engine.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/state.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/state.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/status_file.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/status_file.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/test_base.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/test_base.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/test_benchmark.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/test_benchmark_group.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/test_benchmark_group.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/test_case.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/test_case.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/test_pool.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/test_pool.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/test_reboot_handle.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/test_reboot_handle.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/test_result.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/test_result.py`

 * *Files 18% similar despite different names*

```diff
@@ -56,37 +56,40 @@
 
     def get_log(self, logs):
         log = str()
         try:
             if type(logs) is list:
                 for item in logs:
                     log_content = self._get_log_txt(item)
-                    log = "{} \n\n{}\n\n{}".format(log, item, log_content)
+                    log = "{}\n{}\n{}".format(log, item, log_content)
             else:
                 log = self._get_log_txt(logs)
         except Exception as all_exception:
             print(all_exception)
         return log
 
+    @staticmethod
+    def generate_msg_head(log_name):
+        head = "\n"+"*"*100+"\n"+"*"*15+log_name+"*"*15+"\n"+"*"*100+"\n"
+        return head
+
     def get_test_suite_test_msg(self, test_results):
         print("get_test_suite_test_msg")
         print(test_results)
         msg = ""
         if type(test_results) is list:
             for test_result in test_results:
                 if "xml_path" in test_result.keys():
                     xml_log = self.get_xml_logs(test_result["xml_path"])
-                    msg = msg + "\n \n ****************************************** \n \n"
-                    msg = msg + test_result["name"] + "\n"
-                    msg = msg + "\n" + xml_log
-                elif "msg" in test_result.keys():
-                    msg = msg + str(test_result["msg"])
-                elif "log" in test_result.keys():
+                    msg = msg + self.generate_msg_head(test_result["xml_path"]) + xml_log + "\n"
+                if "msg" in test_result.keys():
+                    msg = msg + self.generate_msg_head("") + str(test_result["msg"])
+                if "log" in test_result.keys():
                     logs = test_result["log"]
-                    msg = msg + str(self.get_log(logs))
+                    msg = msg + self.generate_msg_head("Logs information") + str(self.get_log(logs))
         elif type(test_results) is str:
             msg = test_results
         return msg
 
     @staticmethod
     def check_file_size(path):
         result = False
```

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/test_runner.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/test_runner.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/test_framework/test_suite.py` & `automation_rest_server-3.7.1/automation_rest_server/test_framework/test_suite.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/device/dll/buf.dll` & `automation_rest_server-3.7.1/automation_rest_server/tool/device/dll/buf.dll`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/device/dll/buf.so` & `automation_rest_server-3.7.1/automation_rest_server/tool/device/dll/buf.so`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/device/dll/build.py` & `automation_rest_server-3.7.1/automation_rest_server/tool/device/dll/build.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/device/linux_nvme.py` & `automation_rest_server-3.7.1/automation_rest_server/tool/device/linux_nvme.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/buf.py` & `automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/buf.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/ctype.py` & `automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/ctype.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/get_feature.py` & `automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/get_feature.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/ioctl.py` & `automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/ioctl.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/nvme.py` & `automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/nvme.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/command.py` & `automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/struct/command.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/features.py` & `automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/struct/features.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/hmb.py` & `automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/struct/hmb.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/identify.py` & `automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/struct/identify.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/log_page.py` & `automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/struct/log_page.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/memory.py` & `automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/struct/memory.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/pcie.py` & `automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/struct/pcie.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/struct/registers.py` & `automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/struct/registers.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/device/nvme/utility_vu.py` & `automation_rest_server-3.7.1/automation_rest_server/tool/device/nvme/utility_vu.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/diskpart/diskpart.py` & `automation_rest_server-3.7.1/automation_rest_server/tool/diskpart/diskpart.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/fio/fio.py` & `automation_rest_server-3.7.1/automation_rest_server/tool/fio/fio.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/fio/fio_linux.py` & `automation_rest_server-3.7.1/automation_rest_server/tool/fio/fio_linux.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/fio/tool/fio` & `automation_rest_server-3.7.1/automation_rest_server/tool/fio/tool/fio`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/git/git_operator.py` & `automation_rest_server-3.7.1/automation_rest_server/tool/git/git_operator.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/tool/iometer/iometer.py` & `automation_rest_server-3.7.1/automation_rest_server/tool/iometer/iometer.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/utils/buf.py` & `automation_rest_server-3.7.1/automation_rest_server/utils/buf.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/utils/firmware_path.py` & `automation_rest_server-3.7.1/automation_rest_server/utils/firmware_path.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/utils/log.py` & `automation_rest_server-3.7.1/automation_rest_server/utils/log.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/utils/nose_xml.py` & `automation_rest_server-3.7.1/automation_rest_server/utils/nose_xml.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/utils/pip_operation.py` & `automation_rest_server-3.7.1/automation_rest_server/utils/pip_operation.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/utils/process.py` & `automation_rest_server-3.7.1/automation_rest_server/utils/process.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/utils/serial_tool.py` & `automation_rest_server-3.7.1/automation_rest_server/utils/serial_tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 class CnexSerial(object):
 
     TERA_TERM_PATH = r"C:\Program Files (x86)\teraterm\ttermpro.exe"
 
     def __init__(self, port, baud_rate=115200, timeout=5):
         self.serial_port = port.upper()
         self.baud_rate = baud_rate
-        self.ser = serial.Serial(port=self.serial_port, baudrate=baud_rate, timeout=timeout)
+        self.timeout = timeout
+        self.ser = None
         self.default_pattern = b"UART>"
 
     def close_ttermpro(self):
         cmd = 'wmic process where "Name like \'%ttermpro.exe%\'" get CommandLine,ProcessId'
         output = subprocess.check_output(cmd, shell=True).decode()
         lines = output.strip().split('\n')[1:]
         com_arg = '/C=' + self.serial_port.replace('COM', '')
@@ -59,14 +60,16 @@
     def clearspi1(self):
         self.send_command(b"clearspi 1", b"clearspi complete")
 
     def set_timeout(self, timeout):
         self.ser.timeout = timeout
 
     def send_command(self, cmd_line, wait_pattern=None):
+        self.ser = serial.Serial(port=self.serial_port, baudrate=self.baud_rate, timeout=self.timeout)
+
         wait_pattern = self.default_pattern if wait_pattern is not None else wait_pattern
         if not self.ser.is_open:
             self.ser.open()
         self.ser.flushInput()
         self.ser.write(b"\n")
         log.INFO(self.ser.read_until(self.default_pattern).decode("ascii"))
         for ch in cmd_line:
```

### Comparing `automation_rest_server-3.6.9/automation_rest_server/utils/ssh.py` & `automation_rest_server-3.7.1/automation_rest_server/utils/ssh.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server/utils/system.py` & `automation_rest_server-3.7.1/automation_rest_server/utils/system.py`

 * *Files identical despite different names*

### Comparing `automation_rest_server-3.6.9/automation_rest_server.egg-info/PKG-INFO` & `automation_rest_server-3.7.1/automation_rest_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: automation-rest-server
-Version: 3.6.9
+Version: 3.7.1
 Summary: NVMe production server
 Home-page: https://pypi.org/project/automation_rest_server
 Author: yuwen123441
 Author-email: yuwen123441@126.com
 License: MIT License
 Description: UNKNOWN
 Keywords: runner,server
```

### Comparing `automation_rest_server-3.6.9/automation_rest_server.egg-info/SOURCES.txt` & `automation_rest_server-3.7.1/automation_rest_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

