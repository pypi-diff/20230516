# Comparing `tmp/openimis-be-dhis2_etl-1.0.0.tar.gz` & `tmp/openimis-be-dhis2_etl-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-dhis2_etl-1.0.0.tar", last modified: Fri Nov 11 08:11:38 2022, max compression
+gzip compressed data, was "openimis-be-dhis2_etl-1.1.0.tar", last modified: Tue May 16 21:56:07 2023, max compression
```

## Comparing `openimis-be-dhis2_etl-1.0.0.tar` & `openimis-be-dhis2_etl-1.1.0.tar`

### file list

```diff
@@ -1,64 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:38.730256 openimis-be-dhis2_etl-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      812 2022-11-11 08:11:38.730256 openimis-be-dhis2_etl-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    24252 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:38.726256 openimis-be-dhis2_etl-1.0.0/dhis2_etl/
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:38.726256 openimis-be-dhis2_etl-1.0.0/dhis2_etl/adx_transform/
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/adx_transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:38.726256 openimis-be-dhis2_etl-1.0.0/dhis2_etl/adx_transform/adx_models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/adx_transform/adx_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/adx_transform/adx_models/adx_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/adx_transform/adx_models/adx_definition.py
--rw-r--r--   0 runner    (1001) docker     (121)     2096 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/adx_transform/adx_models/adx_time_period.py
--rw-r--r--   0 runner    (1001) docker     (121)     5456 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/adx_transform/builders.py
--rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/adx_transform/formatters.py
--rw-r--r--   0 runner    (1001) docker     (121)     8148 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:38.726256 openimis-be-dhis2_etl-1.0.0/dhis2_etl/configurations/
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/configurations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3758 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/configurations/generalConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/configurations/moduleConfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:38.726256 openimis-be-dhis2_etl-1.0.0/dhis2_etl/converters/
--rw-r--r--   0 runner    (1001) docker     (121)    15872 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/converters/ClaimConverter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1740 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/converters/FundingConverter.py
--rw-r--r--   0 runner    (1001) docker     (121)    13518 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/converters/InsureeConverter.py
--rw-r--r--   0 runner    (1001) docker     (121)    11664 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/converters/LocationConverter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/converters/OptionSetConverter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1642 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:38.726256 openimis-be-dhis2_etl-1.0.0/dhis2_etl/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:38.726256 openimis-be-dhis2_etl-1.0.0/dhis2_etl/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1355 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/models/dhis2Dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     5701 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/models/dhis2Enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     3070 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/models/dhis2Metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     2228 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/models/dhis2Program.py
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/models/dhis2Type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:38.726256 openimis-be-dhis2_etl-1.0.0/dhis2_etl/scheduled_tasks/
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/scheduled_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      893 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/scheduled_tasks/sync_function.py
--rw-r--r--   0 runner    (1001) docker     (121)     2561 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/scheduled_tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:38.726256 openimis-be-dhis2_etl-1.0.0/dhis2_etl/services/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2652 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/services/claimServices.py
--rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/services/fundingServices.py
--rw-r--r--   0 runner    (1001) docker     (121)     7882 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/services/insureeServices.py
--rw-r--r--   0 runner    (1001) docker     (121)     6597 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/services/locationServices.py
--rw-r--r--   0 runner    (1001) docker     (121)     4705 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/services/optionSetServices.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:38.726256 openimis-be-dhis2_etl-1.0.0/dhis2_etl/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8700 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/tests/adx_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     8594 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/tests/daily_sync_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     7883 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4142 2022-11-11 08:11:29.000000 openimis-be-dhis2_etl-1.0.0/dhis2_etl/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:38.730256 openimis-be-dhis2_etl-1.0.0/openimis_be_dhis2_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      812 2022-11-11 08:11:38.000000 openimis-be-dhis2_etl-1.0.0/openimis_be_dhis2_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1713 2022-11-11 08:11:38.000000 openimis-be-dhis2_etl-1.0.0/openimis_be_dhis2_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 08:11:38.000000 openimis-be-dhis2_etl-1.0.0/openimis_be_dhis2_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-11-11 08:11:38.000000 openimis-be-dhis2_etl-1.0.0/openimis_be_dhis2_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-11 08:11:38.000000 openimis-be-dhis2_etl-1.0.0/openimis_be_dhis2_etl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 08:11:38.730256 openimis-be-dhis2_etl-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1407 2022-11-11 08:11:38.000000 openimis-be-dhis2_etl-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:56:07.377227 openimis-be-dhis2_etl-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-16 21:56:07.373227 openimis-be-dhis2_etl-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21533 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:56:07.369227 openimis-be-dhis2_etl-1.1.0/dhis2_etl/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:56:07.369227 openimis-be-dhis2_etl-1.1.0/dhis2_etl/adx_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/adx_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/adx_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:56:07.369227 openimis-be-dhis2_etl-1.1.0/dhis2_etl/adx_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/adx_transform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:56:07.369227 openimis-be-dhis2_etl-1.1.0/dhis2_etl/adx_transform/adx_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/adx_transform/adx_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/adx_transform/adx_models/adx_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/adx_transform/adx_models/adx_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/adx_transform/adx_models/adx_time_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/adx_transform/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/adx_transform/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:56:07.369227 openimis-be-dhis2_etl-1.1.0/dhis2_etl/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/configurations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/configurations/generalConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/configurations/moduleConfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:56:07.369227 openimis-be-dhis2_etl-1.1.0/dhis2_etl/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/converters/ClaimConverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/converters/FundingConverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13518 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/converters/InsureeConverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/converters/LocationConverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/converters/OptionSetConverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:56:07.369227 openimis-be-dhis2_etl-1.1.0/dhis2_etl/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:56:07.369227 openimis-be-dhis2_etl-1.1.0/dhis2_etl/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/models/dhis2Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/models/dhis2Enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/models/dhis2Metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/models/dhis2Program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/models/dhis2Type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:56:07.373227 openimis-be-dhis2_etl-1.1.0/dhis2_etl/scheduled_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/scheduled_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/scheduled_tasks/sync_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/scheduled_tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:56:07.373227 openimis-be-dhis2_etl-1.1.0/dhis2_etl/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:56:07.373227 openimis-be-dhis2_etl-1.1.0/dhis2_etl/services/adx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/services/adx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/services/adx/categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/services/adx/cubes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/services/adx/data_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/services/adx/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/services/adx/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/services/adx_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/services/claimServices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/services/fundingServices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/services/insureeServices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/services/locationServices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/services/optionSetServices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:56:07.373227 openimis-be-dhis2_etl-1.1.0/dhis2_etl/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/tests/adx_client_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9330 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/tests/adx_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/tests/daily_sync_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-16 21:55:54.000000 openimis-be-dhis2_etl-1.1.0/dhis2_etl/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:56:07.373227 openimis-be-dhis2_etl-1.1.0/openimis_be_dhis2_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-16 21:56:07.000000 openimis-be-dhis2_etl-1.1.0/openimis_be_dhis2_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-16 21:56:07.000000 openimis-be-dhis2_etl-1.1.0/openimis_be_dhis2_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:56:07.000000 openimis-be-dhis2_etl-1.1.0/openimis_be_dhis2_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-16 21:56:07.000000 openimis-be-dhis2_etl-1.1.0/openimis_be_dhis2_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 21:56:07.000000 openimis-be-dhis2_etl-1.1.0/openimis_be_dhis2_etl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:56:07.377227 openimis-be-dhis2_etl-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-16 21:56:06.000000 openimis-be-dhis2_etl-1.1.0/setup.py
```

### Comparing `openimis-be-dhis2_etl-1.0.0/LICENSE` & `openimis-be-dhis2_etl-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/LICENSE.md` & `openimis-be-dhis2_etl-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/PKG-INFO` & `openimis-be-dhis2_etl-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-dhis2_etl
-Version: 1.0.0
+Version: 1.1.0
 Summary: The openIMIS Backend to send data to DHIS2.
 Home-page: https://openimis.org/
 Author: Patrick Delcroix
 Author-email: patrick.delcroix@swisstph.ch
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-dhis2_etl-1.0.0/README.md` & `openimis-be-dhis2_etl-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -72,22 +72,18 @@
 ## development to do
 
 - use django scheduler instead of view for triggering the jobs
 - push the metadata along option set push
 - harmonising Service and Items attributes and Data elements
 - add perms and security if the view triggering the job is kept
 - harmonising usage of insuranceID, InsureeNumber, InsureeID in DHIS2
