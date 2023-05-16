# Comparing `tmp/RobertCommonDriver-0.1.39.tar.gz` & `tmp/RobertCommonDriver-0.1.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonDriver-0.1.39.tar", last modified: Thu Apr 27 02:24:54 2023, max compression
+gzip compressed data, was "RobertCommonDriver-0.1.40.tar", last modified: Tue May 16 09:48:36 2023, max compression
```

## Comparing `RobertCommonDriver-0.1.39.tar` & `RobertCommonDriver-0.1.40.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 02:24:54.797557 RobertCommonDriver-0.1.39/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.39/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.39/MANIFEST.in
--rw-rw-rw-   0        0        0     1744 2023-04-27 02:24:54.797557 RobertCommonDriver-0.1.39/PKG-INFO
--rw-rw-rw-   0        0        0     1059 2022-01-13 07:06:32.000000 RobertCommonDriver-0.1.39/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 02:24:54.723381 RobertCommonDriver-0.1.39/RobertCommonDriver.egg-info/
--rw-rw-rw-   0        0        0     1744 2023-04-27 02:24:54.000000 RobertCommonDriver-0.1.39/RobertCommonDriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2802 2023-04-27 02:24:54.000000 RobertCommonDriver-0.1.39/RobertCommonDriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 02:24:54.000000 RobertCommonDriver-0.1.39/RobertCommonDriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      186 2023-04-27 02:24:54.000000 RobertCommonDriver-0.1.39/RobertCommonDriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-04-27 02:24:54.000000 RobertCommonDriver-0.1.39/RobertCommonDriver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      199 2023-04-19 11:58:47.000000 RobertCommonDriver-0.1.39/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-27 02:24:54.724700 RobertCommonDriver-0.1.39/robertcommondriver/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.39/robertcommondriver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:24:54.725706 RobertCommonDriver-0.1.39/robertcommondriver/system/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:24:54.740725 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/__init__.py
--rw-rw-rw-   0        0        0    87343 2023-03-23 08:25:35.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/bacnet.py
--rw-rw-rw-   0        0        0   495630 2023-04-11 03:08:18.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/bacnetc.py
--rw-rw-rw-   0        0        0     4980 2022-12-01 08:57:24.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/base.py
--rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/iec104.py
--rw-rw-rw-   0        0        0    38296 2022-12-01 08:59:47.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/modbus.py
--rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/obix.py
--rw-rw-rw-   0        0        0    60819 2023-04-03 06:02:51.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/opcda.py
--rw-rw-rw-   0        0        0    17013 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/opcda_openopc.py
--rw-rw-rw-   0        0        0    15955 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/opcua.py
--rw-rw-rw-   0        0        0    33482 2022-12-14 03:05:41.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/plcs7.py
--rw-rw-rw-   0        0        0    16586 2022-12-14 03:07:06.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/driver/snmp.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:24:54.760893 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/__init__.py
--rw-rw-rw-   0        0        0    62987 2023-04-17 09:34:25.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/base.py
--rw-rw-rw-   0        0        0    62781 2023-04-26 10:00:30.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_bacnet.py
--rw-rw-rw-   0        0        0   566042 2023-04-17 09:34:25.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0    46969 2023-04-14 08:33:27.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_iec104.py
--rw-rw-rw-   0        0        0    33803 2023-04-25 09:57:11.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_modbus.py
--rw-rw-rw-   0        0        0    18368 2023-04-27 02:18:02.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_obix.py
--rw-rw-rw-   0        0        0    62003 2023-04-17 09:34:25.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_opcda.py
--rw-rw-rw-   0        0        0    24090 2023-04-24 09:50:15.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_opcua.py
--rw-rw-rw-   0        0        0    43387 2023-04-13 08:35:41.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_plc_ab.py
--rw-rw-rw-   0        0        0    51617 2023-04-13 08:22:42.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0    41508 2023-04-13 08:32:25.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_plc_omron.py
--rw-rw-rw-   0        0        0    32748 2023-04-14 09:33:24.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_plc_s7.py
--rw-rw-rw-   0        0        0    44632 2023-04-14 09:40:13.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_plc_siemens.py
--rw-rw-rw-   0        0        0    13003 2023-04-17 05:43:15.000000 RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_snmp.py
--rw-rw-rw-   0        0        0       42 2023-04-27 02:24:54.797557 RobertCommonDriver-0.1.39/setup.cfg
--rw-rw-rw-   0        0        0     3881 2023-04-27 02:24:37.000000 RobertCommonDriver-0.1.39/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:24:54.762066 RobertCommonDriver-0.1.39/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.39/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:24:54.763074 RobertCommonDriver-0.1.39/tests/test_system/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.39/tests/test_system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:24:54.776646 RobertCommonDriver-0.1.39/tests/test_system/test_driver/
--rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.39/tests/test_system/test_driver/__init__.py
--rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_bacnet.py
--rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_bacnet1.py
--rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_bacnetc.py
--rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_bacnetv1.py
--rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_modbus.py
--rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_obix.py
--rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_opcda.py
--rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_opcua.py
--rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_plcs7.py
--rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_snmp.py
-drwxrwxrwx   0        0        0        0 2023-04-27 02:24:54.795048 RobertCommonDriver-0.1.39/tests/test_system/test_iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/__init__.py
--rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_bacnet1.py
--rw-rw-rw-   0        0        0    22764 2023-04-13 09:16:01.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_bacnet.py
--rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0     1283 2023-04-14 08:30:44.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_iec104.py
--rw-rw-rw-   0        0        0    13461 2023-04-26 06:02:28.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_modbus.py
--rw-rw-rw-   0        0        0     4714 2023-04-13 03:12:39.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_obix.py
--rw-rw-rw-   0        0        0     2288 2023-04-13 02:01:19.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_opcda.py
--rw-rw-rw-   0        0        0     3667 2023-04-24 09:44:00.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_opcua.py
--rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_plc_ab.py
--rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_plc_omron.py
--rw-rw-rw-   0        0        0     7609 2023-04-14 09:31:32.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_plc_s7.py
--rw-rw-rw-   0        0        0     4154 2023-04-14 09:43:43.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_plc_siemens.py
--rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_plc_simenses1.py
--rw-rw-rw-   0        0        0     2292 2023-04-17 05:38:28.000000 RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_snmp.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:48:36.756651 RobertCommonDriver-0.1.40/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.40/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.40/MANIFEST.in
+-rw-rw-rw-   0        0        0     1744 2023-05-16 09:48:36.756651 RobertCommonDriver-0.1.40/PKG-INFO
+-rw-rw-rw-   0        0        0     1059 2022-01-13 07:06:32.000000 RobertCommonDriver-0.1.40/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 09:48:36.681626 RobertCommonDriver-0.1.40/RobertCommonDriver.egg-info/
+-rw-rw-rw-   0        0        0     1744 2023-05-16 09:48:36.000000 RobertCommonDriver-0.1.40/RobertCommonDriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2802 2023-05-16 09:48:36.000000 RobertCommonDriver-0.1.40/RobertCommonDriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 09:48:36.000000 RobertCommonDriver-0.1.40/RobertCommonDriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      186 2023-05-16 09:48:36.000000 RobertCommonDriver-0.1.40/RobertCommonDriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-05-16 09:48:36.000000 RobertCommonDriver-0.1.40/RobertCommonDriver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      199 2023-04-19 11:58:47.000000 RobertCommonDriver-0.1.40/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 09:48:36.681626 RobertCommonDriver-0.1.40/robertcommondriver/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.40/robertcommondriver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:48:36.682664 RobertCommonDriver-0.1.40/robertcommondriver/system/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:48:36.697671 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/__init__.py
+-rw-rw-rw-   0        0        0    87343 2023-03-23 08:25:35.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/bacnet.py
+-rw-rw-rw-   0        0        0   495630 2023-04-11 03:08:18.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/bacnetc.py
+-rw-rw-rw-   0        0        0     6025 2023-05-09 08:30:24.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/base.py
+-rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/iec104.py
+-rw-rw-rw-   0        0        0    38296 2022-12-01 08:59:47.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/modbus.py
+-rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/obix.py
+-rw-rw-rw-   0        0        0    60819 2023-04-03 06:02:51.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/opcda.py
+-rw-rw-rw-   0        0        0    17013 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/opcda_openopc.py
+-rw-rw-rw-   0        0        0    15955 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/opcua.py
+-rw-rw-rw-   0        0        0    33482 2022-12-14 03:05:41.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/plcs7.py
+-rw-rw-rw-   0        0        0    16586 2022-12-14 03:07:06.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/driver/snmp.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:48:36.714684 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/__init__.py
+-rw-rw-rw-   0        0        0    67007 2023-05-09 13:35:59.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/base.py
+-rw-rw-rw-   0        0        0    62759 2023-05-12 07:35:58.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_bacnet.py
+-rw-rw-rw-   0        0        0   566042 2023-04-17 09:34:25.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0    46969 2023-04-14 08:33:27.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_iec104.py
+-rw-rw-rw-   0        0        0    33838 2023-05-16 08:00:18.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_modbus.py
+-rw-rw-rw-   0        0        0    18368 2023-04-27 02:18:02.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_obix.py
+-rw-rw-rw-   0        0        0    62003 2023-04-17 09:34:25.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_opcda.py
+-rw-rw-rw-   0        0        0    24929 2023-05-16 07:04:43.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_opcua.py
+-rw-rw-rw-   0        0        0    43449 2023-05-16 08:00:18.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_plc_ab.py
+-rw-rw-rw-   0        0        0    51679 2023-05-16 08:00:18.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0    41574 2023-05-16 08:00:18.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_plc_omron.py
+-rw-rw-rw-   0        0        0    32863 2023-05-16 08:00:18.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_plc_s7.py
+-rw-rw-rw-   0        0        0    44698 2023-05-16 08:00:18.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_plc_siemens.py
+-rw-rw-rw-   0        0        0    13003 2023-04-17 05:43:15.000000 RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_snmp.py
+-rw-rw-rw-   0        0        0       42 2023-05-16 09:48:36.758043 RobertCommonDriver-0.1.40/setup.cfg
+-rw-rw-rw-   0        0        0     3881 2023-05-16 08:13:01.000000 RobertCommonDriver-0.1.40/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:48:36.715690 RobertCommonDriver-0.1.40/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.40/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:48:36.716692 RobertCommonDriver-0.1.40/tests/test_system/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.40/tests/test_system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:48:36.730853 RobertCommonDriver-0.1.40/tests/test_system/test_driver/
+-rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.40/tests/test_system/test_driver/__init__.py
+-rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_bacnet.py
+-rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_bacnet1.py
+-rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_bacnetc.py
+-rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_bacnetv1.py
+-rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_modbus.py
+-rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_obix.py
+-rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_opcda.py
+-rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_opcua.py
+-rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_plcs7.py
+-rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_snmp.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:48:36.755300 RobertCommonDriver-0.1.40/tests/test_system/test_iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/__init__.py
+-rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_bacnet1.py
+-rw-rw-rw-   0        0        0    22764 2023-04-27 08:47:35.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_bacnet.py
+-rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0     1283 2023-04-14 08:30:44.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_iec104.py
+-rw-rw-rw-   0        0        0    15871 2023-05-08 12:34:54.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_modbus.py
+-rw-rw-rw-   0        0        0     4714 2023-04-13 03:12:39.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_obix.py
+-rw-rw-rw-   0        0        0     2288 2023-04-13 02:01:19.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_opcda.py
+-rw-rw-rw-   0        0        0     3663 2023-05-09 08:04:00.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_opcua.py
+-rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_plc_ab.py
+-rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_plc_omron.py
+-rw-rw-rw-   0        0        0     8219 2023-05-16 07:37:56.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_plc_s7.py
+-rw-rw-rw-   0        0        0     4154 2023-04-14 09:43:43.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_plc_siemens.py
+-rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_plc_simenses1.py
+-rw-rw-rw-   0        0        0     2292 2023-04-17 05:38:28.000000 RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_snmp.py
```

### Comparing `RobertCommonDriver-0.1.39/LICENSE` & `RobertCommonDriver-0.1.40/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/PKG-INFO` & `RobertCommonDriver-0.1.40/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonDriver
-Version: 0.1.39
+Version: 0.1.40
 Summary: Robert Common Driver Library
 Home-page: https://github.com/hun0423/RobertCommonDriver
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonDriver-0.1.39/README.md` & `RobertCommonDriver-0.1.40/README.md`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/RobertCommonDriver.egg-info/PKG-INFO` & `RobertCommonDriver-0.1.40/RobertCommonDriver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonDriver
-Version: 0.1.39
+Version: 0.1.40
 Summary: Robert Common Driver Library
 Home-page: https://github.com/hun0423/RobertCommonDriver
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonDriver-0.1.39/RobertCommonDriver.egg-info/SOURCES.txt` & `RobertCommonDriver-0.1.40/RobertCommonDriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/driver/bacnet.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/driver/bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/driver/bacnetc.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/driver/bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/driver/base.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/driver/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,21 +5,48 @@
 from ipaddress import ip_network, ip_address
 from psutil import net_if_addrs
 from re import compile as re_compile
 
 
 class BaseCommon:
 
-    class RepeatingTimer(Timer):
+    class RepeatingTimer:
 
-        def run(self):
-            self.finished.wait(self.interval)
-            while not self.finished.is_set():
-                self.function(*self.args, **self.kwargs)
-                self.finished.wait(self.interval)
+        def __init__(self, interval, function, args=None, kwargs=None):
+            self.interval = interval
+            self.function = function
+            self.args = args if args is not None else []
+            self.kwargs = kwargs if kwargs is not None else {}
+            self._should_continue = False
+            self.is_running = False
+            self.thread = None
+
+        def is_alive(self):
+            return self._should_continue
+
+        def _handle_function(self):
+            self.is_running = True
+            self.function(self.args, self.kwargs)
+            self.is_running = False
+            self._start_timer()
+
+        def _start_timer(self):
+            if self._should_continue:  # Code could have been running when cancel was called.
+                self.thread = Timer(self.interval, self._handle_function)
+                self.thread.start()
+
+        def start(self):
+            if not self._should_continue and not self.is_running:
+                self._should_continue = True
+                self._start_timer()
+
+        def cancel(self):
+            if self.thread is not None:
+                self._should_continue = False  # Just in case thread is running and cancel fails.
+                self.thread.cancel()
 
     class SimpleTimer:
 
         def __init__(self):
             self.timer = None
 
         def is_running(self):
```

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/driver/modbus.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/driver/modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/driver/obix.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/driver/obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/driver/opcda.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/driver/opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/driver/opcda_openopc.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/driver/opcda_openopc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/driver/opcua.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/driver/opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/driver/plcs7.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/driver/plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/driver/snmp.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/driver/snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/base.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,21 +334,48 @@
             if bytes1 is None or bytes2 is None:
                 return False
             for i in range(length):
                 if bytes1[i + start1] != bytes2[i + start2]:
                     return False
             return True
 
