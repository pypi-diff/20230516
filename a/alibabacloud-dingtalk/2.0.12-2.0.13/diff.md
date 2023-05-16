# Comparing `tmp/alibabacloud_dingtalk-2.0.12.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.12.tar", last modified: Fri May 12 10:18:21 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.13.tar", last modified: Tue May 16 02:06:51 2023, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.12.tar` & `alibabacloud_dingtalk-2.0.13.tar`

### file list

```diff
@@ -1,357 +1,357 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/
--rw-r--r--   0 root         (0) root         (0)    19427 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2309 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1106 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23314 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169621 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46194 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21260 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23341 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90648 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138912 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   153926 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   284895 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    62246 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   201848 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   565599 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4942 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3871 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   138548 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   328853 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42229 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35138 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   101075 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123179 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    85810 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110530 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124904 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   293352 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   387566 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42332 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6576 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10253 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30852 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   220322 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   547684 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7385 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46898 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   515455 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152480 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56301 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45840 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    65285 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   211006 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   267473 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   150160 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   269103 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   195538 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   453174 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   705965 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   116546 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123749 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5096 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     6148 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   312544 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   433417 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   155788 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   302125 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5282 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     5179 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4431 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4668 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9742 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138362 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18903 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5382 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4660 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92926 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137528 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   302532 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   378971 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13884 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18281 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    92472 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   523174 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   756557 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   155140 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108695 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   135110 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23076 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   129226 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   157569 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54521 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31076 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40802 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7507 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76720 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137701 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123420 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60347 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    69069 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260568 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   413706 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    11593 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   174524 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81780 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    93746 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56986 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    83842 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46018 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   361006 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   503423 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26678 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    96217 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   353698 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44880 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    81308 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28559 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65344 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   147980 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16170 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21677 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17519 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18718 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    32237 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110849 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4269 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20486 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53454 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   118368 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8325 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27686 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    29689 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   175082 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   370377 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3772 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   464194 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   687148 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2309 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11743 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2684 2023-05-12 10:18:21.000000 alibabacloud_dingtalk-2.0.12/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/
+-rw-r--r--   0 root         (0) root         (0)    19492 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23314 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169621 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46194 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21260 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23341 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90648 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138912 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   158124 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   299469 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    62246 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   201848 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   569113 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4942 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3871 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   138814 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   331545 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42229 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35138 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   101075 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123179 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    85810 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110530 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124904 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   293352 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   387566 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42332 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6576 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10253 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30852 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   220322 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   547684 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7385 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46898 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515455 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152480 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56301 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45840 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    65285 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   211006 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   267473 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   150160 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   269103 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   195538 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   453174 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   705965 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   116546 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123749 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   312544 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   433417 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   155788 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   302125 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5282 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     5179 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4431 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4668 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9742 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138362 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18903 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92926 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137528 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   302532 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   378971 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13884 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18281 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    92472 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   523174 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   756557 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   155140 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108695 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   135110 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   131349 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   159547 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54521 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31076 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40802 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76720 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137701 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123420 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60347 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    69069 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260568 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413706 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    11593 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   174524 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81780 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    93746 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56986 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    83842 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46018 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   361006 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   503423 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26678 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    96217 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   353698 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44880 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    81308 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28559 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65344 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   147980 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16170 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21677 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17519 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18718 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    32237 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110849 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4269 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20486 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53454 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   118368 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27686 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    29689 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   175082 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   370377 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   464194 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   687148 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11743 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 02:06:51.000000 alibabacloud_dingtalk-2.0.13/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2684 2023-05-16 02:06:50.000000 alibabacloud_dingtalk-2.0.13/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.12/ChangeLog.md` & `alibabacloud_dingtalk-2.0.13/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-05-12 Version: 2.0.12
+- Update AddOfficialAccountFollower.
+
 2023-05-09 Version: 2.0.11
 - Update AddOfficialAccountFollower.
 
 2023-04-28 Version: 2.0.10
 - Update AddOfficialAccountFollower.
 
 2023-04-26 Version: 2.0.0
```

### Comparing `alibabacloud_dingtalk-2.0.12/LICENSE` & `alibabacloud_dingtalk-2.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/PKG-INFO` & `alibabacloud_dingtalk-2.0.13/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.0.12
+Version: 2.0.13
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.12/README-CN.md` & `alibabacloud_dingtalk-2.0.13/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/README.md` & `alibabacloud_dingtalk-2.0.13/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2917,14 +2917,108 @@
         self,
         request: dingtalkattendance__1__0_models.ProcessApproveCreateRequest,
     ) -> dingtalkattendance__1__0_models.ProcessApproveCreateResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkattendance__1__0_models.ProcessApproveCreateHeaders()
         return await self.process_approve_create_with_options_async(request, headers, runtime)
 