-- connection error management and DHIS2 answers parsing/logging (loggin only what matters and not including the 99% succesful)
 - add orgUnit in programs
 - safely remove all personal data (firstname. lastname, ...) because those data should't be shared with a BI systems
-- push population to data set
 - pull population from dataset
-- use optionGroup in indicator iso option when the options are defined in IMIS (but for gender)
-- add DE family in population dataset
-
+- update readme with new policy program
 
 
  
 -------------------------------------------------------------------------------------
 Hisp india documetation for the programs
 -------------------------------------------------------------------------------------
 
@@ -452,64 +448,7 @@
 
 
 ## 4.4 Health Insurance Board/National Insurance Agency
 
 User roles will be created and assigned to a user belonging to Health Insurance Board/National Insurance Agency in the country to allow them to access data for their specific thematic areas such as Beneficiary Enrollments/Coverage, Claims etc. and evaluate across the country/region/district depending upon their administrative authority. They can access reports, perform data analysis and use dashboards.
 
 
-# **ADX Formatting** 
-### ADX Data definition 
-ADX Data definition can be defined using `dhis2_etl.adx_transform.adx_models.ADXMappingCubeDefinition`. 
-```python 
-ADXMappingCubeDefinition(
-    name=str, # Name of ADX Mapping Definition 
-    period_type=ISOFormatPeriodType(), # Format of handled period type, at the moment only ISO Format is supported 
-    groups=[
-        ADXMappingGroupDefinition(
-            comment=str, # Generic comment 
-            dataset=Model, # Django model, used as base for data value calcultions
-            data_values=[
-                ADXMappingDataValueDefinition(
-                    data_element=str, # Name of calculated value 
-                    related_from_dataset_func=function # Function extracting collection from group dataset object
-                    aggregation_function=function # Function transofrming filtered queryset to dataset value 
-                    categories=[
-                        ADXMappingCategoryDefinition(
-                            category_name=str,
-                            category_options=[
-                                ADXCategoryOptionDefinition(
-                                    code=code,
-                                    filter=function # Function Filtering output of `related_from_dataset_func`
-                                )
-    ])])])])
-```
-#### Example definition: [HF Number of insurees](dhis2_etl/tests/adx_tests.py)
-
-### ADX Data Storage 
-`dhis2_etl.adx_transform.adx_mapper.ADXBuilder` is used for creating ADX Data collection
-based on data definition. 
-Example:
-
-```python
-from dhis2_etl.adx_transform.builders import ADXBuilder
-from dhis2_etl.adx_transform.adx_models.adx_definition import ADXMappingGroupDefinition
-
-definition = ADXMappingGroupDefinition(...)
-builder = ADXBuilder(definition)
-period_type = "2019-01-01/P2Y"  # In format accepted by definition.period_type
-org_units = HealthFaciltity.objects.filter(validity_to__isnull=True).values_list("uuid", flat=True)  # All HF
-builder.create_adx_cube(period_type, org_units)  # Returns ADXMapping object
-```
-
-### ADX Formatters
-ADX Formatters allow transforming ADXMapping objects to diffrent formats. 
-At the moment only XML Format is implemented.
-
-```python
-from dhis2_etl.adx_transform.formatters import XMLFormatter
-from dhis2_etl.adx_transform.adx_models.adx_data import ADXMapping
-
-adx_format = ADXMapping(...)
-xml_formatter = XMLFormatter()
-xml_format = xml_formatter.format_adx(adx_format)
-```
-
```

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/adx_transform/adx_models/adx_data.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/adx_transform/adx_models/adx_data.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/adx_transform/adx_models/adx_definition.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/adx_transform/adx_models/adx_definition.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from dataclasses import dataclass
-from typing import List, Callable, Collection, Type
+from typing import Callable, Collection, List, Type
 from uuid import UUID
 
-from django.db.models import QuerySet, Model
+from django.db.models import Model, QuerySet
+
+from dhis2_etl.adx_transform.adx_models.adx_data import Period
 from dhis2_etl.adx_transform.adx_models.adx_time_period import PeriodType
 
 
 @dataclass
 class ADXCategoryOptionDefinition:
     code: str
     filter: Callable[[QuerySet], QuerySet]  # Filtering function takes queryset instance as argument and returns another queryset
@@ -17,25 +19,27 @@
     category_name: str
     category_options: List[ADXCategoryOptionDefinition]
 
 
 @dataclass
 class ADXMappingDataValueDefinition:
     data_element: str
-    aggregation_function: Callable[[QuerySet], str]
-    related_from_dataset_func: Callable[[Model], QuerySet]
-    aggregation_function: Callable[[QuerySet], str]
+    aggregation_func: Callable[[QuerySet], str]
+    dataset_from_orgunit_func: Callable[[Model], QuerySet]
+    period_filter_func: Callable[[QuerySet, Period], QuerySet]
     categories: List[ADXMappingCategoryDefinition]
 
 
+
 @dataclass
 class ADXMappingGroupDefinition:
     comment: str
     dataset: Type[Model]  # HF Etc.
     data_values: List[ADXMappingDataValueDefinition]
+    to_org_unit_code_func: Callable[[Model], str]
 
     @property
     def dataset_repr(self) -> str:
         return str(self.dataset.__name__).upper()
 
 
 @dataclass
```

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/adx_transform/adx_models/adx_time_period.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/adx_transform/adx_models/adx_time_period.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/adx_transform/builders.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/adx_transform/builders.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import itertools
 
 from django.db.models import Q, Model, F
 from typing import Collection, List, Type
