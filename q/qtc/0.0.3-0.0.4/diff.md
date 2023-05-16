# Comparing `tmp/qtc-0.0.3.tar.gz` & `tmp/qtc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtc-0.0.3.tar", last modified: Sun May 14 07:44:49 2023, max compression
+gzip compressed data, was "qtc-0.0.4.tar", last modified: Tue May 16 20:02:20 2023, max compression
```

## Comparing `qtc-0.0.3.tar` & `qtc-0.0.4.tar`

### file list

```diff
@@ -1,79 +1,85 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.515946 qtc-0.0.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       62 2023-04-28 00:35:58.000000 qtc-0.0.3/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      150 2023-05-14 07:44:49.515946 qtc-0.0.3/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2023-04-28 00:35:58.000000 qtc-0.0.3/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.495946 qtc-0.0.3/qtc/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.495946 qtc-0.0.3/qtc/app_configs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-29 15:40:20.000000 qtc-0.0.3/qtc/app_configs/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.495946 qtc-0.0.3/qtc/app_configs/bq/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-29 15:40:25.000000 qtc-0.0.3/qtc/app_configs/bq/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      247 2023-04-29 15:40:25.000000 qtc-0.0.3/qtc/app_configs/bq/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4648 2023-04-29 15:41:30.000000 qtc-0.0.3/qtc/app_configs/bq/params.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.499945 qtc-0.0.3/qtc/app_configs/bq_sim/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-29 15:40:22.000000 qtc-0.0.3/qtc/app_configs/bq_sim/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5745 2023-04-29 15:40:22.000000 qtc-0.0.3/qtc/app_configs/bq_sim/params.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.499945 qtc-0.0.3/qtc/calendar/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/calendar/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10261 2023-04-28 01:40:37.000000 qtc-0.0.3/qtc/calendar/calendar.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.499945 qtc-0.0.3/qtc/consts/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/consts/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6908 2023-04-29 15:42:12.000000 qtc-0.0.3/qtc/consts/enums.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      370 2023-04-30 15:11:38.000000 qtc-0.0.3/qtc/env_config.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5371 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/env_config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.503945 qtc-0.0.3/qtc/ext/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/ext/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1459 2023-04-28 01:41:03.000000 qtc-0.0.3/qtc/ext/configurable.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1145 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/ext/enum.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1992 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/ext/inspect.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2131 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/ext/logging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1453 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/ext/multiprocessing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1037 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/ext/unittest.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.503945 qtc-0.0.3/qtc/file/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/file/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9319 2023-04-28 01:57:29.000000 qtc-0.0.3/qtc/file/file_cache.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16376 2023-04-28 01:57:29.000000 qtc-0.0.3/qtc/file/file_manager.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30307 2023-04-28 01:57:29.000000 qtc-0.0.3/qtc/file/file_serialization.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.503945 qtc-0.0.3/qtc/toolbox/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/toolbox/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-13 06:34:37.000000 qtc-0.0.3/qtc/toolbox/calcs.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.511946 qtc-0.0.3/qtc/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.3/qtc/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2639 2023-04-30 15:30:33.000000 qtc-0.0.3/qtc/utils/cipher_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3931 2023-04-30 15:30:33.000000 qtc-0.0.3/qtc/utils/dash_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27238 2023-04-30 15:30:33.000000 qtc-0.0.3/qtc/utils/datetime_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30426 2023-04-30 15:30:33.000000 qtc-0.0.3/qtc/utils/db_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7567 2023-04-28 02:56:22.000000 qtc-0.0.3/qtc/utils/email_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4540 2023-04-28 01:49:03.000000 qtc-0.0.3/qtc/utils/endpoint_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6612 2023-04-28 03:01:16.000000 qtc-0.0.3/qtc/utils/file_system_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7840 2023-04-28 01:53:01.000000 qtc-0.0.3/qtc/utils/html_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6663 2023-04-28 01:57:29.000000 qtc-0.0.3/qtc/utils/misc_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11079 2023-04-28 01:57:29.000000 qtc-0.0.3/qtc/utils/notebook_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-05-13 06:38:50.000000 qtc-0.0.3/qtc/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.495946 qtc-0.0.3/qtc.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      150 2023-05-14 07:44:49.000000 qtc-0.0.3/qtc.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1500 2023-05-14 07:44:49.000000 qtc-0.0.3/qtc.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-14 07:44:49.000000 qtc-0.0.3/qtc.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-29 14:49:44.000000 qtc-0.0.3/qtc.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       66 2023-05-14 07:44:49.000000 qtc-0.0.3/qtc.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2023-05-14 07:44:49.000000 qtc-0.0.3/qtc.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-14 07:44:49.515946 qtc-0.0.3/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      724 2023-05-13 06:37:41.000000 qtc-0.0.3/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.511946 qtc-0.0.3/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.511946 qtc-0.0.3/tests/ext/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/ext/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1003 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/ext/test_enum.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      580 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/ext/test_inspect.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.511946 qtc-0.0.3/tests/file/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/file/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4834 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/file/test_file_cache.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3244 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/file/test_file_manager.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5806 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/file/test_file_serialization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      431 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/test_env_config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-14 07:44:49.515946 qtc-0.0.3/tests/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      558 2023-04-28 02:46:02.000000 qtc-0.0.3/tests/utils/test_cipher_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3939 2023-04-28 02:45:02.000000 qtc-0.0.3/tests/utils/test_datetime_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2604 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/utils/test_db_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1855 2023-04-28 00:35:58.000000 qtc-0.0.3/tests/utils/test_misc_utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.721361 qtc-0.0.4/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       62 2023-04-28 00:35:58.000000 qtc-0.0.4/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      150 2023-05-16 20:02:20.717361 qtc-0.0.4/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       29 2023-04-28 00:35:58.000000 qtc-0.0.4/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.713361 qtc-0.0.4/qtc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.713361 qtc-0.0.4/qtc/app_configs/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-29 15:40:20.000000 qtc-0.0.4/qtc/app_configs/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.713361 qtc-0.0.4/qtc/app_configs/bq/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-29 15:40:25.000000 qtc-0.0.4/qtc/app_configs/bq/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      247 2023-04-29 15:40:25.000000 qtc-0.0.4/qtc/app_configs/bq/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4648 2023-04-29 15:41:30.000000 qtc-0.0.4/qtc/app_configs/bq/params.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.713361 qtc-0.0.4/qtc/app_configs/bq_sim/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-29 15:40:22.000000 qtc-0.0.4/qtc/app_configs/bq_sim/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5745 2023-04-29 15:40:22.000000 qtc-0.0.4/qtc/app_configs/bq_sim/params.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.713361 qtc-0.0.4/qtc/calendar/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/calendar/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10278 2023-05-16 19:59:16.000000 qtc-0.0.4/qtc/calendar/calendar.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7479 2023-05-16 19:58:25.000000 qtc-0.0.4/qtc/calendar/cn_stock_calendar.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.713361 qtc-0.0.4/qtc/consts/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/consts/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6908 2023-04-29 15:42:12.000000 qtc-0.0.4/qtc/consts/enums.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.713361 qtc-0.0.4/qtc/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 03:32:47.000000 qtc-0.0.4/qtc/data/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.713361 qtc-0.0.4/qtc/data/dal/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 03:33:01.000000 qtc-0.0.4/qtc/data/dal/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1822 2023-05-16 04:08:20.000000 qtc-0.0.4/qtc/data/dal/calendar.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      370 2023-04-30 15:11:38.000000 qtc-0.0.4/qtc/env_config.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5371 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/env_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.717361 qtc-0.0.4/qtc/ext/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/ext/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1459 2023-04-28 01:41:03.000000 qtc-0.0.4/qtc/ext/configurable.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1145 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/ext/enum.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1992 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/ext/inspect.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2131 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/ext/logging.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1453 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/ext/multiprocessing.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1037 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/ext/unittest.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.717361 qtc-0.0.4/qtc/file/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/file/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9319 2023-04-28 01:57:29.000000 qtc-0.0.4/qtc/file/file_cache.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16376 2023-04-28 01:57:29.000000 qtc-0.0.4/qtc/file/file_manager.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30307 2023-04-28 01:57:29.000000 qtc-0.0.4/qtc/file/file_serialization.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.717361 qtc-0.0.4/qtc/toolbox/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/toolbox/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-13 06:34:37.000000 qtc-0.0.4/qtc/toolbox/calcs.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.717361 qtc-0.0.4/qtc/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.4/qtc/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2639 2023-04-30 15:30:33.000000 qtc-0.0.4/qtc/utils/cipher_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3931 2023-04-30 15:30:33.000000 qtc-0.0.4/qtc/utils/dash_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27238 2023-04-30 15:30:33.000000 qtc-0.0.4/qtc/utils/datetime_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    31119 2023-05-16 03:51:59.000000 qtc-0.0.4/qtc/utils/db_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7567 2023-04-28 02:56:22.000000 qtc-0.0.4/qtc/utils/email_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4540 2023-04-28 01:49:03.000000 qtc-0.0.4/qtc/utils/endpoint_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6612 2023-04-28 03:01:16.000000 qtc-0.0.4/qtc/utils/file_system_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7840 2023-04-28 01:53:01.000000 qtc-0.0.4/qtc/utils/html_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6663 2023-04-28 01:57:29.000000 qtc-0.0.4/qtc/utils/misc_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11079 2023-04-28 01:57:29.000000 qtc-0.0.4/qtc/utils/notebook_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-05-16 20:02:15.000000 qtc-0.0.4/qtc/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.713361 qtc-0.0.4/qtc.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      150 2023-05-16 20:02:20.000000 qtc-0.0.4/qtc.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1605 2023-05-16 20:02:20.000000 qtc-0.0.4/qtc.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-16 20:02:20.000000 qtc-0.0.4/qtc.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-29 14:49:44.000000 qtc-0.0.4/qtc.egg-info/not-zip-safe
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       66 2023-05-16 20:02:20.000000 qtc-0.0.4/qtc.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2023-05-16 20:02:20.000000 qtc-0.0.4/qtc.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-16 20:02:20.721361 qtc-0.0.4/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      724 2023-05-13 06:37:41.000000 qtc-0.0.4/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.717361 qtc-0.0.4/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.717361 qtc-0.0.4/tests/ext/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/ext/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1003 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/ext/test_enum.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      580 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/ext/test_inspect.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.717361 qtc-0.0.4/tests/file/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/file/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4834 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/file/test_file_cache.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3244 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/file/test_file_manager.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5806 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/file/test_file_serialization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      431 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/test_env_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-16 20:02:20.717361 qtc-0.0.4/tests/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      558 2023-04-28 02:46:02.000000 qtc-0.0.4/tests/utils/test_cipher_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3939 2023-04-28 02:45:02.000000 qtc-0.0.4/tests/utils/test_datetime_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2604 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/utils/test_db_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1855 2023-04-28 00:35:58.000000 qtc-0.0.4/tests/utils/test_misc_utils.py
```

### Comparing `qtc-0.0.3/qtc/app_configs/bq/params.py` & `qtc-0.0.4/qtc/app_configs/bq/params.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/qtc/app_configs/bq_sim/params.py` & `qtc-0.0.4/qtc/app_configs/bq_sim/params.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/qtc/calendar/calendar.py` & `qtc-0.0.4/qtc/calendar/calendar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import bisect
 import re
 from dateutil.relativedelta import relativedelta
 import qtc.utils.datetime_utils as dtu
 import qtc.utils.misc_utils as mu
 from qtc.consts.enums import OffsetDateType
