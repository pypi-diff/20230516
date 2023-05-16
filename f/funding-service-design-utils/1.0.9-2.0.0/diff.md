# Comparing `tmp/funding-service-design-utils-1.0.9.tar.gz` & `tmp/funding-service-design-utils-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funding-service-design-utils-1.0.9.tar", last modified: Thu Nov  3 16:17:40 2022, max compression
+gzip compressed data, was "funding-service-design-utils-2.0.0.tar", last modified: Tue May 16 08:54:02 2023, max compression
```

## Comparing `funding-service-design-utils-1.0.9.tar` & `funding-service-design-utils-2.0.0.tar`

### file list

```diff
@@ -1,52 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.093984 funding-service-design-utils-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    11924 2022-11-03 16:17:40.093984 funding-service-design-utils-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10093 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.089984 funding-service-design-utils-1.0.9/fsd_utils/
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.089984 funding-service-design-utils-1.0.9/fsd_utils/authentication/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/authentication/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3275 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/authentication/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/authentication/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.089984 funding-service-design-utils-1.0.9/fsd_utils/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9814 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/config/commonconfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/config/configclass.py
--rw-r--r--   0 runner    (1001) docker     (121)     1241 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/config/notify_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.089984 funding-service-design-utils-1.0.9/fsd_utils/gunicorn/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/gunicorn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.089984 funding-service-design-utils-1.0.9/fsd_utils/gunicorn/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/gunicorn/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7757 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/gunicorn/config/devtest.py
--rw-r--r--   0 runner    (1001) docker     (121)     7084 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/gunicorn/config/local.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.093984 funding-service-design-utils-1.0.9/fsd_utils/healthchecks/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/healthchecks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/healthchecks/checkers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/healthchecks/healthcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.093984 funding-service-design-utils-1.0.9/fsd_utils/locale_selector/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/locale_selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/locale_selector/get_lang.py
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/locale_selector/set_lang.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.093984 funding-service-design-utils-1.0.9/fsd_utils/logging/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11916 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.093984 funding-service-design-utils-1.0.9/fsd_utils/sentry/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/sentry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/fsd_utils/sentry/init_sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.093984 funding-service-design-utils-1.0.9/funding_service_design_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11924 2022-11-03 16:17:40.000000 funding-service-design-utils-1.0.9/funding_service_design_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1212 2022-11-03 16:17:40.000000 funding-service-design-utils-1.0.9/funding_service_design_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-03 16:17:40.000000 funding-service-design-utils-1.0.9/funding_service_design_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-11-03 16:17:40.000000 funding-service-design-utils-1.0.9/funding_service_design_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-03 16:17:40.000000 funding-service-design-utils-1.0.9/funding_service_design_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-03 16:17:40.093984 funding-service-design-utils-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:40.093984 funding-service-design-utils-1.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2465 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/tests/test_checkers.py
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/tests/test_get_lang.py
--rw-r--r--   0 runner    (1001) docker     (121)     3043 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/tests/test_healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-11-03 16:17:20.000000 funding-service-design-utils-1.0.9/tests/test_set_lang.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.321351 funding-service-design-utils-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-05-16 08:54:02.321351 funding-service-design-utils-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13906 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.313351 funding-service-design-utils-2.0.0/fsd_test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_test_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.313351 funding-service-design-utils-2.0.0/fsd_test_utils/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_test_utils/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_test_utils/fixtures/db_fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.313351 funding-service-design-utils-2.0.0/fsd_test_utils/test_config/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_test_utils/test_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_test_utils/test_config/useful_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.313351 funding-service-design-utils-2.0.0/fsd_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.317351 funding-service-design-utils-2.0.0/fsd_utils/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/authentication/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/authentication/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/authentication/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/authentication/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.317351 funding-service-design-utils-2.0.0/fsd_utils/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/config/commonconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/config/configclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/config/notify_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.317351 funding-service-design-utils-2.0.0/fsd_utils/gunicorn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/gunicorn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.317351 funding-service-design-utils-2.0.0/fsd_utils/gunicorn/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/gunicorn/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/gunicorn/config/devtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/gunicorn/config/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.317351 funding-service-design-utils-2.0.0/fsd_utils/healthchecks/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/healthchecks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/healthchecks/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/healthchecks/healthcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.317351 funding-service-design-utils-2.0.0/fsd_utils/locale_selector/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/locale_selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/locale_selector/get_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/locale_selector/set_lang.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.317351 funding-service-design-utils-2.0.0/fsd_utils/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.317351 funding-service-design-utils-2.0.0/fsd_utils/sentry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/sentry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/sentry/init_sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.317351 funding-service-design-utils-2.0.0/fsd_utils/simple_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/simple_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/simple_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/simple_utils/date_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.317351 funding-service-design-utils-2.0.0/fsd_utils/toggles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/toggles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/toggles/toggles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.317351 funding-service-design-utils-2.0.0/funding_service_design_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-05-16 08:54:02.000000 funding-service-design-utils-2.0.0/funding_service_design_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 08:54:02.000000 funding-service-design-utils-2.0.0/funding_service_design_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:54:02.000000 funding-service-design-utils-2.0.0/funding_service_design_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-16 08:54:02.000000 funding-service-design-utils-2.0.0/funding_service_design_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-16 08:54:02.000000 funding-service-design-utils-2.0.0/funding_service_design_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 08:54:02.321351 funding-service-design-utils-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.321351 funding-service-design-utils-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/tests/test_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/tests/test_get_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/tests/test_healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/tests/test_set_lang.py
```

### Comparing `funding-service-design-utils-1.0.9/LICENSE` & `funding-service-design-utils-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.9/PKG-INFO` & `funding-service-design-utils-2.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funding-service-design-utils
-Version: 1.0.9
+Version: 2.0.0
 Summary: Utilities used by the DLUHC Funding Service Design Team
 Author-email: DLUHC <FundingServiceDesignTeam@levellingup.gov.uk>
 License: MIT License
         
         Copyright (c) 2022 Crown Copyright (Department for Levelling Up, Housing and Communities)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -82,14 +82,16 @@
 
 ## Local changes
 When working and testing locally, you can also install the `fsd_utils` package from your local filesystem:
 
     pip uninstall -y funding-service-design-utils
     pip install /path/to/your/working/directory/funding-service-design/utils
 