-from uuid import UUID
 
 from dhis2_etl.adx_transform.adx_models.adx_data import Period, ADXDataValue, ADXDataValueAggregation, ADXMappingGroup, \
     ADXMapping
 from dhis2_etl.adx_transform.adx_models.adx_definition import ADXMappingDataValueDefinition, ADXMappingGroupDefinition, \
     ADXMappingCubeDefinition
-from dhis2_etl.utils import build_dhis2_id
 
 
 class ADXDataValueBuilder:
     def __init__(self, adx_mapping_definition: ADXMappingDataValueDefinition):
         self.categories = adx_mapping_definition.categories
-        self.aggregation_func = adx_mapping_definition.aggregation_function
+        self.aggregation_func = adx_mapping_definition.aggregation_func
+        self.period_filter_func = adx_mapping_definition.period_filter_func
         self.data_element = adx_mapping_definition.data_element
-        self.related_from_dataset_func = adx_mapping_definition.related_from_dataset_func
+        self.dataset_from_orgunit_func = adx_mapping_definition.dataset_from_orgunit_func
 
     def create_adx_data_value(self, organization_unit: Model, period: Period) -> List[ADXDataValue]:
         data_values = []
         queryset = self._get_filtered_queryset(organization_unit, period)
         if category_groups := self.__category_groups:
             for group_definition, group_filtering in category_groups:
                 qs = self._filter_queryset_by_category(queryset.all(), group_filtering)
