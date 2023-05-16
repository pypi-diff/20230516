# Comparing `tmp/funding-service-design-utils-2.0.0.tar.gz` & `tmp/funding-service-design-utils-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funding-service-design-utils-2.0.0.tar", last modified: Tue May 16 08:54:02 2023, max compression
+gzip compressed data, was "funding-service-design-utils-2.0.1.tar", last modified: Tue May 16 10:53:05 2023, max compression
```

## Comparing `funding-service-design-utils-2.0.0.tar` & `funding-service-design-utils-2.0.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.321351 funding-service-design-utils-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-05-16 08:54:02.321351 funding-service-design-utils-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13906 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.313351 funding-service-design-utils-2.0.0/fsd_test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_test_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.313351 funding-service-design-utils-2.0.0/fsd_test_utils/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_test_utils/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_test_utils/fixtures/db_fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.313351 funding-service-design-utils-2.0.0/fsd_test_utils/test_config/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_test_utils/test_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_test_utils/test_config/useful_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.313351 funding-service-design-utils-2.0.0/fsd_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.317351 funding-service-design-utils-2.0.0/fsd_utils/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/authentication/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/authentication/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/authentication/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/authentication/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.317351 funding-service-design-utils-2.0.0/fsd_utils/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/config/commonconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/config/configclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/config/notify_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.317351 funding-service-design-utils-2.0.0/fsd_utils/gunicorn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/gunicorn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.317351 funding-service-design-utils-2.0.0/fsd_utils/gunicorn/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/gunicorn/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/gunicorn/config/devtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/gunicorn/config/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.317351 funding-service-design-utils-2.0.0/fsd_utils/healthchecks/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/healthchecks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/healthchecks/checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/healthchecks/healthcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.317351 funding-service-design-utils-2.0.0/fsd_utils/locale_selector/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/locale_selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/locale_selector/get_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/locale_selector/set_lang.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.317351 funding-service-design-utils-2.0.0/fsd_utils/logging/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.317351 funding-service-design-utils-2.0.0/fsd_utils/sentry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/sentry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/sentry/init_sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.317351 funding-service-design-utils-2.0.0/fsd_utils/simple_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/simple_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/simple_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/simple_utils/date_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.317351 funding-service-design-utils-2.0.0/fsd_utils/toggles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/toggles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/fsd_utils/toggles/toggles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.317351 funding-service-design-utils-2.0.0/funding_service_design_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-05-16 08:54:02.000000 funding-service-design-utils-2.0.0/funding_service_design_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 08:54:02.000000 funding-service-design-utils-2.0.0/funding_service_design_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:54:02.000000 funding-service-design-utils-2.0.0/funding_service_design_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-16 08:54:02.000000 funding-service-design-utils-2.0.0/funding_service_design_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-16 08:54:02.000000 funding-service-design-utils-2.0.0/funding_service_design_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 08:54:02.321351 funding-service-design-utils-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:54:02.321351 funding-service-design-utils-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/tests/test_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/tests/test_get_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/tests/test_healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-16 08:53:47.000000 funding-service-design-utils-2.0.0/tests/test_set_lang.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.211896 funding-service-design-utils-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-05-16 10:53:05.211896 funding-service-design-utils-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13906 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.207896 funding-service-design-utils-2.0.1/fsd_test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_test_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.207896 funding-service-design-utils-2.0.1/fsd_test_utils/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_test_utils/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_test_utils/fixtures/db_fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.207896 funding-service-design-utils-2.0.1/fsd_test_utils/test_config/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_test_utils/test_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_test_utils/test_config/useful_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.207896 funding-service-design-utils-2.0.1/fsd_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.207896 funding-service-design-utils-2.0.1/fsd_utils/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/authentication/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/authentication/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/authentication/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/authentication/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.207896 funding-service-design-utils-2.0.1/fsd_utils/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/config/commonconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/config/configclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/config/notify_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.207896 funding-service-design-utils-2.0.1/fsd_utils/gunicorn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/gunicorn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.207896 funding-service-design-utils-2.0.1/fsd_utils/gunicorn/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/gunicorn/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/gunicorn/config/devtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/gunicorn/config/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.211896 funding-service-design-utils-2.0.1/fsd_utils/healthchecks/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/healthchecks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/healthchecks/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/healthchecks/healthcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.211896 funding-service-design-utils-2.0.1/fsd_utils/locale_selector/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/locale_selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/locale_selector/get_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/locale_selector/set_lang.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.211896 funding-service-design-utils-2.0.1/fsd_utils/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.211896 funding-service-design-utils-2.0.1/fsd_utils/sentry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/sentry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/sentry/init_sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.211896 funding-service-design-utils-2.0.1/fsd_utils/simple_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/simple_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/simple_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/simple_utils/date_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.211896 funding-service-design-utils-2.0.1/fsd_utils/toggles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/toggles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/fsd_utils/toggles/toggles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.211896 funding-service-design-utils-2.0.1/funding_service_design_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-05-16 10:53:05.000000 funding-service-design-utils-2.0.1/funding_service_design_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 10:53:05.000000 funding-service-design-utils-2.0.1/funding_service_design_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 10:53:05.000000 funding-service-design-utils-2.0.1/funding_service_design_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-16 10:53:05.000000 funding-service-design-utils-2.0.1/funding_service_design_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-16 10:53:05.000000 funding-service-design-utils-2.0.1/funding_service_design_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 10:53:05.211896 funding-service-design-utils-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:53:05.211896 funding-service-design-utils-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/tests/test_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/tests/test_get_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/tests/test_healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-16 10:52:54.000000 funding-service-design-utils-2.0.1/tests/test_set_lang.py
```

### Comparing `funding-service-design-utils-2.0.0/LICENSE` & `funding-service-design-utils-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/PKG-INFO` & `funding-service-design-utils-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funding-service-design-utils
-Version: 2.0.0
+Version: 2.0.1
 Summary: Utilities used by the DLUHC Funding Service Design Team
 Author-email: DLUHC <FundingServiceDesignTeam@levellingup.gov.uk>
 License: MIT License
         
         Copyright (c) 2022 Crown Copyright (Department for Levelling Up, Housing and Communities)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `funding-service-design-utils-2.0.0/README.md` & `funding-service-design-utils-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/fsd_test_utils/fixtures/db_fixtures.py` & `funding-service-design-utils-2.0.1/fsd_test_utils/fixtures/db_fixtures.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/fsd_utils/__init__.py` & `funding-service-design-utils-2.0.1/fsd_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/fsd_utils/authentication/config.py` & `funding-service-design-utils-2.0.1/fsd_utils/authentication/config.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/fsd_utils/authentication/decorators.py` & `funding-service-design-utils-2.0.1/fsd_utils/authentication/decorators.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/fsd_utils/authentication/models.py` & `funding-service-design-utils-2.0.1/fsd_utils/authentication/models.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/fsd_utils/authentication/utils.py` & `funding-service-design-utils-2.0.1/fsd_utils/authentication/utils.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/fsd_utils/config/commonconfig.py` & `funding-service-design-utils-2.0.1/fsd_utils/config/commonconfig.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/fsd_utils/config/configclass.py` & `funding-service-design-utils-2.0.1/fsd_utils/config/configclass.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/fsd_utils/config/notify_constants.py` & `funding-service-design-utils-2.0.1/fsd_utils/config/notify_constants.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/fsd_utils/gunicorn/config/devtest.py` & `funding-service-design-utils-2.0.1/fsd_utils/gunicorn/config/devtest.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/fsd_utils/gunicorn/config/local.py` & `funding-service-design-utils-2.0.1/fsd_utils/gunicorn/config/local.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/fsd_utils/healthchecks/checkers.py` & `funding-service-design-utils-2.0.1/fsd_utils/healthchecks/checkers.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,17 +22,18 @@
 class DbChecker(CheckerInterface):
     def __init__(self, db):
         self.db = db
         self.name = "check_db"
 
     def check(self):
         from sqlalchemy.exc import SQLAlchemyError
+        from sqlalchemy import text
 
         try:
-            self.db.session.execute("SELECT 1")
+            self.db.session.execute(text("SELECT 1"))
             return True, "OK"
         except SQLAlchemyError:
             current_app.logger.exception("DB Check failed")
             return False, "Fail"
 
 
 class RedisChecker(CheckerInterface):
```