-    class RepeatingTimer(Timer):
+    class RepeatingTimer:
 
-        def run(self):
-            self.finished.wait(self.interval)
-            while not self.finished.is_set():
-                self.function(*self.args, **self.kwargs)
-                self.finished.wait(self.interval)
+        def __init__(self, interval, function, args=None, kwargs=None):
+            self.interval = interval
+            self.function = function
+            self.args = args if args is not None else []
+            self.kwargs = kwargs if kwargs is not None else {}
+            self._should_continue = False
+            self.is_running = False
+            self.thread = None
+
+        def is_alive(self):
+            return self._should_continue
+
+        def _handle_function(self):
+            self.is_running = True
+            self.function(self.args, self.kwargs)
+            self.is_running = False
+            self._start_timer()
+
+        def _start_timer(self):
+            if self._should_continue:  # Code could have been running when cancel was called.
+                self.thread = Timer(self.interval, self._handle_function)
+                self.thread.start()
+
+        def start(self):
+            if not self._should_continue and not self.is_running:
+                self._should_continue = True
+                self._start_timer()
+
+        def cancel(self):
+            if self.thread is not None:
+                self._should_continue = False  # Just in case thread is running and cancel fails.
+                self.thread.cancel()
 
     class SimpleTimer:
 
         def __init__(self):
             self.timer = None
 
         def is_running(self):