@@ -58,63 +57,67 @@
         for combined_option in itertools.product(*options):
             labels = [o.code for o in combined_option]
             group_label = zip(category_names, labels)
             filters.append((group_label, [o.filter for o in combined_option]))
         return filters
 
     def _get_filtered_queryset(self, organization_unit, period):
-        qs = self.related_from_dataset_func(organization_unit)
-        qs = self._filter_period(qs, period)
+        qs = self.dataset_from_orgunit_func(organization_unit)
+        if self.period_filter_func is not None:
+            qs = self.period_filter_func(qs, period)
+        else:
+            qs = _filter_period(qs, period)
         return qs
 
-    def _filter_period(self, qs, period):
-        return qs.filter(validity_from__gte=period.from_date, validity_from__lte=period.to_date)\
-            .filter(Q(validity_to__isnull=True) | Q(legacy_id__isnull=True) | Q(legacy_id=F('id')))
+
+def _filter_period(qs, period):
+    return qs.filter(validity_from__gte=period.from_date, validity_from__lte=period.to_date) \
+        .filter(Q(validity_to__isnull=True) | Q(legacy_id__isnull=True) | Q(legacy_id=F('id')))
 
 
 class ADXGroupBuilder:
     def __init__(self, adx_mapping_definition: ADXMappingGroupDefinition,
                  data_value_mapper: Type[ADXDataValueBuilder] = ADXDataValueBuilder):
         self.adx_mapping_definition = adx_mapping_definition
         self.data_value_mapper = data_value_mapper
 