+Note: When testing locally using the docker runner, docker might use the cached version of fsd_utils. to avoid this and pick up your intended changes, run `docker compose build <service_name> --no-cache` first before running `docker compose up`.
+
 # Utilities
 
 ## The configclass
 Currently the configclass allows for pretty print debugging of config keys and the class from which they are created. This allows devs to quickly diagnoise problems arrising from incorrectly set config. To activate this functionality, one must decorate each config class with the `@configclass` decorator.
 
 ## Common Config
 This defines config values that are common across different services, eg. url patterns. Usage example:
@@ -99,14 +101,15 @@
 
 @configclass
 class DefaultConfig:
     SECRET_KEY = CommonConfig.SECRET_KEY
 
 ```
 
+
 ## Gunicorn
 The gunicorn utility allows consistent configuration of gunicorn across microservices.
 
 To use it,
 First - add run/gunicorn directory in your application with config scripts that import the appropriate config from this util's choice of config files eg.
 
     # in run/gunicorn/local.py
@@ -264,7 +267,79 @@
 * Before the flask app is created initialise Sentry using
 ```
 from fsd_utils import init_sentry
 
 init_sentry()
 ```
 * Set the `SENTRY_DSN` environment variable on the app
+
+## Simple Utils
+Folder to hold miscellaneous simple utilities.
+
+### date_utils
+Date comparison functions that accept an ISO Format string, for use in the frontend determining display logic based on dates.
+
+## Fixtures
+Contains shared fixtures that can be used for unit tests in other repos. To include a fixture from `fsd_utils` in your project, add the following to your `conftest.py`:
+
+    pytest_plugins = ["fsd_test_utils.fixtures.db_fixtures"]
+
+Where the part inside `[]` is the paths to the python files you want to load as fixtures.
+
+### DB_Fixtures
+
+Individual fixtures are explained below, but this is the general expected usage. In the `conftest.py` of your repo, define a fixture that will seed the database with the test data you require and make those records avaialble to tests. That fixture should request `clear_test_data` and `enable_preserve_test_data` to prevent test pollution and ensure a suitable database is available for tests. The tests themselves should only update data that is inserted by that fixture. Examples:
+
+1. Basic Usage
+
+    In conftest.py
+
+        @pytest.fixture(scope="function")
+        def create_test_data(clear_test_data, enable_preserve_test_data):
+            # Logic to insert some test data
+            created_data = [all_created_data]
+
+            yield created_data
+
+            # No teardown logic required as this is covered in clear_test_data
+
+    In your test file
+
+        def test_get_data(create_test_data):
+            id = create_test_data[0].id
+            record = get_record_using_api_under_test(id)
+            assert record.id == id
+
+1. If your tests need to directly manipulate the database, use the `_db` fixture:
+
+        def test_after_update(create_test_data, _db):
+            id = create_test_data[0].id
+            record = get_record(id)
+            record.name = "new name"
+
+            _db.session.add(record)
+            _db.session.commit()
+
+            # Do some further tests post update
+
+1. If you want to be able to inspect the database after running a test:
+
+        @pytest.mark.preserve_test_data(True)
+        def test_get_data(create_test_data):
+            id = create_test_data[0].id
+            record = get_record_using_api_under_test(id)
+            assert record.id == id
+
+    After the test runs, any created data will still be there for manual inspection. It will then be removed at the start of the next test run.
+
+#### clear_test_data
+This fixture is module scoped so at the end of each test file all data is removed from the database (providing `preserve_test_data` is not set - see below.) Helps to prevent test pollution.
+#### enable_preserve_test_data
+This fixture looks for the marker `pytest.mark.preserve_test_data(True)` and if found, test data is not cleared at the end of the test session, allowing you to manually inspect the database to aid debugging.
+
+**Note**: Not intended to be used as a default for tests as it can lead to test pollution, so only use to debug and then remove again.
+#### _db
+Provides direct access to the database for tests. Useful if your test needs to explicitly insert/update records to prepare test data.
+#### recreate_db
+This fixture reads the pytest cache to determine whether the DB can be reused for this test run and then the db is recreated accordingly. Updates the cache value to enable reuse of the DB for future test runs. This is session scoped so the DB is not recreated for each test in a run.
+
+This is requested by `clear_test_data` so you do not need to include it separately in your project if using that fixture.
```