@@ -579,15 +606,14 @@
             try:
                 while self.valid is True:
                     start_bytes = self.recv_bytes(1)
                     if start_bytes == bytes.fromhex('68'):
                         length_bytes = self.recv_bytes(1)
                         length = length_bytes[0]  # 包长
                         datas = self.recv_bytes(length)
-                        # print(f"Recv: {self.format_bytes(start_bytes + length_bytes + datas)}")
                         if 'handle_data' in self.callbacks.keys():
                             self.callbacks['handle_data'](self, start_bytes + length_bytes + datas)
             except socket.timeout as e:
                 pass
             except IOTBaseCommon.NormalException as e:
                 logging.error(e.__str__())
             except IOTBaseCommon.CloseException as e:
@@ -609,16 +635,17 @@
 
         def handle_connect(self):
             if 'handle_connect' in self.callbacks.keys():
                 self.callbacks['handle_connect'](self)
 
     class SocketClient:
 
-        def __init__(self, host: str, port: int, timeout: float, callbacks: Optional[dict] = None):
+        def __init__(self, sock_type: int, host: str, port: int, timeout: float, callbacks: Optional[dict] = None):
             self.valid = True
+            self.sock_type = sock_type
             self.host = host
             self.port = port
             self.sock = None
             self.timeout = timeout
             self.callbacks = {} if callbacks is None else callbacks
             self.connect()
             IOTBaseCommon.function_thread(self.receive, True).start()