+from qtc.ext.enum import Enum
 from qtc.ext.logging import set_logger
 logger = set_logger()
 
-# class CalendarType(Enum):
-#     EXCHANGE = 'Exchange'
-#     FACTOR_MODEL = 'FactorModel'
+class CalendarType(Enum):
+    EXCHANGE = 'Exchange'
+    CN_STOCK = 'CN_STOCK'
 
 
 class Calendar:
-    DEFAULT_TIME_ZONE = 'America/New_York'
+    DEFAULT_TIME_ZONE = 'Asia/Shanghai'
 
     @staticmethod
     def _get_trading_dateids(trading_dateids, start_dateid=None, end_dateid=None):
         start_dateid = min(trading_dateids) if start_dateid is None else int(start_dateid)
         end_dateid = max(trading_dateids) if end_dateid is None else int(end_dateid)
 
         return (dateid for dateid in trading_dateids if dateid >= start_dateid and dateid <= end_dateid)
@@ -190,8 +191,8 @@
         start_dateid, end_dateid = \
             Calendar.infer_start_dateid_end_dateid(trading_dateids=trading_dateids,
                                                    start_date=start_date, end_date=end_date,
                                                    date_range_mode=date_range_mode)
         dateids = list(Calendar.get_trading_dateids(trading_dateids=trading_dateids,
                                                     start_date=start_dateid, end_date=end_dateid))
 