### Comparing `funding-service-design-utils-1.0.9/fsd_utils/__init__.py` & `funding-service-design-utils-2.0.0/fsd_utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,28 @@
-from fsd_utils import authentication  # noqa
+from fsd_utils import authentication
 from fsd_utils import gunicorn  # noqa
 from fsd_utils import healthchecks
 from fsd_utils import logging  # noqa
+from fsd_utils import toggles
 from fsd_utils.config.commonconfig import CommonConfig  # noqa
 from fsd_utils.config.configclass import configclass  # noqa
 from fsd_utils.config.notify_constants import NotifyConstants  # noqa
 from fsd_utils.locale_selector.set_lang import LanguageSelector
+from fsd_utils.sentry.init_sentry import clear_sentry
 from fsd_utils.sentry.init_sentry import init_sentry
+from fsd_utils.simple_utils import date_utils  # noqa
+
 
 __all__ = [
     configclass,
     logging,
     gunicorn,
     authentication,
     CommonConfig,
     NotifyConstants,
     healthchecks,
     LanguageSelector,
     init_sentry,
+    clear_sentry,
+    date_utils,
+    toggles,
 ]
```

### Comparing `funding-service-design-utils-1.0.9/fsd_utils/authentication/decorators.py` & `funding-service-design-utils-2.0.0/fsd_utils/authentication/decorators.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,57 @@
 from functools import wraps
+from typing import List
 
 from flask import abort
 from flask import current_app
 from flask import g
 from flask import redirect
 from flask import request
 from fsd_utils.authentication.utils import validate_token_rs256
 from jwt import ExpiredSignatureError
 from jwt import PyJWTError
 
 from .config import config_var_auth_host
 from .config import config_var_user_token_cookie_name
 from .config import signout_route
+from .config import user_route
+from .models import User
 
 
 def _failed_redirect():
     authenticator_host = current_app.config[config_var_auth_host]
 
     return abort(redirect(authenticator_host + signout_route))
 
 
+def _failed_roles_redirect(roles_required: List[str]):
+    authenticator_host = current_app.config[config_var_auth_host]
+
+    return abort(
+        redirect(
+            authenticator_host
+            + user_route
+            + "?roles_required="
+            + "|".join(roles_required)
+        )
+    )
+
+
 def _check_access_token(auto_redirect=True):
     """
     Check the expected auth cookie for a
     valid JWT token.
     :param auto_redirect: (bool) redirect on failed authentication if True
     :return:
         - If a valid JWT token is found then return token claims
         - If no valid token is found:
             -- If auto_redirect is True then issue a _failed_redirect()
             -- If auto_redirect is False then return False
     """
-    user_token_cookie_name = current_app.config[
-        config_var_user_token_cookie_name
-    ]
+    user_token_cookie_name = current_app.config[config_var_user_token_cookie_name]
 
     login_cookie = request.cookies.get(user_token_cookie_name)
     if not login_cookie:
         if auto_redirect:
             _failed_redirect()
         return False
 
@@ -45,57 +59,81 @@
         return validate_token_rs256(login_cookie)
     except (PyJWTError, ExpiredSignatureError):
         if auto_redirect:
             _failed_redirect()
         return False
 
 
-def login_required(f):
+def login_required(f=None, roles_required: List[str] = None):
     """
-    Execute function if request contains valid JWT
-    and pass account auth params to route as attributes
-    on the flask request global 'g' object:
-        - g.account_id: (str) users account id
-        - g.is_authenticated: (bool) authentication status
-        - g.logout_url: (str) the service sign-out url
-    If no valid auth JWT found then redirect to
-    service config invalid login route
+     Execute function if request contains valid JWT
+     and pass account auth params to route as attributes
+     on the flask request global 'g' object:
+         - g.account_id: (str) users account id
+         - g.is_authenticated: (bool) authentication status
+         - g.user - this holds a User object and associated attributes
+         - g.logout_url: (str) the service sign-out url
+     If no valid auth JWT found then redirect to
+     service config invalid login route
+    :param f:
+    :param roles_required: (List(str), optional) a list of the
+            roles required to access the decorated route
+    :return:
     """
+    if f is None:
+        return lambda f: login_required(f=f, roles_required=roles_required)
 
     @wraps(f)