@@ -631,31 +658,27 @@
             self.exit()
 
         def exit(self):
             self.valid = False
             self.close()
 
         def connect(self):
-            self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            self.sock = socket.socket(socket.AF_INET, self.sock_type)
             self.sock.settimeout(self.timeout)  # 设置连接超时
             self.sock.connect((self.host, self.port))
             self.sock.settimeout(None)
 
         def close(self):
             if self.sock:
                 self.sock.close()
 
         def send(self, datas: bytes):
-            # print(f"Send: {self.format_bytes(datas)}")
             if self.sock:
                 self.sock.send(datas)
 
-        def format_bytes(self, data: bytes) -> str:
-            return ' '.join(["%02X" % x for x in data]).strip()
-
         def check_invalid(self) -> bool:
             return self.valid
 
         def recv_bytes(self, length: int) -> Optional[bytes]:
             data = b''
             while self.check_invalid() is True and len(data) < length:
                 rec_length = length - len(data)
@@ -671,15 +694,14 @@
             try:
                 while self.valid is True:
                     start_bytes = self.recv_bytes(1)
                     if start_bytes == bytes.fromhex('68'):
                         length_bytes = self.recv_bytes(1)
                         length = length_bytes[0]  # 包长
                         datas = self.recv_bytes(length)
-                        # print(f"Recv: {self.format_bytes(start_bytes + length_bytes + datas)}")
                         if 'handle_data' in self.callbacks.keys():
                             self.callbacks['handle_data'](self, start_bytes + length_bytes + datas)
             except socket.timeout as e:
                 pass
             except IOTBaseCommon.NormalException as e:
                 logging.error(e.__str__())
             except IOTBaseCommon.CloseException as e:
@@ -699,14 +721,108 @@
             self.close()
             self.valid = False
 
         def handle_connect(self):
             if 'handle_connect' in self.callbacks.keys():
                 self.callbacks['handle_connect'](self)
 
+    class SocketHandle:
+
+        def __init__(self, conn: Optional[Any] = None, address: Optional[tuple] = None, server: Optional[Any] = None):
+            self.conn = conn
+            self.address = address
+            self.server = server
+            self.valid = True
+            IOTBaseCommon.function_thread(self.receive, True).start()
+
+        def __str__(self):
+            if isinstance(self.address, tuple) and len(self.address) >= 2:
+                return f"{self.address[0]}:{self.address[1]}"
+            return str(self.address)
+
+        def __del__(self):
+            self.exit()
+
+        def exit(self):
+            self.valid = False
+            self.conn.close()
+
+        def check_invalid(self) -> bool:
+            return self.valid
+
+        def receive(self):
+            while self.valid is True:
+                data = None
+                try:
+                    data = self.conn.recv(1024)
+                    if data is not None and len(data) > 0:
+                        pass
+                    else:
+                        self.valid = False
+                        raise Exception(f"recv 0")
+                except Exception as e:
+                    pass
+
+    class SocketServer:
+
+        def __init__(self, sock_type: int, host: str, port: int, timeout: float, size: int, callbacks: Optional[dict] = None, handle_class: Optional[Any] = None, **kwargs):
+            self.valid = True
+            self.sock_type = sock_type
+            self.host = host
+            self.port = port
+            self.size = size
+            self.sock = None
+            self.kwargs = kwargs
+            self.timeout = timeout
+            self.handle_class = handle_class
+            self.callbacks = {} if callbacks is None else callbacks
+            self.sockets = {}
+            self.connect()
+
+        def __str__(self):
+            return f"{self.host}:{self.port}"
+
+        def __del__(self):
+            self.exit()
+
+        def exit(self):
+            self.valid = False
+            for n, sock in self.sockets.items():
+                try:
+                    if sock:
+                        if hasattr(sock, 'exit'):
+                            sock.exit()
+                except Exception as e:
+                    pass
+            self.sockets = {}
+            self.close()
+
+        def connect(self):
+            self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+            self.sock.bind((self.host, self.port))
+            self.sock.listen(self.size)
+
+            IOTBaseCommon.function_thread(self.accept, True).start()
+
+        def socks(self):
+            return self.sockets
+
+        def accept(self):
+            while self.valid is True:
+                conn, address = self.sock.accept()  # 接收连接
+                if self.handle_class is not None:
+                    self.sockets[f"{address[0]}:{address[1]}"] = self.handle_class(conn, address, self)
+                else:
+                    self.sockets[f"{address[0]}:{address[1]}"] = IOTBaseCommon.SocketHandle(conn, address, self)
+
+        def close(self):
+            if self.sock:
+                self.sock.close()
+
     # 重构
     class IOTNetMessage:
 
         def __init__(self):
             self.heads: Optional[bytearray] = None
             self.contents: Optional[bytearray] = None
             self.sends: Optional[bytearray] = None
