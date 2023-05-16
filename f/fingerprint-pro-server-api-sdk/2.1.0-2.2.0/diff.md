# Comparing `tmp/fingerprint-pro-server-api-sdk-2.1.0.tar.gz` & `tmp/fingerprint-pro-server-api-sdk-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fingerprint-pro-server-api-sdk-2.1.0.tar", last modified: Fri Feb  3 23:10:45 2023, max compression
+gzip compressed data, was "fingerprint-pro-server-api-sdk-2.2.0.tar", last modified: Tue May 16 13:49:15 2023, max compression
```

## Comparing `fingerprint-pro-server-api-sdk-2.1.0.tar` & `fingerprint-pro-server-api-sdk-2.2.0.tar`

### file list

```diff
@@ -1,52 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 23:10:45.533052 fingerprint-pro-server-api-sdk-2.1.0/
--rw-r--r--   0 root         (0) root         (0)     1069 2023-02-03 23:10:19.000000 fingerprint-pro-server-api-sdk-2.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    11139 2023-02-03 23:10:45.533052 fingerprint-pro-server-api-sdk-2.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7643 2023-02-03 23:10:42.000000 fingerprint-pro-server-api-sdk-2.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 23:10:45.521052 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/
--rw-r--r--   0 root         (0) root         (0)     2979 2023-02-03 23:10:42.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 23:10:45.521052 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/api/
--rw-r--r--   0 root         (0) root         (0)      165 2023-02-03 23:10:42.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11598 2023-02-03 23:10:42.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/api/fingerprint_api.py
--rw-r--r--   0 root         (0) root         (0)    25588 2023-02-03 23:10:42.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/api_client.py
--rw-r--r--   0 root         (0) root         (0)     8894 2023-02-03 23:10:42.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/configuration.py
--rw-r--r--   0 root         (0) root         (0)      362 2023-02-03 23:10:19.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/extend_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 23:10:45.533052 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/
--rw-r--r--   0 root         (0) root         (0)     2717 2023-02-03 23:10:42.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4280 2023-02-03 23:10:41.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/botd_detection_result.py
--rw-r--r--   0 root         (0) root         (0)     4628 2023-02-03 23:10:41.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/botd_error.py
--rw-r--r--   0 root         (0) root         (0)     5944 2023-02-03 23:10:41.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/botd_result.py
--rw-r--r--   0 root         (0) root         (0)     9277 2023-02-03 23:10:41.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/browser_details.py
--rw-r--r--   0 root         (0) root         (0)     3642 2023-02-03 23:10:41.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/confidence.py
--rw-r--r--   0 root         (0) root         (0)     3428 2023-02-03 23:10:41.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/error_event403_response.py
--rw-r--r--   0 root         (0) root         (0)     5134 2023-02-03 23:10:41.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/error_event403_response_error.py
--rw-r--r--   0 root         (0) root         (0)     3428 2023-02-03 23:10:41.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/error_event404_response.py
--rw-r--r--   0 root         (0) root         (0)     4705 2023-02-03 23:10:41.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/error_event404_response_error.py
--rw-r--r--   0 root         (0) root         (0)     3448 2023-02-03 23:10:41.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/error_visits403.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-02-03 23:10:41.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/event_response.py
--rw-r--r--   0 root         (0) root         (0)     4776 2023-02-03 23:10:41.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/identification_error.py
--rw-r--r--   0 root         (0) root         (0)     9377 2023-02-03 23:10:41.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/ip_location.py
--rw-r--r--   0 root         (0) root         (0)     3276 2023-02-03 23:10:41.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/ip_location_city.py
--rw-r--r--   0 root         (0) root         (0)     3949 2023-02-03 23:10:41.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/location.py
--rw-r--r--   0 root         (0) root         (0)     3781 2023-02-03 23:10:19.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/many_requests_response.py
--rw-r--r--   0 root         (0) root         (0)     4219 2023-02-03 23:10:42.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/products_response.py
--rw-r--r--   0 root         (0) root         (0)     3998 2023-02-03 23:10:42.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/products_response_botd.py
--rw-r--r--   0 root         (0) root         (0)     4230 2023-02-03 23:10:42.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/products_response_identification.py
--rw-r--r--   0 root         (0) root         (0)    16816 2023-02-03 23:10:42.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/products_response_identification_data.py
--rw-r--r--   0 root         (0) root         (0)     6501 2023-02-03 23:10:42.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/response.py
--rw-r--r--   0 root         (0) root         (0)    14805 2023-02-03 23:10:42.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/response_visits.py
--rw-r--r--   0 root         (0) root         (0)     3929 2023-02-03 23:10:42.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/seen_at.py
--rw-r--r--   0 root         (0) root         (0)     3901 2023-02-03 23:10:42.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/subdivision.py
--rw-r--r--   0 root         (0) root         (0)    14174 2023-02-03 23:10:42.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/visit.py
--rw-r--r--   0 root         (0) root         (0)    16182 2023-02-03 23:10:42.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/webhook_visit.py
--rw-r--r--   0 root         (0) root         (0)    13535 2023-02-03 23:10:42.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 23:10:45.521052 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11139 2023-02-03 23:10:45.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2264 2023-02-03 23:10:45.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-03 23:10:45.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-02-03 23:10:45.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-02-03 23:10:45.000000 fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      473 2023-02-03 23:10:45.533052 fingerprint-pro-server-api-sdk-2.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3054 2023-02-03 23:10:42.000000 fingerprint-pro-server-api-sdk-2.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 23:10:45.533052 fingerprint-pro-server-api-sdk-2.1.0/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-03 23:10:19.000000 fingerprint-pro-server-api-sdk-2.1.0/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16338 2023-02-03 23:10:43.000000 fingerprint-pro-server-api-sdk-2.1.0/test/test_fingerprint_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:49:15.753661 fingerprint-pro-server-api-sdk-2.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-05-16 13:48:47.000000 fingerprint-pro-server-api-sdk-2.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    14727 2023-05-16 13:49:15.753661 fingerprint-pro-server-api-sdk-2.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9145 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:49:15.737661 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/
+-rw-r--r--   0 root         (0) root         (0)     5486 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:49:15.741661 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/api/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11598 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/api/fingerprint_api.py
+-rw-r--r--   0 root         (0) root         (0)    25588 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/api_client.py
+-rw-r--r--   0 root         (0) root         (0)     8894 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/configuration.py
+-rw-r--r--   0 root         (0) root         (0)      362 2023-05-16 13:48:47.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/extend_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:49:15.753661 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/
+-rw-r--r--   0 root         (0) root         (0)     5224 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4885 2023-05-16 13:49:10.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/botd_detection_result.py
+-rw-r--r--   0 root         (0) root         (0)     7320 2023-05-16 13:49:10.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/botd_result.py
+-rw-r--r--   0 root         (0) root         (0)     9277 2023-05-16 13:49:10.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/browser_details.py
+-rw-r--r--   0 root         (0) root         (0)     3642 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/confidence.py
+-rw-r--r--   0 root         (0) root         (0)     3428 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/error_event403_response.py
+-rw-r--r--   0 root         (0) root         (0)     5134 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/error_event403_response_error.py
+-rw-r--r--   0 root         (0) root         (0)     3428 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/error_event404_response.py
+-rw-r--r--   0 root         (0) root         (0)     4705 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/error_event404_response_error.py
+-rw-r--r--   0 root         (0) root         (0)     3448 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/error_visits403.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/event_response.py
+-rw-r--r--   0 root         (0) root         (0)     4776 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/identification_error.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_block_list_result.py
+-rw-r--r--   0 root         (0) root         (0)     4615 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_block_list_result_details.py
+-rw-r--r--   0 root         (0) root         (0)     3821 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_info_result.py
+-rw-r--r--   0 root         (0) root         (0)     4082 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_info_result_v4.py
+-rw-r--r--   0 root         (0) root         (0)     4082 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_info_result_v6.py
+-rw-r--r--   0 root         (0) root         (0)     9377 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_location.py
+-rw-r--r--   0 root         (0) root         (0)     3276 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_location_city.py
+-rw-r--r--   0 root         (0) root         (0)     3949 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/location.py
+-rw-r--r--   0 root         (0) root         (0)     3781 2023-05-16 13:48:47.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/many_requests_response.py
+-rw-r--r--   0 root         (0) root         (0)     4667 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/product_error.py
+-rw-r--r--   0 root         (0) root         (0)    10616 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/products_response.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/products_response_botd.py
+-rw-r--r--   0 root         (0) root         (0)     4230 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/products_response_identification.py
+-rw-r--r--   0 root         (0) root         (0)    16816 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/products_response_identification_data.py
+-rw-r--r--   0 root         (0) root         (0)     6501 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/response.py
+-rw-r--r--   0 root         (0) root         (0)    14805 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/response_visits.py
+-rw-r--r--   0 root         (0) root         (0)     3929 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/seen_at.py
+-rw-r--r--   0 root         (0) root         (0)     4081 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_emulator.py
+-rw-r--r--   0 root         (0) root         (0)     4051 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_emulator_data.py
+-rw-r--r--   0 root         (0) root         (0)     4097 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_incognito.py
+-rw-r--r--   0 root         (0) root         (0)     3636 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_incognito_data.py
+-rw-r--r--   0 root         (0) root         (0)     4093 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_ip_blocklist.py
+-rw-r--r--   0 root         (0) root         (0)     4013 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_ip_info.py
+-rw-r--r--   0 root         (0) root         (0)     4033 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     3622 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_proxy_data.py
+-rw-r--r--   0 root         (0) root         (0)     4081 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_root_apps.py
+-rw-r--r--   0 root         (0) root         (0)     4029 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_root_apps_data.py
+-rw-r--r--   0 root         (0) root         (0)     4061 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_tampering.py
+-rw-r--r--   0 root         (0) root         (0)     4001 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_tor.py
+-rw-r--r--   0 root         (0) root         (0)     3584 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_tor_data.py
+-rw-r--r--   0 root         (0) root         (0)     3965 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_vpn.py
+-rw-r--r--   0 root         (0) root         (0)     3901 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/subdivision.py
+-rw-r--r--   0 root         (0) root         (0)     4748 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/tampering_result.py
+-rw-r--r--   0 root         (0) root         (0)    14174 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/visit.py
+-rw-r--r--   0 root         (0) root         (0)     4128 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/vpn_result.py
+-rw-r--r--   0 root         (0) root         (0)     4691 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/vpn_result_methods.py
+-rw-r--r--   0 root         (0) root         (0)     4078 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/webhook_signal_response_emulator.py
+-rw-r--r--   0 root         (0) root         (0)     3649 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/webhook_signal_response_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     4056 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/webhook_signal_response_root_apps.py
+-rw-r--r--   0 root         (0) root         (0)     3611 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/webhook_signal_response_tor.py
+-rw-r--r--   0 root         (0) root         (0)    22987 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/webhook_visit.py
+-rw-r--r--   0 root         (0) root         (0)    13535 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:49:15.741661 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14727 2023-05-16 13:49:15.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3968 2023-05-16 13:49:15.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 13:49:15.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-05-16 13:49:15.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-16 13:49:15.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      473 2023-05-16 13:49:15.753661 fingerprint-pro-server-api-sdk-2.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3054 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:49:15.753661 fingerprint-pro-server-api-sdk-2.2.0/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 13:48:47.000000 fingerprint-pro-server-api-sdk-2.2.0/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16976 2023-05-16 13:49:13.000000 fingerprint-pro-server-api-sdk-2.2.0/test/test_fingerprint_api.py
```

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/LICENSE` & `fingerprint-pro-server-api-sdk-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/PKG-INFO` & `fingerprint-pro-server-api-sdk-2.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: fingerprint-pro-server-api-sdk
-Version: 2.1.0
+Version: 2.2.0
 Summary: Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.
 Home-page: https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk
 Author: Fingerprint
 Author-email: support@fingerprint.com
 License: MIT
 Keywords: Swagger,Fingerprint Pro Server API,browser,detection,fingerprint,identification,fingerprinting,browser-fingerprinting,browser-fingerprint,fraud-detection,fraud,audio-fingerprinting,fingerprintjs,fingerprintjs-pro,visitor-identifier
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
@@ -58,15 +57,15 @@
 
 # Fingerprint Pro Server Python SDK
 Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 3
-- Package version: 2.1.0
+- Package version: 2.2.0
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -174,38 +173,64 @@
 ------------ | ------------- | ------------- | -------------
 *FingerprintApi* | [**get_event**](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/FingerprintApi.md#get_event) | **GET** /events/{request_id} | Get event by requestId
 *FingerprintApi* | [**get_visits**](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/FingerprintApi.md#get_visits) | **GET** /visitors/{visitor_id} | Get visits by visitorId
 
 ## Documentation For Models
 
  - [BotdDetectionResult](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/BotdDetectionResult.md)
- - [BotdError](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/BotdError.md)
  - [BotdResult](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/BotdResult.md)
  - [BrowserDetails](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/BrowserDetails.md)
  - [Confidence](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/Confidence.md)
  - [ErrorEvent403Response](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ErrorEvent403Response.md)
  - [ErrorEvent403ResponseError](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ErrorEvent403ResponseError.md)
  - [ErrorEvent404Response](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ErrorEvent404Response.md)
  - [ErrorEvent404ResponseError](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ErrorEvent404ResponseError.md)
  - [ErrorVisits403](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ErrorVisits403.md)
  - [EventResponse](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/EventResponse.md)
  - [IPLocation](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/IPLocation.md)
  - [IPLocationCity](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/IPLocationCity.md)
  - [IdentificationError](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/IdentificationError.md)
+ - [IpBlockListResult](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/IpBlockListResult.md)
+ - [IpBlockListResultDetails](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/IpBlockListResultDetails.md)
+ - [IpInfoResult](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/IpInfoResult.md)
+ - [IpInfoResultV4](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/IpInfoResultV4.md)
+ - [IpInfoResultV6](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/IpInfoResultV6.md)
  - [Location](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/Location.md)
  - [ManyRequestsResponse](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ManyRequestsResponse.md)
+ - [ProductError](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ProductError.md)
  - [ProductsResponse](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ProductsResponse.md)
  - [ProductsResponseBotd](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ProductsResponseBotd.md)
  - [ProductsResponseIdentification](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ProductsResponseIdentification.md)
  - [ProductsResponseIdentificationData](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ProductsResponseIdentificationData.md)
  - [Response](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/Response.md)
  - [ResponseVisits](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ResponseVisits.md)
  - [SeenAt](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SeenAt.md)
+ - [SignalResponseEmulator](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseEmulator.md)
+ - [SignalResponseEmulatorData](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseEmulatorData.md)
+ - [SignalResponseIncognito](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseIncognito.md)
+ - [SignalResponseIncognitoData](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseIncognitoData.md)
+ - [SignalResponseIpBlocklist](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseIpBlocklist.md)
+ - [SignalResponseIpInfo](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseIpInfo.md)
+ - [SignalResponseProxy](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseProxy.md)
+ - [SignalResponseProxyData](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseProxyData.md)
+ - [SignalResponseRootApps](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseRootApps.md)
+ - [SignalResponseRootAppsData](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseRootAppsData.md)
+ - [SignalResponseTampering](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseTampering.md)
+ - [SignalResponseTor](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseTor.md)
+ - [SignalResponseTorData](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseTorData.md)
+ - [SignalResponseVpn](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseVpn.md)
  - [Subdivision](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/Subdivision.md)
+ - [TamperingResult](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/TamperingResult.md)
  - [Visit](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/Visit.md)
+ - [VpnResult](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/VpnResult.md)
+ - [VpnResultMethods](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/VpnResultMethods.md)
+ - [WebhookSignalResponseEmulator](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/WebhookSignalResponseEmulator.md)
+ - [WebhookSignalResponseProxy](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/WebhookSignalResponseProxy.md)
+ - [WebhookSignalResponseRootApps](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/WebhookSignalResponseRootApps.md)
+ - [WebhookSignalResponseTor](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/WebhookSignalResponseTor.md)
  - [WebhookVisit](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/WebhookVisit.md)
 
 ## Documentation For Authorization
 
 
 ## ApiKeyHeader
 
@@ -219,9 +244,7 @@
 - **API key parameter name**: api_key
 - **Location**: URL query string
 
 
 ## Author
 
 support@fingerprint.com
-
-
```