-    def decorated(*args, **kwargs):
-        token_payload = _check_access_token()
+    def _wrapper(*args, **kwargs):
+        if (
+            current_app.config.get("FLASK_ENV") == "development"
+            and current_app.config.get("DEBUG_USER_ROLE")
+            and current_app.config.get("DEBUG_USER")
+        ):
+            g.account_id = "dev-account-id"
+            g.user = User(**current_app.config.get("DEBUG_USER"))
+        else:
+            token_payload = _check_access_token()
+            g.account_id = token_payload.get("accountId")
+            g.user = User.set_with_token(token_payload)
+
         authenticator_host = current_app.config[config_var_auth_host]
-        g.account_id = token_payload.get("accountId")
-        g.is_authenticated = True
         g.logout_url = authenticator_host + signout_route
+        g.is_authenticated = True
+        if roles_required:
+            if not any(
+                role_required in g.user.roles for role_required in roles_required
+            ):
+                _failed_roles_redirect(roles_required)
         return f(*args, **kwargs)
 
-    return decorated
+    return _wrapper
 
 
 def login_requested(f):
     """
     If request contains valid JWT
     then pass account auth params to route as attributes
     on the flask request global 'g' object:
         - g.account_id: (str) users account id
         - g.is_authenticated: (bool) authentication status
+        - g.user - this holds a User object and associated attributes
         - g.logout_url: (str) the service sign-out url
     If no valid auth JWT found then update the g.is_authenticated
     variable to False and the g.account_id to None
     """
 
     @wraps(f)
     def decorated(*args, **kwargs):
         token_payload = _check_access_token(auto_redirect=False)
         authenticator_host = current_app.config[config_var_auth_host]
         g.logout_url = authenticator_host + signout_route
         if token_payload and isinstance(token_payload, dict):
             g.account_id = token_payload.get("accountId")
+            g.user = User.set_with_token(token_payload)
             g.is_authenticated = True
         else:
             g.account_id = None
             g.is_authenticated = False
         return f(*args, **kwargs)
 
     return decorated
```

### Comparing `funding-service-design-utils-1.0.9/fsd_utils/config/configclass.py` & `funding-service-design-utils-2.0.0/fsd_utils/config/configclass.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.9/fsd_utils/config/notify_constants.py` & `funding-service-design-utils-2.0.0/fsd_utils/config/notify_constants.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.9/fsd_utils/gunicorn/config/devtest.py` & `funding-service-design-utils-2.0.0/fsd_utils/gunicorn/config/devtest.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,17 +149,17 @@
 #
 #       A string of "debug", "info", "warning", "error", "critical"
 #
 
 
 class CustomLogger(Logger):
     def now(self):
-        return datetime.datetime.now(
-            tz=pytz.timezone("Europe/London")
-        ).strftime("%d-%b-%y %H:%M:%S")
+        return datetime.datetime.now(tz=pytz.timezone("Europe/London")).strftime(
+            "%d-%b-%y %H:%M:%S"
+        )
 
 
 logger_class = CustomLogger
 
 errorlog = "-"
 loglevel = "info"
 accesslog = "-"
@@ -222,21 +222,17 @@
     import threading
     import sys
     import traceback
 
     id2name = {th.ident: th.name for th in threading.enumerate()}
     code = []
     for threadId, stack in sys._current_frames().items():
-        code.append(
-            "\n# Thread: %s(%d)" % (id2name.get(threadId, ""), threadId)
-        )
+        code.append("\n# Thread: %s(%d)" % (id2name.get(threadId, ""), threadId))
         for filename, lineno, name, line in traceback.extract_stack(stack):
-            code.append(
-                'File: "%s", line %d, in %s' % (filename, lineno, name)
-            )
+            code.append('File: "%s", line %d, in %s' % (filename, lineno, name))
             if line:
                 code.append("  %s" % (line.strip()))
     worker.log.debug("\n".join(code))
 
 
 def worker_abort(worker):
     worker.log.info("worker received SIGABRT signal")
@@ -252,10 +248,8 @@
         if not self.path_filter.match(req_path):
             return True  # log this entry
         # ... additional conditions can be added here ...
         return False  # do not log this entry
 
 
 def on_starting(server):
-    server.log.access_log.addFilter(
-        RequestPathFilter(path_re=r"^/healthcheck$")
-    )
+    server.log.access_log.addFilter(RequestPathFilter(path_re=r"^/healthcheck$"))
```

### Comparing `funding-service-design-utils-1.0.9/fsd_utils/gunicorn/config/local.py` & `funding-service-design-utils-2.0.0/fsd_utils/gunicorn/config/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,17 +147,17 @@
 #
 #       A string of "debug", "info", "warning", "error", "critical"
 #
 
 
 class CustomLogger(Logger):
     def now(self):
-        return datetime.datetime.now(
-            tz=pytz.timezone("Europe/London")
-        ).strftime("%d-%b-%y %H:%M:%S")
+        return datetime.datetime.now(tz=pytz.timezone("Europe/London")).strftime(
+            "%d-%b-%y %H:%M:%S"
+        )
 
 
 logger_class = CustomLogger
 
 errorlog = "-"
 loglevel = "info"
 accesslog = "-"