```

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_bacnet.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_bacnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
             pass
         return bacnet_device
 
     def control(self, status: bool = True):
         self.logging(content=f"control({status})", pos=self.stack_pos)
         if status is True:
             enable_sleeping()
-            run(spin=self.bacnet_cmd_interval/5, sigterm=None, sigusr1=None)
+            run(spin=0.05, sigterm=None, sigusr1=None)
         else:
             stop()
 
     def discover(self, low_device_id: Optional[int] = None, high_device_id: Optional[int] = None, target_address: Optional[str] = None) -> bool:
         request = WhoIsRequest()
         if low_device_id is not None:
             request.deviceInstanceRangeLowLimit = low_device_id
```

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_bacnet_mstp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_iec104.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_iec104.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_modbus.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_modbus.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,22 +396,23 @@
 
                     client.set_timeout(self.configs.get('timeout', 5))
                     client.set_verbose(True)
                     self.clients[address] = client
         return self.clients.get(address)
 
     def _release_client(self, address: str):
+        client = self.clients.get(address)
         try:
-            client = self.clients.get(address)
             if client:
                 client.close()
-                del self.clients[address]
-            client = None
         except Exception as e:
             pass
+        finally:
+            if address in self.clients.keys():
+                del self.clients[address]
 
     def _change_fun_code(self, fun_code: int, **kwargs):
         if kwargs.get('mode', 0) == 0:  # read
             if fun_code == modbus_tk_defines.READ_HOLDING_REGISTERS or fun_code == modbus_tk_defines.WRITE_MULTIPLE_REGISTERS or fun_code == modbus_tk_defines.READ_WRITE_MULTIPLE_REGISTERS:
                 fun_code = modbus_tk_defines.READ_HOLDING_REGISTERS
             elif fun_code == modbus_tk_defines.READ_COILS or fun_code == modbus_tk_defines.WRITE_SINGLE_COIL or fun_code == modbus_tk_defines.WRITE_MULTIPLE_COILS:
                 fun_code = modbus_tk_defines.READ_COILS