#### html2text {}

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1 Name: fingerprint-pro-server-api-sdk Version: 2.1.0
+Metadata-Version: 2.1 Name: fingerprint-pro-server-api-sdk Version: 2.2.0
 Summary: Fingerprint Pro Server API allows you to get information about
 visitors and about individual events in a server environment. This API can be
 used for data exports, decision-making, and data analysis scenarios. Home-page:
 https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk Author:
 Fingerprint Author-email: support@fingerprint.com License: MIT Keywords:
 Swagger,Fingerprint Pro Server
 API,browser,detection,fingerprint,identification,fingerprinting,browser-
 fingerprinting,browser-fingerprint,fraud-detection,fraud,audio-
-fingerprinting,fingerprintjs,fingerprintjs-pro,visitor-identifier Platform:
-UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
-Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
-License Classifier: Programming Language :: Python :: 2 Classifier: Programming
-Language :: Python Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.4 Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: Implementation :: PyPy Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Topic :: Security
-Description-Content-Type: text/markdown License-File: LICENSE
+fingerprinting,fingerprintjs,fingerprintjs-pro,visitor-identifier Classifier:
+Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
+Developers Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 2 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2.7 Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python ::
+Implementation :: PyPy Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Classifier: Topic :: Security Description-Content-Type: text/
+markdown License-File: LICENSE
                               [Fingerprint_logo]
  [PyPI] [coverage] [CI_badge] [CI_badge] [CI_badge] [https://img.shields.io/:
                license-mit-blue.svg?style=flat] [Discord_server]
 # Fingerprint Pro Server Python SDK Fingerprint Pro Server API allows you to
 get information about visitors and about individual events in a server
 environment. This API can be used for data exports, decision-making, and data
 analysis scenarios. This Python package is automatically generated by the
 [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project: -
-API version: 3 - Package version: 2.1.0 - Build package:
+API version: 3 - Package version: 2.2.0 - Build package:
 io.swagger.codegen.v3.generators.python.PythonClientCodegen ## Requirements.
 Python 2.7 and 3.4+ ## Installation & Usage ### pip install You can install the
 package directly from the Github ```sh pip install git+https://github.com/
 fingerprintjs/fingerprint-pro-server-api-python-sdk.git ``` Or from the PyPI
 ```sh pip install fingerprint_pro_server_api_sdk ``` Then import the package:
 ```python import fingerprint_pro_server_api_sdk ``` ### Setuptools Install via
 [Setuptools](http://pypi.python.org/pypi/setuptools). ```sh python setup.py
@@ -78,55 +78,103 @@
 (https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/
 main/docs/FingerprintApi.md#get_event) | **GET** /events/{request_id} | Get
 event by requestId *FingerprintApi* | [**get_visits**](https://github.com/
 fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
 FingerprintApi.md#get_visits) | **GET** /visitors/{visitor_id} | Get visits by
 visitorId ## Documentation For Models - [BotdDetectionResult](https://
 github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
-BotdDetectionResult.md) - [BotdError](https://github.com/fingerprintjs/
-fingerprint-pro-server-api-python-sdk/blob/main/docs/BotdError.md) -
-[BotdResult](https://github.com/fingerprintjs/fingerprint-pro-server-api-
-python-sdk/blob/main/docs/BotdResult.md) - [BrowserDetails](https://github.com/
-fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
-BrowserDetails.md) - [Confidence](https://github.com/fingerprintjs/fingerprint-
-pro-server-api-python-sdk/blob/main/docs/Confidence.md) -
-[ErrorEvent403Response](https://github.com/fingerprintjs/fingerprint-pro-
-server-api-python-sdk/blob/main/docs/ErrorEvent403Response.md) -
-[ErrorEvent403ResponseError](https://github.com/fingerprintjs/fingerprint-pro-
-server-api-python-sdk/blob/main/docs/ErrorEvent403ResponseError.md) -
+BotdDetectionResult.md) - [BotdResult](https://github.com/fingerprintjs/
+fingerprint-pro-server-api-python-sdk/blob/main/docs/BotdResult.md) -
+[BrowserDetails](https://github.com/fingerprintjs/fingerprint-pro-server-api-
+python-sdk/blob/main/docs/BrowserDetails.md) - [Confidence](https://github.com/
+fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+Confidence.md) - [ErrorEvent403Response](https://github.com/fingerprintjs/
+fingerprint-pro-server-api-python-sdk/blob/main/docs/ErrorEvent403Response.md)
+- [ErrorEvent403ResponseError](https://github.com/fingerprintjs/fingerprint-
+pro-server-api-python-sdk/blob/main/docs/ErrorEvent403ResponseError.md) -
 [ErrorEvent404Response](https://github.com/fingerprintjs/fingerprint-pro-
 server-api-python-sdk/blob/main/docs/ErrorEvent404Response.md) -
 [ErrorEvent404ResponseError](https://github.com/fingerprintjs/fingerprint-pro-
 server-api-python-sdk/blob/main/docs/ErrorEvent404ResponseError.md) -
 [ErrorVisits403](https://github.com/fingerprintjs/fingerprint-pro-server-api-
 python-sdk/blob/main/docs/ErrorVisits403.md) - [EventResponse](https://
 github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
 EventResponse.md) - [IPLocation](https://github.com/fingerprintjs/fingerprint-
 pro-server-api-python-sdk/blob/main/docs/IPLocation.md) - [IPLocationCity]
 (https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/
 main/docs/IPLocationCity.md) - [IdentificationError](https://github.com/
 fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
-IdentificationError.md) - [Location](https://github.com/fingerprintjs/
-fingerprint-pro-server-api-python-sdk/blob/main/docs/Location.md) -
-[ManyRequestsResponse](https://github.com/fingerprintjs/fingerprint-pro-server-
-api-python-sdk/blob/main/docs/ManyRequestsResponse.md) - [ProductsResponse]
-(https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/
-main/docs/ProductsResponse.md) - [ProductsResponseBotd](https://github.com/
+IdentificationError.md) - [IpBlockListResult](https://github.com/fingerprintjs/
+fingerprint-pro-server-api-python-sdk/blob/main/docs/IpBlockListResult.md) -
+[IpBlockListResultDetails](https://github.com/fingerprintjs/fingerprint-pro-
+server-api-python-sdk/blob/main/docs/IpBlockListResultDetails.md) -
+[IpInfoResult](https://github.com/fingerprintjs/fingerprint-pro-server-api-
+python-sdk/blob/main/docs/IpInfoResult.md) - [IpInfoResultV4](https://
+github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+IpInfoResultV4.md) - [IpInfoResultV6](https://github.com/fingerprintjs/
+fingerprint-pro-server-api-python-sdk/blob/main/docs/IpInfoResultV6.md) -
+[Location](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-
+sdk/blob/main/docs/Location.md) - [ManyRequestsResponse](https://github.com/
 fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+ManyRequestsResponse.md) - [ProductError](https://github.com/fingerprintjs/
+fingerprint-pro-server-api-python-sdk/blob/main/docs/ProductError.md) -
+[ProductsResponse](https://github.com/fingerprintjs/fingerprint-pro-server-api-
+python-sdk/blob/main/docs/ProductsResponse.md) - [ProductsResponseBotd](https:/
+/github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
 ProductsResponseBotd.md) - [ProductsResponseIdentification](https://github.com/
 fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
 ProductsResponseIdentification.md) - [ProductsResponseIdentificationData]
 (https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/
 main/docs/ProductsResponseIdentificationData.md) - [Response](https://
 github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
 Response.md) - [ResponseVisits](https://github.com/fingerprintjs/fingerprint-
 pro-server-api-python-sdk/blob/main/docs/ResponseVisits.md) - [SeenAt](https://
 github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
-SeenAt.md) - [Subdivision](https://github.com/fingerprintjs/fingerprint-pro-
-server-api-python-sdk/blob/main/docs/Subdivision.md) - [Visit](https://
+SeenAt.md) - [SignalResponseEmulator](https://github.com/fingerprintjs/
+fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseEmulator.md)
+- [SignalResponseEmulatorData](https://github.com/fingerprintjs/fingerprint-
+pro-server-api-python-sdk/blob/main/docs/SignalResponseEmulatorData.md) -
+[SignalResponseIncognito](https://github.com/fingerprintjs/fingerprint-pro-
+server-api-python-sdk/blob/main/docs/SignalResponseIncognito.md) -
+[SignalResponseIncognitoData](https://github.com/fingerprintjs/fingerprint-pro-
+server-api-python-sdk/blob/main/docs/SignalResponseIncognitoData.md) -
+[SignalResponseIpBlocklist](https://github.com/fingerprintjs/fingerprint-pro-
+server-api-python-sdk/blob/main/docs/SignalResponseIpBlocklist.md) -
+[SignalResponseIpInfo](https://github.com/fingerprintjs/fingerprint-pro-server-
+api-python-sdk/blob/main/docs/SignalResponseIpInfo.md) - [SignalResponseProxy]
+(https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/
+main/docs/SignalResponseProxy.md) - [SignalResponseProxyData](https://
+github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+SignalResponseProxyData.md) - [SignalResponseRootApps](https://github.com/
+fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+SignalResponseRootApps.md) - [SignalResponseRootAppsData](https://github.com/
+fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+SignalResponseRootAppsData.md) - [SignalResponseTampering](https://github.com/
+fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+SignalResponseTampering.md) - [SignalResponseTor](https://github.com/
+fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+SignalResponseTor.md) - [SignalResponseTorData](https://github.com/
+fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+SignalResponseTorData.md) - [SignalResponseVpn](https://github.com/
+fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+SignalResponseVpn.md) - [Subdivision](https://github.com/fingerprintjs/
+fingerprint-pro-server-api-python-sdk/blob/main/docs/Subdivision.md) -
+[TamperingResult](https://github.com/fingerprintjs/fingerprint-pro-server-api-
+python-sdk/blob/main/docs/TamperingResult.md) - [Visit](https://github.com/
+fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/Visit.md) -
+[VpnResult](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-
+sdk/blob/main/docs/VpnResult.md) - [VpnResultMethods](https://github.com/
+fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+VpnResultMethods.md) - [WebhookSignalResponseEmulator](https://github.com/
+fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+WebhookSignalResponseEmulator.md) - [WebhookSignalResponseProxy](https://
+github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+WebhookSignalResponseProxy.md) - [WebhookSignalResponseRootApps](https://
+github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+WebhookSignalResponseRootApps.md) - [WebhookSignalResponseTor](https://
 github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
-Visit.md) - [WebhookVisit](https://github.com/fingerprintjs/fingerprint-pro-
-server-api-python-sdk/blob/main/docs/WebhookVisit.md) ## Documentation For
-Authorization ## ApiKeyHeader - **Type**: API key - **API key parameter name**:
-Auth-API-Key - **Location**: HTTP header ## ApiKeyQuery - **Type**: API key -
-**API key parameter name**: api_key - **Location**: URL query string ## Author
-support@fingerprint.com
+WebhookSignalResponseTor.md) - [WebhookVisit](https://github.com/fingerprintjs/
+fingerprint-pro-server-api-python-sdk/blob/main/docs/WebhookVisit.md) ##
+Documentation For Authorization ## ApiKeyHeader - **Type**: API key - **API key
+parameter name**: Auth-API-Key - **Location**: HTTP header ## ApiKeyQuery -
+**Type**: API key - **API key parameter name**: api_key - **Location**: URL
+query string ## Author support@fingerprint.com
```

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/__init__.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,68 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     Fingerprint Pro Server API
 
     Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-# import apis into sdk package
-from fingerprint_pro_server_api_sdk.api.fingerprint_api import FingerprintApi
-# import ApiClient
-from fingerprint_pro_server_api_sdk.api_client import ApiClient
-from fingerprint_pro_server_api_sdk.configuration import Configuration
-# import models into sdk package
+# import models into model package
 from fingerprint_pro_server_api_sdk.models.botd_detection_result import BotdDetectionResult
-from fingerprint_pro_server_api_sdk.models.botd_error import BotdError
 from fingerprint_pro_server_api_sdk.models.botd_result import BotdResult
 from fingerprint_pro_server_api_sdk.models.browser_details import BrowserDetails
 from fingerprint_pro_server_api_sdk.models.confidence import Confidence
 from fingerprint_pro_server_api_sdk.models.error_event403_response import ErrorEvent403Response
 from fingerprint_pro_server_api_sdk.models.error_event403_response_error import ErrorEvent403ResponseError
 from fingerprint_pro_server_api_sdk.models.error_event404_response import ErrorEvent404Response
 from fingerprint_pro_server_api_sdk.models.error_event404_response_error import ErrorEvent404ResponseError
 from fingerprint_pro_server_api_sdk.models.error_visits403 import ErrorVisits403
 from fingerprint_pro_server_api_sdk.models.event_response import EventResponse
 from fingerprint_pro_server_api_sdk.models.ip_location import IPLocation
 from fingerprint_pro_server_api_sdk.models.ip_location_city import IPLocationCity
 from fingerprint_pro_server_api_sdk.models.identification_error import IdentificationError
+from fingerprint_pro_server_api_sdk.models.ip_block_list_result import IpBlockListResult
+from fingerprint_pro_server_api_sdk.models.ip_block_list_result_details import IpBlockListResultDetails
+from fingerprint_pro_server_api_sdk.models.ip_info_result import IpInfoResult
+from fingerprint_pro_server_api_sdk.models.ip_info_result_v4 import IpInfoResultV4
+from fingerprint_pro_server_api_sdk.models.ip_info_result_v6 import IpInfoResultV6
 from fingerprint_pro_server_api_sdk.models.location import Location
 from fingerprint_pro_server_api_sdk.models.many_requests_response import ManyRequestsResponse
+from fingerprint_pro_server_api_sdk.models.product_error import ProductError
 from fingerprint_pro_server_api_sdk.models.products_response import ProductsResponse
 from fingerprint_pro_server_api_sdk.models.products_response_botd import ProductsResponseBotd
 from fingerprint_pro_server_api_sdk.models.products_response_identification import ProductsResponseIdentification
 from fingerprint_pro_server_api_sdk.models.products_response_identification_data import ProductsResponseIdentificationData
 from fingerprint_pro_server_api_sdk.models.response import Response
 from fingerprint_pro_server_api_sdk.models.response_visits import ResponseVisits
 from fingerprint_pro_server_api_sdk.models.seen_at import SeenAt
+from fingerprint_pro_server_api_sdk.models.signal_response_emulator import SignalResponseEmulator
+from fingerprint_pro_server_api_sdk.models.signal_response_emulator_data import SignalResponseEmulatorData
+from fingerprint_pro_server_api_sdk.models.signal_response_incognito import SignalResponseIncognito
+from fingerprint_pro_server_api_sdk.models.signal_response_incognito_data import SignalResponseIncognitoData
+from fingerprint_pro_server_api_sdk.models.signal_response_ip_blocklist import SignalResponseIpBlocklist
+from fingerprint_pro_server_api_sdk.models.signal_response_ip_info import SignalResponseIpInfo
+from fingerprint_pro_server_api_sdk.models.signal_response_proxy import SignalResponseProxy
+from fingerprint_pro_server_api_sdk.models.signal_response_proxy_data import SignalResponseProxyData
+from fingerprint_pro_server_api_sdk.models.signal_response_root_apps import SignalResponseRootApps
+from fingerprint_pro_server_api_sdk.models.signal_response_root_apps_data import SignalResponseRootAppsData
+from fingerprint_pro_server_api_sdk.models.signal_response_tampering import SignalResponseTampering
+from fingerprint_pro_server_api_sdk.models.signal_response_tor import SignalResponseTor
+from fingerprint_pro_server_api_sdk.models.signal_response_tor_data import SignalResponseTorData
+from fingerprint_pro_server_api_sdk.models.signal_response_vpn import SignalResponseVpn
 from fingerprint_pro_server_api_sdk.models.subdivision import Subdivision
+from fingerprint_pro_server_api_sdk.models.tampering_result import TamperingResult
 from fingerprint_pro_server_api_sdk.models.visit import Visit
+from fingerprint_pro_server_api_sdk.models.vpn_result import VpnResult
+from fingerprint_pro_server_api_sdk.models.vpn_result_methods import VpnResultMethods
+from fingerprint_pro_server_api_sdk.models.webhook_signal_response_emulator import WebhookSignalResponseEmulator
+from fingerprint_pro_server_api_sdk.models.webhook_signal_response_proxy import WebhookSignalResponseProxy
+from fingerprint_pro_server_api_sdk.models.webhook_signal_response_root_apps import WebhookSignalResponseRootApps
+from fingerprint_pro_server_api_sdk.models.webhook_signal_response_tor import WebhookSignalResponseTor
 from fingerprint_pro_server_api_sdk.models.webhook_visit import WebhookVisit
```

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/api/fingerprint_api.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/api/fingerprint_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         collection_formats = {}
 
         path_params = {}
         if 'request_id' in params:
             path_params['request_id'] = params['request_id']  # noqa: E501
 
         query_params = []
-        query_params.append(('ii', 'fingerprint-pro-server-python-sdk/2.1.0'))
+        query_params.append(('ii', 'fingerprint-pro-server-python-sdk/2.2.0'))
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -208,15 +208,15 @@
         collection_formats = {}
 
         path_params = {}
         if 'visitor_id' in params:
             path_params['visitor_id'] = params['visitor_id']  # noqa: E501
 
         query_params = []
-        query_params.append(('ii', 'fingerprint-pro-server-python-sdk/2.1.0'))
+        query_params.append(('ii', 'fingerprint-pro-server-python-sdk/2.2.0'))
         if 'request_id' in params:
             query_params.append(('request_id', params['request_id']))  # noqa: E501
         if 'linked_id' in params:
             query_params.append(('linked_id', params['linked_id']))  # noqa: E501
         if 'limit' in params:
             query_params.append(('limit', params['limit']))  # noqa: E501
         if 'before' in params:
```

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/api_client.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/2.1.0/python'
+        self.user_agent = 'Swagger-Codegen/2.2.0/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/configuration.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,9 +259,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3\n"\
-               "SDK Package Version: 2.1.0".\
+               "SDK Package Version: 2.2.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/botd_detection_result.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/botd_detection_result.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,26 +24,31 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'result': 'str'
+        'result': 'str',
+        'type': 'str'
     }
 
     attribute_map = {
-        'result': 'result'
+        'result': 'result',
+        'type': 'type'
     }
 
-    def __init__(self, result=None):  # noqa: E501
+    def __init__(self, result=None, type=None):  # noqa: E501
         """BotdDetectionResult - a model defined in Swagger"""  # noqa: E501
         self._result = None
+        self._type = None
         self.discriminator = None
         self.result = result
+        if type is not None:
+            self.type = type
 
     @property
     def result(self):
         """Gets the result of this BotdDetectionResult.  # noqa: E501
 
         Bot detection result:  * `notDetected` - the visitor is not a bot  * `good` - good bot detected, such as Google bot, Baidu Spider, AlexaBot and so on  * `bad` - bad bot detected, such as Selenium, Puppeteer, Playwright, headless browsers, and so on   # noqa: E501
 
@@ -68,14 +73,35 @@
             raise ValueError(
                 "Invalid value for `result` ({0}), must be one of {1}"  # noqa: E501
                 .format(result, allowed_values)
             )
 
         self._result = result
 
+    @property
+    def type(self):
+        """Gets the type of this BotdDetectionResult.  # noqa: E501
+
+
+        :return: The type of this BotdDetectionResult.  # noqa: E501
+        :rtype: str
+        """
+        return self._type
+
+    @type.setter
+    def type(self, type):
+        """Sets the type of this BotdDetectionResult.
+
+
+        :param type: The type of this BotdDetectionResult.  # noqa: E501
+        :type: str
+        """
+
+        self._type = type
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/botd_error.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/product_error.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class BotdError(object):
+class ProductError(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -34,39 +34,39 @@
 
     attribute_map = {
         'code': 'code',
         'message': 'message'
     }
 
     def __init__(self, code=None, message=None):  # noqa: E501
-        """BotdError - a model defined in Swagger"""  # noqa: E501
+        """ProductError - a model defined in Swagger"""  # noqa: E501
         self._code = None
         self._message = None
         self.discriminator = None
         self.code = code
         self.message = message
 
     @property
     def code(self):
-        """Gets the code of this BotdError.  # noqa: E501
+        """Gets the code of this ProductError.  # noqa: E501
 
         Error code:  * `TooManyRequests` - the limit on secret API key requests per second has been exceeded  * `Failed` - internal server error   # noqa: E501
 
-        :return: The code of this BotdError.  # noqa: E501
+        :return: The code of this ProductError.  # noqa: E501
         :rtype: str
         """
         return self._code
 
     @code.setter
     def code(self, code):
-        """Sets the code of this BotdError.
+        """Sets the code of this ProductError.
 
         Error code:  * `TooManyRequests` - the limit on secret API key requests per second has been exceeded  * `Failed` - internal server error   # noqa: E501
 
-        :param code: The code of this BotdError.  # noqa: E501
+        :param code: The code of this ProductError.  # noqa: E501
         :type: str
         """
         if code is None:
             raise ValueError("Invalid value for `code`, must not be `None`")  # noqa: E501
         allowed_values = ["TooManyRequests", "Failed"]  # noqa: E501
         if (code not in allowed_values):
             raise ValueError(
@@ -74,28 +74,28 @@
                 .format(code, allowed_values)
             )
 
         self._code = code
 
     @property
     def message(self):
-        """Gets the message of this BotdError.  # noqa: E501
+        """Gets the message of this ProductError.  # noqa: E501
 
 
-        :return: The message of this BotdError.  # noqa: E501
+        :return: The message of this ProductError.  # noqa: E501
         :rtype: str
         """
         return self._message
 
     @message.setter
     def message(self, message):
-        """Sets the message of this BotdError.
+        """Sets the message of this ProductError.
 
 
-        :param message: The message of this BotdError.  # noqa: E501
+        :param message: The message of this ProductError.  # noqa: E501
         :type: str
         """
         if message is None:
             raise ValueError("Invalid value for `message`, must not be `None`")  # noqa: E501
 
         self._message = message
 
@@ -116,15 +116,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(BotdError, dict):
+        if issubclass(ProductError, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -132,18 +132,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, BotdError):
+        if not isinstance(other, ProductError):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, BotdError):
+        if not isinstance(other, ProductError):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/botd_result.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/botd_result.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,34 +27,44 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'ip': 'str',
         'time': 'datetime',
         'url': 'str',
+        'user_agent': 'str',
+        'request_id': 'str',
         'bot': 'BotdDetectionResult'
     }
 
     attribute_map = {
         'ip': 'ip',
         'time': 'time',
         'url': 'url',
+        'user_agent': 'userAgent',
+        'request_id': 'requestId',
         'bot': 'bot'
     }
 
-    def __init__(self, ip=None, time=None, url=None, bot=None):  # noqa: E501
+    def __init__(self, ip=None, time=None, url=None, user_agent=None, request_id=None, bot=None):  # noqa: E501
         """BotdResult - a model defined in Swagger"""  # noqa: E501
         self._ip = None
         self._time = None
         self._url = None
+        self._user_agent = None
+        self._request_id = None
         self._bot = None
         self.discriminator = None
         self.ip = ip
         self.time = time
         self.url = url
+        if user_agent is not None:
+            self.user_agent = user_agent
+        if request_id is not None:
+            self.request_id = request_id
         self.bot = bot
 
     @property
     def ip(self):
         """Gets the ip of this BotdResult.  # noqa: E501
 
         IP address of the requesting browser or bot.  # noqa: E501
@@ -125,14 +135,56 @@
         """
         if url is None:
             raise ValueError("Invalid value for `url`, must not be `None`")  # noqa: E501
 
         self._url = url
 
     @property
+    def user_agent(self):
+        """Gets the user_agent of this BotdResult.  # noqa: E501
+
+
+        :return: The user_agent of this BotdResult.  # noqa: E501
+        :rtype: str
+        """
+        return self._user_agent
+
+    @user_agent.setter
+    def user_agent(self, user_agent):
+        """Sets the user_agent of this BotdResult.
+
+
+        :param user_agent: The user_agent of this BotdResult.  # noqa: E501
+        :type: str
+        """
+
+        self._user_agent = user_agent
+
+    @property
+    def request_id(self):
+        """Gets the request_id of this BotdResult.  # noqa: E501
+
+
+        :return: The request_id of this BotdResult.  # noqa: E501
+        :rtype: str
+        """
+        return self._request_id
+
+    @request_id.setter
+    def request_id(self, request_id):
+        """Sets the request_id of this BotdResult.
+
+
+        :param request_id: The request_id of this BotdResult.  # noqa: E501
+        :type: str
+        """
+
+        self._request_id = request_id
+
+    @property
     def bot(self):
         """Gets the bot of this BotdResult.  # noqa: E501
 
 
         :return: The bot of this BotdResult.  # noqa: E501
         :rtype: BotdDetectionResult
         """
```

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/browser_details.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/browser_details.py`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/confidence.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/confidence.py`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/error_event403_response.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/error_event403_response.py`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/error_event403_response_error.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/error_event403_response_error.py`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/error_event404_response.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/error_event404_response.py`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/error_event404_response_error.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/error_event404_response_error.py`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/error_visits403.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/error_visits403.py`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/event_response.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/event_response.py`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/identification_error.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/identification_error.py`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/ip_location.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_location.py`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/ip_location_city.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_location_city.py`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/location.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/location.py`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/many_requests_response.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/many_requests_response.py`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/products_response.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/products_response_botd.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,87 +11,87 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ProductsResponse(object):
+class ProductsResponseBotd(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'identification': 'ProductsResponseIdentification',
-        'botd': 'ProductsResponseBotd'
+        'data': 'BotdResult',
+        'error': 'ProductError'
     }
 
     attribute_map = {
-        'identification': 'identification',
-        'botd': 'botd'
+        'data': 'data',
+        'error': 'error'
     }
 
-    def __init__(self, identification=None, botd=None):  # noqa: E501
-        """ProductsResponse - a model defined in Swagger"""  # noqa: E501
-        self._identification = None
-        self._botd = None
+    def __init__(self, data=None, error=None):  # noqa: E501
+        """ProductsResponseBotd - a model defined in Swagger"""  # noqa: E501
+        self._data = None
+        self._error = None
         self.discriminator = None
-        if identification is not None:
-            self.identification = identification
-        if botd is not None:
-            self.botd = botd
+        if data is not None:
+            self.data = data
+        if error is not None:
+            self.error = error
 
     @property
-    def identification(self):
-        """Gets the identification of this ProductsResponse.  # noqa: E501
+    def data(self):
+        """Gets the data of this ProductsResponseBotd.  # noqa: E501
 
 
-        :return: The identification of this ProductsResponse.  # noqa: E501
-        :rtype: ProductsResponseIdentification
+        :return: The data of this ProductsResponseBotd.  # noqa: E501
+        :rtype: BotdResult
         """
-        return self._identification
+        return self._data
 
-    @identification.setter
-    def identification(self, identification):
-        """Sets the identification of this ProductsResponse.
+    @data.setter
+    def data(self, data):
+        """Sets the data of this ProductsResponseBotd.
 
 
-        :param identification: The identification of this ProductsResponse.  # noqa: E501
-        :type: ProductsResponseIdentification
+        :param data: The data of this ProductsResponseBotd.  # noqa: E501
+        :type: BotdResult
         """
 
-        self._identification = identification
+        self._data = data
 
     @property
-    def botd(self):
-        """Gets the botd of this ProductsResponse.  # noqa: E501
+    def error(self):
+        """Gets the error of this ProductsResponseBotd.  # noqa: E501
 
 
-        :return: The botd of this ProductsResponse.  # noqa: E501
-        :rtype: ProductsResponseBotd
+        :return: The error of this ProductsResponseBotd.  # noqa: E501
+        :rtype: ProductError
         """
-        return self._botd
+        return self._error
 
-    @botd.setter
-    def botd(self, botd):
-        """Sets the botd of this ProductsResponse.
+    @error.setter
+    def error(self, error):
+        """Sets the error of this ProductsResponseBotd.
 
 
-        :param botd: The botd of this ProductsResponse.  # noqa: E501
-        :type: ProductsResponseBotd
+        :param error: The error of this ProductsResponseBotd.  # noqa: E501
+        :type: ProductError
         """
 
-        self._botd = botd
+        self._error = error
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ProductsResponse, dict):
+        if issubclass(ProductsResponseBotd, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,18 +122,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ProductsResponse):
+        if not isinstance(other, ProductsResponseBotd):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ProductsResponse):
+        if not isinstance(other, ProductsResponseBotd):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/products_response_botd.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_ip_blocklist.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,84 +11,84 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ProductsResponseBotd(object):
+class SignalResponseIpBlocklist(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'data': 'BotdResult',
-        'error': 'BotdError'
+        'data': 'IpBlockListResult',
+        'error': 'ProductError'
     }
 
     attribute_map = {
         'data': 'data',
         'error': 'error'
     }
 
     def __init__(self, data=None, error=None):  # noqa: E501
-        """ProductsResponseBotd - a model defined in Swagger"""  # noqa: E501
+        """SignalResponseIpBlocklist - a model defined in Swagger"""  # noqa: E501
         self._data = None
         self._error = None
         self.discriminator = None
         if data is not None:
             self.data = data
         if error is not None:
             self.error = error
 
     @property
     def data(self):
-        """Gets the data of this ProductsResponseBotd.  # noqa: E501
+        """Gets the data of this SignalResponseIpBlocklist.  # noqa: E501
 
 
-        :return: The data of this ProductsResponseBotd.  # noqa: E501
-        :rtype: BotdResult
+        :return: The data of this SignalResponseIpBlocklist.  # noqa: E501
+        :rtype: IpBlockListResult
         """
         return self._data
 
     @data.setter
     def data(self, data):
-        """Sets the data of this ProductsResponseBotd.
+        """Sets the data of this SignalResponseIpBlocklist.
 
 
-        :param data: The data of this ProductsResponseBotd.  # noqa: E501
-        :type: BotdResult
+        :param data: The data of this SignalResponseIpBlocklist.  # noqa: E501
+        :type: IpBlockListResult
         """
 
         self._data = data
 
     @property
     def error(self):
-        """Gets the error of this ProductsResponseBotd.  # noqa: E501
+        """Gets the error of this SignalResponseIpBlocklist.  # noqa: E501
 
 
-        :return: The error of this ProductsResponseBotd.  # noqa: E501
-        :rtype: BotdError
+        :return: The error of this SignalResponseIpBlocklist.  # noqa: E501
+        :rtype: ProductError
         """
         return self._error
 
     @error.setter
     def error(self, error):
-        """Sets the error of this ProductsResponseBotd.
+        """Sets the error of this SignalResponseIpBlocklist.
 
 
-        :param error: The error of this ProductsResponseBotd.  # noqa: E501
-        :type: BotdError
+        :param error: The error of this SignalResponseIpBlocklist.  # noqa: E501
+        :type: ProductError
         """
 
         self._error = error
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -106,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ProductsResponseBotd, dict):
+        if issubclass(SignalResponseIpBlocklist, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,18 +122,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ProductsResponseBotd):
+        if not isinstance(other, SignalResponseIpBlocklist):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ProductsResponseBotd):
+        if not isinstance(other, SignalResponseIpBlocklist):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/products_response_identification.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/products_response_identification.py`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/products_response_identification_data.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/products_response_identification_data.py`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/response.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/response.py`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/response_visits.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/response_visits.py`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/seen_at.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/seen_at.py`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/subdivision.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/subdivision.py`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/visit.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/visit.py`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/models/webhook_visit.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/webhook_visit.py`

 * *Files 27% similar despite different names*

```diff
@@ -26,17 +26,27 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'visitor_id': 'str',
         'client_referrer': 'str',
+        'user_agent': 'str',
+        'bot': 'BotdDetectionResult',
+        'ip_info': 'IpInfoResult',
+        'incognito': 'bool',
+        'root_apps': 'WebhookSignalResponseRootApps',
+        'emulator': 'WebhookSignalResponseEmulator',
+        'ip_blocklist': 'IpBlockListResult',
+        'tor': 'WebhookSignalResponseTor',
+        'vpn': 'VpnResult',
+        'proxy': 'WebhookSignalResponseProxy',
+        'tampering': 'TamperingResult',
         'request_id': 'str',
         'browser_details': 'BrowserDetails',
-        'incognito': 'bool',
         'ip': 'str',
         'ip_location': 'IPLocation',
         'timestamp': 'int',
         'time': 'datetime',
         'url': 'str',
         'tag': 'dict(str, object)',
         'linked_id': 'str',
@@ -45,37 +55,57 @@
         'first_seen_at': 'SeenAt',
         'last_seen_at': 'SeenAt'
     }
 
     attribute_map = {
         'visitor_id': 'visitorId',
         'client_referrer': 'clientReferrer',
+        'user_agent': 'userAgent',
+        'bot': 'bot',
+        'ip_info': 'ipInfo',
+        'incognito': 'incognito',
+        'root_apps': 'rootApps',
+        'emulator': 'emulator',
+        'ip_blocklist': 'ipBlocklist',
+        'tor': 'tor',
+        'vpn': 'vpn',
+        'proxy': 'proxy',
+        'tampering': 'tampering',
         'request_id': 'requestId',
         'browser_details': 'browserDetails',
-        'incognito': 'incognito',
         'ip': 'ip',
         'ip_location': 'ipLocation',
         'timestamp': 'timestamp',
         'time': 'time',
         'url': 'url',
         'tag': 'tag',
         'linked_id': 'linkedId',
         'confidence': 'confidence',
         'visitor_found': 'visitorFound',
         'first_seen_at': 'firstSeenAt',
         'last_seen_at': 'lastSeenAt'
     }
 