@@ -223,21 +223,17 @@
     import threading
     import sys
     import traceback
 
     id2name = {th.ident: th.name for th in threading.enumerate()}
     code = []
     for threadId, stack in sys._current_frames().items():
-        code.append(
-            "\n# Thread: %s(%d)" % (id2name.get(threadId, ""), threadId)
-        )
+        code.append("\n# Thread: %s(%d)" % (id2name.get(threadId, ""), threadId))
         for filename, lineno, name, line in traceback.extract_stack(stack):
-            code.append(
-                'File: "%s", line %d, in %s' % (filename, lineno, name)
-            )
+            code.append('File: "%s", line %d, in %s' % (filename, lineno, name))
             if line:
                 code.append("  %s" % (line.strip()))
     worker.log.debug("\n".join(code))
 
 
 def worker_abort(worker):
     worker.log.info("worker received SIGABRT signal")
```

### Comparing `funding-service-design-utils-1.0.9/fsd_utils/healthchecks/checkers.py` & `funding-service-design-utils-2.0.0/fsd_utils/healthchecks/checkers.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-1.0.9/fsd_utils/healthchecks/healthcheck.py` & `funding-service-design-utils-2.0.0/fsd_utils/healthchecks/healthcheck.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,33 @@
+import os
+
 from flask import current_app
 
 
 class Healthcheck(object):
     def __init__(self, app):
         self.flask_app = app
-        self.flask_app.add_url_rule(
-            "/healthcheck", view_func=self.healthcheck_view
-        )
+        self.flask_app.add_url_rule("/healthcheck", view_func=self.healthcheck_view)
         self.checkers = []
 
     def healthcheck_view(self):
         responseCode = 200
         response = {"checks": []}
+        version = os.getenv("GITHUB_SHA")
+        if version:
+            response["version"] = version
         for checker in self.checkers:
             try:
                 result = checker.check()
-                current_app.logger.debug(
-                    f"Check {checker.name} returned {result}"
-                )
+                current_app.logger.debug(f"Check {checker.name} returned {result}")
                 response["checks"].append({checker.name: result[1]})
                 if result[0] is False:
                     responseCode = 500
             except Exception:
-                response["checks"].append(
-                    {checker.name: "Failed - check logs"}
-                )
+                response["checks"].append({checker.name: "Failed - check logs"})
                 current_app.logger.exception(
                     f"Check {checker.name} failed with an exception"
                 )
                 responseCode = 500
         return response, responseCode
 
     def add_check(self, checker):
```

### Comparing `funding-service-design-utils-1.0.9/fsd_utils/locale_selector/set_lang.py` & `funding-service-design-utils-2.0.0/fsd_utils/locale_selector/set_lang.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,15 @@
         def get_cookie_domain(cookie_domain):
             if not cookie_domain:
                 return None
             else:
                 return cookie_domain
 
         response = make_response(
-            redirect(
-                request.referrer or request.args.get("return_url") or "/", 302
-            )
+            redirect(request.referrer or request.args.get("return_url") or "/", 302)
         )
         response.set_cookie(
             CommonConfig.FSD_LANG_COOKIE_NAME,
             locale,
             domain=get_cookie_domain(current_app.config["COOKIE_DOMAIN"]),
             max_age=86400 * 30,  # 30 days
         )
```

### Comparing `funding-service-design-utils-1.0.9/fsd_utils/logging/logging.py` & `funding-service-design-utils-2.0.0/fsd_utils/logging/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,34 +70,33 @@
             logging.DEBUG,
             "Received request {method} {url}",
             extra=_common_request_extra_log_context(),
         )
 
     @app.after_request
     def after_request(response):
-        current_app.logger.log(
-            logging.ERROR
-            if response.status_code // 100 == 5
-            else logging.INFO,
-            "{method} {url} {status}",
-            extra={
-                "status": response.status_code,
-                "duration_real": (
-                    (time.perf_counter() - request.before_request_real_time)
-                    if hasattr(request, "before_request_real_time")
-                    else None
-                ),
-                "duration_process": (
-                    (time.process_time() - request.before_request_process_time)
-                    if hasattr(request, "before_request_process_time")
-                    else None
-                ),
-                **_common_request_extra_log_context(),
-            },
-        )
+        if request.path != "/healthcheck":
+            current_app.logger.log(
+                logging.INFO,
+                "{method} {url} {status}",
+                extra={
+                    "status": response.status_code,
+                    "duration_real": (
+                        (time.perf_counter() - request.before_request_real_time)
+                        if hasattr(request, "before_request_real_time")
+                        else None
+                    ),
+                    "duration_process": (
+                        (time.process_time() - request.before_request_process_time)
+                        if hasattr(request, "before_request_process_time")
+                        else None
+                    ),
+                    **_common_request_extra_log_context(),
+                },
+            )
         return response
 
     logging.getLogger().addHandler(logging.NullHandler())
     # Werkzeug logging
     werkzeug_logger = logging.getLogger("werkzeug")
     # Disable default werkzeug logging
     werkzeug_logger.disabled = True