+    def retain_leave_types_with_options(
+        self,
+        request: dingtalkattendance__1__0_models.RetainLeaveTypesRequest,
+        headers: dingtalkattendance__1__0_models.RetainLeaveTypesHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkattendance__1__0_models.RetainLeaveTypesResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.leave_codes):
+            body['leaveCodes'] = request.leave_codes
+        if not UtilClient.is_unset(request.op_user_id):
+            body['opUserId'] = request.op_user_id
+        if not UtilClient.is_unset(request.source):
+            body['source'] = request.source
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='RetainLeaveTypes',
+            version='attendance_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/attendance/vacations/types/change',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkattendance__1__0_models.RetainLeaveTypesResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def retain_leave_types_with_options_async(
+        self,
+        request: dingtalkattendance__1__0_models.RetainLeaveTypesRequest,
+        headers: dingtalkattendance__1__0_models.RetainLeaveTypesHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkattendance__1__0_models.RetainLeaveTypesResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.leave_codes):
+            body['leaveCodes'] = request.leave_codes
+        if not UtilClient.is_unset(request.op_user_id):
+            body['opUserId'] = request.op_user_id
+        if not UtilClient.is_unset(request.source):
+            body['source'] = request.source
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='RetainLeaveTypes',
+            version='attendance_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/attendance/vacations/types/change',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkattendance__1__0_models.RetainLeaveTypesResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def retain_leave_types(
+        self,
+        request: dingtalkattendance__1__0_models.RetainLeaveTypesRequest,
+    ) -> dingtalkattendance__1__0_models.RetainLeaveTypesResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkattendance__1__0_models.RetainLeaveTypesHeaders()
+        return self.retain_leave_types_with_options(request, headers, runtime)
+
+    async def retain_leave_types_async(
+        self,
+        request: dingtalkattendance__1__0_models.RetainLeaveTypesRequest,
+    ) -> dingtalkattendance__1__0_models.RetainLeaveTypesResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkattendance__1__0_models.RetainLeaveTypesHeaders()
+        return await self.retain_leave_types_with_options_async(request, headers, runtime)
+
     def save_custom_water_mark_template_with_options(
         self,
         request: dingtalkattendance__1__0_models.SaveCustomWaterMarkTemplateRequest,
         headers: dingtalkattendance__1__0_models.SaveCustomWaterMarkTemplateHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkattendance__1__0_models.SaveCustomWaterMarkTemplateResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -7701,14 +7701,431 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ProcessApproveCreateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class RetainLeaveTypesHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class RetainLeaveTypesRequest(TeaModel):
+    def __init__(
+        self,
+        leave_codes: List[str] = None,
+        op_user_id: str = None,
+        source: int = None,
+    ):
+        self.leave_codes = leave_codes
+        self.op_user_id = op_user_id
+        self.source = source
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.leave_codes is not None:
+            result['leaveCodes'] = self.leave_codes
+        if self.op_user_id is not None:
+            result['opUserId'] = self.op_user_id
+        if self.source is not None:
+            result['source'] = self.source
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('leaveCodes') is not None:
+            self.leave_codes = m.get('leaveCodes')
+        if m.get('opUserId') is not None:
+            self.op_user_id = m.get('opUserId')
+        if m.get('source') is not None:
+            self.source = m.get('source')
+        return self
+
+
+class RetainLeaveTypesResponseBodyResultLeaveCertificate(TeaModel):
+    def __init__(
+        self,
+        duration: float = None,
+        enable: bool = None,
+        prompt_information: str = None,
+        unit: str = None,
+    ):
+        self.duration = duration
+        self.enable = enable
+        self.prompt_information = prompt_information
+        self.unit = unit
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.duration is not None:
+            result['duration'] = self.duration
+        if self.enable is not None:
+            result['enable'] = self.enable
+        if self.prompt_information is not None:
+            result['promptInformation'] = self.prompt_information
+        if self.unit is not None:
+            result['unit'] = self.unit
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('duration') is not None:
+            self.duration = m.get('duration')
+        if m.get('enable') is not None:
+            self.enable = m.get('enable')
+        if m.get('promptInformation') is not None:
+            self.prompt_information = m.get('promptInformation')
+        if m.get('unit') is not None:
+            self.unit = m.get('unit')
+        return self
+
+
+class RetainLeaveTypesResponseBodyResultSubmitTimeRule(TeaModel):
+    def __init__(
+        self,
+        enable_time_limit: bool = None,
+        time_type: str = None,
+        time_unit: str = None,
+        time_value: int = None,
+    ):
+        self.enable_time_limit = enable_time_limit
+        self.time_type = time_type
+        self.time_unit = time_unit
+        self.time_value = time_value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.enable_time_limit is not None:
+            result['enableTimeLimit'] = self.enable_time_limit
+        if self.time_type is not None:
+            result['timeType'] = self.time_type
+        if self.time_unit is not None:
+            result['timeUnit'] = self.time_unit
+        if self.time_value is not None:
+            result['timeValue'] = self.time_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('enableTimeLimit') is not None:
+            self.enable_time_limit = m.get('enableTimeLimit')
+        if m.get('timeType') is not None:
+            self.time_type = m.get('timeType')
+        if m.get('timeUnit') is not None:
+            self.time_unit = m.get('timeUnit')
+        if m.get('timeValue') is not None:
+            self.time_value = m.get('timeValue')
+        return self
+
+
+class RetainLeaveTypesResponseBodyResultVisibilityRules(TeaModel):
+    def __init__(
+        self,
+        type: str = None,
+        visible: List[str] = None,
+    ):
+        self.type = type
+        self.visible = visible
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.type is not None:
+            result['type'] = self.type
+        if self.visible is not None:
+            result['visible'] = self.visible
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        if m.get('visible') is not None:
+            self.visible = m.get('visible')
+        return self
+
+
+class RetainLeaveTypesResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        biz_type: str = None,
+        hours_in_per_day: int = None,
+        leave_certificate: RetainLeaveTypesResponseBodyResultLeaveCertificate = None,
+        leave_code: str = None,
+        leave_hour_ceil: str = None,
+        leave_name: str = None,
+        leave_time_ceil: bool = None,
+        leave_time_ceil_min_unit: str = None,
+        leave_view_unit: str = None,
+        lieu_delay_num: int = None,
+        lieu_delay_unit: str = None,
+        max_leave_time: int = None,
+        min_leave_hour: float = None,
+        natural_day_leave: bool = None,
+        paid_leave: bool = None,
+        submit_time_rule: RetainLeaveTypesResponseBodyResultSubmitTimeRule = None,
+        visibility_rules: List[RetainLeaveTypesResponseBodyResultVisibilityRules] = None,
+        when_can_leave: str = None,
+    ):
+        self.biz_type = biz_type
+        self.hours_in_per_day = hours_in_per_day
+        self.leave_certificate = leave_certificate
+        self.leave_code = leave_code
+        self.leave_hour_ceil = leave_hour_ceil
+        self.leave_name = leave_name
+        self.leave_time_ceil = leave_time_ceil
+        self.leave_time_ceil_min_unit = leave_time_ceil_min_unit
+        self.leave_view_unit = leave_view_unit
+        self.lieu_delay_num = lieu_delay_num
+        self.lieu_delay_unit = lieu_delay_unit
+        self.max_leave_time = max_leave_time
+        self.min_leave_hour = min_leave_hour
+        self.natural_day_leave = natural_day_leave
+        self.paid_leave = paid_leave
+        self.submit_time_rule = submit_time_rule
+        self.visibility_rules = visibility_rules
+        self.when_can_leave = when_can_leave
+
+    def validate(self):
+        if self.leave_certificate:
+            self.leave_certificate.validate()
+        if self.submit_time_rule:
+            self.submit_time_rule.validate()
+        if self.visibility_rules:
+            for k in self.visibility_rules:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.biz_type is not None:
+            result['bizType'] = self.biz_type
+        if self.hours_in_per_day is not None:
+            result['hoursInPerDay'] = self.hours_in_per_day
+        if self.leave_certificate is not None:
+            result['leaveCertificate'] = self.leave_certificate.to_map()
+        if self.leave_code is not None:
+            result['leaveCode'] = self.leave_code
+        if self.leave_hour_ceil is not None:
+            result['leaveHourCeil'] = self.leave_hour_ceil
+        if self.leave_name is not None:
+            result['leaveName'] = self.leave_name
+        if self.leave_time_ceil is not None:
+            result['leaveTimeCeil'] = self.leave_time_ceil
+        if self.leave_time_ceil_min_unit is not None:
+            result['leaveTimeCeilMinUnit'] = self.leave_time_ceil_min_unit
+        if self.leave_view_unit is not None:
+            result['leaveViewUnit'] = self.leave_view_unit
+        if self.lieu_delay_num is not None:
+            result['lieuDelayNum'] = self.lieu_delay_num
+        if self.lieu_delay_unit is not None:
+            result['lieuDelayUnit'] = self.lieu_delay_unit
+        if self.max_leave_time is not None:
+            result['maxLeaveTime'] = self.max_leave_time
+        if self.min_leave_hour is not None:
+            result['minLeaveHour'] = self.min_leave_hour
+        if self.natural_day_leave is not None:
+            result['naturalDayLeave'] = self.natural_day_leave
+        if self.paid_leave is not None:
+            result['paidLeave'] = self.paid_leave
+        if self.submit_time_rule is not None:
+            result['submitTimeRule'] = self.submit_time_rule.to_map()
+        result['visibilityRules'] = []
+        if self.visibility_rules is not None:
+            for k in self.visibility_rules:
+                result['visibilityRules'].append(k.to_map() if k else None)
+        if self.when_can_leave is not None:
+            result['whenCanLeave'] = self.when_can_leave
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('bizType') is not None:
+            self.biz_type = m.get('bizType')
+        if m.get('hoursInPerDay') is not None:
+            self.hours_in_per_day = m.get('hoursInPerDay')
+        if m.get('leaveCertificate') is not None:
+            temp_model = RetainLeaveTypesResponseBodyResultLeaveCertificate()
+            self.leave_certificate = temp_model.from_map(m['leaveCertificate'])
+        if m.get('leaveCode') is not None:
+            self.leave_code = m.get('leaveCode')
+        if m.get('leaveHourCeil') is not None:
+            self.leave_hour_ceil = m.get('leaveHourCeil')
+        if m.get('leaveName') is not None:
+            self.leave_name = m.get('leaveName')
+        if m.get('leaveTimeCeil') is not None:
+            self.leave_time_ceil = m.get('leaveTimeCeil')
+        if m.get('leaveTimeCeilMinUnit') is not None:
+            self.leave_time_ceil_min_unit = m.get('leaveTimeCeilMinUnit')
+        if m.get('leaveViewUnit') is not None:
+            self.leave_view_unit = m.get('leaveViewUnit')
+        if m.get('lieuDelayNum') is not None:
+            self.lieu_delay_num = m.get('lieuDelayNum')
+        if m.get('lieuDelayUnit') is not None:
+            self.lieu_delay_unit = m.get('lieuDelayUnit')
+        if m.get('maxLeaveTime') is not None:
+            self.max_leave_time = m.get('maxLeaveTime')
+        if m.get('minLeaveHour') is not None:
+            self.min_leave_hour = m.get('minLeaveHour')
+        if m.get('naturalDayLeave') is not None:
+            self.natural_day_leave = m.get('naturalDayLeave')
+        if m.get('paidLeave') is not None:
+            self.paid_leave = m.get('paidLeave')
+        if m.get('submitTimeRule') is not None:
+            temp_model = RetainLeaveTypesResponseBodyResultSubmitTimeRule()
+            self.submit_time_rule = temp_model.from_map(m['submitTimeRule'])
+        self.visibility_rules = []
+        if m.get('visibilityRules') is not None:
+            for k in m.get('visibilityRules'):
+                temp_model = RetainLeaveTypesResponseBodyResultVisibilityRules()
+                self.visibility_rules.append(temp_model.from_map(k))
+        if m.get('whenCanLeave') is not None:
+            self.when_can_leave = m.get('whenCanLeave')
+        return self
+
+
+class RetainLeaveTypesResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: List[RetainLeaveTypesResponseBodyResult] = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            for k in self.result:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['result'] = []
+        if self.result is not None:
+            for k in self.result:
+                result['result'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.result = []
+        if m.get('result') is not None:
+            for k in m.get('result'):
+                temp_model = RetainLeaveTypesResponseBodyResult()
+                self.result.append(temp_model.from_map(k))
+        return self
+
+
+class RetainLeaveTypesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: RetainLeaveTypesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = RetainLeaveTypesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class SaveCustomWaterMarkTemplateHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -523,19 +523,21 @@
     def __init__(
         self,
         account_period: str = None,
         amount: str = None,
         amount_with_tax: str = None,
         check_code: str = None,
         check_time: str = None,
+        drawer_name: str = None,
         drew_date: str = None,
         electronic_url: str = None,
         finance_type: str = None,
         fund_type: str = None,
         general_invoice_detail_volist: List[BatchAddInvoiceRequestGeneralInvoiceVOListGeneralInvoiceDetailVOList] = None,
+        image_url: str = None,
         invoice_code: str = None,
         invoice_no: str = None,
         invoice_status: str = None,
         invoice_type: str = None,
         machine_code: str = None,
         oil_flag: str = None,
         payee: str = None,
@@ -564,19 +566,21 @@
         voucher_status: str = None,
     ):
         self.account_period = account_period
         self.amount = amount
         self.amount_with_tax = amount_with_tax
         self.check_code = check_code
         self.check_time = check_time
+        self.drawer_name = drawer_name
         self.drew_date = drew_date
         self.electronic_url = electronic_url
         self.finance_type = finance_type
         self.fund_type = fund_type
         self.general_invoice_detail_volist = general_invoice_detail_volist
+        self.image_url = image_url
         self.invoice_code = invoice_code
         self.invoice_no = invoice_no
         self.invoice_status = invoice_status
         self.invoice_type = invoice_type
         self.machine_code = machine_code
         self.oil_flag = oil_flag
         self.payee = payee
@@ -634,26 +638,30 @@
             result['amount'] = self.amount
         if self.amount_with_tax is not None:
             result['amountWithTax'] = self.amount_with_tax
         if self.check_code is not None:
             result['checkCode'] = self.check_code
         if self.check_time is not None:
             result['checkTime'] = self.check_time
+        if self.drawer_name is not None:
+            result['drawerName'] = self.drawer_name
         if self.drew_date is not None:
             result['drewDate'] = self.drew_date
         if self.electronic_url is not None:
             result['electronicUrl'] = self.electronic_url
         if self.finance_type is not None:
             result['financeType'] = self.finance_type
         if self.fund_type is not None:
             result['fundType'] = self.fund_type
         result['generalInvoiceDetailVOList'] = []
         if self.general_invoice_detail_volist is not None:
             for k in self.general_invoice_detail_volist:
                 result['generalInvoiceDetailVOList'].append(k.to_map() if k else None)
+        if self.image_url is not None:
+            result['imageUrl'] = self.image_url
         if self.invoice_code is not None:
             result['invoiceCode'] = self.invoice_code
         if self.invoice_no is not None:
             result['invoiceNo'] = self.invoice_no
         if self.invoice_status is not None:
             result['invoiceStatus'] = self.invoice_status
         if self.invoice_type is not None:
@@ -726,27 +734,31 @@
             self.amount = m.get('amount')
         if m.get('amountWithTax') is not None:
             self.amount_with_tax = m.get('amountWithTax')
         if m.get('checkCode') is not None:
             self.check_code = m.get('checkCode')
         if m.get('checkTime') is not None:
             self.check_time = m.get('checkTime')
+        if m.get('drawerName') is not None:
+            self.drawer_name = m.get('drawerName')
         if m.get('drewDate') is not None:
             self.drew_date = m.get('drewDate')
         if m.get('electronicUrl') is not None:
             self.electronic_url = m.get('electronicUrl')
         if m.get('financeType') is not None:
             self.finance_type = m.get('financeType')
         if m.get('fundType') is not None:
             self.fund_type = m.get('fundType')
         self.general_invoice_detail_volist = []
         if m.get('generalInvoiceDetailVOList') is not None:
             for k in m.get('generalInvoiceDetailVOList'):
                 temp_model = BatchAddInvoiceRequestGeneralInvoiceVOListGeneralInvoiceDetailVOList()
                 self.general_invoice_detail_volist.append(temp_model.from_map(k))
+        if m.get('imageUrl') is not None:
+            self.image_url = m.get('imageUrl')
         if m.get('invoiceCode') is not None:
             self.invoice_code = m.get('invoiceCode')
         if m.get('invoiceNo') is not None:
             self.invoice_no = m.get('invoiceNo')
         if m.get('invoiceStatus') is not None:
             self.invoice_status = m.get('invoiceStatus')
         if m.get('invoiceType') is not None:
@@ -9342,19 +9354,21 @@
     def __init__(
         self,
         account_period: str = None,
         amount: str = None,
         amount_with_tax: str = None,
         check_code: str = None,
         check_time: str = None,
+        drawer_name: str = None,
         drew_date: str = None,
         electronic_url: str = None,
         finance_type: str = None,
         fund_type: str = None,
         general_invoice_detail_volist: List[UpdateApplyReceiptAndInvoiceRelatedRequestGeneralInvoiceVOListGeneralInvoiceDetailVOList] = None,
+        image_url: str = None,
         invoice_code: str = None,
         invoice_no: str = None,
         invoice_status: str = None,
         invoice_type: str = None,
         machine_code: str = None,
         oil_flag: str = None,
         payee: str = None,
@@ -9383,19 +9397,21 @@
         voucher_status: str = None,
     ):
         self.account_period = account_period
         self.amount = amount
         self.amount_with_tax = amount_with_tax
         self.check_code = check_code
         self.check_time = check_time
+        self.drawer_name = drawer_name
         self.drew_date = drew_date
         self.electronic_url = electronic_url
         self.finance_type = finance_type
         self.fund_type = fund_type
         self.general_invoice_detail_volist = general_invoice_detail_volist
+        self.image_url = image_url
         self.invoice_code = invoice_code
         self.invoice_no = invoice_no
         self.invoice_status = invoice_status
         self.invoice_type = invoice_type
         self.machine_code = machine_code
         self.oil_flag = oil_flag
         self.payee = payee
@@ -9453,26 +9469,30 @@
             result['amount'] = self.amount
         if self.amount_with_tax is not None:
             result['amountWithTax'] = self.amount_with_tax
         if self.check_code is not None:
             result['checkCode'] = self.check_code
         if self.check_time is not None:
             result['checkTime'] = self.check_time
+        if self.drawer_name is not None:
+            result['drawerName'] = self.drawer_name
         if self.drew_date is not None:
             result['drewDate'] = self.drew_date
         if self.electronic_url is not None:
             result['electronicUrl'] = self.electronic_url
         if self.finance_type is not None:
             result['financeType'] = self.finance_type
         if self.fund_type is not None:
             result['fundType'] = self.fund_type
         result['generalInvoiceDetailVOList'] = []
         if self.general_invoice_detail_volist is not None:
             for k in self.general_invoice_detail_volist:
                 result['generalInvoiceDetailVOList'].append(k.to_map() if k else None)
+        if self.image_url is not None:
+            result['imageUrl'] = self.image_url
         if self.invoice_code is not None:
             result['invoiceCode'] = self.invoice_code
         if self.invoice_no is not None:
             result['invoiceNo'] = self.invoice_no
         if self.invoice_status is not None:
             result['invoiceStatus'] = self.invoice_status
         if self.invoice_type is not None:
@@ -9545,27 +9565,31 @@
             self.amount = m.get('amount')
         if m.get('amountWithTax') is not None:
             self.amount_with_tax = m.get('amountWithTax')
         if m.get('checkCode') is not None:
             self.check_code = m.get('checkCode')
         if m.get('checkTime') is not None:
             self.check_time = m.get('checkTime')
+        if m.get('drawerName') is not None:
+            self.drawer_name = m.get('drawerName')
         if m.get('drewDate') is not None:
             self.drew_date = m.get('drewDate')
         if m.get('electronicUrl') is not None:
             self.electronic_url = m.get('electronicUrl')
         if m.get('financeType') is not None:
             self.finance_type = m.get('financeType')
         if m.get('fundType') is not None:
             self.fund_type = m.get('fundType')
         self.general_invoice_detail_volist = []
         if m.get('generalInvoiceDetailVOList') is not None:
             for k in m.get('generalInvoiceDetailVOList'):
                 temp_model = UpdateApplyReceiptAndInvoiceRelatedRequestGeneralInvoiceVOListGeneralInvoiceDetailVOList()
                 self.general_invoice_detail_volist.append(temp_model.from_map(k))
+        if m.get('imageUrl') is not None:
+            self.image_url = m.get('imageUrl')
         if m.get('invoiceCode') is not None:
             self.invoice_code = m.get('invoiceCode')
         if m.get('invoiceNo') is not None:
             self.invoice_no = m.get('invoiceNo')
         if m.get('invoiceStatus') is not None:
             self.invoice_status = m.get('invoiceStatus')
         if m.get('invoiceType') is not None:
@@ -10565,19 +10589,21 @@
     def __init__(
         self,
         account_period: str = None,
         amount: str = None,
         amount_with_tax: str = None,
         check_code: str = None,
         check_time: str = None,
+        drawer_name: str = None,
         drew_date: str = None,
         electronic_url: str = None,
         finance_type: str = None,
         fund_type: str = None,
         general_invoice_detail_volist: List[UpdateInvoiceAbandonStatusRequestBlueGeneralInvoiceVOGeneralInvoiceDetailVOList] = None,
+        image_url: str = None,
         invoice_code: str = None,
         invoice_no: str = None,
         invoice_status: str = None,
         invoice_type: str = None,
         machine_code: str = None,
         oil_flag: str = None,
         payee: str = None,
@@ -10606,19 +10632,21 @@
         voucher_status: str = None,
     ):
         self.account_period = account_period
         self.amount = amount
         self.amount_with_tax = amount_with_tax
         self.check_code = check_code
         self.check_time = check_time
+        self.drawer_name = drawer_name
         self.drew_date = drew_date
         self.electronic_url = electronic_url
         self.finance_type = finance_type
         self.fund_type = fund_type
         self.general_invoice_detail_volist = general_invoice_detail_volist
+        self.image_url = image_url
         self.invoice_code = invoice_code
         self.invoice_no = invoice_no
         self.invoice_status = invoice_status
         self.invoice_type = invoice_type
         self.machine_code = machine_code
         self.oil_flag = oil_flag
         self.payee = payee
@@ -10676,26 +10704,30 @@
             result['amount'] = self.amount
         if self.amount_with_tax is not None:
             result['amountWithTax'] = self.amount_with_tax
         if self.check_code is not None:
             result['checkCode'] = self.check_code
         if self.check_time is not None:
             result['checkTime'] = self.check_time
+        if self.drawer_name is not None:
+            result['drawerName'] = self.drawer_name
         if self.drew_date is not None:
             result['drewDate'] = self.drew_date
         if self.electronic_url is not None:
             result['electronicUrl'] = self.electronic_url
         if self.finance_type is not None:
             result['financeType'] = self.finance_type
         if self.fund_type is not None:
             result['fundType'] = self.fund_type
         result['generalInvoiceDetailVOList'] = []
         if self.general_invoice_detail_volist is not None:
             for k in self.general_invoice_detail_volist:
                 result['generalInvoiceDetailVOList'].append(k.to_map() if k else None)
+        if self.image_url is not None:
+            result['imageUrl'] = self.image_url
         if self.invoice_code is not None:
             result['invoiceCode'] = self.invoice_code
         if self.invoice_no is not None:
             result['invoiceNo'] = self.invoice_no
         if self.invoice_status is not None:
             result['invoiceStatus'] = self.invoice_status
         if self.invoice_type is not None:
@@ -10768,27 +10800,31 @@
             self.amount = m.get('amount')
         if m.get('amountWithTax') is not None:
             self.amount_with_tax = m.get('amountWithTax')
         if m.get('checkCode') is not None:
             self.check_code = m.get('checkCode')
         if m.get('checkTime') is not None:
             self.check_time = m.get('checkTime')
+        if m.get('drawerName') is not None:
+            self.drawer_name = m.get('drawerName')
         if m.get('drewDate') is not None:
             self.drew_date = m.get('drewDate')
         if m.get('electronicUrl') is not None:
             self.electronic_url = m.get('electronicUrl')
         if m.get('financeType') is not None:
             self.finance_type = m.get('financeType')
         if m.get('fundType') is not None:
             self.fund_type = m.get('fundType')
         self.general_invoice_detail_volist = []
         if m.get('generalInvoiceDetailVOList') is not None:
             for k in m.get('generalInvoiceDetailVOList'):
                 temp_model = UpdateInvoiceAbandonStatusRequestBlueGeneralInvoiceVOGeneralInvoiceDetailVOList()
                 self.general_invoice_detail_volist.append(temp_model.from_map(k))
+        if m.get('imageUrl') is not None:
+            self.image_url = m.get('imageUrl')
         if m.get('invoiceCode') is not None:
             self.invoice_code = m.get('invoiceCode')
         if m.get('invoiceNo') is not None:
             self.invoice_no = m.get('invoiceNo')
         if m.get('invoiceStatus') is not None:
             self.invoice_status = m.get('invoiceStatus')
         if m.get('invoiceType') is not None:
@@ -11263,19 +11299,21 @@
     def __init__(
         self,
         account_period: str = None,
         amount: str = None,
         amount_with_tax: str = None,
         check_code: str = None,
         check_time: str = None,
+        drawer_name: str = None,
         drew_date: str = None,
         electronic_url: str = None,
         finance_type: str = None,
         fund_type: str = None,
         general_invoice_detail_volist: List[UpdateInvoiceAbandonStatusRequestRedGeneralInvoiceVOGeneralInvoiceDetailVOList] = None,
+        image_url: str = None,
         invoice_code: str = None,
         invoice_no: str = None,
         invoice_status: str = None,
         invoice_type: str = None,
         machine_code: str = None,
         oil_flag: str = None,
         payee: str = None,
@@ -11304,19 +11342,21 @@
         voucher_status: str = None,
     ):
         self.account_period = account_period
         self.amount = amount
         self.amount_with_tax = amount_with_tax
         self.check_code = check_code
         self.check_time = check_time
+        self.drawer_name = drawer_name
         self.drew_date = drew_date
         self.electronic_url = electronic_url
         self.finance_type = finance_type
         self.fund_type = fund_type
         self.general_invoice_detail_volist = general_invoice_detail_volist
+        self.image_url = image_url
         self.invoice_code = invoice_code
         self.invoice_no = invoice_no
         self.invoice_status = invoice_status
         self.invoice_type = invoice_type
         self.machine_code = machine_code
         self.oil_flag = oil_flag
         self.payee = payee
@@ -11374,26 +11414,30 @@
             result['amount'] = self.amount
         if self.amount_with_tax is not None:
             result['amountWithTax'] = self.amount_with_tax
         if self.check_code is not None:
             result['checkCode'] = self.check_code
         if self.check_time is not None:
             result['checkTime'] = self.check_time
+        if self.drawer_name is not None:
+            result['drawerName'] = self.drawer_name
         if self.drew_date is not None:
             result['drewDate'] = self.drew_date
         if self.electronic_url is not None:
             result['electronicUrl'] = self.electronic_url
         if self.finance_type is not None:
             result['financeType'] = self.finance_type
         if self.fund_type is not None:
             result['fundType'] = self.fund_type
         result['generalInvoiceDetailVOList'] = []
         if self.general_invoice_detail_volist is not None:
             for k in self.general_invoice_detail_volist:
                 result['generalInvoiceDetailVOList'].append(k.to_map() if k else None)
+        if self.image_url is not None:
+            result['imageUrl'] = self.image_url
         if self.invoice_code is not None:
             result['invoiceCode'] = self.invoice_code
         if self.invoice_no is not None:
             result['invoiceNo'] = self.invoice_no
         if self.invoice_status is not None:
             result['invoiceStatus'] = self.invoice_status
         if self.invoice_type is not None:
@@ -11466,27 +11510,31 @@
             self.amount = m.get('amount')
         if m.get('amountWithTax') is not None:
             self.amount_with_tax = m.get('amountWithTax')
         if m.get('checkCode') is not None:
             self.check_code = m.get('checkCode')
         if m.get('checkTime') is not None:
             self.check_time = m.get('checkTime')
+        if m.get('drawerName') is not None:
+            self.drawer_name = m.get('drawerName')
         if m.get('drewDate') is not None:
             self.drew_date = m.get('drewDate')
         if m.get('electronicUrl') is not None:
             self.electronic_url = m.get('electronicUrl')
         if m.get('financeType') is not None:
             self.finance_type = m.get('financeType')
         if m.get('fundType') is not None:
             self.fund_type = m.get('fundType')
         self.general_invoice_detail_volist = []
         if m.get('generalInvoiceDetailVOList') is not None:
             for k in m.get('generalInvoiceDetailVOList'):
                 temp_model = UpdateInvoiceAbandonStatusRequestRedGeneralInvoiceVOGeneralInvoiceDetailVOList()
                 self.general_invoice_detail_volist.append(temp_model.from_map(k))
+        if m.get('imageUrl') is not None:
+            self.image_url = m.get('imageUrl')
         if m.get('invoiceCode') is not None:
             self.invoice_code = m.get('invoiceCode')
         if m.get('invoiceNo') is not None:
             self.invoice_no = m.get('invoiceNo')
         if m.get('invoiceStatus') is not None:
             self.invoice_status = m.get('invoiceStatus')
         if m.get('invoiceType') is not None:
@@ -12151,19 +12199,21 @@
     def __init__(
         self,
         account_period: str = None,
         amount: str = None,
         amount_with_tax: str = None,
         check_code: str = None,
         check_time: str = None,
+        drawer_name: str = None,
         drew_date: str = None,
         electronic_url: str = None,
         finance_type: str = None,
         fund_type: str = None,
         general_invoice_detail_volist: List[UpdateInvoiceAccountPeriodRequestGeneralInvoiceVOListGeneralInvoiceDetailVOList] = None,
+        image_url: str = None,
         invoice_code: str = None,
         invoice_no: str = None,
         invoice_status: str = None,
         invoice_type: str = None,
         machine_code: str = None,
         oil_flag: str = None,
         payee: str = None,
@@ -12192,19 +12242,21 @@
         voucher_status: str = None,
     ):
         self.account_period = account_period
         self.amount = amount
         self.amount_with_tax = amount_with_tax
         self.check_code = check_code
         self.check_time = check_time
+        self.drawer_name = drawer_name
         self.drew_date = drew_date
         self.electronic_url = electronic_url
         self.finance_type = finance_type
         self.fund_type = fund_type
         self.general_invoice_detail_volist = general_invoice_detail_volist
+        self.image_url = image_url
         self.invoice_code = invoice_code
         self.invoice_no = invoice_no
         self.invoice_status = invoice_status
         self.invoice_type = invoice_type
         self.machine_code = machine_code
         self.oil_flag = oil_flag
         self.payee = payee
@@ -12262,26 +12314,30 @@
             result['amount'] = self.amount
         if self.amount_with_tax is not None:
             result['amountWithTax'] = self.amount_with_tax
         if self.check_code is not None:
             result['checkCode'] = self.check_code
         if self.check_time is not None:
             result['checkTime'] = self.check_time
+        if self.drawer_name is not None:
+            result['drawerName'] = self.drawer_name
         if self.drew_date is not None:
             result['drewDate'] = self.drew_date
         if self.electronic_url is not None:
             result['electronicUrl'] = self.electronic_url
         if self.finance_type is not None:
             result['financeType'] = self.finance_type
         if self.fund_type is not None:
             result['fundType'] = self.fund_type
         result['generalInvoiceDetailVOList'] = []
         if self.general_invoice_detail_volist is not None:
             for k in self.general_invoice_detail_volist:
                 result['generalInvoiceDetailVOList'].append(k.to_map() if k else None)
+        if self.image_url is not None:
+            result['imageUrl'] = self.image_url
         if self.invoice_code is not None:
             result['invoiceCode'] = self.invoice_code
         if self.invoice_no is not None:
             result['invoiceNo'] = self.invoice_no
         if self.invoice_status is not None:
             result['invoiceStatus'] = self.invoice_status
         if self.invoice_type is not None:
@@ -12354,27 +12410,31 @@
             self.amount = m.get('amount')
         if m.get('amountWithTax') is not None:
             self.amount_with_tax = m.get('amountWithTax')
         if m.get('checkCode') is not None:
             self.check_code = m.get('checkCode')
         if m.get('checkTime') is not None:
             self.check_time = m.get('checkTime')
+        if m.get('drawerName') is not None:
+            self.drawer_name = m.get('drawerName')
         if m.get('drewDate') is not None:
             self.drew_date = m.get('drewDate')
         if m.get('electronicUrl') is not None:
             self.electronic_url = m.get('electronicUrl')
         if m.get('financeType') is not None:
             self.finance_type = m.get('financeType')
         if m.get('fundType') is not None:
             self.fund_type = m.get('fundType')
         self.general_invoice_detail_volist = []
         if m.get('generalInvoiceDetailVOList') is not None:
             for k in m.get('generalInvoiceDetailVOList'):
                 temp_model = UpdateInvoiceAccountPeriodRequestGeneralInvoiceVOListGeneralInvoiceDetailVOList()
                 self.general_invoice_detail_volist.append(temp_model.from_map(k))
+        if m.get('imageUrl') is not None:
+            self.image_url = m.get('imageUrl')
         if m.get('invoiceCode') is not None:
             self.invoice_code = m.get('invoiceCode')
         if m.get('invoiceNo') is not None:
             self.invoice_no = m.get('invoiceNo')
         if m.get('invoiceStatus') is not None:
             self.invoice_status = m.get('invoiceStatus')
         if m.get('invoiceType') is not None:
@@ -13705,19 +13765,21 @@
     def __init__(
         self,
         account_period: str = None,
         amount: str = None,
         amount_with_tax: str = None,
         check_code: str = None,
         check_time: str = None,
+        drawer_name: str = None,
         drew_date: str = None,
         electronic_url: str = None,
         finance_type: str = None,
         fund_type: str = None,
         general_invoice_detail_volist: List[UpdateInvoiceAndReceiptRelatedRequestGeneralInvoiceVOGeneralInvoiceDetailVOList] = None,
+        image_url: str = None,
         invoice_code: str = None,
         invoice_no: str = None,
         invoice_status: str = None,
         invoice_type: str = None,
         machine_code: str = None,
         oil_flag: str = None,
         payee: str = None,
@@ -13746,19 +13808,21 @@
         voucher_status: str = None,
     ):
         self.account_period = account_period
         self.amount = amount
         self.amount_with_tax = amount_with_tax
         self.check_code = check_code
         self.check_time = check_time
+        self.drawer_name = drawer_name
         self.drew_date = drew_date
         self.electronic_url = electronic_url
         self.finance_type = finance_type
         self.fund_type = fund_type
         self.general_invoice_detail_volist = general_invoice_detail_volist
+        self.image_url = image_url
         self.invoice_code = invoice_code
         self.invoice_no = invoice_no
         self.invoice_status = invoice_status
         self.invoice_type = invoice_type
         self.machine_code = machine_code
         self.oil_flag = oil_flag
         self.payee = payee
@@ -13816,26 +13880,30 @@
             result['amount'] = self.amount
         if self.amount_with_tax is not None:
             result['amountWithTax'] = self.amount_with_tax
         if self.check_code is not None:
             result['checkCode'] = self.check_code
         if self.check_time is not None:
             result['checkTime'] = self.check_time
+        if self.drawer_name is not None:
+            result['drawerName'] = self.drawer_name
         if self.drew_date is not None:
             result['drewDate'] = self.drew_date
         if self.electronic_url is not None:
             result['electronicUrl'] = self.electronic_url
         if self.finance_type is not None:
             result['financeType'] = self.finance_type
         if self.fund_type is not None:
             result['fundType'] = self.fund_type
         result['generalInvoiceDetailVOList'] = []
         if self.general_invoice_detail_volist is not None:
             for k in self.general_invoice_detail_volist:
                 result['generalInvoiceDetailVOList'].append(k.to_map() if k else None)
+        if self.image_url is not None:
+            result['imageUrl'] = self.image_url
         if self.invoice_code is not None:
             result['invoiceCode'] = self.invoice_code
         if self.invoice_no is not None:
             result['invoiceNo'] = self.invoice_no
         if self.invoice_status is not None:
             result['invoiceStatus'] = self.invoice_status
         if self.invoice_type is not None:
@@ -13908,27 +13976,31 @@
             self.amount = m.get('amount')
         if m.get('amountWithTax') is not None:
             self.amount_with_tax = m.get('amountWithTax')
         if m.get('checkCode') is not None:
             self.check_code = m.get('checkCode')
         if m.get('checkTime') is not None:
             self.check_time = m.get('checkTime')
+        if m.get('drawerName') is not None:
+            self.drawer_name = m.get('drawerName')
         if m.get('drewDate') is not None:
             self.drew_date = m.get('drewDate')
         if m.get('electronicUrl') is not None:
             self.electronic_url = m.get('electronicUrl')
         if m.get('financeType') is not None:
             self.finance_type = m.get('financeType')
         if m.get('fundType') is not None:
             self.fund_type = m.get('fundType')
         self.general_invoice_detail_volist = []
         if m.get('generalInvoiceDetailVOList') is not None:
             for k in m.get('generalInvoiceDetailVOList'):
                 temp_model = UpdateInvoiceAndReceiptRelatedRequestGeneralInvoiceVOGeneralInvoiceDetailVOList()
                 self.general_invoice_detail_volist.append(temp_model.from_map(k))
+        if m.get('imageUrl') is not None:
+            self.image_url = m.get('imageUrl')
         if m.get('invoiceCode') is not None:
             self.invoice_code = m.get('invoiceCode')
         if m.get('invoiceNo') is not None:
             self.invoice_no = m.get('invoiceNo')
         if m.get('invoiceStatus') is not None:
             self.invoice_status = m.get('invoiceStatus')
         if m.get('invoiceType') is not None:
@@ -14703,19 +14775,21 @@
     def __init__(
         self,
         account_period: str = None,
         amount: str = None,
         amount_with_tax: str = None,
         check_code: str = None,
         check_time: str = None,
+        drawer_name: str = None,
         drew_date: str = None,
         electronic_url: str = None,
         finance_type: str = None,
         fund_type: str = None,
         general_invoice_detail_volist: List[UpdateInvoiceVerifyStatusRequestGeneralInvoiceVOListGeneralInvoiceDetailVOList] = None,
+        image_url: str = None,
         invoice_code: str = None,
         invoice_no: str = None,
         invoice_status: str = None,
         invoice_type: str = None,
         machine_code: str = None,
         oil_flag: str = None,
         payee: str = None,
@@ -14744,19 +14818,21 @@
         voucher_status: str = None,
     ):
         self.account_period = account_period
         self.amount = amount
         self.amount_with_tax = amount_with_tax
         self.check_code = check_code
         self.check_time = check_time
+        self.drawer_name = drawer_name
         self.drew_date = drew_date
         self.electronic_url = electronic_url
         self.finance_type = finance_type
         self.fund_type = fund_type
         self.general_invoice_detail_volist = general_invoice_detail_volist
+        self.image_url = image_url
         self.invoice_code = invoice_code
         self.invoice_no = invoice_no
         self.invoice_status = invoice_status
         self.invoice_type = invoice_type
         self.machine_code = machine_code
         self.oil_flag = oil_flag
         self.payee = payee
@@ -14814,26 +14890,30 @@
             result['amount'] = self.amount
         if self.amount_with_tax is not None:
             result['amountWithTax'] = self.amount_with_tax
         if self.check_code is not None:
             result['checkCode'] = self.check_code
         if self.check_time is not None:
             result['checkTime'] = self.check_time
+        if self.drawer_name is not None:
+            result['drawerName'] = self.drawer_name
         if self.drew_date is not None:
             result['drewDate'] = self.drew_date
         if self.electronic_url is not None:
             result['electronicUrl'] = self.electronic_url
         if self.finance_type is not None:
             result['financeType'] = self.finance_type
         if self.fund_type is not None:
             result['fundType'] = self.fund_type
         result['generalInvoiceDetailVOList'] = []
         if self.general_invoice_detail_volist is not None:
             for k in self.general_invoice_detail_volist:
                 result['generalInvoiceDetailVOList'].append(k.to_map() if k else None)
+        if self.image_url is not None:
+            result['imageUrl'] = self.image_url
         if self.invoice_code is not None:
             result['invoiceCode'] = self.invoice_code
         if self.invoice_no is not None:
             result['invoiceNo'] = self.invoice_no
         if self.invoice_status is not None:
             result['invoiceStatus'] = self.invoice_status
         if self.invoice_type is not None:
@@ -14906,27 +14986,31 @@
             self.amount = m.get('amount')
         if m.get('amountWithTax') is not None:
             self.amount_with_tax = m.get('amountWithTax')
         if m.get('checkCode') is not None:
             self.check_code = m.get('checkCode')
         if m.get('checkTime') is not None:
             self.check_time = m.get('checkTime')
+        if m.get('drawerName') is not None:
+            self.drawer_name = m.get('drawerName')
         if m.get('drewDate') is not None:
             self.drew_date = m.get('drewDate')
         if m.get('electronicUrl') is not None:
             self.electronic_url = m.get('electronicUrl')
         if m.get('financeType') is not None:
             self.finance_type = m.get('financeType')
         if m.get('fundType') is not None:
             self.fund_type = m.get('fundType')
         self.general_invoice_detail_volist = []
         if m.get('generalInvoiceDetailVOList') is not None:
             for k in m.get('generalInvoiceDetailVOList'):
                 temp_model = UpdateInvoiceVerifyStatusRequestGeneralInvoiceVOListGeneralInvoiceDetailVOList()
                 self.general_invoice_detail_volist.append(temp_model.from_map(k))
+        if m.get('imageUrl') is not None:
+            self.image_url = m.get('imageUrl')
         if m.get('invoiceCode') is not None:
             self.invoice_code = m.get('invoiceCode')
         if m.get('invoiceNo') is not None:
             self.invoice_no = m.get('invoiceNo')
         if m.get('invoiceStatus') is not None:
             self.invoice_status = m.get('invoiceStatus')
         if m.get('invoiceType') is not None:
```

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2400,14 +2400,16 @@
             body['extra'] = request.extra
         if not UtilClient.is_unset(request.id):
             body['id'] = request.id
         if not UtilClient.is_unset(request.is_all_day):
             body['isAllDay'] = request.is_all_day
         if not UtilClient.is_unset(request.location):
             body['location'] = request.location
+        if not UtilClient.is_unset(request.online_meeting_info):
+            body['onlineMeetingInfo'] = request.online_meeting_info
         if not UtilClient.is_unset(request.recurrence):
             body['recurrence'] = request.recurrence
         if not UtilClient.is_unset(request.reminders):
             body['reminders'] = request.reminders
         if not UtilClient.is_unset(request.start):
             body['start'] = request.start
         if not UtilClient.is_unset(request.summary):
@@ -2458,14 +2460,16 @@
             body['extra'] = request.extra
         if not UtilClient.is_unset(request.id):
             body['id'] = request.id
         if not UtilClient.is_unset(request.is_all_day):
             body['isAllDay'] = request.is_all_day
         if not UtilClient.is_unset(request.location):
             body['location'] = request.location
+        if not UtilClient.is_unset(request.online_meeting_info):
+            body['onlineMeetingInfo'] = request.online_meeting_info
         if not UtilClient.is_unset(request.recurrence):
             body['recurrence'] = request.recurrence
         if not UtilClient.is_unset(request.reminders):
             body['reminders'] = request.reminders
         if not UtilClient.is_unset(request.start):
             body['start'] = request.start
         if not UtilClient.is_unset(request.summary):
```

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -8766,14 +8766,41 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('displayName') is not None:
             self.display_name = m.get('displayName')
         return self
 
 
+class PatchEventRequestOnlineMeetingInfo(TeaModel):
+    def __init__(
+        self,
+        type: str = None,
+    ):
+        self.type = type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.type is not None:
+            result['type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        return self
+
+
 class PatchEventRequestRecurrencePattern(TeaModel):
     def __init__(
         self,
         day_of_month: int = None,
         days_of_week: str = None,
         index: str = None,
         interval: int = None,
@@ -8976,40 +9003,44 @@
         attendees: List[PatchEventRequestAttendees] = None,
         description: str = None,
         end: PatchEventRequestEnd = None,
         extra: Dict[str, str] = None,
         id: str = None,
         is_all_day: bool = None,
         location: PatchEventRequestLocation = None,
+        online_meeting_info: PatchEventRequestOnlineMeetingInfo = None,
         recurrence: PatchEventRequestRecurrence = None,
         reminders: List[PatchEventRequestReminders] = None,
         start: PatchEventRequestStart = None,
         summary: str = None,
     ):
         self.attendees = attendees
         self.description = description
         self.end = end
         self.extra = extra
         self.id = id
         self.is_all_day = is_all_day
         self.location = location
+        self.online_meeting_info = online_meeting_info
         self.recurrence = recurrence
         self.reminders = reminders
         self.start = start
         self.summary = summary
 
     def validate(self):
         if self.attendees:
             for k in self.attendees:
                 if k:
                     k.validate()
         if self.end:
             self.end.validate()
         if self.location:
             self.location.validate()
+        if self.online_meeting_info:
+            self.online_meeting_info.validate()
         if self.recurrence:
             self.recurrence.validate()
         if self.reminders:
             for k in self.reminders:
                 if k:
                     k.validate()
         if self.start:
@@ -9033,14 +9064,16 @@
             result['extra'] = self.extra
         if self.id is not None:
             result['id'] = self.id
         if self.is_all_day is not None:
             result['isAllDay'] = self.is_all_day
         if self.location is not None:
             result['location'] = self.location.to_map()
+        if self.online_meeting_info is not None:
+            result['onlineMeetingInfo'] = self.online_meeting_info.to_map()
         if self.recurrence is not None:
             result['recurrence'] = self.recurrence.to_map()
         result['reminders'] = []
         if self.reminders is not None:
             for k in self.reminders:
                 result['reminders'].append(k.to_map() if k else None)
         if self.start is not None:
@@ -9066,14 +9099,17 @@
         if m.get('id') is not None:
             self.id = m.get('id')
         if m.get('isAllDay') is not None:
             self.is_all_day = m.get('isAllDay')
         if m.get('location') is not None:
             temp_model = PatchEventRequestLocation()
             self.location = temp_model.from_map(m['location'])
+        if m.get('onlineMeetingInfo') is not None:
+            temp_model = PatchEventRequestOnlineMeetingInfo()
+            self.online_meeting_info = temp_model.from_map(m['onlineMeetingInfo'])
         if m.get('recurrence') is not None:
             temp_model = PatchEventRequestRecurrence()
             self.recurrence = temp_model.from_map(m['recurrence'])
         self.reminders = []
         if m.get('reminders') is not None:
             for k in m.get('reminders'):
                 temp_model = PatchEventRequestReminders()
@@ -9205,14 +9241,53 @@
         if m.get('displayName') is not None:
             self.display_name = m.get('displayName')
         if m.get('meetingRooms') is not None:
             self.meeting_rooms = m.get('meetingRooms')
         return self
 
 
+class PatchEventResponseBodyOnlineMeetingInfo(TeaModel):
+    def __init__(
+        self,
+        conference_id: str = None,
+        type: str = None,
+        url: str = None,
+    ):
+        self.conference_id = conference_id
+        self.type = type
+        self.url = url
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.conference_id is not None:
+            result['conferenceId'] = self.conference_id
+        if self.type is not None:
+            result['type'] = self.type
+        if self.url is not None:
+            result['url'] = self.url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('conferenceId') is not None:
+            self.conference_id = m.get('conferenceId')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        if m.get('url') is not None:
+            self.url = m.get('url')
+        return self
+
+
 class PatchEventResponseBodyOrganizer(TeaModel):
     def __init__(
         self,
         display_name: str = None,
         id: str = None,
         response_status: str = None,
         self_: bool = None,
@@ -9460,28 +9535,30 @@
         attendees: List[PatchEventResponseBodyAttendees] = None,
         create_time: str = None,
         description: str = None,
         end: PatchEventResponseBodyEnd = None,
         id: str = None,
         is_all_day: bool = None,
         location: PatchEventResponseBodyLocation = None,
+        online_meeting_info: PatchEventResponseBodyOnlineMeetingInfo = None,
         organizer: PatchEventResponseBodyOrganizer = None,
         recurrence: PatchEventResponseBodyRecurrence = None,
         reminders: List[PatchEventResponseBodyReminders] = None,
         start: PatchEventResponseBodyStart = None,
         summary: str = None,
         update_time: str = None,
     ):
         self.attendees = attendees
         self.create_time = create_time
         self.description = description
         self.end = end
         self.id = id
         self.is_all_day = is_all_day
         self.location = location
+        self.online_meeting_info = online_meeting_info
         self.organizer = organizer
         self.recurrence = recurrence
         self.reminders = reminders
         self.start = start
         self.summary = summary
         self.update_time = update_time
 
@@ -9490,14 +9567,16 @@
             for k in self.attendees:
                 if k:
                     k.validate()
         if self.end:
             self.end.validate()
         if self.location:
             self.location.validate()
+        if self.online_meeting_info:
+            self.online_meeting_info.validate()
         if self.organizer:
             self.organizer.validate()
         if self.recurrence:
             self.recurrence.validate()
         if self.reminders:
             for k in self.reminders:
                 if k:
@@ -9523,14 +9602,16 @@
             result['end'] = self.end.to_map()
         if self.id is not None:
             result['id'] = self.id
         if self.is_all_day is not None:
             result['isAllDay'] = self.is_all_day
         if self.location is not None:
             result['location'] = self.location.to_map()
+        if self.online_meeting_info is not None:
+            result['onlineMeetingInfo'] = self.online_meeting_info.to_map()
         if self.organizer is not None:
             result['organizer'] = self.organizer.to_map()
         if self.recurrence is not None:
             result['recurrence'] = self.recurrence.to_map()
         result['reminders'] = []
         if self.reminders is not None:
             for k in self.reminders:
@@ -9560,14 +9641,17 @@
         if m.get('id') is not None:
             self.id = m.get('id')
         if m.get('isAllDay') is not None:
             self.is_all_day = m.get('isAllDay')
         if m.get('location') is not None:
             temp_model = PatchEventResponseBodyLocation()
             self.location = temp_model.from_map(m['location'])
+        if m.get('onlineMeetingInfo') is not None:
+            temp_model = PatchEventResponseBodyOnlineMeetingInfo()
+            self.online_meeting_info = temp_model.from_map(m['onlineMeetingInfo'])
         if m.get('organizer') is not None:
             temp_model = PatchEventResponseBodyOrganizer()
             self.organizer = temp_model.from_map(m['organizer'])
         if m.get('recurrence') is not None:
             temp_model = PatchEventResponseBodyRecurrence()
             self.recurrence = temp_model.from_map(m['recurrence'])
         self.reminders = []
```

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.core import TeaCore
+from typing import Dict
 
 from alibabacloud_gateway_spi.client import Client as SPIClient
 from alibabacloud_tea_openapi.client import Client as OpenApiClient
 from alibabacloud_tea_openapi import models as open_api_models
 from alibabacloud_gateway_dingtalk.client import Client as GatewayClientClient
 from alibabacloud_tea_util.client import Client as UtilClient
 from alibabacloud_dingtalk.micro_app_1_0 import models as dingtalkmicro_app__1__0_models
@@ -21,14 +22,15 @@
     def __init__(
         self, 
         config: open_api_models.Config,
     ):
         super().__init__(config)
         self._client = GatewayClientClient()
         self._spi = self._client
+        self._signature_algorithm = 'v2'
         self._endpoint_rule = ''
         if UtilClient.empty(self._endpoint):
             self._endpoint = 'api.dingtalk.com'
 
     def add_app_roles_to_member_with_options(
         self,
         agent_id: str,
@@ -331,14 +333,72 @@
         role_id: str,
         request: dingtalkmicro_app__1__0_models.AddMemberToAppRoleRequest,
     ) -> dingtalkmicro_app__1__0_models.AddMemberToAppRoleResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkmicro_app__1__0_models.AddMemberToAppRoleHeaders()
         return await self.add_member_to_app_role_with_options_async(agent_id, role_id, request, headers, runtime)
 
+    def anhei_test_888with_options(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkmicro_app__1__0_models.AnheiTest888Response:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='AnheiTest888',
+            version='microApp_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/microApp/anheiTest888',
+            method='POST',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkmicro_app__1__0_models.AnheiTest888Response(),
+            self.execute(params, req, runtime)
+        )
+
+    async def anhei_test_888with_options_async(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkmicro_app__1__0_models.AnheiTest888Response:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='AnheiTest888',
+            version='microApp_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/microApp/anheiTest888',
+            method='POST',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkmicro_app__1__0_models.AnheiTest888Response(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def anhei_test_888(self) -> dingtalkmicro_app__1__0_models.AnheiTest888Response:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.anhei_test_888with_options(headers, runtime)
+
+    async def anhei_test_888_async(self) -> dingtalkmicro_app__1__0_models.AnheiTest888Response:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.anhei_test_888with_options_async(headers, runtime)
+
     def create_apaas_app_with_options(
         self,
         request: dingtalkmicro_app__1__0_models.CreateApaasAppRequest,
         headers: dingtalkmicro_app__1__0_models.CreateApaasAppHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkmicro_app__1__0_models.CreateApaasAppResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -541,14 +541,85 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AddMemberToAppRoleResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class AnheiTest888ResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        return self
+
+
+class AnheiTest888Response(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AnheiTest888ResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = AnheiTest888ResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateApaasAppHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.0.12
+Version: 2.0.13
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.12/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.13/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.12/setup.py` & `alibabacloud_dingtalk-2.0.13/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 12/05/2023
+Created on 16/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