-    def create_adx_group(self, period: Period, org_unit: UUID):
+    def create_adx_group(self, period: Period, org_unit_obj: Model, org_unit: str):
         return ADXMappingGroup(
-            org_unit=build_dhis2_id(org_unit),
+            org_unit=org_unit,
             period=period.representation,
             data_set=self.adx_mapping_definition.dataset_repr,
-            data_values=self._build_group_data_values(period, org_unit),
+            data_values=self._build_group_data_values(period, org_unit_obj),
             comment=self.adx_mapping_definition.comment
         )
 
-    def _build_group_data_values(self, period: Period, org_unit: UUID):
+    def _build_group_data_values(self, period: Period, org_unit_obj: object):
         data_values = []
         for data_value in self.adx_mapping_definition.data_values:
-            org_unit_obj = self.adx_mapping_definition.dataset.objects.get(uuid=org_unit)
             values = self.data_value_mapper(data_value).create_adx_data_value(org_unit_obj, period)
             data_values.extend(values)
         return data_values
 
 
 class ADXBuilder:
     def __init__(self, adx_mapping_definition: ADXMappingCubeDefinition,
                  group_mapper: Type[ADXGroupBuilder] = ADXGroupBuilder):
         self.adx_mapping_definition = adx_mapping_definition
         self.group_mapper = group_mapper
 
-    def create_adx_cube(self, period: str, org_units: Collection[UUID]) -> ADXMapping:
+    def create_adx_cube(self, period: str, org_units: Collection[Model]) -> ADXMapping:
         period = self._period_str_to_obj(period)
         return ADXMapping(
             name=self.adx_mapping_definition.name,
             groups=self._build_adx_groups(period, org_units)
         )
 
-    def _build_adx_groups(self, period: Period, org_units: Collection[UUID]):
+    def _build_adx_groups(self, period: Period, org_units: Collection[Model]):
         groups = []
         for group_definition in self.adx_mapping_definition.groups:
             group_mapper = self.group_mapper(group_definition)
-            for org_unit in org_units:
-                groups.append(group_mapper.create_adx_group(period, org_unit))
+            for org_unit_obj in org_units:
+                org_unit = group_definition.to_org_unit_code_func(org_unit_obj)
+                groups.append(group_mapper.create_adx_group(period, org_unit_obj, org_unit))
         return groups
 
     def _period_str_to_obj(self, period: str):
         return self.adx_mapping_definition.period_type.build_period(period)
```

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/adx_transform/formatters.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/adx_transform/formatters.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/apps.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/apps.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,21 @@
 
 DEFAULT_CFG = {
     "dhis2" : {
         "host":"https://play.dhis2.org/2.35",
         "username":"admin",
         "password":"district"
     },
+    "adx": {
+        "endpoint": "api/dataValueSets",
+        "content_type": "application/adx+xml",
+        # https://docs.dhis2.org/en/develop/using-the-api/dhis-core-version-master/data.html#webapi_data_values_import_parameters
+        "data_element_id_scheme": "code",
+        "org_unit_id_scheme": "code",
+    },
     "salt":"LeSalt",
     "jsonOutPath":'C:/temp',
     "scheduled_integration": {
         "claims":  False,
         "policies": False,
         "contribution": False,
         "product": False,
@@ -243,8 +250,8 @@
     #     "4" : "Secondary school",
     #     "5" : "Secondary school",
     #     "6" : "Secondary school",
     #     "7" : "University",
     #     "8" : "Postgraduate studies",
     #     "9" : "PhD",
     #     "10" : "Other" # default        
-    # }
+    # }
```

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/configurations/generalConfiguration.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/configurations/generalConfiguration.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 class GeneralConfiguration(BaseConfiguration):
 
     @classmethod
     def build_configuration(cls, cfg):
         config = cls.get_config()
         config.dhis2 = cfg['dhis2']