@@ -134,17 +133,15 @@
     if os.environ.get("CF_INSTANCE_INDEX"):
         handler.addFilter(AppInstanceFilter())
 
     return handler
 
 
 def get_json_log_format():
-    return LOG_FORMAT + "".join(
-        f" %({key})s" for key in LOG_FORMAT_EXTRA_JSON_KEYS
-    )
+    return LOG_FORMAT + "".join(f" %({key})s" for key in LOG_FORMAT_EXTRA_JSON_KEYS)
 
 
 class AppInstanceFilter(logging.Filter):
     def __init__(self):
         self.instance_index = os.environ["CF_INSTANCE_INDEX"]
 
     def filter(self, record):
@@ -306,17 +303,15 @@
 
     def formatTime(self, record, datefmt: str | None = ...) -> str:
         ct = self.converter(record.created)
         if datefmt:
             s = time.strftime(datefmt, ct)
         else:
             s = (
-                datetime.datetime.fromtimestamp(
-                    record.created, datetime.timezone.utc
-                )
+                datetime.datetime.fromtimestamp(record.created, datetime.timezone.utc)
                 .astimezone()
                 .isoformat(sep=" ", timespec="milliseconds")
             )
         return s
 
     def process_log_record(self, log_record):
         for key, newkey in (
```

### Comparing `funding-service-design-utils-1.0.9/fsd_utils/sentry/init_sentry.py` & `funding-service-design-utils-2.0.0/fsd_utils/sentry/init_sentry.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 import sentry_sdk
 from fsd_utils import CommonConfig
 from sentry_sdk.integrations.flask import FlaskIntegration
 
 
 def _traces_sampler(sampling_context):
     wsgi_environ = sampling_context.get("wsgi_environ")
-    if wsgi_environ and wsgi_environ.get("PATH_INFO") == "/healthcheck":
+    if wsgi_environ and (
+        wsgi_environ.get("PATH_INFO") == "/healthcheck"
+        or wsgi_environ.get("HTTP_USER_AGENT" == "locust performance tests")
+    ):
         # Drop this transaction, by setting its sample rate to 0%
         return 0
     else:
         # Default sample rate for all others (replaces traces_sample_rate)
         return 0.1
 
 
@@ -21,7 +24,12 @@
             environment=CommonConfig.FLASK_ENV,
             integrations=[
                 FlaskIntegration(),
             ],
             traces_sampler=_traces_sampler,
             release=getenv("GITHUB_SHA"),
         )
+
+
+def clear_sentry():
+    if getenv("SENTRY_DSN"):
+        sentry_sdk.set_user(None)
```

### Comparing `funding-service-design-utils-1.0.9/funding_service_design_utils.egg-info/PKG-INFO` & `funding-service-design-utils-2.0.0/funding_service_design_utils.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funding-service-design-utils
-Version: 1.0.9
+Version: 2.0.0
 Summary: Utilities used by the DLUHC Funding Service Design Team
 Author-email: DLUHC <FundingServiceDesignTeam@levellingup.gov.uk>
 License: MIT License
         
         Copyright (c) 2022 Crown Copyright (Department for Levelling Up, Housing and Communities)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -82,14 +82,16 @@
 
 ## Local changes
 When working and testing locally, you can also install the `fsd_utils` package from your local filesystem:
 
     pip uninstall -y funding-service-design-utils
     pip install /path/to/your/working/directory/funding-service-design/utils
 
+Note: When testing locally using the docker runner, docker might use the cached version of fsd_utils. to avoid this and pick up your intended changes, run `docker compose build <service_name> --no-cache` first before running `docker compose up`.
+
 # Utilities
 
 ## The configclass
 Currently the configclass allows for pretty print debugging of config keys and the class from which they are created. This allows devs to quickly diagnoise problems arrising from incorrectly set config. To activate this functionality, one must decorate each config class with the `@configclass` decorator.
 
 ## Common Config
 This defines config values that are common across different services, eg. url patterns. Usage example:
@@ -99,14 +101,15 @@
 
 @configclass
 class DefaultConfig:
     SECRET_KEY = CommonConfig.SECRET_KEY
 
 ```
 
+
 ## Gunicorn
 The gunicorn utility allows consistent configuration of gunicorn across microservices.
 
 To use it,
 First - add run/gunicorn directory in your application with config scripts that import the appropriate config from this util's choice of config files eg.
 
     # in run/gunicorn/local.py
@@ -264,7 +267,79 @@
 * Before the flask app is created initialise Sentry using
 ```
 from fsd_utils import init_sentry
 
 init_sentry()
 ```
 * Set the `SENTRY_DSN` environment variable on the app
+
+## Simple Utils
+Folder to hold miscellaneous simple utilities.
+
+### date_utils
+Date comparison functions that accept an ISO Format string, for use in the frontend determining display logic based on dates.
+
+## Fixtures
+Contains shared fixtures that can be used for unit tests in other repos. To include a fixture from `fsd_utils` in your project, add the following to your `conftest.py`:
+
+    pytest_plugins = ["fsd_test_utils.fixtures.db_fixtures"]
+
+Where the part inside `[]` is the paths to the python files you want to load as fixtures.
+
+### DB_Fixtures
+
+Individual fixtures are explained below, but this is the general expected usage. In the `conftest.py` of your repo, define a fixture that will seed the database with the test data you require and make those records avaialble to tests. That fixture should request `clear_test_data` and `enable_preserve_test_data` to prevent test pollution and ensure a suitable database is available for tests. The tests themselves should only update data that is inserted by that fixture. Examples:
+
+1. Basic Usage
+
+    In conftest.py
+
+        @pytest.fixture(scope="function")
+        def create_test_data(clear_test_data, enable_preserve_test_data):
+            # Logic to insert some test data
+            created_data = [all_created_data]
+
+            yield created_data
+
+            # No teardown logic required as this is covered in clear_test_data
+
+    In your test file
+
+        def test_get_data(create_test_data):
+            id = create_test_data[0].id
+            record = get_record_using_api_under_test(id)
+            assert record.id == id
+
+1. If your tests need to directly manipulate the database, use the `_db` fixture:
+
+        def test_after_update(create_test_data, _db):
+            id = create_test_data[0].id
+            record = get_record(id)
+            record.name = "new name"
+
+            _db.session.add(record)
+            _db.session.commit()
+
+            # Do some further tests post update
+
+1. If you want to be able to inspect the database after running a test:
+
+        @pytest.mark.preserve_test_data(True)
+        def test_get_data(create_test_data):
+            id = create_test_data[0].id
+            record = get_record_using_api_under_test(id)
+            assert record.id == id
+
+    After the test runs, any created data will still be there for manual inspection. It will then be removed at the start of the next test run.
+
+#### clear_test_data
+This fixture is module scoped so at the end of each test file all data is removed from the database (providing `preserve_test_data` is not set - see below.) Helps to prevent test pollution.
+#### enable_preserve_test_data
+This fixture looks for the marker `pytest.mark.preserve_test_data(True)` and if found, test data is not cleared at the end of the test session, allowing you to manually inspect the database to aid debugging.
+
+**Note**: Not intended to be used as a default for tests as it can lead to test pollution, so only use to debug and then remove again.
+#### _db
+Provides direct access to the database for tests. Useful if your test needs to explicitly insert/update records to prepare test data.
+#### recreate_db
+This fixture reads the pytest cache to determine whether the DB can be reused for this test run and then the db is recreated accordingly. Updates the cache value to enable reuse of the DB for future test runs. This is session scoped so the DB is not recreated for each test in a run.
+
+This is requested by `clear_test_data` so you do not need to include it separately in your project if using that fixture.
```

### Comparing `funding-service-design-utils-1.0.9/funding_service_design_utils.egg-info/SOURCES.txt` & `funding-service-design-utils-2.0.0/funding_service_design_utils.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
+fsd_test_utils/__init__.py
+fsd_test_utils/fixtures/__init__.py
+fsd_test_utils/fixtures/db_fixtures.py
+fsd_test_utils/test_config/__init__.py
+fsd_test_utils/test_config/useful_config.py
 fsd_utils/__init__.py
 fsd_utils/authentication/__init__.py
 fsd_utils/authentication/config.py
 fsd_utils/authentication/decorators.py
+fsd_utils/authentication/models.py
 fsd_utils/authentication/utils.py
 fsd_utils/config/__init__.py
 fsd_utils/config/commonconfig.py
 fsd_utils/config/configclass.py
 fsd_utils/config/notify_constants.py
 fsd_utils/gunicorn/__init__.py
 fsd_utils/gunicorn/config/__init__.py
@@ -21,18 +27,25 @@
 fsd_utils/locale_selector/__init__.py
 fsd_utils/locale_selector/get_lang.py
 fsd_utils/locale_selector/set_lang.py
 fsd_utils/logging/__init__.py
 fsd_utils/logging/logging.py
 fsd_utils/sentry/__init__.py
 fsd_utils/sentry/init_sentry.py
+fsd_utils/simple_utils/__init__.py
+fsd_utils/simple_utils/data_utils.py
+fsd_utils/simple_utils/date_utils.py
+fsd_utils/toggles/__init__.py
+fsd_utils/toggles/toggles.py
 funding_service_design_utils.egg-info/PKG-INFO
 funding_service_design_utils.egg-info/SOURCES.txt
 funding_service_design_utils.egg-info/dependency_links.txt
 funding_service_design_utils.egg-info/requires.txt
 funding_service_design_utils.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
+tests/test_authentication.py
 tests/test_checkers.py
+tests/test_data_utils.py
 tests/test_get_lang.py
 tests/test_healthcheck.py
 tests/test_set_lang.py