-        return dateids, start_dateid, end_dateid
+        return dateids, start_dateid, end_dateid
```

### Comparing `qtc-0.0.3/qtc/consts/enums.py` & `qtc-0.0.4/qtc/consts/enums.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/qtc/env_config.py` & `qtc-0.0.4/qtc/env_config.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/qtc/ext/configurable.py` & `qtc-0.0.4/qtc/ext/configurable.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/qtc/ext/enum.py` & `qtc-0.0.4/qtc/ext/enum.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/qtc/ext/inspect.py` & `qtc-0.0.4/qtc/ext/inspect.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/qtc/ext/logging.py` & `qtc-0.0.4/qtc/ext/logging.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/qtc/ext/multiprocessing.py` & `qtc-0.0.4/qtc/ext/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/qtc/ext/unittest.py` & `qtc-0.0.4/qtc/ext/unittest.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/qtc/file/file_cache.py` & `qtc-0.0.4/qtc/file/file_cache.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/qtc/file/file_manager.py` & `qtc-0.0.4/qtc/file/file_manager.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/qtc/file/file_serialization.py` & `qtc-0.0.4/qtc/file/file_serialization.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/qtc/utils/cipher_utils.py` & `qtc-0.0.4/qtc/utils/cipher_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/qtc/utils/dash_utils.py` & `qtc-0.0.4/qtc/utils/dash_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/qtc/utils/datetime_utils.py` & `qtc-0.0.4/qtc/utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/qtc/utils/db_utils.py` & `qtc-0.0.4/qtc/utils/db_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import pandas as pd
 import sqlalchemy
 from urllib.parse import quote
 from typing import Optional, Dict
 from qtc.consts.enums import DBType
 import qtc.env_config as ecfg
 import qtc.utils.misc_utils as mu