+        config.adx = cfg['adx']
         config.salt = cfg['salt']
         config.insureeProgram = cfg['insureeProgram']
         config.claimProgram = cfg['claimProgram']
         config.fundingProgram = cfg['fundingProgram']
         config.populationDataset = cfg['populationDataset']
         config.optionSet = cfg['optionSet']
         # config.genderCodes = cfg['genderCodes']
@@ -30,14 +31,18 @@
         config.scheduled_integration = cfg['scheduled_integration']
 
     @classmethod
     def get_dhis2(cls):
         return cls.get_config().dhis2
 
     @classmethod
+    def get_adx(cls):
+        return cls.get_config().adx
+
+    @classmethod
     def get_insuree_program(cls):
         return cls.get_config().insureeProgram
 
     @classmethod
     def get_salt(cls):
         return cls.get_config().salt
```

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/converters/ClaimConverter.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/converters/ClaimConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/converters/FundingConverter.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/converters/FundingConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/converters/InsureeConverter.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/converters/InsureeConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/converters/LocationConverter.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/converters/LocationConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/converters/OptionSetConverter.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/converters/OptionSetConverter.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/converters/__init__.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/models/dhis2Dataset.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/models/dhis2Dataset.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/models/dhis2Enum.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/models/dhis2Enum.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/models/dhis2Metadata.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/models/dhis2Metadata.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/models/dhis2Program.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/models/dhis2Program.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/models/dhis2Type.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/models/dhis2Type.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/scheduled_tasks/sync_function.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/scheduled_tasks/sync_function.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/scheduled_tasks/utils.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/scheduled_tasks/utils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/services/claimServices.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/services/claimServices.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/services/fundingServices.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/services/fundingServices.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/services/insureeServices.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/services/insureeServices.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/services/locationServices.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/services/locationServices.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/services/optionSetServices.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/services/optionSetServices.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/tests/adx_tests.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/tests/adx_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 from dataclasses import asdict
 from typing import List
 from xml.etree import ElementTree
 
 from django.test import TestCase
+
 from location.models import HealthFacility, Location
 
 from dhis2_etl.adx_transform.formatters import XMLFormatter
 from dhis2_etl.adx_transform.builders import ADXBuilder
 from dhis2_etl.adx_transform.adx_models.adx_definition import ADXMappingDataValueDefinition, \
     ADXMappingCategoryDefinition, ADXCategoryOptionDefinition, ADXMappingCubeDefinition, ADXMappingGroupDefinition
 from dhis2_etl.utils import build_dhis2_id
@@ -15,25 +16,25 @@
 
 from insuree.models import Gender
 from insuree.test_helpers import create_test_insuree
 from location.test_helpers import create_test_health_facility
 from dhis2_etl.adx_transform.adx_models.adx_time_period import ISOFormatPeriodType, PeriodParsingException
 
 
-class ADXTestCase(TestCase):
-    _50_YEARS_AGO = datetime.datetime(2022, 7, 1)-datetime.timedelta(days=365*50)
+class ADXTests(TestCase):
+    _50_YEARS_AGO = datetime.datetime(2022, 7, 1) - datetime.timedelta(days=365 * 50)
     AGE_CATEGORY_DEFINITION = ADXMappingCategoryDefinition(
         category_name="ageGroup",
         category_options=[
             ADXCategoryOptionDefinition(
                 code="<=50yo",
-                filter=lambda insuree_qs: insuree_qs.filter(dob__gte=ADXTestCase._50_YEARS_AGO)),
+                filter=lambda insuree_qs: insuree_qs.filter(dob__gte=ADXTests._50_YEARS_AGO)),
             ADXCategoryOptionDefinition(
                 code=">50yo",
-                filter=lambda insuree_qs: insuree_qs.filter(dob__lt=ADXTestCase._50_YEARS_AGO))
+                filter=lambda insuree_qs: insuree_qs.filter(dob__lt=ADXTests._50_YEARS_AGO))
         ]
     )
     SEX_CATEGORY_DEFINITION = ADXMappingCategoryDefinition(
         category_name="sex",
         category_options=[
             ADXCategoryOptionDefinition(
                 code="M", filter=lambda insuree_qs: insuree_qs.filter(gender__code='M')),
@@ -45,38 +46,44 @@
     TEST_ADX_DEFINITION = ADXMappingCubeDefinition(
         name='TEST_HF_ADX_DEFINITION',
         period_type=ISOFormatPeriodType(),
         groups=[
             ADXMappingGroupDefinition(
                 comment="Test Comment",
                 dataset=HealthFacility,
+                to_org_unit_code_func=lambda hf: build_dhis2_id(hf.uuid),
                 data_values=[
                     ADXMappingDataValueDefinition(
                         data_element="NB_INSUREES",
-                        related_from_dataset_func=lambda hf: hf.insurees,
-                        aggregation_function=lambda insuress_qs: str(insuress_qs.count()),
+                        dataset_from_orgunit_func=lambda hf: hf.insurees,
+                        aggregation_func=lambda insurees_qs: str(insurees_qs.count()),
+                        period_filter_func=lambda qs, period: qs.filter(validity_from__gte=period.from_date,
+                                                                        validity_from__lte=period.to_date),
                         categories=[AGE_CATEGORY_DEFINITION, SEX_CATEGORY_DEFINITION]
                     )
                 ]
             )
         ]
     )
 
     TEST_ADX_DEFINITION_NO_CAT = ADXMappingCubeDefinition(
         name='TEST_HF_ADX_DEFINITION',
         period_type=ISOFormatPeriodType(),
         groups=[
             ADXMappingGroupDefinition(
                 comment="Test Comment",
                 dataset=HealthFacility,
+                to_org_unit_code_func=lambda hf: build_dhis2_id(hf.uuid),
                 data_values=[
                     ADXMappingDataValueDefinition(
                         data_element="NB_INSUREES",
-                        related_from_dataset_func=lambda hf: hf.insurees,
-                        aggregation_function=lambda insuress_qs: str(insuress_qs.count()),
+                        dataset_from_orgunit_func=lambda hf: hf.insurees,
+                        aggregation_func=lambda insuress_qs: str(insuress_qs.count()),
+                        period_filter_func=lambda qs, period: qs.filter(validity_from__gte=period.from_date,
+                                                                        validity_from__lte=period.to_date),
                         categories=[]
                     )
                 ]
             )
         ]
     )
 
@@ -110,15 +117,15 @@
         xml_formatter = XMLFormatter()
         xml_format = xml_formatter.format_adx(adx_format)
         expected = ElementTree.fromstring(self.EXPECTED_XML_DUMP)
         self.assertEqual(ElementTree.tostring(expected), ElementTree.tostring(xml_format))
 
     def _create_test_adx(self, test_period=VALID_TEST_PERIOD, test_definition=TEST_ADX_DEFINITION):
         builder = ADXBuilder(test_definition)
-        org_units = [self._TEST_HF.uuid]
+        org_units = [self._TEST_HF]
         return builder.create_adx_cube(test_period, org_units)
 
     @classmethod
     def _create_test_organization_unit(cls):
         # First valid district
         district = Location.objects.filter(type='D', validity_to__isnull=True).first()
         cls._TEST_HF = create_test_health_facility('HFT', district.id)
@@ -197,13 +204,13 @@
         }
         cls.EXPECTED_XML_DUMP = F'''<adx><group org_unit="{org_unit}" period="2019-01-01/P2Y" data_set="HEALTHFACILITY" comment="Test Comment"><dataValue data_element="NB_INSUREES" value="1" ageGroup="&lt;=50yo" sex="M" /><dataValue data_element="NB_INSUREES" value="2" ageGroup="&lt;=50yo" sex="F" /><dataValue data_element="NB_INSUREES" value="0" ageGroup="&gt;50yo" sex="M" /><dataValue data_element="NB_INSUREES" value="0" ageGroup="&gt;50yo" sex="F" /></group></adx>'''
 
     @classmethod
     def _create_test_insuree(cls, chfid: str, sex: str, dob: str, validity: str) -> List[Insuree]:
         return create_test_insuree(
             True,
-            {'chf_id': chfid,
-             'gender': Gender.objects.get(code=sex),
-             'dob': dob,
-             'health_facility': cls._TEST_HF,
-             'validity_from': validity}
+            custom_props={'chf_id': chfid,
+                          'gender': Gender.objects.get(code=sex),
+                          'dob': dob,
+                          'health_facility': cls._TEST_HF,
+                          'validity_from': validity}
         )
```

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/tests/daily_sync_tests.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/tests/daily_sync_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,12 +144,12 @@
         if in_timeframe > 0:
             raise ValueError(f"Test setup failed, there are unexpected entries added between {timeframe}")
 
     @classmethod
     def _create_test_insuree(cls, chfid: str, sex: str, dob: str, validity: str) -> List[Insuree]:
         return create_test_insuree(
             True,
-            {'chf_id': chfid,
-             'gender': Gender.objects.get(code=sex),
-             'dob': dob,
-             'validity_from': validity}
+            custom_props={'chf_id': chfid,
+                          'gender': Gender.objects.get(code=sex),
+                          'dob': dob,
+                          'validity_from': validity}
         )