```

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_obix.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_opcda.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_opcua.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_opcua.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,44 +208,46 @@
             else:
                 raise Exception(str(value))
         except Exception as e:
             self.logging(content=f"get value({name}) fail({e.__str__()})", level='ERROR', source=name, pos=self.stack_pos)
         return None
 
     def _get_client(self):
+        if self.client is not None:
+            try:
+                root = self.client.get_root_node().get_children()
+            except Exception as e:
+                self._release_client()
+
         if self.client is None:
-            client = Client(self.configs.get('endpoint'), timeout=self.configs.get('timeout', 4))
-            if len(self.configs.get('security', '')) > 0:   # Basic256Sha256,SignAndEncrypt,certificate-example.der,private-key-example.pem
-                client.set_security_string(self.configs.get('security', ''))
-            auth = self.configs.get('auth', {})
-            if isinstance(auth, str) and len(auth) >= 0:
-                auth = json.loads(auth)
-            if 'type' in auth.keys():
-                if auth['type'] == 'UserName':
-                    client.set_user(auth['user'])
-                    client.set_password(auth['password'])
-                elif auth['type'] == 'Certificate':
-                    client.load_client_certificate(auth['client_certificate'])
-                    client.load_private_key(auth['private_key'])
-
-            client.secure_channel_timeout = self.configs.get('channel_timeout', 10000)
-            client.session_timeout = self.configs.get('session_timeout', 10000)
+            try:
+                client = Client(self.configs.get('endpoint'), timeout=self.configs.get('timeout', 4))
+                if len(self.configs.get('security', '')) > 0:   # Basic256Sha256,SignAndEncrypt,certificate-example.der,private-key-example.pem
+                    client.set_security_string(self.configs.get('security', ''))
+                auth = self.configs.get('auth', {})
+                if isinstance(auth, str) and len(auth) >= 0:
+                    auth = json.loads(auth)
+                if 'type' in auth.keys():
+                    if auth['type'] == 'UserName':
+                        client.set_user(auth['user'])
+                        client.set_password(auth['password'])
+                    elif auth['type'] == 'Certificate':
+                        client.load_client_certificate(auth['client_certificate'])
+                        client.load_private_key(auth['private_key'])
 
-            client.connect()
-            client.load_type_definitions()
+                client.secure_channel_timeout = self.configs.get('channel_timeout', 10000)
+                client.session_timeout = self.configs.get('session_timeout', 10000)
 
-            # IOTBaseCommon.function_thread(embed, True).start()
+                client.connect()
+                client.load_type_definitions()
 
-            self.client = client
-        else:
-            try:
-                root = self.client.get_root_node().get_children()
+                self.client = client
             except Exception as e:
-                self._release_client()
-                raise Exception(f"connect faile: {e.__str__()}")
+                raise e
+
         return self.client
 
     def _release_client(self):
         try:
             if self.client is not None:
                 if self.sub is not None:
                     for sub in self.subs:
@@ -255,20 +257,21 @@
             pass
         try:
             if self.client:
                 self.client.disconnect()
         except:
             pass
         self.subs = []
+        self.sub = None
         self.client = None
         self.devices = {}
 
     def _get_sub(self):
         if self.sub is None:
-            sub = self._get_client().create_subscription(self.configs.get('subscript_interval', 500), self.SubHandler(callbacks={'datachange_notification': self._datachange_notification}))
+            sub = self._get_client().create_subscription(self.configs.get('subscript_interval', 500), self.SubHandler(callbacks={'datachange_notification': self._datachange_notification, 'event_notification': self._event_notification, 'status_change_notification': self._status_change_notification}))
             self.sub = sub
         return self.sub
 
     def _brower_child(self, parent, node, max_deep: int, ignore: list, results: dict):
         stack = [self.BrowerState(parent, node, 0)]
         while len(stack) > 0:
             if self._get_client() is not None:
@@ -293,22 +296,29 @@
                     results[point_name] = self.create_point(point_name=point_name, point_name_alias=point_name, point_node_id=nid.to_string(), point_node_path=path, point_value=str(val_to_string(val)), point_description='' if desc is None else desc.to_string())
                     self.logging(content=f"scan {len(results)} point({path})", pos=self.stack_pos)
 
     def _datachange_notification(self, node, val, data):
         try:
             if data.monitored_item.Value.StatusCode.is_good():
                 if val is not None:
+                    self.logging(content=f"datachange {node.nodeid.to_string()}({str(val_to_string(val))})")
                     self.update_device(self.configs.get('endpoint'), node.nodeid.to_string(), **self.gen_read_write_result(True, str(val_to_string(val)), point_time=IOTBaseCommon.get_datetime_str()))
                 else:
                     raise Exception(f"value is none")
             else:
                 raise Exception(f"{data.monitored_item.Value.StatusCode}")
         except Exception as e:
             self.update_device(self.configs.get('endpoint'), node.nodeid.to_string(), **self.gen_read_write_result(False, e.__str__()))
 
+    def _event_notification(self, event):
+        self.logging(content=f"event notification({str(event)})", pos=self.stack_pos)
+
+    def _status_change_notification(self, event):
+        self.logging(content=f"status change notification({str(event)})", pos=self.stack_pos)
+
     def _create_monitored_items(self, event, dispatcher):
         for idx in range(len(event.response_params)):
             if event.response_params[idx].StatusCode.is_good():
                 node_id = event.request_params.ItemsToCreate[idx].ItemToMonitor.NodeId
                 self.logging(content=f"opcua create sub node({node_id})", pos=self.stack_pos)
 
     def _modify_monitored_items(self, event, dispatcher):
@@ -320,36 +330,39 @@
     def _delete_monitored_items(self, event, dispatcher):
         for idx in range(len(event.response_params)):
             if event.response_params[idx].StatusCode.is_good():
                 node_id = event.request_params.ItemsToCreate[idx].ItemToMonitor.NodeId
                 self.logging(content=f"opcua delete sub node({node_id})", pos=self.stack_pos)
 
     def _read(self, read_items: list):
-        if len(read_items) > 0:
+        if len(read_items) > 0 or len(self.devices) > 0:
             try:
                 if self._get_client():
-                    items = []
-                    for item in read_items:
-                        node = self._get_client().get_node(item)
-                        if node:
-                            items.append((item, node))
-
-                    nodes = IOTBaseCommon.chunk_list(items, self.configs.get('subscript_add', 1000))
-                    if self._get_sub() is not None:
-                        for _nodes in nodes:
-                            subs = [node for id, node in _nodes]
-                            ids = [id for id, node in _nodes]
-                            sub_nodes = self._get_sub().subscribe_data_change(subs)
-                            for index, sub_node in enumerate(sub_nodes):
-                                if isinstance(sub_node, ua.StatusCode):
-                                    self.update_device(self.configs.get('endpoint'), ids[index], **self.gen_read_write_result(False, sub_node.name))
-                                else:
-                                    self.update_device(self.configs.get('endpoint'), ids[index], sub_node=sub_node)
-                                    self.subs.append(sub_node)
+                    if len(read_items) > 0:
+                        items = []
+                        for item in read_items:
+                            node = self._get_client().get_node(item)
+                            if node:
+                                items.append((item, node))
+
+                        nodes = IOTBaseCommon.chunk_list(items, self.configs.get('subscript_add', 1000))
+                        if self._get_sub() is not None:
+                            for _nodes in nodes:
+                                subs = [node for id, node in _nodes]
+                                ids = [id for id, node in _nodes]
+                                sub_nodes = self._get_sub().subscribe_data_change(subs)
+                                for index, sub_node in enumerate(sub_nodes):
+                                    if isinstance(sub_node, ua.StatusCode):
+                                        self.update_device(self.configs.get('endpoint'), ids[index], **self.gen_read_write_result(False, sub_node.name))
+                                    else:
+                                        self.update_device(self.configs.get('endpoint'), ids[index], sub_node=sub_node)
+                                        self.subs.append(sub_node)
+                                self.logging(content=f"subscribe size({len(sub_nodes)})")
             except Exception as e:
+                self._release_client()
                 for item in read_items:
                     self.update_device(self.configs.get('endpoint'), item, **self.gen_read_write_result(False, e.__str__()))
                 self.logging(content=f"opcua read fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
 
     def _write(self, node, value):
         try:
             if self._get_client():
```

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_plc_ab.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_plc_ab.py`

 * *Files 0% similar despite different names*

```diff
@@ -739,27 +739,29 @@
 
     def _get_address_info(self, device_address: str) -> dict:
         # ip/port/slot
         info_list = device_address.split('/')
         return {'host': info_list[0] if len(info_list) > 1 else '', 'port': int(float(info_list[1])) if len(info_list) > 2 else 44818, 'slot': int(float(info_list[2])) if len(info_list) > 3 else 0}
 
     def _release_client(self, address: str):
+        client = self.clients.get(address)
         try:
-            client = self.clients.get(address)
             if client:
                 client.exit()
-                del self.clients[address]
-            client = None
         except Exception as e:
             pass
+        finally:
+            if address in self.clients.keys():
+                del self.clients[address]
 
     def _get_client(self, address: str):
         client = self.clients.get(address)
         if client is not None and client.get_connected() is False:
             self._release_client(address)
+            client = None
 
         if client is None:
             info = self._get_address_info(address)
             if len(info) > 0:
                 client = AllenBradleyClient(info['host'], info['port'], info['slot'], self.configs.get('timeout'))
                 client.logging(call_logging=self.logging)
                 result = client.connect()