+import qtc.utils.cipher_utils as cu
 from qtc.ext.logging import set_logger
 logger = set_logger()
 
 import warnings
 warnings.filterwarnings('ignore')
 
 
@@ -590,8 +591,28 @@
             index_elements=sql_table.primary_key.columns,  # index elements are primary keys of a table
             set_=update_stmt  # the SET part of an INSERT statement
         )
 
         # execute upsert statement
         conn.execute(upsert_stmt)
 
-    return method
+    return method
+
+
+def get_os_env_conn(**db_config):
+    db_type = db_config.get('db_type', 'POSTGRES')
+    host = db_config.get('host', os.getenv('DB_HOST', None))
+    port = db_config.get('port', os.getenv('DB_PORT', None))
+    user = db_config.get('user', os.getenv('DB_USER', None))
+    password = db_config.get('password', os.getenv('DB_PASSWORD', None))
+    database = db_config.get('database', os.getenv('DB_DATABASE', None))
+
+    conn = _get_engine(
+        db_type=db_type,
+        host=host,
+        port=port,
+        user=user,
+        password=cu.from_salted(secret_str=password),
+        database=database
+    ).connect()
+
+    return conn
```

### Comparing `qtc-0.0.3/qtc/utils/email_utils.py` & `qtc-0.0.4/qtc/utils/email_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/qtc/utils/endpoint_utils.py` & `qtc-0.0.4/qtc/utils/endpoint_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/qtc/utils/file_system_utils.py` & `qtc-0.0.4/qtc/utils/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/qtc/utils/html_utils.py` & `qtc-0.0.4/qtc/utils/html_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/qtc/utils/misc_utils.py` & `qtc-0.0.4/qtc/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/qtc/utils/notebook_utils.py` & `qtc-0.0.4/qtc/utils/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/qtc.egg-info/SOURCES.txt` & `qtc-0.0.4/qtc.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,20 @@
 qtc/app_configs/bq/__init__.py
 qtc/app_configs/bq/constants.py
 qtc/app_configs/bq/params.py
 qtc/app_configs/bq_sim/__init__.py
 qtc/app_configs/bq_sim/params.py
 qtc/calendar/__init__.py
 qtc/calendar/calendar.py
+qtc/calendar/cn_stock_calendar.py
 qtc/consts/__init__.py
 qtc/consts/enums.py
+qtc/data/__init__.py
+qtc/data/dal/__init__.py
+qtc/data/dal/calendar.py
 qtc/ext/__init__.py
 qtc/ext/configurable.py
 qtc/ext/enum.py
 qtc/ext/inspect.py
 qtc/ext/logging.py
 qtc/ext/multiprocessing.py
 qtc/ext/unittest.py
```

### Comparing `qtc-0.0.3/setup.py` & `qtc-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/tests/ext/test_enum.py` & `qtc-0.0.4/tests/ext/test_enum.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/tests/ext/test_inspect.py` & `qtc-0.0.4/tests/ext/test_inspect.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/tests/file/test_file_cache.py` & `qtc-0.0.4/tests/file/test_file_cache.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/tests/file/test_file_manager.py` & `qtc-0.0.4/tests/file/test_file_manager.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/tests/file/test_file_serialization.py` & `qtc-0.0.4/tests/file/test_file_serialization.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/tests/utils/test_cipher_utils.py` & `qtc-0.0.4/tests/utils/test_cipher_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/tests/utils/test_datetime_utils.py` & `qtc-0.0.4/tests/utils/test_datetime_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/tests/utils/test_db_utils.py` & `qtc-0.0.4/tests/utils/test_db_utils.py`

 * *Files identical despite different names*

### Comparing `qtc-0.0.3/tests/utils/test_misc_utils.py` & `qtc-0.0.4/tests/utils/test_misc_utils.py`

 * *Files identical despite different names*