-    def __init__(self, visitor_id=None, client_referrer=None, request_id=None, browser_details=None, incognito=None, ip=None, ip_location=None, timestamp=None, time=None, url=None, tag=None, linked_id=None, confidence=None, visitor_found=None, first_seen_at=None, last_seen_at=None):  # noqa: E501
+    def __init__(self, visitor_id=None, client_referrer=None, user_agent=None, bot=None, ip_info=None, incognito=None, root_apps=None, emulator=None, ip_blocklist=None, tor=None, vpn=None, proxy=None, tampering=None, request_id=None, browser_details=None, ip=None, ip_location=None, timestamp=None, time=None, url=None, tag=None, linked_id=None, confidence=None, visitor_found=None, first_seen_at=None, last_seen_at=None):  # noqa: E501
         """WebhookVisit - a model defined in Swagger"""  # noqa: E501
         self._visitor_id = None
         self._client_referrer = None
+        self._user_agent = None
+        self._bot = None
+        self._ip_info = None
+        self._incognito = None
+        self._root_apps = None
+        self._emulator = None
+        self._ip_blocklist = None
+        self._tor = None
+        self._vpn = None
+        self._proxy = None
+        self._tampering = None
         self._request_id = None
         self._browser_details = None
-        self._incognito = None
         self._ip = None
         self._ip_location = None
         self._timestamp = None
         self._time = None
         self._url = None
         self._tag = None
         self._linked_id = None