```

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_plc_mitsubishi.py`

 * *Files 0% similar despite different names*

```diff
@@ -896,27 +896,29 @@
 
     def _get_address_info(self, device_address: str) -> dict:
         # version/ip/port
         info_list = device_address.split('/')
         return {'host': info_list[1] if len(info_list) > 1 else '', 'port': int(float(info_list[2])) if len(info_list) > 2 else 102, 'type': int(float(info_list[0])) if len(info_list) > 1 else 2}
 
     def _release_client(self, address: str):
+        client = self.clients.get(address)
         try:
-            client = self.clients.get(address)
             if client:
                 client.exit()
-                del self.clients[address]
-            client = None
         except Exception as e:
             pass
+        finally:
+            if address in self.clients.keys():
+                del self.clients[address]
 
     def _get_client(self, address: str):
         client = self.clients.get(address)
         if client is not None and client.get_connected() is False:
             self._release_client(address)
+            client = None
 
         if client is None:
             info = self._get_address_info(address)
             if 'type' in info.keys():
                 client = MitsubishiClient(MitsubishiVersion(info['type']), info['host'], info['port'], self.configs.get('timeout'))
                 client.logging(call_logging=self.logging)
                 result = client.connect()
```

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_plc_omron.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_plc_omron.py`

 * *Files 0% similar despite different names*

```diff
@@ -689,23 +689,25 @@
         return {'host': info_list[0] if len(info_list) > 1 else '', 'port': int(float(info_list[1])) if len(info_list) > 2 else 9600, 'sa1': int(float(info_list[2])) if len(info_list) > 3 else 11}
 
     def _release_client(self, address: str):
         try:
             client = self.clients.get(address)
             if client:
                 client.exit()
-                del self.clients[address]
-            client = None
         except Exception as e:
             pass
+        finally:
+            if address in self.clients.keys():
+                del self.clients[address]
 
     def _get_client(self, address: str):
         client = self.clients.get(address)
         if client is not None and client.get_connected() is False:
             self._release_client(address)
+            client = None
 
         if client is None:
             info = self._get_address_info(address)
             if len(info) > 0:
                 client = OmronFinsClient(info['host'], info['port'], info['sa1'], self.configs.get('timeout'))
                 client.logging(call_logging=self.logging)
                 result = client.connect()
```

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_plc_s7.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_plc_s7.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,34 +374,36 @@
 
     def _get_address_info(self, device_address: str) -> dict:
         # ip/port/rack/slot
         info_list = device_address.split('/')
         return {'host': info_list[0] if len(info_list) > 0 else '', 'port': int(float(info_list[1])) if len(info_list) > 1 else 102, 'rack': int(float(info_list[2])) if len(info_list) > 2 else 0, 'slot': int(float(info_list[3])) if len(info_list) > 3 else 1, 'type': '' if len(info_list) > 2 else 'plc200'}
 
     def _release_client(self, address: str):
+        client = self.clients.get(address)
         try:
-            client = self.clients.get(address)
             if client:
                 client.disconnect()
                 client.destroy()
-                del self.clients[address]
-            client = None
         except Exception as e:
             pass
+        finally:
+            if address in self.clients.keys():
+                del self.clients[address]
 
     def _load_library(self):
         if IOTBaseCommon.is_windows():
             library = self.configs.get('library')
             if isinstance(library, str) and len(library) > 0 and IOTBaseCommon.check_file_exist(library):
                 load_library(library)
 
     def _get_client(self, address: str):
         client = self.clients.get(address)
-        if client is not None and client.get_connected() is False:
+        if client is not None and (client.get_connected() is False or str(client.get_cpu_state()) != 'S7CpuStatusRun'):
             self._release_client(address)
+            client = None
 
         if client is None:
             info = self._get_address_info(address)
             if 'type' in info.keys():
                 self._load_library()
                 client = snap7_client.Client()
                 if client:
```

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_plc_siemens.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_plc_siemens.py`

 * *Files 0% similar despite different names*

```diff
@@ -755,23 +755,25 @@
         return {'host': info_list[1] if len(info_list) > 1 else '', 'port': int(float(info_list[2])) if len(info_list) > 2 else 102, 'rack': int(float(info_list[3])) if len(info_list) > 3 else 0, 'slot': int(float(info_list[4])) if len(info_list) > 4 else 1, 'type': int(float(info_list[0])) if len(info_list) > 1 else 1}
 
     def _release_client(self, address: str):
         try:
             client = self.clients.get(address)
             if client:
                 client.exit()
-                del self.clients[address]
-            client = None
         except Exception as e:
             pass
+        finally:
+            if address in self.clients.keys():
+                del self.clients[address]
 
     def _get_client(self, address: str):
         client = self.clients.get(address)
         if client is not None and client.get_connected() is False:
             self._release_client(address)
+            client = None
 
         if client is None:
             info = self._get_address_info(address)
             if 'type' in info.keys():
                 client = SiemensS7Client(SiemensS7Version(info['type']), info['host'], info['port'], info['rack'], info['slot'], self.configs.get('timeout'))
                 client.logging(call_logging=self.logging)
                 result = client.connect()
```

### Comparing `RobertCommonDriver-0.1.39/robertcommondriver/system/iot/iot_snmp.py` & `RobertCommonDriver-0.1.40/robertcommondriver/system/iot/iot_snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/setup.py` & `RobertCommonDriver-0.1.40/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'RobertCommonDriver'
 DESCRIPTION = 'Robert Common Driver Library'
 URL = 'https://github.com/hun0423/RobertCommonDriver'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.39'