```

### Comparing `funding-service-design-utils-1.0.9/pyproject.toml` & `funding-service-design-utils-2.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "funding-service-design-utils"
-version = "1.0.9"
+version = "2.0.0"
 authors = [
   { name="DLUHC", email="FundingServiceDesignTeam@levellingup.gov.uk" },
 ]
 description = "Utilities used by the DLUHC Funding Service Design Team"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10,<4.0"
@@ -24,12 +24,18 @@
     "python-dotenv>=0.20.0,<0.21.0",
     "rich>=12.4.4,<13.0.0",
     "Flask>=2.1.1,<3.0.0",
     "python-json-logger>=2.0.2,<3.0.0",
     "gunicorn>=20.1.0,<21.0.0",
     "pytz>=2022.1",
     "PyJWT[crypto]>=2.4.0",
-    "sentry-sdk[flask]>=1.9.9,<2.0.0"
+    "sentry-sdk[flask]>=1.9.9,<2.0.0",
+    "requests",
+    "flipper-client>=1.3.1",
+    "flask-redis==0.4.0",
+    "Flask-Migrate",
+    "Flask-SQLAlchemy>=3.0.3",
+    "sqlalchemy-utils>=0.38.3"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/communitiesuk/funding-service-design-utils"
```

### Comparing `funding-service-design-utils-1.0.9/tests/test_checkers.py` & `funding-service-design-utils-2.0.0/tests/test_checkers.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         mock_db.session = Mock()
         mock_db.session.execute.return_value = True
         db_checker = DbChecker(mock_db)
 
         result = db_checker.check()
         assert result[0] is True, "Unexpected check result"
         assert result[1] == "OK", "Unexpected check message"
-        mock_db.session.execute.assert_called_with("SELECT 1")
+        mock_db.session.execute.assert_called_once_with("SELECT 1")
 
     def testDbCheck_fail(self, flask_test_client):
         mock_db = Mock()
         mock_db.session = Mock()
         mock_db.session.execute.side_effect = ArgumentError
         db_checker = DbChecker(mock_db)
```

### Comparing `funding-service-design-utils-1.0.9/tests/test_get_lang.py` & `funding-service-design-utils-2.0.0/tests/test_get_lang.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,40 @@
+import pytest
 from fsd_utils.locale_selector.get_lang import get_lang
 
 
 class TestGetLang:
+    def test_get_lang_query_arg_valid(self, flask_test_client):
+        with flask_test_client.application.test_request_context("/?lang=cy"):
+            assert get_lang() == "cy"
+
+    def test_get_lang_query_arg_invalid(self, flask_test_client):
+        with flask_test_client.application.test_request_context("/?lang=fr"):
+            with pytest.raises(
+                ValueError,
+                match=(
+                    "Invalid language code. Supported codes" + " are 'cy' and 'en'."
+                ),
+            ):
+                get_lang()
+
     def test_get_lang_cookie_preference(self, flask_test_client):
         with flask_test_client.application.test_request_context(
             "/", headers={"Cookie": "language=cy"}
         ):
             assert get_lang() == "cy"
 
     def test_get_lang_accept_language_preference_en(self, flask_test_client):
         with flask_test_client.application.test_request_context(
             "/",
             headers={"Accept-Language": "en,en-GB;q=0.9,cy;q=0.8,en-US;q=0.7"},
         ):
             assert get_lang() == "en"
 
-    # TODO: restore this when Welsh language translation completed
-    # def test_get_lang_accept_language_preference_cy(self, flask_test_client):
-    #     with flask_test_client.application.test_request_context(
-    #         "/",
-    #         headers={"Accept-Language": "cy,en;q=0.9,en-GB;q=0.8,en-US;q=0.7"}, # noqa: E501
-    #     ):
-    #         assert get_lang() == "cy"
+    def test_get_lang_accept_language_preference_cy(self, flask_test_client):
+        with flask_test_client.application.test_request_context(
+            "/",
+            headers={
+                "Accept-Language": "cy,en;q=0.9,en-GB;q=0.8,en-US;q=0.7"
+            },  # noqa: E501
+        ):
+            assert get_lang() == "cy"
```

### Comparing `funding-service-design-utils-1.0.9/tests/test_set_lang.py` & `funding-service-design-utils-2.0.0/tests/test_set_lang.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,13 @@
 
 from fsd_utils.locale_selector.set_lang import LanguageSelector
 
 
 def test_set_lang(flask_test_client):
     mock_app = Mock()
     set_lang = LanguageSelector(mock_app)
-    mock_app.add_url_rule.assert_called_with(
-        "/language/<locale>", view_func=ANY
-    )
+    mock_app.add_url_rule.assert_called_with("/language/<locale>", view_func=ANY)
     with flask_test_client.application.test_request_context():
         response = set_lang.select_language("cy")
         response_cookie = response.headers.get("Set-Cookie")
         assert response_cookie is not None, "No cookie set for language"
         assert response_cookie.split(";")[0] == ("language" + "=cy")
```