@@ -83,17 +113,37 @@
         self._visitor_found = None
         self._first_seen_at = None
         self._last_seen_at = None
         self.discriminator = None
         self.visitor_id = visitor_id
         if client_referrer is not None:
             self.client_referrer = client_referrer
+        if user_agent is not None:
+            self.user_agent = user_agent
+        if bot is not None:
+            self.bot = bot
+        if ip_info is not None:
+            self.ip_info = ip_info
+        self.incognito = incognito
+        if root_apps is not None:
+            self.root_apps = root_apps
+        if emulator is not None:
+            self.emulator = emulator
+        if ip_blocklist is not None:
+            self.ip_blocklist = ip_blocklist
+        if tor is not None:
+            self.tor = tor
+        if vpn is not None:
+            self.vpn = vpn
+        if proxy is not None:
+            self.proxy = proxy
+        if tampering is not None:
+            self.tampering = tampering
         self.request_id = request_id
         self.browser_details = browser_details
-        self.incognito = incognito
         self.ip = ip
         self.ip_location = ip_location
         self.timestamp = timestamp
         self.time = time
         self.url = url
         if tag is not None:
             self.tag = tag
@@ -145,14 +195,249 @@
         :param client_referrer: The client_referrer of this WebhookVisit.  # noqa: E501
         :type: str
         """
 
         self._client_referrer = client_referrer
 
     @property
+    def user_agent(self):
+        """Gets the user_agent of this WebhookVisit.  # noqa: E501
+
+
+        :return: The user_agent of this WebhookVisit.  # noqa: E501
+        :rtype: str
+        """
+        return self._user_agent
+
+    @user_agent.setter
+    def user_agent(self, user_agent):
+        """Sets the user_agent of this WebhookVisit.
+
+
+        :param user_agent: The user_agent of this WebhookVisit.  # noqa: E501
+        :type: str
+        """
+
+        self._user_agent = user_agent
+
+    @property
+    def bot(self):
+        """Gets the bot of this WebhookVisit.  # noqa: E501
+
+
+        :return: The bot of this WebhookVisit.  # noqa: E501
+        :rtype: BotdDetectionResult
+        """
+        return self._bot
+
+    @bot.setter
+    def bot(self, bot):
+        """Sets the bot of this WebhookVisit.
+
+
+        :param bot: The bot of this WebhookVisit.  # noqa: E501
+        :type: BotdDetectionResult
+        """
+
+        self._bot = bot
+
+    @property
+    def ip_info(self):
+        """Gets the ip_info of this WebhookVisit.  # noqa: E501
+
+
+        :return: The ip_info of this WebhookVisit.  # noqa: E501
+        :rtype: IpInfoResult
+        """
+        return self._ip_info
+
+    @ip_info.setter
+    def ip_info(self, ip_info):
+        """Sets the ip_info of this WebhookVisit.
+
+
+        :param ip_info: The ip_info of this WebhookVisit.  # noqa: E501
+        :type: IpInfoResult
+        """
+
+        self._ip_info = ip_info
+
+    @property
+    def incognito(self):
+        """Gets the incognito of this WebhookVisit.  # noqa: E501
+
+        Flag if user used incognito session.  # noqa: E501
+
+        :return: The incognito of this WebhookVisit.  # noqa: E501
+        :rtype: bool
+        """
+        return self._incognito
+
+    @incognito.setter
+    def incognito(self, incognito):
+        """Sets the incognito of this WebhookVisit.
+
+        Flag if user used incognito session.  # noqa: E501
+
+        :param incognito: The incognito of this WebhookVisit.  # noqa: E501
+        :type: bool
+        """
+        if incognito is None:
+            raise ValueError("Invalid value for `incognito`, must not be `None`")  # noqa: E501
+
+        self._incognito = incognito
+
+    @property
+    def root_apps(self):
+        """Gets the root_apps of this WebhookVisit.  # noqa: E501
+
+
+        :return: The root_apps of this WebhookVisit.  # noqa: E501
+        :rtype: WebhookSignalResponseRootApps
+        """
+        return self._root_apps
+
+    @root_apps.setter
+    def root_apps(self, root_apps):
+        """Sets the root_apps of this WebhookVisit.
+
+
+        :param root_apps: The root_apps of this WebhookVisit.  # noqa: E501
+        :type: WebhookSignalResponseRootApps
+        """
+
+        self._root_apps = root_apps
+
+    @property
+    def emulator(self):
+        """Gets the emulator of this WebhookVisit.  # noqa: E501
+
+
+        :return: The emulator of this WebhookVisit.  # noqa: E501
+        :rtype: WebhookSignalResponseEmulator
+        """
+        return self._emulator
+
+    @emulator.setter
+    def emulator(self, emulator):
+        """Sets the emulator of this WebhookVisit.
+
+
+        :param emulator: The emulator of this WebhookVisit.  # noqa: E501
+        :type: WebhookSignalResponseEmulator
+        """
+
+        self._emulator = emulator
+
+    @property
+    def ip_blocklist(self):
+        """Gets the ip_blocklist of this WebhookVisit.  # noqa: E501
+
+
+        :return: The ip_blocklist of this WebhookVisit.  # noqa: E501
+        :rtype: IpBlockListResult
+        """
+        return self._ip_blocklist
+
+    @ip_blocklist.setter
+    def ip_blocklist(self, ip_blocklist):
+        """Sets the ip_blocklist of this WebhookVisit.
+
+
+        :param ip_blocklist: The ip_blocklist of this WebhookVisit.  # noqa: E501
+        :type: IpBlockListResult
+        """
+
+        self._ip_blocklist = ip_blocklist
+
+    @property
+    def tor(self):
+        """Gets the tor of this WebhookVisit.  # noqa: E501
+
+
+        :return: The tor of this WebhookVisit.  # noqa: E501
+        :rtype: WebhookSignalResponseTor
+        """
+        return self._tor
+
+    @tor.setter
+    def tor(self, tor):
+        """Sets the tor of this WebhookVisit.
+
+
+        :param tor: The tor of this WebhookVisit.  # noqa: E501
+        :type: WebhookSignalResponseTor
+        """
+
+        self._tor = tor
+
+    @property
+    def vpn(self):
+        """Gets the vpn of this WebhookVisit.  # noqa: E501
+
+
+        :return: The vpn of this WebhookVisit.  # noqa: E501
+        :rtype: VpnResult
+        """
+        return self._vpn
+
+    @vpn.setter
+    def vpn(self, vpn):
+        """Sets the vpn of this WebhookVisit.
+
+
+        :param vpn: The vpn of this WebhookVisit.  # noqa: E501
+        :type: VpnResult
+        """
+
+        self._vpn = vpn
+
+    @property
+    def proxy(self):
+        """Gets the proxy of this WebhookVisit.  # noqa: E501
+
+
+        :return: The proxy of this WebhookVisit.  # noqa: E501
+        :rtype: WebhookSignalResponseProxy
+        """
+        return self._proxy
+
+    @proxy.setter
+    def proxy(self, proxy):
+        """Sets the proxy of this WebhookVisit.
+
+
+        :param proxy: The proxy of this WebhookVisit.  # noqa: E501
+        :type: WebhookSignalResponseProxy
+        """
+
+        self._proxy = proxy
+
+    @property
+    def tampering(self):
+        """Gets the tampering of this WebhookVisit.  # noqa: E501
+
+
+        :return: The tampering of this WebhookVisit.  # noqa: E501
+        :rtype: TamperingResult
+        """
+        return self._tampering
+
+    @tampering.setter
+    def tampering(self, tampering):
+        """Sets the tampering of this WebhookVisit.
+
+
+        :param tampering: The tampering of this WebhookVisit.  # noqa: E501
+        :type: TamperingResult
+        """
+
+        self._tampering = tampering
+
+    @property
     def request_id(self):
         """Gets the request_id of this WebhookVisit.  # noqa: E501
 
         Unique identifier of the user's identification request.  # noqa: E501
 
         :return: The request_id of this WebhookVisit.  # noqa: E501
         :rtype: str