-DATE = '2023-04-27'
+VERSION = '0.1.40'
+DATE = '2023-05-16'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_bacnet.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_bacnet1.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_bacnetc.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_bacnetv1.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_bacnetv1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_modbus.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_obix.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_opcda.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_opcua.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_plcs7.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_driver/test_snmp.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_driver/test_snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_bacnet1.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_bacnet.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_bacnet_mstp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_iec104.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_iec104.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_modbus.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_modbus.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,40 @@
     # 轮询全部
     while True:
         dict_result_scrap = modbus_driver.read()
         print(dict_result_scrap)
         time.sleep(2)
 
 
+def test_read2():
+    #配置项
+    dict_config = {
+                        'multi_read': 100,                             # 批量读取个数
+                        'cmd_interval': 0.3,                         # 命令间隔
+                        'time_out': 5                                 # 超时时间
+                    }
+    #点表
+    dict_point = {}
+    dict_point['modbus_1'] = {'point_writable': True, 'point_name': 'modbus_1', 'point_device_address': '127.0.0.1/502',  'point_slave_id': 26, 'point_fun_code': 2, 'point_address': 1, 'point_data_type': 8, 'point_data_length': 1, 'point_scale':'1'}
+    dict_point['modbus_2'] = {'point_writable': True, 'point_name': 'modbus_2', 'point_device_address': '127.0.0.1/502',  'point_slave_id': 26, 'point_fun_code': 2, 'point_address': 2, 'point_data_type': 8, 'point_data_length': 1, 'point_scale':'1'}
+    dict_point['modbus_3'] = {'point_writable': True, 'point_name': 'modbus_3', 'point_device_address': '127.0.0.1/502',  'point_slave_id': 26, 'point_fun_code': 2, 'point_address': 3, 'point_data_type': 8, 'point_data_length': 1, 'point_scale':'1'}
+    dict_point['modbus_4'] = {'point_writable': True, 'point_name': 'modbus_3', 'point_device_address': '127.0.0.1/502',  'point_slave_id': 26, 'point_fun_code': 2, 'point_address': 4, 'point_data_type': 8, 'point_data_length': 1, 'point_scale':'1'}
+    dict_point['modbus_5'] = {'point_writable': True, 'point_name': 'modbus_4', 'point_device_address': '127.0.0.1/502',  'point_slave_id': 26, 'point_fun_code': 2, 'point_address': 5, 'point_data_type': 8, 'point_data_length': 1, 'point_scale':'1'}
+    dict_point['modbus_6'] = {'point_writable': True, 'point_name': 'modbus_6', 'point_device_address': '127.0.0.1/502',  'point_slave_id': 26, 'point_fun_code': 2, 'point_address': 6, 'point_data_type': 8, 'point_data_length': 1, 'point_scale':'1'}
+    dict_point['modbus_7'] = {'point_writable': True, 'point_name': 'modbus_7', 'point_device_address': '127.0.0.1/502',  'point_slave_id': 26, 'point_fun_code': 2, 'point_address': 7, 'point_data_type': 8, 'point_data_length': 1, 'point_scale':'1'}
+
+    modbus_driver = IOTModbus(configs=dict_config, points=dict_point)
+    modbus_driver.logging(call_logging=logging_print)
+    # 轮询全部
+    while True:
+        dict_result_scrap = modbus_driver.read()
+        print(dict_result_scrap)
+        time.sleep(2)
+
+
 def test_write():
     # 配置项
     dict_config = {
         'multi_read': 100,  # 批量读取个数
         'cmd_interval': 0.3,  # 命令间隔
         'time_out': 5  # 超时时间
     }
@@ -122,9 +148,9 @@
     while True:
         #for name, point in dict_point.items():
         #    point['point_value'] = random.randint(1, 100)
         client.simulate(points=dict_point)
         time.sleep(10)
 
 
-test_read1()
+test_read2()
```

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_obix.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_opcda.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_opcua.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_opcua.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     client.logging(call_logging=logging_print)
     while True:
         try:
             result = client.read()
             print(result)
         except Exception as e:
             print(e.__str__())
-        time.sleep(1)
+        time.sleep(5)
 
 
 def test_write():
     dict_config = {
         'endpoint': 'opc.tcp://localhost:4841/freeopcua/server/',
         'timeout': 4,
         'security': '',  #
@@ -99,8 +99,8 @@
     while True:
         for name, point in dict_point.items():
             point['point_value'] = f"{random.randint(1, 100)}"
         client.simulate(points=dict_point)
         time.sleep(1)
 
 
-test_simulate()
+test_read()
```

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_plc_ab.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_plc_ab.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_plc_mitsubishi.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_plc_omron.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_plc_omron.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_plc_s7.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_plc_s7.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,8 +85,24 @@
             re = client.read()
             print(re)
         except Exception as e:
             print(f"error: {e.__str__()}")
         time.sleep(4)
 
 
-test_read()
+def test_read1():
+    dict_config = {'multi_read': 20, 'cmd_interval': 0.3, 'send_timeout': 15, 'rec_timeout': 3500}
+    dict_point = {}
+    dict_point['plc1'] = {'point_writable': True, 'point_name': 'plc1', 'point_device_address': '127.0.0.1/102/0/1', 'point_address': 'DB1,INT1', 'point_scale': '1'}
+
+    client = IOTPlcS7(configs=dict_config, points=dict_point)
+    client.logging(call_logging=logging_print)
+    while True:
+        try:
+            re = client.read()
+            print(re)
+        except Exception as e:
+            print(f"error: {e.__str__()}")
+        time.sleep(4)
+
+
+test_read1()
```

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_plc_siemens.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_plc_siemens.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.39/tests/test_system/test_iot/test_iot_snmp.py` & `RobertCommonDriver-0.1.40/tests/test_system/test_iot/test_iot_snmp.py`

 * *Files identical despite different names*