```

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/utils.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/utils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/dhis2_etl/views.py` & `openimis-be-dhis2_etl-1.1.0/dhis2_etl/views.py`

 * *Files identical despite different names*

### Comparing `openimis-be-dhis2_etl-1.0.0/openimis_be_dhis2_etl.egg-info/PKG-INFO` & `openimis-be-dhis2_etl-1.1.0/openimis_be_dhis2_etl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-dhis2-etl
-Version: 1.0.0
+Version: 1.1.0
 Summary: The openIMIS Backend to send data to DHIS2.
 Home-page: https://openimis.org/
 Author: Patrick Delcroix
 Author-email: patrick.delcroix@swisstph.ch
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-dhis2_etl-1.0.0/openimis_be_dhis2_etl.egg-info/SOURCES.txt` & `openimis-be-dhis2_etl-1.1.0/openimis_be_dhis2_etl.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 setup.py
 dhis2_etl/__init__.py
 dhis2_etl/admin.py
 dhis2_etl/apps.py
 dhis2_etl/urls.py
 dhis2_etl/utils.py
 dhis2_etl/views.py
+dhis2_etl/adx_client/__init__.py
+dhis2_etl/adx_client/client.py
 dhis2_etl/adx_transform/__init__.py
 dhis2_etl/adx_transform/builders.py
 dhis2_etl/adx_transform/formatters.py
 dhis2_etl/adx_transform/adx_models/__init__.py
 dhis2_etl/adx_transform/adx_models/adx_data.py
 dhis2_etl/adx_transform/adx_models/adx_definition.py
 dhis2_etl/adx_transform/adx_models/adx_time_period.py