### Comparing `funding-service-design-utils-2.0.0/fsd_utils/healthchecks/healthcheck.py` & `funding-service-design-utils-2.0.1/fsd_utils/healthchecks/healthcheck.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/fsd_utils/locale_selector/get_lang.py` & `funding-service-design-utils-2.0.1/fsd_utils/locale_selector/get_lang.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/fsd_utils/locale_selector/set_lang.py` & `funding-service-design-utils-2.0.1/fsd_utils/locale_selector/set_lang.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/fsd_utils/logging/logging.py` & `funding-service-design-utils-2.0.1/fsd_utils/logging/logging.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/fsd_utils/sentry/init_sentry.py` & `funding-service-design-utils-2.0.1/fsd_utils/sentry/init_sentry.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/fsd_utils/toggles/toggles.py` & `funding-service-design-utils-2.0.1/fsd_utils/toggles/toggles.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/funding_service_design_utils.egg-info/PKG-INFO` & `funding-service-design-utils-2.0.1/funding_service_design_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funding-service-design-utils
-Version: 2.0.0
+Version: 2.0.1
 Summary: Utilities used by the DLUHC Funding Service Design Team
 Author-email: DLUHC <FundingServiceDesignTeam@levellingup.gov.uk>
 License: MIT License
         
         Copyright (c) 2022 Crown Copyright (Department for Levelling Up, Housing and Communities)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `funding-service-design-utils-2.0.0/funding_service_design_utils.egg-info/SOURCES.txt` & `funding-service-design-utils-2.0.1/funding_service_design_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/pyproject.toml` & `funding-service-design-utils-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "funding-service-design-utils"
-version = "2.0.0"
+version = "2.0.1"
 authors = [
   { name="DLUHC", email="FundingServiceDesignTeam@levellingup.gov.uk" },
 ]
 description = "Utilities used by the DLUHC Funding Service Design Team"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10,<4.0"
```