@@ -193,39 +478,14 @@
         """
         if browser_details is None:
             raise ValueError("Invalid value for `browser_details`, must not be `None`")  # noqa: E501
 
         self._browser_details = browser_details
 
     @property
-    def incognito(self):
-        """Gets the incognito of this WebhookVisit.  # noqa: E501
-
-        Flag if user used incognito session.  # noqa: E501
-
-        :return: The incognito of this WebhookVisit.  # noqa: E501
-        :rtype: bool
-        """
-        return self._incognito
-
-    @incognito.setter
-    def incognito(self, incognito):
-        """Sets the incognito of this WebhookVisit.
-
-        Flag if user used incognito session.  # noqa: E501
-
-        :param incognito: The incognito of this WebhookVisit.  # noqa: E501
-        :type: bool
-        """
-        if incognito is None:
-            raise ValueError("Invalid value for `incognito`, must not be `None`")  # noqa: E501
-
-        self._incognito = incognito
-
-    @property
     def ip(self):
         """Gets the ip of this WebhookVisit.  # noqa: E501
 
 
         :return: The ip of this WebhookVisit.  # noqa: E501
         :rtype: str
         """
```

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk/rest.py` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/fingerprint_pro_server_api_sdk.egg-info/PKG-INFO` & `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: fingerprint-pro-server-api-sdk
-Version: 2.1.0
+Version: 2.2.0
 Summary: Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.
 Home-page: https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk
 Author: Fingerprint
 Author-email: support@fingerprint.com
 License: MIT
 Keywords: Swagger,Fingerprint Pro Server API,browser,detection,fingerprint,identification,fingerprinting,browser-fingerprinting,browser-fingerprint,fraud-detection,fraud,audio-fingerprinting,fingerprintjs,fingerprintjs-pro,visitor-identifier
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
@@ -58,15 +57,15 @@
 
 # Fingerprint Pro Server Python SDK
 Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 3
-- Package version: 2.1.0
+- Package version: 2.2.0
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -174,38 +173,64 @@
 ------------ | ------------- | ------------- | -------------
 *FingerprintApi* | [**get_event**](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/FingerprintApi.md#get_event) | **GET** /events/{request_id} | Get event by requestId
 *FingerprintApi* | [**get_visits**](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/FingerprintApi.md#get_visits) | **GET** /visitors/{visitor_id} | Get visits by visitorId
 
 ## Documentation For Models
 
  - [BotdDetectionResult](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/BotdDetectionResult.md)
- - [BotdError](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/BotdError.md)
  - [BotdResult](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/BotdResult.md)
  - [BrowserDetails](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/BrowserDetails.md)
  - [Confidence](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/Confidence.md)
  - [ErrorEvent403Response](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ErrorEvent403Response.md)
  - [ErrorEvent403ResponseError](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ErrorEvent403ResponseError.md)
  - [ErrorEvent404Response](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ErrorEvent404Response.md)
  - [ErrorEvent404ResponseError](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ErrorEvent404ResponseError.md)
  - [ErrorVisits403](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ErrorVisits403.md)
  - [EventResponse](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/EventResponse.md)
  - [IPLocation](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/IPLocation.md)
  - [IPLocationCity](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/IPLocationCity.md)
  - [IdentificationError](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/IdentificationError.md)
+ - [IpBlockListResult](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/IpBlockListResult.md)
+ - [IpBlockListResultDetails](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/IpBlockListResultDetails.md)
+ - [IpInfoResult](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/IpInfoResult.md)
+ - [IpInfoResultV4](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/IpInfoResultV4.md)
+ - [IpInfoResultV6](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/IpInfoResultV6.md)
  - [Location](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/Location.md)
  - [ManyRequestsResponse](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ManyRequestsResponse.md)
+ - [ProductError](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ProductError.md)
  - [ProductsResponse](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ProductsResponse.md)
  - [ProductsResponseBotd](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ProductsResponseBotd.md)
  - [ProductsResponseIdentification](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ProductsResponseIdentification.md)
  - [ProductsResponseIdentificationData](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ProductsResponseIdentificationData.md)
  - [Response](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/Response.md)
  - [ResponseVisits](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/ResponseVisits.md)
  - [SeenAt](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SeenAt.md)
+ - [SignalResponseEmulator](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseEmulator.md)
+ - [SignalResponseEmulatorData](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseEmulatorData.md)
+ - [SignalResponseIncognito](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseIncognito.md)
+ - [SignalResponseIncognitoData](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseIncognitoData.md)
+ - [SignalResponseIpBlocklist](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseIpBlocklist.md)
+ - [SignalResponseIpInfo](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseIpInfo.md)
+ - [SignalResponseProxy](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseProxy.md)
+ - [SignalResponseProxyData](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseProxyData.md)
+ - [SignalResponseRootApps](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseRootApps.md)
+ - [SignalResponseRootAppsData](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseRootAppsData.md)
+ - [SignalResponseTampering](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseTampering.md)
+ - [SignalResponseTor](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseTor.md)
+ - [SignalResponseTorData](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseTorData.md)
+ - [SignalResponseVpn](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseVpn.md)
  - [Subdivision](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/Subdivision.md)
+ - [TamperingResult](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/TamperingResult.md)
  - [Visit](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/Visit.md)
+ - [VpnResult](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/VpnResult.md)
+ - [VpnResultMethods](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/VpnResultMethods.md)
+ - [WebhookSignalResponseEmulator](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/WebhookSignalResponseEmulator.md)
+ - [WebhookSignalResponseProxy](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/WebhookSignalResponseProxy.md)
+ - [WebhookSignalResponseRootApps](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/WebhookSignalResponseRootApps.md)
+ - [WebhookSignalResponseTor](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/WebhookSignalResponseTor.md)
  - [WebhookVisit](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/WebhookVisit.md)
 
 ## Documentation For Authorization
 
 
 ## ApiKeyHeader
 
@@ -219,9 +244,7 @@
 - **API key parameter name**: api_key
 - **Location**: URL query string
 
 
 ## Author
 
 support@fingerprint.com
-
-
```

#### html2text {}

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1 Name: fingerprint-pro-server-api-sdk Version: 2.1.0
+Metadata-Version: 2.1 Name: fingerprint-pro-server-api-sdk Version: 2.2.0
 Summary: Fingerprint Pro Server API allows you to get information about
 visitors and about individual events in a server environment. This API can be
 used for data exports, decision-making, and data analysis scenarios. Home-page:
 https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk Author:
 Fingerprint Author-email: support@fingerprint.com License: MIT Keywords:
 Swagger,Fingerprint Pro Server
 API,browser,detection,fingerprint,identification,fingerprinting,browser-
 fingerprinting,browser-fingerprint,fraud-detection,fraud,audio-
-fingerprinting,fingerprintjs,fingerprintjs-pro,visitor-identifier Platform:
-UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
-Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
-License Classifier: Programming Language :: Python :: 2 Classifier: Programming
-Language :: Python Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.4 Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: Implementation :: PyPy Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Topic :: Security
-Description-Content-Type: text/markdown License-File: LICENSE
+fingerprinting,fingerprintjs,fingerprintjs-pro,visitor-identifier Classifier:
+Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
+Developers Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 2 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2.7 Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python ::
+Implementation :: PyPy Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Classifier: Topic :: Security Description-Content-Type: text/
+markdown License-File: LICENSE
                               [Fingerprint_logo]
  [PyPI] [coverage] [CI_badge] [CI_badge] [CI_badge] [https://img.shields.io/:
                license-mit-blue.svg?style=flat] [Discord_server]
 # Fingerprint Pro Server Python SDK Fingerprint Pro Server API allows you to
 get information about visitors and about individual events in a server
 environment. This API can be used for data exports, decision-making, and data
 analysis scenarios. This Python package is automatically generated by the
 [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project: -
-API version: 3 - Package version: 2.1.0 - Build package:
+API version: 3 - Package version: 2.2.0 - Build package:
 io.swagger.codegen.v3.generators.python.PythonClientCodegen ## Requirements.
 Python 2.7 and 3.4+ ## Installation & Usage ### pip install You can install the
 package directly from the Github ```sh pip install git+https://github.com/
 fingerprintjs/fingerprint-pro-server-api-python-sdk.git ``` Or from the PyPI
 ```sh pip install fingerprint_pro_server_api_sdk ``` Then import the package:
 ```python import fingerprint_pro_server_api_sdk ``` ### Setuptools Install via
 [Setuptools](http://pypi.python.org/pypi/setuptools). ```sh python setup.py
@@ -78,55 +78,103 @@
 (https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/
 main/docs/FingerprintApi.md#get_event) | **GET** /events/{request_id} | Get
 event by requestId *FingerprintApi* | [**get_visits**](https://github.com/
 fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
 FingerprintApi.md#get_visits) | **GET** /visitors/{visitor_id} | Get visits by
 visitorId ## Documentation For Models - [BotdDetectionResult](https://
 github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
-BotdDetectionResult.md) - [BotdError](https://github.com/fingerprintjs/
-fingerprint-pro-server-api-python-sdk/blob/main/docs/BotdError.md) -
-[BotdResult](https://github.com/fingerprintjs/fingerprint-pro-server-api-
-python-sdk/blob/main/docs/BotdResult.md) - [BrowserDetails](https://github.com/
-fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
-BrowserDetails.md) - [Confidence](https://github.com/fingerprintjs/fingerprint-
-pro-server-api-python-sdk/blob/main/docs/Confidence.md) -
-[ErrorEvent403Response](https://github.com/fingerprintjs/fingerprint-pro-
-server-api-python-sdk/blob/main/docs/ErrorEvent403Response.md) -
-[ErrorEvent403ResponseError](https://github.com/fingerprintjs/fingerprint-pro-
-server-api-python-sdk/blob/main/docs/ErrorEvent403ResponseError.md) -
+BotdDetectionResult.md) - [BotdResult](https://github.com/fingerprintjs/
+fingerprint-pro-server-api-python-sdk/blob/main/docs/BotdResult.md) -
+[BrowserDetails](https://github.com/fingerprintjs/fingerprint-pro-server-api-
+python-sdk/blob/main/docs/BrowserDetails.md) - [Confidence](https://github.com/
+fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+Confidence.md) - [ErrorEvent403Response](https://github.com/fingerprintjs/
+fingerprint-pro-server-api-python-sdk/blob/main/docs/ErrorEvent403Response.md)
+- [ErrorEvent403ResponseError](https://github.com/fingerprintjs/fingerprint-
+pro-server-api-python-sdk/blob/main/docs/ErrorEvent403ResponseError.md) -
 [ErrorEvent404Response](https://github.com/fingerprintjs/fingerprint-pro-
 server-api-python-sdk/blob/main/docs/ErrorEvent404Response.md) -
 [ErrorEvent404ResponseError](https://github.com/fingerprintjs/fingerprint-pro-
 server-api-python-sdk/blob/main/docs/ErrorEvent404ResponseError.md) -
 [ErrorVisits403](https://github.com/fingerprintjs/fingerprint-pro-server-api-
 python-sdk/blob/main/docs/ErrorVisits403.md) - [EventResponse](https://
 github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
 EventResponse.md) - [IPLocation](https://github.com/fingerprintjs/fingerprint-
 pro-server-api-python-sdk/blob/main/docs/IPLocation.md) - [IPLocationCity]
 (https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/
 main/docs/IPLocationCity.md) - [IdentificationError](https://github.com/
 fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
-IdentificationError.md) - [Location](https://github.com/fingerprintjs/
-fingerprint-pro-server-api-python-sdk/blob/main/docs/Location.md) -
-[ManyRequestsResponse](https://github.com/fingerprintjs/fingerprint-pro-server-
-api-python-sdk/blob/main/docs/ManyRequestsResponse.md) - [ProductsResponse]
-(https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/
-main/docs/ProductsResponse.md) - [ProductsResponseBotd](https://github.com/
+IdentificationError.md) - [IpBlockListResult](https://github.com/fingerprintjs/
+fingerprint-pro-server-api-python-sdk/blob/main/docs/IpBlockListResult.md) -
+[IpBlockListResultDetails](https://github.com/fingerprintjs/fingerprint-pro-
+server-api-python-sdk/blob/main/docs/IpBlockListResultDetails.md) -
+[IpInfoResult](https://github.com/fingerprintjs/fingerprint-pro-server-api-
+python-sdk/blob/main/docs/IpInfoResult.md) - [IpInfoResultV4](https://
+github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+IpInfoResultV4.md) - [IpInfoResultV6](https://github.com/fingerprintjs/
+fingerprint-pro-server-api-python-sdk/blob/main/docs/IpInfoResultV6.md) -
+[Location](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-
+sdk/blob/main/docs/Location.md) - [ManyRequestsResponse](https://github.com/
 fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+ManyRequestsResponse.md) - [ProductError](https://github.com/fingerprintjs/
+fingerprint-pro-server-api-python-sdk/blob/main/docs/ProductError.md) -
+[ProductsResponse](https://github.com/fingerprintjs/fingerprint-pro-server-api-
+python-sdk/blob/main/docs/ProductsResponse.md) - [ProductsResponseBotd](https:/
+/github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
 ProductsResponseBotd.md) - [ProductsResponseIdentification](https://github.com/
 fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
 ProductsResponseIdentification.md) - [ProductsResponseIdentificationData]
 (https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/
 main/docs/ProductsResponseIdentificationData.md) - [Response](https://
 github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
 Response.md) - [ResponseVisits](https://github.com/fingerprintjs/fingerprint-
 pro-server-api-python-sdk/blob/main/docs/ResponseVisits.md) - [SeenAt](https://
 github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
-SeenAt.md) - [Subdivision](https://github.com/fingerprintjs/fingerprint-pro-
-server-api-python-sdk/blob/main/docs/Subdivision.md) - [Visit](https://
+SeenAt.md) - [SignalResponseEmulator](https://github.com/fingerprintjs/
+fingerprint-pro-server-api-python-sdk/blob/main/docs/SignalResponseEmulator.md)
+- [SignalResponseEmulatorData](https://github.com/fingerprintjs/fingerprint-
+pro-server-api-python-sdk/blob/main/docs/SignalResponseEmulatorData.md) -
+[SignalResponseIncognito](https://github.com/fingerprintjs/fingerprint-pro-
+server-api-python-sdk/blob/main/docs/SignalResponseIncognito.md) -
+[SignalResponseIncognitoData](https://github.com/fingerprintjs/fingerprint-pro-
+server-api-python-sdk/blob/main/docs/SignalResponseIncognitoData.md) -
+[SignalResponseIpBlocklist](https://github.com/fingerprintjs/fingerprint-pro-
+server-api-python-sdk/blob/main/docs/SignalResponseIpBlocklist.md) -
+[SignalResponseIpInfo](https://github.com/fingerprintjs/fingerprint-pro-server-
+api-python-sdk/blob/main/docs/SignalResponseIpInfo.md) - [SignalResponseProxy]
+(https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/
+main/docs/SignalResponseProxy.md) - [SignalResponseProxyData](https://
+github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+SignalResponseProxyData.md) - [SignalResponseRootApps](https://github.com/
+fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+SignalResponseRootApps.md) - [SignalResponseRootAppsData](https://github.com/
+fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+SignalResponseRootAppsData.md) - [SignalResponseTampering](https://github.com/
+fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+SignalResponseTampering.md) - [SignalResponseTor](https://github.com/
+fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+SignalResponseTor.md) - [SignalResponseTorData](https://github.com/
+fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+SignalResponseTorData.md) - [SignalResponseVpn](https://github.com/
+fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+SignalResponseVpn.md) - [Subdivision](https://github.com/fingerprintjs/
+fingerprint-pro-server-api-python-sdk/blob/main/docs/Subdivision.md) -
+[TamperingResult](https://github.com/fingerprintjs/fingerprint-pro-server-api-
+python-sdk/blob/main/docs/TamperingResult.md) - [Visit](https://github.com/
+fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/Visit.md) -
+[VpnResult](https://github.com/fingerprintjs/fingerprint-pro-server-api-python-
+sdk/blob/main/docs/VpnResult.md) - [VpnResultMethods](https://github.com/
+fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+VpnResultMethods.md) - [WebhookSignalResponseEmulator](https://github.com/
+fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+WebhookSignalResponseEmulator.md) - [WebhookSignalResponseProxy](https://
+github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+WebhookSignalResponseProxy.md) - [WebhookSignalResponseRootApps](https://
+github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
+WebhookSignalResponseRootApps.md) - [WebhookSignalResponseTor](https://
 github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/docs/
-Visit.md) - [WebhookVisit](https://github.com/fingerprintjs/fingerprint-pro-
-server-api-python-sdk/blob/main/docs/WebhookVisit.md) ## Documentation For
-Authorization ## ApiKeyHeader - **Type**: API key - **API key parameter name**:
-Auth-API-Key - **Location**: HTTP header ## ApiKeyQuery - **Type**: API key -
-**API key parameter name**: api_key - **Location**: URL query string ## Author
-support@fingerprint.com
+WebhookSignalResponseTor.md) - [WebhookVisit](https://github.com/fingerprintjs/
+fingerprint-pro-server-api-python-sdk/blob/main/docs/WebhookVisit.md) ##
+Documentation For Authorization ## ApiKeyHeader - **Type**: API key - **API key
+parameter name**: Auth-API-Key - **Location**: HTTP header ## ApiKeyQuery -
+**Type**: API key - **API key parameter name**: api_key - **Location**: URL
+query string ## Author support@fingerprint.com
```

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/setup.py` & `fingerprint-pro-server-api-sdk-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import pathlib
 import re
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "fingerprint-pro-server-api-sdk"
-VERSION = "2.1.0"
+VERSION = "2.2.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `fingerprint-pro-server-api-sdk-2.1.0/test/test_fingerprint_api.py` & `fingerprint-pro-server-api-sdk-2.2.0/test/test_fingerprint_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from fingerprint_pro_server_api_sdk import Configuration, ManyRequestsResponse, ErrorVisits403, ErrorEvent403Response, \
     ErrorEvent404Response
 from fingerprint_pro_server_api_sdk.api.fingerprint_api import FingerprintApi  # noqa: E501
 from fingerprint_pro_server_api_sdk.rest import KnownApiException
 
 API_KEY = 'private_key'
 
-VERSION = '2.1.0'
+VERSION = '2.2.0'
 
 
 class MockPoolManager(object):
     def __init__(self, tc):
         self._tc = tc
         self._reqs = []
 
@@ -109,20 +109,28 @@
 
     def test_get_visits_correct_data(self):
         """Test checks correct code run result in default scenario"""
         mock_pool = MockPoolManager(self)
         self.api.api_client.rest_client.pool_manager = mock_pool
         mock_file1 = 'visits_limit_1.json'
         mock_file2 = 'visits_limit_500.json'
+        mock_file3 = 'visits_limit_500.json'
+        mock_file4 = 'visits_limit_500.json'
         mock_pool.expect_request('GET', TestFingerprintApi.get_get_visits_method_path(visitor_id=mock_file1),
                                  fields=[self.integration_info], headers=self.request_headers,
                                  preload_content=True, timeout=None)
         mock_pool.expect_request('GET', TestFingerprintApi.get_get_visits_method_path(visitor_id=mock_file2),
                                  fields=[self.integration_info], headers=self.request_headers,
                                  preload_content=True, timeout=None)
+        mock_pool.expect_request('GET', TestFingerprintApi.get_get_visits_method_path(visitor_id=mock_file3),
+                                 fields=[self.integration_info], headers=self.request_headers,
+                                 preload_content=True, timeout=None)
+        mock_pool.expect_request('GET', TestFingerprintApi.get_get_visits_method_path(visitor_id=mock_file4),
+                                 fields=[self.integration_info], headers=self.request_headers,
+                                 preload_content=True, timeout=None)
         self.api.get_visits(mock_file1)
         self.api.get_visits(mock_file2)
 
     def test_get_visits_error_403(self):
         """Test checks correct code run result in case of 403 error"""
         mock_pool = MockPoolManager(self)
         self.api.api_client.rest_client.pool_manager = mock_pool
```