@@ -31,20 +33,28 @@
 dhis2_etl/models/dhis2Metadata.py
 dhis2_etl/models/dhis2Program.py
 dhis2_etl/models/dhis2Type.py
 dhis2_etl/scheduled_tasks/__init__.py
 dhis2_etl/scheduled_tasks/sync_function.py
 dhis2_etl/scheduled_tasks/utils.py
 dhis2_etl/services/__init__.py
+dhis2_etl/services/adx_service.py
 dhis2_etl/services/claimServices.py
 dhis2_etl/services/fundingServices.py
 dhis2_etl/services/insureeServices.py
 dhis2_etl/services/locationServices.py
 dhis2_etl/services/optionSetServices.py
+dhis2_etl/services/adx/__init__.py
+dhis2_etl/services/adx/categories.py
+dhis2_etl/services/adx/cubes.py
+dhis2_etl/services/adx/data_values.py
+dhis2_etl/services/adx/groups.py
+dhis2_etl/services/adx/utils.py
 dhis2_etl/tests/__init__.py
+dhis2_etl/tests/adx_client_tests.py
 dhis2_etl/tests/adx_tests.py
 dhis2_etl/tests/daily_sync_tests.py
 openimis_be_dhis2_etl.egg-info/PKG-INFO
 openimis_be_dhis2_etl.egg-info/SOURCES.txt
 openimis_be_dhis2_etl.egg-info/dependency_links.txt
 openimis_be_dhis2_etl.egg-info/requires.txt
 openimis_be_dhis2_etl.egg-info/top_level.txt
```

### Comparing `openimis-be-dhis2_etl-1.0.0/setup.py` & `openimis-be-dhis2_etl-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-dhis2_etl',
-    version='1.0.0',
+    version='v1.1.0',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend to send data to DHIS2.',
     # long_description=README,
     url='https://openimis.org/',
     author='Patrick Delcroix',
```