### Comparing `funding-service-design-utils-2.0.0/tests/conftest.py` & `funding-service-design-utils-2.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/tests/test_authentication.py` & `funding-service-design-utils-2.0.1/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/tests/test_checkers.py` & `funding-service-design-utils-2.0.1/tests/test_checkers.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,26 +25,26 @@
         mock_db.session = Mock()
         mock_db.session.execute.return_value = True
         db_checker = DbChecker(mock_db)
 
         result = db_checker.check()
         assert result[0] is True, "Unexpected check result"
         assert result[1] == "OK", "Unexpected check message"
-        mock_db.session.execute.assert_called_once_with("SELECT 1")
+        mock_db.session.execute.assert_called_once()
 
     def testDbCheck_fail(self, flask_test_client):
         mock_db = Mock()
         mock_db.session = Mock()
         mock_db.session.execute.side_effect = ArgumentError
         db_checker = DbChecker(mock_db)
 
         result = db_checker.check()
         assert result[0] is False, "Unexpected check result"
         assert result[1] == "Fail", "Unexpected check message"
-        mock_db.session.execute.assert_called_with("SELECT 1")
+        mock_db.session.execute.assert_called_once()
 
     def testRedis_pass(self, flask_test_client):
         mock_redis = Mock()
         mock_redis.client_list.return_value = []
         redis_checker = RedisChecker(mock_redis)
         result = redis_checker.check()
         assert result[0] is True, "Unexpected result"
```

### Comparing `funding-service-design-utils-2.0.0/tests/test_data_utils.py` & `funding-service-design-utils-2.0.1/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/tests/test_get_lang.py` & `funding-service-design-utils-2.0.1/tests/test_get_lang.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/tests/test_healthcheck.py` & `funding-service-design-utils-2.0.1/tests/test_healthcheck.py`

 * *Files identical despite different names*

### Comparing `funding-service-design-utils-2.0.0/tests/test_set_lang.py` & `funding-service-design-utils-2.0.1/tests/test_set_lang.py`

 * *Files identical despite different names*

