# Comparing `tmp/cloudlift-1.5.7.tar.gz` & `tmp/cloudlift-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudlift-1.5.7.tar", last modified: Thu Feb  2 12:17:55 2023, max compression
+gzip compressed data, was "cloudlift-2.0.0.tar", last modified: Tue May 16 10:33:20 2023, max compression
```

## Comparing `cloudlift-1.5.7.tar` & `cloudlift-2.0.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-02-02 12:17:55.688549 cloudlift-1.5.7/
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)     1062 2020-04-14 13:38:03.000000 cloudlift-1.5.7/LICENSE
--rwxrwxrwx   0 shoan     (1000) shoan     (1000)       40 2020-02-21 06:48:18.000000 cloudlift-1.5.7/MANIFEST.in
--rw-r--r--   0 shoan     (1000) shoan     (1000)     9544 2023-02-02 12:17:55.682537 cloudlift-1.5.7/PKG-INFO
--rw-r--r--   0 shoan     (1000) shoan     (1000)     9243 2023-02-02 08:10:32.000000 cloudlift-1.5.7/README.md
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-02-02 12:17:52.882519 cloudlift-1.5.7/cloudlift/
--rw-r--r--   0 shoan     (1000) shoan     (1000)     6237 2023-02-02 08:10:32.000000 cloudlift-1.5.7/cloudlift/__init__.py
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-02-02 12:17:54.005394 cloudlift-1.5.7/cloudlift/config/
--rw-r--r--   0 shoan     (1000) shoan     (1000)      266 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/config/__init__.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      669 2023-02-02 12:14:14.000000 cloudlift-1.5.7/cloudlift/config/account.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      448 2023-02-02 08:10:32.000000 cloudlift-1.5.7/cloudlift/config/banner.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      621 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/config/decimal_encoder.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     2408 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/config/diff.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     1844 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/config/dynamodb_configuration.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)    17379 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/config/environment_configuration.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      546 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/config/logging.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     2129 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/config/mfa.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     4387 2023-01-25 11:43:34.000000 cloudlift-1.5.7/cloudlift/config/parameter_store.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      704 2023-02-02 12:14:14.000000 cloudlift-1.5.7/cloudlift/config/pre_flight.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     3516 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/config/region.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)    10706 2022-12-20 15:02:42.000000 cloudlift-1.5.7/cloudlift/config/service_configuration.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      161 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/config/stack.py
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-02-02 12:17:55.187184 cloudlift-1.5.7/cloudlift/deployment/
--rw-r--r--   0 shoan     (1000) shoan     (1000)      373 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/deployment/__init__.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     3154 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/deployment/changesets.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)    34242 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/deployment/cluster_template_generator.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      267 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/deployment/configs.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     6321 2023-01-25 11:43:34.000000 cloudlift-1.5.7/cloudlift/deployment/deployer.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     6981 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/deployment/ecr_client.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)    17824 2023-02-02 12:14:14.000000 cloudlift-1.5.7/cloudlift/deployment/ecs.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      996 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/deployment/editor.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     8032 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/deployment/environment_creator.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      896 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/deployment/progress.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     6646 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/deployment/service_creator.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     6730 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/deployment/service_information_fetcher.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)    37398 2023-01-25 11:43:34.000000 cloudlift-1.5.7/cloudlift/deployment/service_template_generator.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     4397 2023-02-02 08:10:32.000000 cloudlift-1.5.7/cloudlift/deployment/service_updater.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     6173 2023-01-25 11:43:34.000000 cloudlift-1.5.7/cloudlift/deployment/task_definition_creator.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     1257 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/deployment/template_generator.py
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-02-02 12:17:55.371182 cloudlift-1.5.7/cloudlift/exceptions/
--rw-r--r--   0 shoan     (1000) shoan     (1000)       46 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/exceptions/__init__.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)      154 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/exceptions/exceptions.py
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-02-02 12:17:55.516182 cloudlift-1.5.7/cloudlift/session/
--rw-r--r--   0 shoan     (1000) shoan     (1000)       30 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/session/__init__.py
--rw-r--r--   0 shoan     (1000) shoan     (1000)     1874 2022-12-15 11:12:05.000000 cloudlift-1.5.7/cloudlift/session/session_creator.py
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-02-02 12:17:55.579478 cloudlift-1.5.7/cloudlift/version/
--rw-r--r--   0 shoan     (1000) shoan     (1000)       17 2023-02-02 12:14:14.000000 cloudlift-1.5.7/cloudlift/version/__init__.py
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-02-02 12:17:53.173203 cloudlift-1.5.7/cloudlift.egg-info/
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)     9544 2023-02-02 12:17:51.000000 cloudlift-1.5.7/cloudlift.egg-info/PKG-INFO
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)     1585 2023-02-02 12:17:52.000000 cloudlift-1.5.7/cloudlift.egg-info/SOURCES.txt
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)        1 2023-02-02 12:17:52.000000 cloudlift-1.5.7/cloudlift.egg-info/dependency_links.txt
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)       63 2023-02-02 12:17:52.000000 cloudlift-1.5.7/cloudlift.egg-info/entry_points.txt
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)      384 2023-02-02 12:17:52.000000 cloudlift-1.5.7/cloudlift.egg-info/requires.txt
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)       10 2023-02-02 12:17:52.000000 cloudlift-1.5.7/cloudlift.egg-info/top_level.txt
--rw-rw-rw-   0 shoan     (1000) shoan     (1000)        1 2020-01-19 03:14:24.000000 cloudlift-1.5.7/cloudlift.egg-info/zip-safe
--rw-r--r--   0 shoan     (1000) shoan     (1000)      100 2021-03-16 11:07:35.000000 cloudlift-1.5.7/pyproject.toml
--rw-r--r--   0 shoan     (1000) shoan     (1000)      383 2022-12-15 11:12:05.000000 cloudlift-1.5.7/requirements.txt
--rw-r--r--   0 shoan     (1000) shoan     (1000)       38 2023-02-02 12:17:55.690535 cloudlift-1.5.7/setup.cfg
--rw-r--r--   0 shoan     (1000) shoan     (1000)      774 2022-12-15 11:12:05.000000 cloudlift-1.5.7/setup.py
-drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-02-02 12:17:55.634257 cloudlift-1.5.7/test/
--rw-r--r--   0 shoan     (1000) shoan     (1000)     5303 2022-12-15 11:12:06.000000 cloudlift-1.5.7/test/test_cloudlift.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-05-16 10:33:20.275573 cloudlift-2.0.0/
+-rw-rw-rw-   0 shoan     (1000) shoan     (1000)     1062 2020-04-14 13:38:03.000000 cloudlift-2.0.0/LICENSE
+-rwxrwxrwx   0 shoan     (1000) shoan     (1000)       40 2020-02-21 06:48:18.000000 cloudlift-2.0.0/MANIFEST.in
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    13572 2023-05-16 10:33:20.268571 cloudlift-2.0.0/PKG-INFO
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    13271 2023-04-26 12:53:28.000000 cloudlift-2.0.0/README.md
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-05-16 10:33:17.377204 cloudlift-2.0.0/cloudlift/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     6400 2023-04-26 12:53:28.000000 cloudlift-2.0.0/cloudlift/__init__.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-05-16 10:33:18.675498 cloudlift-2.0.0/cloudlift/config/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      266 2022-12-15 11:12:05.000000 cloudlift-2.0.0/cloudlift/config/__init__.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      669 2023-02-02 12:14:14.000000 cloudlift-2.0.0/cloudlift/config/account.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      448 2023-02-02 08:10:32.000000 cloudlift-2.0.0/cloudlift/config/banner.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      621 2022-12-15 11:12:05.000000 cloudlift-2.0.0/cloudlift/config/decimal_encoder.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     2408 2022-12-15 11:12:05.000000 cloudlift-2.0.0/cloudlift/config/diff.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     1844 2022-12-15 11:12:05.000000 cloudlift-2.0.0/cloudlift/config/dynamodb_configuration.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    20687 2023-04-26 12:53:28.000000 cloudlift-2.0.0/cloudlift/config/environment_configuration.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      546 2022-12-15 11:12:05.000000 cloudlift-2.0.0/cloudlift/config/logging.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     2129 2022-12-15 11:12:05.000000 cloudlift-2.0.0/cloudlift/config/mfa.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     4387 2023-01-25 11:43:34.000000 cloudlift-2.0.0/cloudlift/config/parameter_store.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     2568 2023-04-26 12:53:28.000000 cloudlift-2.0.0/cloudlift/config/pre_flight.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     3516 2022-12-15 11:12:05.000000 cloudlift-2.0.0/cloudlift/config/region.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    10986 2023-04-26 12:53:28.000000 cloudlift-2.0.0/cloudlift/config/service_configuration.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      161 2022-12-15 11:12:05.000000 cloudlift-2.0.0/cloudlift/config/stack.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-05-16 10:33:19.830103 cloudlift-2.0.0/cloudlift/deployment/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      373 2022-12-15 11:12:05.000000 cloudlift-2.0.0/cloudlift/deployment/__init__.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     3154 2022-12-15 11:12:05.000000 cloudlift-2.0.0/cloudlift/deployment/changesets.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    41448 2023-04-26 12:53:28.000000 cloudlift-2.0.0/cloudlift/deployment/cluster_template_generator.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      267 2022-12-15 11:12:05.000000 cloudlift-2.0.0/cloudlift/deployment/configs.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     6321 2023-01-25 11:43:34.000000 cloudlift-2.0.0/cloudlift/deployment/deployer.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     6981 2022-12-15 11:12:05.000000 cloudlift-2.0.0/cloudlift/deployment/ecr_client.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    17824 2023-02-02 12:14:14.000000 cloudlift-2.0.0/cloudlift/deployment/ecs.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      996 2022-12-15 11:12:05.000000 cloudlift-2.0.0/cloudlift/deployment/editor.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     8032 2022-12-15 11:12:05.000000 cloudlift-2.0.0/cloudlift/deployment/environment_creator.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      896 2022-12-15 11:12:05.000000 cloudlift-2.0.0/cloudlift/deployment/progress.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     6646 2022-12-15 11:12:05.000000 cloudlift-2.0.0/cloudlift/deployment/service_creator.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     6730 2022-12-15 11:12:05.000000 cloudlift-2.0.0/cloudlift/deployment/service_information_fetcher.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)    40455 2023-04-26 12:53:28.000000 cloudlift-2.0.0/cloudlift/deployment/service_template_generator.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     4397 2023-02-02 08:10:32.000000 cloudlift-2.0.0/cloudlift/deployment/service_updater.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     6527 2023-04-26 12:53:28.000000 cloudlift-2.0.0/cloudlift/deployment/task_definition_creator.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     1257 2022-12-15 11:12:05.000000 cloudlift-2.0.0/cloudlift/deployment/template_generator.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-05-16 10:33:19.957507 cloudlift-2.0.0/cloudlift/exceptions/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)       46 2022-12-15 11:12:05.000000 cloudlift-2.0.0/cloudlift/exceptions/__init__.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      154 2022-12-15 11:12:05.000000 cloudlift-2.0.0/cloudlift/exceptions/exceptions.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-05-16 10:33:20.094513 cloudlift-2.0.0/cloudlift/session/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)       30 2022-12-15 11:12:05.000000 cloudlift-2.0.0/cloudlift/session/__init__.py
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     1874 2022-12-15 11:12:05.000000 cloudlift-2.0.0/cloudlift/session/session_creator.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-05-16 10:33:20.152843 cloudlift-2.0.0/cloudlift/version/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)       17 2023-04-26 12:53:28.000000 cloudlift-2.0.0/cloudlift/version/__init__.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-05-16 10:33:17.698067 cloudlift-2.0.0/cloudlift.egg-info/
+-rw-rw-rw-   0 shoan     (1000) shoan     (1000)    13572 2023-05-16 10:33:16.000000 cloudlift-2.0.0/cloudlift.egg-info/PKG-INFO
+-rw-rw-rw-   0 shoan     (1000) shoan     (1000)     1585 2023-05-16 10:33:16.000000 cloudlift-2.0.0/cloudlift.egg-info/SOURCES.txt
+-rw-rw-rw-   0 shoan     (1000) shoan     (1000)        1 2023-05-16 10:33:16.000000 cloudlift-2.0.0/cloudlift.egg-info/dependency_links.txt
+-rw-rw-rw-   0 shoan     (1000) shoan     (1000)       63 2023-05-16 10:33:16.000000 cloudlift-2.0.0/cloudlift.egg-info/entry_points.txt
+-rw-rw-rw-   0 shoan     (1000) shoan     (1000)      384 2023-05-16 10:33:16.000000 cloudlift-2.0.0/cloudlift.egg-info/requires.txt
+-rw-rw-rw-   0 shoan     (1000) shoan     (1000)       10 2023-05-16 10:33:16.000000 cloudlift-2.0.0/cloudlift.egg-info/top_level.txt
+-rw-rw-rw-   0 shoan     (1000) shoan     (1000)        1 2020-01-19 03:14:24.000000 cloudlift-2.0.0/cloudlift.egg-info/zip-safe
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      100 2021-03-16 11:07:35.000000 cloudlift-2.0.0/pyproject.toml
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      383 2022-12-15 11:12:05.000000 cloudlift-2.0.0/requirements.txt
+-rw-r--r--   0 shoan     (1000) shoan     (1000)       38 2023-05-16 10:33:20.277567 cloudlift-2.0.0/setup.cfg
+-rw-r--r--   0 shoan     (1000) shoan     (1000)      774 2022-12-15 11:12:05.000000 cloudlift-2.0.0/setup.py
+drwxr-xr-x   0 shoan     (1000) shoan     (1000)        0 2023-05-16 10:33:20.216720 cloudlift-2.0.0/test/
+-rw-r--r--   0 shoan     (1000) shoan     (1000)     5303 2022-12-15 11:12:06.000000 cloudlift-2.0.0/test/test_cloudlift.py
```

### Comparing `cloudlift-1.5.7/LICENSE` & `cloudlift-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/README.md` & `cloudlift-2.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: cloudlift
+Version: 2.0.0
+Summary: Cloudlift makes it easier to launch dockerized services in AWS ECS
+Home-page: https://github.com/GetSimpl/cloudlift
+License: UNKNOWN
+Platform: UNKNOWN
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Cloudlift
 
 Cloudlift is built by Simpl developers to make it easier to launch dockerized
 services in AWS ECS.
 
 Cloudlift is a command-line tool for dockerized services to be deployed in AWS
 ECS. It's very simple to use. That's possible because this is heavily
@@ -28,15 +39,15 @@
 ### 2. Install cloudlift
 
 ```sh
 pip install cloudlift
 ```
 
 
-### 2. Configure AWS
+### 3. Configure AWS
 
 ```perl
 aws configure
 ```
 
 Enter the AWS Access Key ID, AWS Secret Access Key. You can find instructions
 here on how to get Access Key ID and Secret Access Key here at
@@ -94,28 +105,106 @@
 ```
 
 This opens the environment configuration in the `VISUAL` editor. Update this to
 make changes to the environment.
 
 ### Create a new service
 
-#### 1. Upload configuration to Parameter Store
+### Object Structure
+The configuration object is structured as follows:
+
+```json
+{
+    "notifications_arn": "string",
+    "services": {
+        "Test123": {
+            "command": "string/null",
+            "custom_metrics": {
+                "metrics_port": "string",
+                "metrics_path": "string"
+            },
+            "http_interface": {
+                "container_port": "number",
+                "internal": "boolean",
+                "restrict_access_to": ["string", "string"]
+            },
+            "volume": {
+                "efs_id" : "string",
+                "efs_directory_path" : "string",
+                "container_path" : "string"
+            },
+            "memory_reservation": "number",
+            "logging": "string/null"
+        }
+    }
+}
+```
+### Required Fields
+
+The following fields are required in the configuration object:
+
+- `notifications_arn`: A string representing the Amazon Resource Name (ARN) of the SNS topic to which notifications will be sent.
+
+- `services`: An object representing the services to be configured. The keys of this object are the names of the services, and the values are objects containing configuration information for each service.
+
+
+### Service Configuration
+
+Each service object must contain the following fields:
+
+- `command`: A string or null value representing the command to be run in the Docker container. If this field is null, the command specified in the Dockerfile will be used.
+
+- `memory_reservation`: A number representing the soft memory limit for the container. The hard limit will automatically be set to 1.5 times the soft limit.
+
+In addition, a service object may contain any of the following optional fields:
+
+- `custom_metrics`: An object containing configuration information for exporting custom metrics to a Prometheus server. This field is only used if custom metrics are required.
+
+
+    > **NOTE:** If you use custom metrics, Your ECS container Network mode will be `awsvpc`. 
+
+    > **⚠ WARNING:** If you are adding custom metrics to your existing service, there will be a downtime.
+
+  - `metrics_port`: A string representing the port number on which custom metrics are exported.
+  
+  - `metrics_path`: A string representing the path on which custom metrics are exported.
+
+- `http_interface`: An object containing configuration information for setting up an Application Load Balancer (ALB) for the service. This field is only used if an ALB is required.
+
+  - `container_port`: A number representing the port number on which the service is running inside the container.
+  
+  - `internal`: A boolean value indicating whether the ALB should be internal. If set to false, the ALB will be public.
+  
+  - `restrict_access_to`: An array of strings representing the IP addresses that should be allowed to access the ALB.
+
+- `volume`: An object containing configuration information for mounting an Amazon Elastic File System (EFS) volume to the service. This field is only used if an EFS volume is required.
+
+  - `efs_id`: A string representing the ID of the EFS volume to be mounted.
+  
+  - `efs_directory_path`: A string representing the directory path on the EFS volume to be mounted.
+  
+  - `container_path`: A string representing the mount path inside the container.
+
+- `logging`: A string or null value representing the log driver to be used. Valid options are "fluentd", "awslogs", or null. If this field is null, the default log driver (CloudWatch Logs) will be used.
+
+
+### 1. Upload configuration to Parameter Store
 
 During create_service and deployment `cloudlift` pulls the config from AWS
 Parameter Store to apply it on the task definition. Configurations are stored in
 path with the convention `/<environment>/<service>/<key>`
 
 ```sh
 cloudlift edit_config -e <environment-name>
 ```
 
   _NOTE_: This is *not* required for every deployment. It's required only when
   config needs to be changed.
 
-#### 2. Create service
+### 2. Create service
 
 In the repository for the application, run -
 
 ```sh
   cloudlift create_service -e <environment-name>
 ```
 
@@ -135,46 +224,87 @@
                   ]
               },
               "memory_reservation": 100
           }
       }
   }
 ```
+### 3. Deploy service
 
-Definitions -
-
-`services`: Map of all ECS services with configuration for current application
+This command build the image (only if the version is unavailable in ECR), pushes to ECR and updates the ECS 
+service task definition. It supports `--build-arg` argument of `docker build` command as well to pass
+custom build time arguments
 
-`command`: Override command in Dockerfile
+```sh
+  cloudlift deploy_service -e <environment-name>
+```
 
-`custom_metrics`: Configuration for custom metrics if required, do not include this if the service does not write/export custom metrics
+For example, you can pass your SSH key as a build argument to docker build
 
-> **NOTE:** If you use custom metrics, Your ECS container Network mode will be `awsvpc`. 
+```sh
+  cloudlift deploy_service --build-arg SSH_KEY "\"`cat ~/.ssh/id_rsa`\"" -e <environment-name>
+```
+This example is bit comprehensive to show
+- it can execute shell commands with "`".
+- It's wrapped with double quotes to avoid line-breaks in SSH keys breaking the command.
 
-> **⚠ WARNING:** If you are adding custom metrics to your existing service, there will be a downtime.
+### 4. Starting shell on container instance for service
 
-`http_interface`: Configuration for HTTP interface if required, do not include
-this if the services does not require a HTTP interface
+You can start a shell on a container instance which is running a task for given
+application using the `start_session` command. One pre-requisite for this is
+installing the session manager plugin for `awscli`. To install session manager
+plugin follow the [guide](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html#install-plugin-macos)
 
-`container_port`: Port in which the process is exposed inside container
+```sh
+  cloudlift start_session -e <environment-name>
+```
 
-`internal`: Scheme of loadbalancer. If internal, the loadbalancer is accessible
-only within the VPC
+MFA code can be passed as parameter `--mfa` or you will be prompted to enter
+the MFA code.
 
-`restrict_access_to`: List of CIDR to which HTTP interface is restricted to.
 
-`memory_reservation`: Memory size reserved for each task in MBs. This is a soft
-limit, i.e. at least this much memory will be available, and upto whatever
-memory is free in running container instance. Minimum: 10 MB, Maximum: 8000 MB
+## Example
 
-`volume`: Configuration for EFS volume mount if required, do not include this if the service does not required volume mount
+### 1. Service configuration:
+```json
+{
+  "notifications_arn": "arn:aws:sns:us-east-1:123456789012:MyTopic",
+  "services": {
+    "Test123": {
+      "command": null,
+      "custom_metrics": {
+        "metrics_port": "8080",
+        "metrics_path": "/metrics"
+      },
+      "http_interface": {
+        "container_port": 3000,
+        "internal": false,
+        "restrict_access_to": ["192.0.2.0/24", "198.51.100.0/24"]
+      },
+      "volume": {
+        "efs_id": "fs-0123456789abcdef",
+        "efs_directory_path": "/mydata",
+        "container_path": "/data"
+      },
+      "memory_reservation": 256,
+      "logging": "fluentd"
+    }
+  }
+}
+```
+In this example, we are configuring a service named Test123. The service has the following configuration:
 
-#### Examples:
+- `command`: The command to be run in the Docker container is not specified, so the command specified in the Dockerfile will be used.
+- `custom_metrics`: Custom metrics will be exported to a Prometheus server running on port 8080, with the metrics available at the path "/metrics".
+- `http_interface`: An Application Load Balancer (ALB) will be set up for the service on port 3000. The ALB will be public and will allow access only from the IP addresses in the restrict_access_to array.
+- `volume`: An Amazon Elastic File System (EFS) volume with ID fs-0123456789abcdef will be mounted to the service. The volume will be mounted at the directory path "/mydata" on the EFS volume, and at the path "/data" inside the container.
+- `memory_reservation`: The soft memory limit for the container is set to 256 MB, so the hard limit will be automatically set to 384 MB.
+- `logging`: Logs will be sent to a Fluentd log driver.
 
-1. Service configuration with custom metrics:
+### 2. Service configuration with custom metrics:
 ```json
   {
       "notifications_arn": "<SNS Topic ARN>",
       "services": {
           "Test123": {
               "command": null,
               "custom_metrics": {
@@ -189,15 +319,15 @@
                   ]
               },
               "memory_reservation": 100
           }
       }
   }
 ```
-2. Service configuration with volume mount:
+### 3. Service configuration with volume mount:
 ```json
   {
       "notifications_arn": "<SNS Topic ARN>",
       "services": {
           "Test123": {
               "command": null,
               "volume": {
@@ -213,15 +343,15 @@
                   ]
               },
               "memory_reservation": 100
           }
       }
   }
 ```
-3. Service configuration with http interface only:
+### 4. Service configuration with http interface only:
 ```json
   {
       "notifications_arn": "<SNS Topic ARN>",
       "services": {
           "Test123": {
               "command": null,
               "http_interface": {
@@ -232,70 +362,38 @@
                   ]
               },
               "memory_reservation": 100
           }
       }
   }
 ```
-4. Service configuration with http interface without AWS CW logging.
+### 5. Service configuration with http interface without AWS CW logging.
+
+> **_NOTE:_** Do not use `logging: null` in production. Once container  gets deleted all logs will be lost. Logging configuration should be one of the following: `awslog`, `fluentd`,`null`
 
-`Note: Do not use `logging: false` in production. Once conatiner deleted all logs will be lost`.
 ```json
   {
       "notifications_arn": "<SNS Topic ARN>",
       "services": {
           "Test123": {
               "command": null,
               "http_interface": {
                   "container_port": 80,
                   "internal": false,
                   "restrict_access_to": [
                       "0.0.0.0/0"
                   ]
               },
               "memory_reservation": 100,
-              "logging": false
+              "logging": null
           }
       }
   }
 ```
 
-#### 3. Deploy service
-
-This command build the image (only if the version is unavailable in ECR), pushes to ECR and updates the ECS 
-service task definition. It supports `--build-arg` argument of `docker build` command as well to pass
-custom build time arguments
-
-```sh
-  cloudlift deploy_service -e <environment-name>
-```
-
-For example, you can pass your SSH key as a build argument to docker build
-
-```sh
-  cloudlift deploy_service --build-arg SSH_KEY "\"`cat ~/.ssh/id_rsa`\"" -e <environment-name>
-```
-This example is bit comprehensive to show
-- it can execute shell commands with "`".
-- It's wrapped with double quotes to avoid line-breaks in SSH keys breaking the command.
-
-### 6. Starting shell on container instance for service
-
-You can start a shell on a container instance which is running a task for given
-application using the `start_session` command. One pre-requisite for this is
-installing the session manager plugin for `awscli`. To install session manager
-plugin follow the [guide](https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html#install-plugin-macos)
-
-```sh
-  cloudlift start_session -e <environment-name>
-```
-
-MFA code can be passed as parameter `--mfa` or you will be prompted to enter
-the MFA code.
-
 ## Contributing to cloudlift
 
 ### Setup
 
 #### Use the latest git master 
 
 ```sh
@@ -325,7 +423,9 @@
 ```sh
 pytest -s test/test_cloudlift.py
 ```
 
 This tests expects to have an access to AWS console.
 Since there's no extensive test coverage, it's better to manually test the
 impacted areas whenever there's a code change.
+
+
```

### Comparing `cloudlift-1.5.7/cloudlift/__init__.py` & `cloudlift-2.0.0/cloudlift/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import functools
 
 import boto3
 import click
 from botocore.exceptions import ClientError
 
 from cloudlift.config import highlight_production, highlight_user_account_details
+from cloudlift.config.pre_flight import check_stack_exists
 from cloudlift.deployment.configs import deduce_name
 from cloudlift.deployment import EnvironmentCreator, editor
 from cloudlift.config.logging import log_err
 from cloudlift.deployment.service_creator import ServiceCreator
 from cloudlift.deployment.service_information_fetcher import ServiceInformationFetcher
 from cloudlift.deployment.service_updater import ServiceUpdater
 from cloudlift.deployment.task_definition_creator import TaskDefinitionCreator
@@ -67,21 +68,23 @@
 
 
 @cli.command(help="Create a new service. This can contain multiple \
 ECS services")
 @_require_environment
 @_require_name
 def create_service(name, environment):
+    check_stack_exists(name, environment, "create")
     ServiceCreator(name, environment).create()
 
 
 @cli.command(help="Update existing service.")
 @_require_environment
 @_require_name
 def update_service(name, environment):
+    check_stack_exists(name, environment, "update")
     ServiceCreator(name, environment).update()
 
 
 @cli.command(help="Create a new environment")
 @click.option('--environment', '-e', prompt='environment',
               help='environment')
 def create_environment(environment):
```

### Comparing `cloudlift-1.5.7/cloudlift/config/account.py` & `cloudlift-2.0.0/cloudlift/config/account.py`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/cloudlift/config/decimal_encoder.py` & `cloudlift-2.0.0/cloudlift/config/decimal_encoder.py`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/cloudlift/config/diff.py` & `cloudlift-2.0.0/cloudlift/config/diff.py`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/cloudlift/config/dynamodb_configuration.py` & `cloudlift-2.0.0/cloudlift/config/dynamodb_configuration.py`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/cloudlift/config/environment_configuration.py` & `cloudlift-2.0.0/cloudlift/config/service_configuration.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,391 +1,285 @@
-"""
-This module handles global cloudlift configuration that is custom to
-the organization using cloudlift
-"""
-import ipaddress
+'''
+This module abstracts implementation of storing, editing and
+retrieving service configuration.
+'''
+
 import json
-from distutils.version import LooseVersion
+from time import sleep
 
-import boto3
 import dictdiffer
 from botocore.exceptions import ClientError
-from click import confirm, edit, prompt
+from click import confirm, edit
+from cloudlift.exceptions import UnrecoverableException
 from jsonschema import validate
 from jsonschema.exceptions import ValidationError
+from stringcase import pascalcase
 
+from cloudlift.config import DecimalEncoder, print_json_changes, get_resource_for
+# import config.mfa as mfa
+from cloudlift.config.logging import log_bold, log_err, log_warning, log
 from cloudlift.version import VERSION
-from cloudlift.exceptions import UnrecoverableException
-from cloudlift.config import DecimalEncoder, print_json_changes
 from cloudlift.config.dynamodb_configuration import DynamodbConfiguration
 from cloudlift.config.pre_flight import check_sns_topic_exists
 
-# import config.mfa as mfa
-from cloudlift.config.logging import log_bold, log_err, log_warning
-
-ENVIRONMENT_CONFIGURATION_TABLE = 'environment_configurations'
 
+SERVICE_CONFIGURATION_TABLE = 'service_configurations'
 
-class EnvironmentConfiguration(object):
+class ServiceConfiguration(object):
     '''
-        Handles configuration in DynamoDB for cloudlift
+        Handles configuration in DynamoDB for services
     '''
 
-    def __init__(self, environment=None):
+    def __init__(self, service_name, environment):
+        self.service_name = service_name
         self.environment = environment
+        self.new_service = False
+        # TODO: Use the below two lines when all parameter store actions
+        # require MFA
+        #
+        # mfa_region = get_region_for_environment(environment)
+        # mfa_session = mfa.get_mfa_session(mfa_region)
+        # ssm_client = mfa_session.client('ssm')
+        self.dynamodb_resource = get_resource_for('dynamodb',environment)
+        self.table = DynamodbConfiguration(SERVICE_CONFIGURATION_TABLE, [
+            ('service_name', self.service_name), ('environment', self.environment)])._get_table()
 
-        session = boto3.session.Session()
-        self.dynamodb = session.resource('dynamodb')
-        self.table = DynamodbConfiguration(ENVIRONMENT_CONFIGURATION_TABLE, [
-                       ('environment', self.environment)])._get_table()
-
-    def get_config(self, cloudlift_version=VERSION):
+    def edit_config(self):
         '''
-            Get configuration from DynamoDB
+            Open editor to update configuration
         '''
 
         try:
-            configuration_response = self.table.get_item(
-                Key={
-                    'environment': self.environment
-                },
-                ConsistentRead=True,
-                AttributesToGet=[
-                    'configuration'
-                ]
-            )
-            existing_configuration = configuration_response['Item']['configuration']
-            previous_cloudlift_version = existing_configuration.pop("cloudlift_version", None)
-            # print(f"Previous cloudlift version in environment config is {previous_cloudlift_version}")
-            if previous_cloudlift_version and LooseVersion(cloudlift_version) < LooseVersion(previous_cloudlift_version):
-                raise UnrecoverableException(f'Cloudlift Version {previous_cloudlift_version} was used to '
-                                             f'create this service. You are using version {cloudlift_version}, '
-                                             f'which is older and can cause corruption. Please upgrade to at least '
-                                             f'version {previous_cloudlift_version} to proceed.\n\nUpgrade to the '
-                                             f'latest version (Recommended):\n'
-                                             f'\tpip install -U cloudlift\n\nOR\n\nUpgrade to a compatible version:\n'
-                                             f'\tpip install -U cloudlift=={previous_cloudlift_version}')
-            return existing_configuration
-        except ClientError:
-            raise UnrecoverableException("Unable to fetch environment configuration from DynamoDB.")
-        except KeyError:
-            raise UnrecoverableException("Environment configuration not found. Does this environment exist?")
-
-    def update_config(self):
-
-        if not self._env_config_exists():
-            self._create_config()
-        self._edit_config()
-
-    def get_all_environments(self):
-        response = self.table.scan(
-            TableName=ENVIRONMENT_CONFIGURATION_TABLE,
-            AttributesToGet=[
-                'environment',
-            ],
-            Limit=10,
-            Select='SPECIFIC_ATTRIBUTES',
-            ScanFilter={},
-            ConsistentRead=True
-        )
-        return [env['environment'] for env in response['Items']]
-
-    def _env_config_exists(self):
-        response = self.table.get_item(
-            Key={
-                'environment': self.environment,
-            }
-        )
-        return response.get('Item') is not None
-
-    def _create_config(self):
-        log_warning(
-            "\nConfiguration for this environment was not found in DynamoDB.\
-            \nInitiating prompts for setting up configuration.\
-            \nIf this environment was previously configured, please ensure\
-            \ndefault region is the same as previously used. Otherwise, use\
-            \nthe same configuration.\n"
-        )
-        region = prompt("AWS region for environment", default='ap-south-1')
-        vpc_cidr = ipaddress.IPv4Network(prompt("VPC CIDR", default='10.10.10.10/16'))
-        nat_eip = prompt("Allocation ID Elastic IP for NAT")
-        public_subnet_1_cidr = prompt(
-            "Public Subnet 1 CIDR", default=list(vpc_cidr.subnets(new_prefix=22))[0])
-        public_subnet_2_cidr = prompt(
-            "Public Subnet 2 CIDR", default=list(vpc_cidr.subnets(new_prefix=22))[1])
-        private_subnet_1_cidr = prompt(
-            "Private Subnet 1 CIDR", default=list(vpc_cidr.subnets(new_prefix=22))[2])
-        private_subnet_2_cidr = prompt(
-            "Private Subnet 2 CIDR", default=list(vpc_cidr.subnets(new_prefix=22))[3])
-        cluster_min_instances = prompt("Min instances in cluster", default=1)
-        cluster_max_instances = prompt("Max instances in cluster", default=5)
-        cluster_instance_type = prompt("Instance type", default='m5.xlarge')
-        key_name = prompt("SSH key name")
-        notifications_arn = prompt("Notification SNS ARN")
-        ssl_certificate_arn = prompt("SSL certificate ARN")
-        environment_configuration = {self.environment: {
-            "region": region,
-            "vpc": {
-                "cidr": str(vpc_cidr),
-                "nat-gateway": {
-                    "elastic-ip-allocation-id": nat_eip
-                },
-                "subnets": {
-                    "public": {
-                        "subnet-1": {
-                            "cidr": str(public_subnet_1_cidr)
-                        },
-                        "subnet-2": {
-                            "cidr": str(public_subnet_2_cidr)
-                        }
-                    },
-                    "private": {
-                        "subnet-1": {
-                            "cidr": str(private_subnet_1_cidr)
-                        },
-                        "subnet-2": {
-                            "cidr": str(private_subnet_2_cidr)
-                        }
-                    }
-                }
-            },
-            "cluster": {
-                "min_instances": cluster_min_instances,
-                "max_instances": cluster_max_instances,
-                "instance_type": cluster_instance_type,
-                "key_name": key_name
-            },
-            "environment": {
-                "notifications_arn": notifications_arn,
-                "ssl_certificate_arn": ssl_certificate_arn
-            },
-        }, 'cloudlift_version': VERSION}
-        self._set_config(environment_configuration)
-        pass
+            from cloudlift.version import VERSION
+            current_configuration = self.get_config(VERSION)
 
-    def _edit_config(self):
-        '''
-            Open editor to update configuration
-        '''
-        try:
-            current_configuration = self.get_config()
-            previous_cloudlift_version = current_configuration.pop('cloudlift_version', None)
             updated_configuration = edit(
                 json.dumps(
                     current_configuration,
                     indent=4,
                     sort_keys=True,
                     cls=DecimalEncoder
                 )
             )
 
             if updated_configuration is None:
-                log_warning("No changes made.")
+                if self.new_service:
+                    self.set_config(current_configuration)
+                    log_warning("Using default configuration.")
+                else:
+                    log_warning("No changes made.")
             else:
                 updated_configuration = json.loads(updated_configuration)
                 differences = list(dictdiffer.diff(
                     current_configuration,
                     updated_configuration
                 ))
                 if not differences:
                     log_warning("No changes made.")
-                    updated_configuration['cloudlift_version']=VERSION
-                    self._set_config(updated_configuration)
-                    # self.update_cloudlift_version()
                 else:
                     print_json_changes(differences)
                     if confirm('Do you want update the config?'):
-                        self._set_config(updated_configuration)
-                        # self.update_cloudlift_version()
+                        self.set_config(updated_configuration)
                     else:
                         log_warning("Changes aborted.")
         except ClientError:
-            raise UnrecoverableException("Unable to fetch environment configuration from DynamoDB.")
+            raise UnrecoverableException("Unable to fetch service configuration from DynamoDB.")
 
-    def _set_config(self, config):
+    def get_config(self, cloudlift_version):
+        '''
+            Get configuration from DynamoDB
+        '''
+
+        try:
+            configuration_response = self.table.get_item(
+                Key={
+                    'service_name': self.service_name,
+                    'environment': self.environment
+                },
+                ConsistentRead=True,
+                AttributesToGet=[
+                    'configuration'
+                ]
+            )
+            if 'Item' in configuration_response:
+                existing_configuration = configuration_response['Item']['configuration']
+
+                from distutils.version import LooseVersion
+                previous_cloudlift_version = existing_configuration.pop("cloudlift_version", None)
+                if LooseVersion(cloudlift_version) < LooseVersion(previous_cloudlift_version):
+                    raise UnrecoverableException(f'Cloudlift Version {previous_cloudlift_version} was used to '
+                                                 f'create this service. You are using version {cloudlift_version}, '
+                                                 f'which is older and can cause corruption. Please upgrade to at least '
+                                                 f'version {previous_cloudlift_version} to proceed.\n\nUpgrade to the '
+                                                 f'latest version (Recommended):\n'
+                                                 f'\tpip install -U cloudlift\n\nOR\n\nUpgrade to a compatible version:\n'
+                                                 f'\tpip install -U cloudlift=={previous_cloudlift_version}')
+            else:
+                existing_configuration = self._default_service_configuration()
+                self.new_service = True
+
+            return existing_configuration
+        except ClientError:
+            raise UnrecoverableException("Unable to fetch service configuration from DynamoDB.")
+
+    def set_config(self, config):
         '''
             Set configuration in DynamoDB
         '''
-        self._validate_changes(config)
         config['cloudlift_version'] = VERSION
-        sns_arn = config[self.environment]['environment']['notifications_arn']
-        check_sns_topic_exists(sns_arn, self.environment)
-
+        self._validate_changes(config)
+        check_sns_topic_exists(config['notifications_arn'], self.environment)
         try:
             configuration_response = self.table.update_item(
-                TableName=ENVIRONMENT_CONFIGURATION_TABLE,
+                TableName=SERVICE_CONFIGURATION_TABLE,
                 Key={
+                    'service_name': self.service_name,
                     'environment': self.environment
                 },
                 UpdateExpression='SET configuration = :configuration',
                 ExpressionAttributeValues={
                     ':configuration': config
                 },
                 ReturnValues="UPDATED_NEW"
             )
             return configuration_response
         except ClientError:
-            raise UnrecoverableException("Unable to store environment configuration in DynamoDB.")
-        pass
+            raise UnrecoverableException("Unable to store service configuration in DynamoDB.")
 
     def update_cloudlift_version(self):
         '''
             Updates cloudlift version in service configuration
         '''
-        print(f"setting cloudlift version to {VERSION}")
         config = self.get_config(VERSION)
-        self._set_config(config)
+        self.set_config(config)
 
     def _validate_changes(self, configuration):
-        log_bold("\nValidating schema..")
-        # TODO: add cidr etc validation
-        schema = {
-            # "$schema": "http://json-schema.org/draft-04/schema#",
-            "title": "configuration",
+        service_schema = {
+            "title": "service",
             "type": "object",
             "properties": {
-                self.environment: {
+                "http_interface": {
                     "type": "object",
                     "properties": {
-                        "cluster": {
-                            "type": "object",
-                            "properties": {
-                                "min_instances": {"type": "integer"},
-                                "max_instances": {"type": "integer"},
-                                "instance_type": {"type": "string"},
-                                "key_name": {"type": "string"}
-                            },
-                            "required": [
-                                "min_instances",
-                                "max_instances",
-                                "instance_type",
-                                "key_name"
-                            ]
+                        "internal": {
+                            "type": "boolean"
+                        },
+                        "restrict_access_to": {
+                            "type": "array",
+                            "items": {
+                                "type": "string"
+                            }
                         },
-                        "environment": {
-                            "type": "object",
-                            "properties": {
-                                "notifications_arn": {"type": "string"},
-                                "ssl_certificate_arn": {"type": "string"}
-                            },
-                            "required": [
-                                "notifications_arn",
-                                "ssl_certificate_arn"
-                            ]
+                        "container_port": {
+                            "type": "number"
                         },
-                        "region": {"type": "string"},
-                        "vpc": {
-                            "type": "object",
-                            "properties": {
-                                "cidr": {
-                                    "type": "string"
-                                },
-                                "nat-gateway": {
-                                    "type": "object",
-                                    "properties": {
-                                        "elastic-ip-allocation-id": {
-                                            "type": "string"
-                                        }
-                                    },
-                                    "required": [
-                                        "elastic-ip-allocation-id"
-                                    ]
-                                },
-                                "subnets": {
-                                    "type": "object",
-                                    "properties": {
-                                        "private": {
-                                            "type": "object",
-                                            "properties": {
-                                                "subnet-1": {
-                                                    "type": "object",
-                                                    "properties": {
-                                                        "cidr": {
-                                                            "type": "string"
-                                                        }
-                                                    },
-                                                    "required": [
-                                                        "cidr"
-                                                    ]
-                                                },
-                                                "subnet-2": {
-                                                    "type": "object",
-                                                    "properties": {
-                                                        "cidr": {
-                                                            "type": "string"
-                                                        }
-                                                    },
-                                                    "required": [
-                                                        "cidr"
-                                                    ]
-                                                }
-                                            },
-                                            "required": [
-                                                "subnet-1",
-                                                "subnet-2"
-                                            ]
-                                        },
-                                        "public": {
-                                            "type": "object",
-                                            "properties": {
-                                                "subnet-1": {
-                                                    "type": "object",
-                                                    "properties": {
-                                                        "cidr": {
-                                                            "type": "string"
-                                                        }
-                                                    },
-                                                    "required": [
-                                                        "cidr"
-                                                    ]
-                                                },
-                                                "subnet-2": {
-                                                    "type": "object",
-                                                    "properties": {
-                                                        "cidr": {
-                                                            "type": "string"
-                                                        }
-                                                    },
-                                                    "required": [
-                                                        "cidr"
-                                                    ]
-                                                }
-                                            },
-                                            "required": [
-                                                "subnet-1",
-                                                "subnet-2"
-                                            ]
-                                        }
-                                    },
-                                    "required": [
-                                        "private",
-                                        "public"
-                                    ]
-                                }
-                            },
-                            "required": [
-                                "cidr",
-                                "nat-gateway",
-                                "subnets"
-                            ]
+                        "health_check_path": {
+                            "type": "string",
+                            "pattern": "^\/.*$"
                         }
-
                     },
                     "required": [
-                        "cluster",
-                        "environment",
-                        "region",
-                        "vpc"
+                        "internal",
+                        "restrict_access_to",
+                        "container_port"
+                    ]
+                },
+                "custom_metrics": {
+                    "type": "object",
+                    "properties": {
+                        "metrics_port" : {"type": "string"},
+                        "metrics_path": {"type": "string"}
+                    }
+                },
+                "volume": {
+                    "type": "object",
+                    "properties": {
+                        "efs_id" : {"type": "string"},
+                        "efs_directory_path" : {"type": "string"},
+                        "container_path" : {"type": "string"}
+                    }
+                },
+                "memory_reservation": {
+                    "type": "number",
+                    "minimum": 10,
+                    "maximum": 30000
+                },
+                "fargate": {
+                    "type": "object",
+                    "properties": {
+                        "cpu": {
+                            "type": "number",
+                            "minimum": 256,
+                            "maximum": 4096
+                        },
+                        "memory": {
+                            "type": "number",
+                            "minimum": 512,
+                            "maximum": 30720
+                        }
+                    }
+                },
+                "command": {
+                    "oneOf": [
+                        {"type": "string"},
+                        {"type": "null"}
+                    ]
+                },
+                "spot_deployment": {
+                    "type": "boolean"
+                },
+                "logging": {
+                    "oneOf": [
+                        {"type": "string", "pattern": "^(awslogs|fluentd|null)$"},
+                        {"type": "null"}
                     ]
                 }
             },
-            "required": [self.environment]
+            "required": ["memory_reservation", "command"]
+        }
+        schema = {
+            # "$schema": "http://json-schema.org/draft-04/schema#",
+            "title": "configuration",
+            "type": "object",
+            "properties": {
+                "notifications_arn": {
+                    "type": "string"
+                },
+                "services": {
+                    "type": "object",
+                    "patternProperties": {
+                        "^[a-zA-Z]+$": service_schema
+                    }
+                },
+                "cloudlift_version": {
+                    "type": "string"
+                }
+            },
+            "required": ["cloudlift_version", "services", "notifications_arn"]
         }
         try:
             validate(configuration, schema)
         except ValidationError as validation_error:
-            error_path = str(".".join(list(validation_error.relative_path)))
-            if error_path:
-                raise UnrecoverableException(validation_error.message + " in " + error_path)
+            if validation_error.relative_path:
+                raise UnrecoverableException(validation_error.message + " in " +
+                        str(".".join(list(validation_error.relative_path))))
             else:
                 raise UnrecoverableException(validation_error.message)
         log_bold("Schema valid!")
+
+    def _default_service_configuration(self):
+        return {
+            u'notifications_arn': None,
+            u'services': {
+                pascalcase(self.service_name): {
+                    u'http_interface': {
+                        u'internal': False,
+                        u'restrict_access_to': [u'0.0.0.0/0'],
+                        u'container_port': 80,
+                        u'health_check_path': u'/elb-check'
+                    },
+                    u'memory_reservation': 250,
+                    u'command': None,
+                    u'spot_deployment': False
+                }
+            }
+        }
```

### Comparing `cloudlift-1.5.7/cloudlift/config/logging.py` & `cloudlift-2.0.0/cloudlift/config/logging.py`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/cloudlift/config/mfa.py` & `cloudlift-2.0.0/cloudlift/config/mfa.py`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/cloudlift/config/parameter_store.py` & `cloudlift-2.0.0/cloudlift/config/parameter_store.py`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/cloudlift/config/region.py` & `cloudlift-2.0.0/cloudlift/config/region.py`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/cloudlift/deployment/changesets.py` & `cloudlift-2.0.0/cloudlift/deployment/changesets.py`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/cloudlift/deployment/cluster_template_generator.py` & `cloudlift-2.0.0/cloudlift/deployment/cluster_template_generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import json
 import re
 
 from cfn_flip import to_yaml
 from stringcase import camelcase, pascalcase
 from troposphere import (Base64, FindInMap, Output, Parameter, Ref, Sub,
                          cloudformation, Export, GetAtt, Tags)
-from troposphere.autoscaling import (AutoScalingGroup, LaunchTemplateSpecification,
-                                     ScalingPolicy)
+from troposphere.autoscaling import (AutoScalingGroup, LaunchTemplateSpecification, NotificationConfigurations,
+                                     ScalingPolicy, MixedInstancesPolicy, LaunchTemplateOverrides, InstancesDistribution )
+from troposphere.autoscaling import LaunchTemplate as ASGLaunchTemplate
 from troposphere.cloudwatch import Alarm, MetricDimension
 from troposphere.ec2 import (VPC, InternetGateway, NatGateway, Route,
                              RouteTable, SecurityGroup, Subnet,
                              SubnetRouteTableAssociation, VPCGatewayAttachment,SecurityGroupIngress,
                              LaunchTemplateData, LaunchTemplate, IamInstanceProfile, LaunchTemplateBlockDeviceMapping, EBSBlockDevice)
 from troposphere.ecs import Cluster
 from troposphere.elasticache import SubnetGroup as ElastiCacheSubnetGroup
@@ -21,28 +22,32 @@
 from troposphere.rds import DBSubnetGroup
 from troposphere.servicediscovery import PrivateDnsNamespace
 
 from cloudlift.config import DecimalEncoder
 from cloudlift.config import get_client_for, get_region_for_environment
 from cloudlift.deployment.template_generator import TemplateGenerator
 from cloudlift.version import VERSION
+from cloudlift.config.logging import log_warning
 
 
 class ClusterTemplateGenerator(TemplateGenerator):
     """
         This class generates CloudFormation template for a environment cluster
     """
 
     def __init__(self, environment, environment_configuration, desired_instances=None):
         super(ClusterTemplateGenerator, self).__init__(environment)
         self.configuration = environment_configuration
-        if desired_instances is None:
-            self.desired_instances = str(self.configuration['cluster']['min_instances'])
-        else:
-            self.desired_instances = str(desired_instances)
+        self.desired_instances = desired_instances
+        if not 'spot_min_instances' in self.configuration['cluster']:
+            self.configuration['cluster']['spot_min_instances'] = 0
+        if not 'spot_max_instances' in self.configuration['cluster']:
+            self.configuration['cluster']['spot_max_instances'] = 0
+        if not 'allocation_strategy' in self.configuration['cluster']:
+            self.configuration['cluster']['allocation_strategy'] = 'capacity-optimized'
         self.private_subnets = []
         self.public_subnets = []
         self._get_availability_zones()
         self.team_name = (self.notifications_arn.split(':')[-1])
 
     def generate_cluster(self):
         self.__validate_parameters()
@@ -332,32 +337,14 @@
         cluster = Cluster('Cluster', ClusterName=Ref('AWS::StackName'))
         self.template.add_resource(cluster)
         self._add_ec2_auto_scaling()
         self._add_cluster_alarms(cluster)
         return cluster
 
     def _add_cluster_alarms(self, cluster):
-        ec2_hosts_high_cpu_alarm = Alarm(
-            'Ec2HostsHighCPUAlarm',
-            EvaluationPeriods=1,
-            Dimensions=[
-                MetricDimension(Name='AutoScalingGroupName',
-                                Value=Ref(self.auto_scaling_group))
-            ],
-            AlarmActions=[Ref(self.notification_sns_arn)],
-            AlarmDescription='Alarm if CPU too high or metric disappears \
-indicating instance is down',
-            Namespace='AWS/EC2',
-            Period=60,
-            ComparisonOperator='GreaterThanThreshold',
-            Statistic='Average',
-            Threshold='60',
-            MetricName='CPUUtilization'
-        )
-        self.template.add_resource(ec2_hosts_high_cpu_alarm)
         cluster_high_cpu_alarm = Alarm(
             'ClusterHighCPUAlarm',
             EvaluationPeriods=1,
             Dimensions=[
                 MetricDimension(Name='ClusterName', Value=Ref(cluster))
             ],
             AlarmActions=[
@@ -386,48 +373,29 @@
             Period=300,
             ComparisonOperator='GreaterThanThreshold',
             Statistic='Average',
             Threshold='60',
             MetricName='MemoryUtilization'
         )
         self.template.add_resource(cluster_high_memory_alarm)
-        self.cluster_high_memory_reservation_autoscale_alarm = Alarm(
-            'ClusterHighMemoryReservationAlarm',
-            EvaluationPeriods=1,
-            Dimensions=[
-                MetricDimension(Name='ClusterName', Value=Ref(cluster))
-            ],
-            AlarmActions=[
-                Ref(self.cluster_scaling_policy)
-            ],
-            AlarmDescription='Alarm if memory reservation is over 75% \
-for cluster.',
-            Namespace='AWS/ECS',
-            Period=300,
-            ComparisonOperator='GreaterThanThreshold',
-            Statistic='Average',
-            Threshold='75',
-            MetricName='MemoryReservation'
-        )
-        self.template.add_resource(
-            self.cluster_high_memory_reservation_autoscale_alarm)
+
         self.cluster_high_memory_reservation_user_notification_alarm = Alarm(
             'ClusterHighMemoryReservationUserNotifcationAlarm',
             EvaluationPeriods=3,
             Dimensions=[
                 MetricDimension(Name='ClusterName', Value=Ref(cluster))
             ],
             AlarmActions=[
                 Ref(self.notification_sns_arn)
             ],
             OKActions=[
                 Ref(self.notification_sns_arn)
             ],
             AlarmDescription='Alarm if memory reservation is over 75% \
-for cluster for 15 minutes.',
+                for cluster for 15 minutes.',
             Namespace='AWS/ECS',
             Period=300,
             ComparisonOperator='GreaterThanThreshold',
             Statistic='Average',
             Threshold='75',
             MetricName='MemoryReservation'
         )
@@ -473,51 +441,58 @@
                     'IpProtocol': -1
                 }
             ],
             VpcId=Ref(self.vpc),
             GroupDescription=Sub("${AWS::StackName}-databases")
         )
         self.template.add_resource(database_security_group)
-        user_data = Base64(Sub('\n'.join([
-            "#!/bin/bash",
-            "yum update -y",
-            "yum install -y aws-cfn-bootstrap",
-            "/opt/aws/bin/cfn-init -v --region ${AWS::Region} --stack ${AWS::StackName} --resource LaunchTemplate",
-            "/opt/aws/bin/cfn-signal -e $? --region ${AWS::Region} --stack ${AWS::StackName} --resource AutoScalingGroup",
-            "yum install -y https://s3.amazonaws.com/ec2-downloads-windows/SSMAgent/latest/linux_amd64/amazon-ssm-agent.rpm",
-            "systemctl enable amazon-ssm-agent",
-            "systemctl start amazon-ssm-agent",
-            ""])))
-        lc_metadata = cloudformation.Init({
-            "config": cloudformation.InitConfig(
-                files=cloudformation.InitFiles({
-                    "/etc/cfn/cfn-hup.conf": cloudformation.InitFile(
-                        content=Sub(
-                            '\n'.join([
-                                    '[main]',
-                                    'stack=${AWS::StackId}',
-                                    'region=${AWS::Region}',
+        deployment_types = ['OnDemand', 'Spot']
+        for deployment_type in deployment_types:
+            lc_metadata_override = ''
+            if deployment_type == 'Spot':
+                lc_metadata_override = '\n'.join([
+                    'echo ECS_ENABLE_SPOT_INSTANCE_DRAINING=true >> /etc/ecs/ecs.config',
+                ])
+            user_data = Base64(Sub('\n'.join([
+                "#!/bin/bash",
+                "yum update -y",
+                "yum install -y aws-cfn-bootstrap",
+                "/opt/aws/bin/cfn-init -v --region ${AWS::Region} --stack ${AWS::StackName} --resource LaunchTemplate"+deployment_type,
+                "/opt/aws/bin/cfn-signal -e $? --region ${AWS::Region} --stack ${AWS::StackName} --resource AutoScalingGroup"+deployment_type,
+                "yum install -y https://s3.amazonaws.com/ec2-downloads-windows/SSMAgent/latest/linux_amd64/amazon-ssm-agent.rpm",
+                "systemctl enable amazon-ssm-agent",
+                "systemctl start amazon-ssm-agent",
+                ""])))
+            lc_metadata = cloudformation.Init({
+                "config": cloudformation.InitConfig(
+                    files=cloudformation.InitFiles({
+                        "/etc/cfn/cfn-hup.conf": cloudformation.InitFile(
+                            content=Sub(
+                                '\n'.join([
+                                        '[main]',
+                                        'stack=${AWS::StackId}',
+                                        'region=${AWS::Region}',
+                                        ''
+                                    ])
+                                ),
+                            mode='256',  # TODO: Why 256
+                            owner="root",
+                            group="root"
+                        ),
+                        "/etc/cfn/hooks.d/cfn-auto-reloader.conf": cloudformation.InitFile(
+                            content=Sub(
+                                '\n'.join([
+                                    '[cfn-auto-reloader-hook]',
+                                    'triggers=post.update',
+                                    'path=Resources.ContainerInstances.Metadata.AWS::CloudFormation::Init',
+                                    'action=/opt/aws/bin/cfn-init -v --region ${AWS::Region} --stack ${AWS::StackName} --resource LaunchTemplate'+deployment_type,
                                     ''
                                 ])
                             ),
-                        mode='256',  # TODO: Why 256
-                        owner="root",
-                        group="root"
-                    ),
-                    "/etc/cfn/hooks.d/cfn-auto-reloader.conf": cloudformation.InitFile(
-                        content=Sub(
-                            '\n'.join([
-                                '[cfn-auto-reloader-hook]',
-                                'triggers=post.update',
-                                'path=Resources.ContainerInstances.Metadata.AWS::CloudFormation::Init',
-                                'action=/opt/aws/bin/cfn-init -v --region ${AWS::Region} --stack ${AWS::StackName} --resource LaunchTemplate',
-                                ''
-                            ])
                         ),
-                    ),
                     "/etc/dnsmasq.conf": cloudformation.InitFile(
                         content=Sub(
                             '\n'.join([
                                 '# Server Configuration',
                                 'listen-address=127.0.0.1',
                                 'port=53',
                                 'bind-interfaces',
@@ -530,146 +505,229 @@
                                 'neg-ttl=60',
                                 'domain-needed',
                                 'bogus-priv',
                             ])
                         ),
                     )
                 }),
-                services={
-                    "sysvinit": cloudformation.InitServices({
-                        "cfn-hup": cloudformation.InitService(
-                            enabled=True,
-                            ensureRunning=True,
-                            files=['/etc/cfn/cfn-hup.conf',
-                                   '/etc/cfn/hooks.d/cfn-auto-reloader.conf']
-                        )
-                    })
-                },
-                commands={
-                    '01_add_instance_to_cluster': {
-                        'command': Sub(
-                            'echo "ECS_CLUSTER=${Cluster}\nECS_RESERVED_MEMORY=256" > /etc/ecs/ecs.config'
+                    services={
+                        "sysvinit": cloudformation.InitServices({
+                            "cfn-hup": cloudformation.InitService(
+                                enabled=True,
+                                ensureRunning=True,
+                                files=['/etc/cfn/cfn-hup.conf',
+                                    '/etc/cfn/hooks.d/cfn-auto-reloader.conf']
+                            )
+                        })
+                    },
+                    commands={
+                        '01_add_instance_to_cluster': {
+                            'command': Sub(
+                                '\n'.join([
+                                'echo ECS_CLUSTER=${Cluster} >> /etc/ecs/ecs.config',
+                                'echo ECS_RESERVED_MEMORY=256 >> /etc/ecs/ecs.config',
+                                'echo ECS_AVAILABLE_LOGGING_DRIVERS=\'["awslogs","fluentd"]\' >> /etc/ecs/ecs.config',
+                                'echo ECS_INSTANCE_ATTRIBUTES=\'{"deployment_type": "'+ deployment_type.lower() + '"}\' >> /etc/ecs/ecs.config',
+                                lc_metadata_override,
+                                ]).strip()
+                            )
+                        },
+                        '02_set_nameserver': {
+                            'command': "INTERFACE=$(curl --silent http://169.254.169.254/latest/meta-data/network/interfaces/macs/ | head -n1); IS_IT_CLASSIC=$(curl --write-out %{http_code} --silent --output /dev/null http://169.254.169.254/latest/meta-data/network/interfaces/macs/${INTERFACE}/vpc-id); if [[ $IS_IT_CLASSIC == '404' ]]; then bash -c \"echo 'supersede domain-name-servers 127.0.0.1, 172.16.0.23;' >> /etc/dhcp/dhclient.conf && echo 'nameserver 172.16.0.23' > /etc/resolv.dnsmasq\"; else  bash -c \"echo 'supersede domain-name-servers 127.0.0.1, 169.254.169.253;' >> /etc/dhcp/dhclient.conf && echo 'nameserver 169.254.169.253' > /etc/resolv.dnsmasq\"; fi"
+                        },
+                        '03_install_dnsmasq_package': {
+                            'command': 'yum install -y dnsmasq bind-utils'
+                        },
+                        '04_create_group': {
+                            'command': 'groupadd -r dnsmasq'
+                        },
+                        '05_create_user': {
+                            'command': 'useradd -r -g dnsmasq dnsmasq'
+                        },
+                        '06_add_locahost_nameserver': {
+                            'command': "sed -i '/search ap-south-1.compute.internal/a nameserver 127.0.0.1' /etc/resolv.conf"
+                        },
+                        '07_enable_dnsmasq_service': {
+                            'command': 'pidof systemd && systemctl restart dnsmasq.service || service dnsmasq restart'
+                        },
+                        '08_start_dnsmasq_service': {
+                            'command': 'pidof systemd && systemctl enable  dnsmasq.service || chkconfig dnsmasq on'
+                        },
+                        '09_configure_dhclient': {
+                            'command': 'bash -c "dhclient"'
+                        }
+            })})
+            launch_template_data = LaunchTemplateData(
+                'LaunchTemplateData',
+                UserData=user_data,
+                IamInstanceProfile=IamInstanceProfile(
+                    Arn=GetAtt(instance_profile, 'Arn')
+                ),
+                SecurityGroupIds=[GetAtt(self.sg_hosts, 'GroupId')],
+                ImageId=FindInMap("AWSRegionToAMI", Ref("AWS::Region"), "AMI"),
+                KeyName=Ref(self.key_pair),
+                BlockDeviceMappings=[
+                    LaunchTemplateBlockDeviceMapping(
+                        DeviceName="/dev/xvda",
+                        Ebs=EBSBlockDevice(
+                            VolumeType="gp3"
                         )
+                    )
+                ]
+            )
+            launch_template = LaunchTemplate(
+                "LaunchTemplate"+deployment_type,
+                LaunchTemplateData=launch_template_data,
+                LaunchTemplateName=self.env + "-LaunchTemplate"+deployment_type,
+                Metadata=lc_metadata
+            )
+            
+            overrides_instances = []
+            instance_types = self.configuration['cluster']['instance_type'].split(",")
+            if deployment_type == 'OnDemand':
+                overrides_instances.append(LaunchTemplateOverrides(InstanceType=str(instance_types[0])))
+            elif deployment_type == 'Spot':
+                for instance_type in instance_types:
+                    overrides_instances.append(LaunchTemplateOverrides(InstanceType=str(instance_type)))
+            # , PauseTime='PT15M', WaitOnResourceSignals=True, MaxBatchSize=1, MinInstancesInService=1)
+            up = AutoScalingRollingUpdate('AutoScalingRollingUpdate')
+            # TODO: clean up
+            subnets = list(self.private_subnets)
+            spot_instance_pools = {}
+            if 'allocation_strategy' in self.configuration['cluster'] and self.configuration['cluster']['allocation_strategy'] == 'lowest-price':
+                spot_instance_pools = {
+                    'SpotInstancePools' : self.configuration['cluster']['spot_instance_pools']
+                }
+            self.auto_scaling_group = AutoScalingGroup(
+                "AutoScalingGroup"+deployment_type,
+                UpdatePolicy=up,
+                DesiredCapacity=str(self.desired_instances if (self.desired_instances is not None) and self.desired_instances >= 1 else self.configuration['cluster']['min_instances'] if deployment_type == 'OnDemand' else self.configuration['cluster']['spot_min_instances']),
+                Tags=[
+                    {
+                        'PropagateAtLaunch': True,
+                        'Value': Sub('${AWS::StackName} - ECS Host'),
+                        'Key': 'Name'
                     },
-                    '02_set_nameserver': {
-                        'command': "INTERFACE=$(curl --silent http://169.254.169.254/latest/meta-data/network/interfaces/macs/ | head -n1); IS_IT_CLASSIC=$(curl --write-out %{http_code} --silent --output /dev/null http://169.254.169.254/latest/meta-data/network/interfaces/macs/${INTERFACE}/vpc-id); if [[ $IS_IT_CLASSIC == '404' ]]; then bash -c \"echo 'supersede domain-name-servers 127.0.0.1, 172.16.0.23;' >> /etc/dhcp/dhclient.conf && echo 'nameserver 172.16.0.23' > /etc/resolv.dnsmasq\"; else  bash -c \"echo 'supersede domain-name-servers 127.0.0.1, 169.254.169.253;' >> /etc/dhcp/dhclient.conf && echo 'nameserver 169.254.169.253' > /etc/resolv.dnsmasq\"; fi"
-                    },
-                    '03_install_dnsmasq_package': {
-                        'command': 'yum install -y dnsmasq bind-utils'
-                    },
-                    '04_create_group': {
-                        'command': 'groupadd -r dnsmasq'
-                    },
-                    '05_create_user': {
-                        'command': 'useradd -r -g dnsmasq dnsmasq'
-                    },
-                    '06_add_locahost_nameserver': {
-                        'command': "sed -i '/search ap-south-1.compute.internal/a nameserver 127.0.0.1' /etc/resolv.conf"
-                    },
-                    '07_enable_dnsmasq_service': {
-                        'command': 'pidof systemd && systemctl restart dnsmasq.service || service dnsmasq restart'
-                    },
-                    '08_start_dnsmasq_service': {
-                        'command': 'pidof systemd && systemctl enable  dnsmasq.service || chkconfig dnsmasq on'
+                    {
+                        'PropagateAtLaunch': True,
+                        'Key': 'environment',
+                        'Value': self.env
                     },
-                    '09_configure_dhclient': {
-                        'command': 'bash -c "dhclient"'
-                    }
-                }
-            )
-        })
-        launch_template_data = LaunchTemplateData(
-            'LaunchTemplateData',
-            UserData=user_data,
-            IamInstanceProfile=IamInstanceProfile(
-                Arn=GetAtt(instance_profile, 'Arn')
-            ),
-            SecurityGroupIds=[GetAtt(self.sg_hosts, 'GroupId')],
-            InstanceType=Ref('InstanceType'),
-            ImageId=FindInMap("AWSRegionToAMI", Ref("AWS::Region"), "AMI"),
-            KeyName=Ref(self.key_pair),
-            BlockDeviceMappings=[
-                LaunchTemplateBlockDeviceMapping(
-                    DeviceName="/dev/xvda",
-                    Ebs=EBSBlockDevice(
-                        VolumeType="gp3"
+                    {'PropagateAtLaunch': True, 'Key': 'Team',
+                        'Value': self.team_name}
+                ],
+                MinSize=Ref('OnDemandMinSize') if deployment_type == 'OnDemand' else Ref('SpotMinSize'),
+                MaxSize=Ref('OnDemandMaxSize') if deployment_type == 'OnDemand' else Ref('SpotMaxSize'),
+                VPCZoneIdentifier=[Ref(subnets.pop()), Ref(subnets.pop())],
+                NotificationConfigurations=[
+                    NotificationConfigurations(
+                        NotificationTypes=[
+                            "autoscaling:EC2_INSTANCE_LAUNCH_ERROR"],
+                        TopicARN=Ref(self.notification_sns_arn)
+                    )
+                ],
+                MixedInstancesPolicy=MixedInstancesPolicy(
+                    LaunchTemplate=ASGLaunchTemplate(
+                        LaunchTemplateSpecification=LaunchTemplateSpecification(
+                            LaunchTemplateId=Ref(launch_template),
+                            Version=GetAtt(launch_template, 'LatestVersionNumber')
+                        ),
+                        Overrides=overrides_instances
+                    ),
+                    InstancesDistribution=InstancesDistribution(
+                        OnDemandBaseCapacity=0,
+                        OnDemandPercentageAboveBaseCapacity=0 if deployment_type == 'Spot' else 100,
+                        SpotAllocationStrategy="capacity-optimized" if deployment_type == 'OnDemand' else self.configuration['cluster']['allocation_strategy'],
+                        **spot_instance_pools 
                     )
+                ),
+                CreationPolicy=CreationPolicy(
+                    ResourceSignal=ResourceSignal(Timeout='PT15M')
                 )
-            ]
-        )
-        launch_template = LaunchTemplate(
-            "LaunchTemplate",
-            LaunchTemplateData=launch_template_data,
-            Metadata=lc_metadata
-        )
-        self.template.add_resource(launch_template)
-        # , PauseTime='PT15M', WaitOnResourceSignals=True, MaxBatchSize=1, MinInstancesInService=1)
-        up = AutoScalingRollingUpdate('AutoScalingRollingUpdate')
-        # TODO: clean up
-        subnets = list(self.private_subnets)
-        self.auto_scaling_group = AutoScalingGroup(
-            "AutoScalingGroup",
-            UpdatePolicy=up,
-            DesiredCapacity=self.desired_instances,
-            Tags=[
-                {
-                    'PropagateAtLaunch': True,
-                    'Value': Sub('${AWS::StackName} - ECS Host'),
-                    'Key': 'Name'
-                },
-                {
-                    'PropagateAtLaunch': True,
-                    'Key': 'environment',
-                    'Value': self.env
-                },
-                {'PropagateAtLaunch': True, 'Key': 'Team', 'Value': self.team_name}
-            ],
-            MinSize=Ref('MinSize'),
-            MaxSize=Ref('MaxSize'),
-            VPCZoneIdentifier=[Ref(subnets.pop()), Ref(subnets.pop())],
-            LaunchTemplate=LaunchTemplateSpecification(
-                LaunchTemplateId=Ref(launch_template),
-                Version=GetAtt(launch_template, 'LatestVersionNumber')
-            ),
-            CreationPolicy=CreationPolicy(
-                ResourceSignal=ResourceSignal(Timeout='PT15M')
-            )
-        )
-        self.template.add_resource(self.auto_scaling_group)
-        self.cluster_scaling_policy = ScalingPolicy(
-            'AutoScalingPolicy',
-            AdjustmentType='ChangeInCapacity',
-            AutoScalingGroupName=Ref(self.auto_scaling_group),
-            Cooldown="300",
-            PolicyType='SimpleScaling',
-            ScalingAdjustment=1
-        )
-        self.template.add_resource(self.cluster_scaling_policy)
+            )
+            self.cluster_scaling_policy = ScalingPolicy(
+                'AutoScalingPolicy'+deployment_type,
+                AdjustmentType='ChangeInCapacity',
+                AutoScalingGroupName=Ref(self.auto_scaling_group),
+                Cooldown="300",
+                PolicyType='SimpleScaling',
+                ScalingAdjustment=1
+            )
+            ec2_hosts_high_cpu_alarm = Alarm(
+                'Ec2HostsHighCPUAlarm'+deployment_type,
+                EvaluationPeriods=1,
+                Dimensions=[
+                    MetricDimension(Name='AutoScalingGroupName',
+                                    Value=Ref(self.auto_scaling_group))
+                ],
+                AlarmActions=[Ref(self.notification_sns_arn)],
+                AlarmDescription='Alarm if CPU too high or metric disappears \
+                    indicating instance is down',
+                Namespace='AWS/EC2',
+                Period=60,
+                ComparisonOperator='GreaterThanThreshold',
+                Statistic='Average',
+                Threshold='60',
+                MetricName='CPUUtilization'
+            )
+            self.cluster_high_memory_reservation_autoscale_alarm = Alarm(
+                'ClusterHighMemoryReservationAlarm'+deployment_type,
+                EvaluationPeriods=1,
+                Dimensions=[
+                    MetricDimension(Name='ClusterName',
+                                    Value=Ref('AWS::StackName'))
+                ],
+                AlarmActions=[
+                    Ref(self.cluster_scaling_policy)
+                ],
+                AlarmDescription='Alarm if memory reservation is over 75% \
+                    for cluster.',
+                Namespace='AWS/ECS',
+                Period=300,
+                ComparisonOperator='GreaterThanThreshold',
+                Statistic='Average',
+                Threshold='75',
+                MetricName='MemoryReservation'
+            )
+            if 'spot_min_instances' in self.configuration['cluster'] and deployment_type == 'Spot' and self.configuration['cluster']['spot_min_instances'] == 0:
+                log_warning("Skipping spot fleet")
+            elif 'min_instances' in self.configuration['cluster'] and deployment_type == 'OnDemand' and self.configuration['cluster']['min_instances'] == 0:
+                log_warning("Skipping on-demand fleet")
+            else:
+                self.template.add_resource(launch_template)
+                self.template.add_resource(self.auto_scaling_group)
+                self.template.add_resource(ec2_hosts_high_cpu_alarm)
+                self.template.add_resource(self.cluster_scaling_policy)
+                self.template.add_resource(self.cluster_high_memory_reservation_autoscale_alarm)
 
     def _add_cluster_parameters(self):
         self.template.add_parameter(Parameter(
             "Environment",
             Description='',
             Type="String",
             Default="")
         )
         self.key_pair = Parameter(
             "KeyPair", Description='', Type="AWS::EC2::KeyPair::KeyName", Default="")
         self.template.add_parameter(self.key_pair)
         self.template.add_parameter(Parameter(
-            "MinSize", Description='', Type="String", Default=str(self.configuration['cluster']['min_instances'])))
+            "OnDemandMinSize", Description='', Type="String", Default=str(self.configuration['cluster']['min_instances'])))
+        self.template.add_parameter(Parameter(
+            "OnDemandMaxSize", Description='', Type="String", Default=str(self.configuration['cluster']['max_instances'])))
+        self.template.add_parameter(Parameter(
+            "SpotMinSize", Description='', Type="String", Default=str(self.configuration['cluster']['spot_min_instances'])))
         self.template.add_parameter(Parameter(
-            "MaxSize", Description='', Type="String", Default=str(self.configuration['cluster']['max_instances'])))
+            "SpotMaxSize", Description='', Type="String", Default=str(self.configuration['cluster']['spot_max_instances'])))
         self.notification_sns_arn = Parameter("NotificationSnsArn",
                                               Description='',
                                               Type="String",
                                               Default=self.notifications_arn)
         self.template.add_parameter(self.notification_sns_arn)
         self.template.add_parameter(Parameter(
-            "InstanceType", Description='', Type="String", Default=self.configuration['cluster']['instance_type']))
+            "InstanceTypes", Description='', Type="String", Default=str(self.configuration['cluster']['instance_type'])))
 
     def _add_mappings(self):
         # Pick from https://docs.aws.amazon.com/AmazonECS/latest/developerguide/al2ami.html
         ssm_client = get_client_for('ssm', self.env)
         ami_response = ssm_client.get_parameter(
             Name='/aws/service/ecs/optimized-ami/amazon-linux-2/recommended')
         ami_id = json.loads(ami_response['Parameter']['Value'])['image_id']
@@ -680,15 +738,17 @@
 
     def _add_cluster_outputs(self):
         self._add_stack_outputs()
         metadata = {
             'env': self.env,
             'min_instances': str(self.configuration['cluster']['min_instances']),
             'max_instances': str(self.configuration['cluster']['max_instances']),
-            'instance_type': self.configuration['cluster']['instance_type'],
+            'spot_min_instances': str(self.configuration['cluster']['spot_min_instances']),
+            'spot_max_instances': str(self.configuration['cluster']['spot_max_instances']),
+            'instance_types': self.configuration['cluster']['instance_type'],
             'key_name': self.configuration['cluster']['key_name'],
             'cloudlift_version': VERSION
         }
         self.template.add_output(Output(
             "CloudliftOptions",
             Description="Options used with cloudlift when building this cluster",
             Value=json.dumps(metadata))
@@ -716,36 +776,53 @@
             Value=Ref(public_subnets.pop()))
         )
         self.template.add_output(Output(
             "PublicSubnet2",
             Description="ID of the 2nd subnet",
             Value=Ref(public_subnets.pop()))
         )
-        self.template.add_output(Output(
-            "AutoScalingGroup",
-            Description="AutoScaling group for ECS container instances",
-            Value=Ref('AutoScalingGroup'))
-        )
+        if self.configuration['cluster']['spot_min_instances'] > 0:
+            self.template.add_output(Output(
+                "AutoScalingGroupSpot",
+                Description="Spot AutoScaling group for ECS container instances",
+                Value=Ref('AutoScalingGroupSpot'))
+            )
+        if self.configuration['cluster']['min_instances'] > 0:
+            self.template.add_output(Output(
+                "AutoScalingGroupOnDemand",
+                Description="On-Demand AutoScaling group for ECS container instances",
+                Value=Ref('AutoScalingGroupOnDemand'))
+            )
         self.template.add_output(Output(
             "SecurityGroupAlb",
             Description="Security group ID for ALB",
             Value=Ref('SecurityGroupAlb'))
         )
         self.template.add_output(Output(
             "MinInstances",
-            Description="Minimum instances in cluster",
+            Description="Minimum on-demand instances in cluster",
             Value=str(self.configuration['cluster']['min_instances']))
         )
         self.template.add_output(Output(
             "MaxInstances",
-            Description="Maximum instances in cluster",
+            Description="Maximum on-demand instances in cluster",
             Value=str(self.configuration['cluster']['max_instances']))
         )
         self.template.add_output(Output(
-            "InstanceType",
+            "SpotMinInstances",
+            Description="Minimum spot instances in cluster",
+            Value=str(self.configuration['cluster']['spot_min_instances']))
+        )
+        self.template.add_output(Output(
+            "SpotMaxInstances",
+            Description="Maximum spot instances in cluster",
+            Value=str(self.configuration['cluster']['spot_max_instances']))
+        )
+        self.template.add_output(Output(
+            "InstanceTypes",
             Description="EC2 instance type",
             Value=str(self.configuration['cluster']['instance_type']))
         )
         self.template.add_output(Output(
             "KeyName",
             Description="Key Pair name for accessing the instances",
             Value=str(self.configuration['cluster']['key_name']))
@@ -758,51 +835,66 @@
         )
         self.template.add_output(Output(
             "SecurityGroupEC2Host",
             Export=Export("{self.env}Ec2Host".format(**locals())),
             Description="EC2Host Security group ID",
             Value=Ref('SecurityGroupEc2Hosts'))
         )
+        if 'ecs_instance_default_lifecycle_type' in self.configuration['cluster']:
+            self.template.add_output(Output(
+                "ECSClusterDefaultInstanceLifecycle",
+                Export=Export("{self.env}ECSClusterDefaultInstanceLifecycle".format(**locals())),
+                Description="Default instance type for ECS cluster",
+                Value=str(self.configuration['cluster']['ecs_instance_default_lifecycle_type']))
+            )
 
 
     def _add_metadata(self):
         self.template.set_metadata({
             'AWS::CloudFormation::Interface': {
                 'ParameterGroups': [
                     {
                         'Label': {
                             'default': 'Cluster Configuration'
                         },
                         'Parameters': [
                             'KeyPair',
                             'Environment',
-                            'MinSize',
-                            'MaxSize',
-                            'InstanceType',
+                            'OnDemandMinSize',
+                            'OnDemandMaxSize',
+                            'SpotMinSize',
+                            'SpotMaxSize',
+                            'InstanceTypes',
                             'VPC',
                             'Subnet1',
                             'Subnet2',
                             'NotificationSnsArn'
                         ]
                     },
                 ],
                 'ParameterLabels': {
                     'Environment': {
                         'default': 'Enter the environment e.g. dev or staging or sandbox or production'
                     },
-                    'InstanceType': {
+                    'InstanceTypes': {
                         'default': 'Type of instance'
                     },
                     'KeyPair': {
                         'default': 'Select the key with which you want to login to the ec2 instances'},
-                    'MaxSize': {
-                        'default': 'Max. no. of instances in cluster'
+                    'SpotMaxSize': {
+                        'default': 'Max. no. of instances in Spot cluster'
+                    },
+                    'SpotMinSize': {
+                        'default': 'Min. no. of instances in Spot cluster'
+                    },
+                    'OnDemandMinSize': {
+                        'default': 'Min. no. of instances in On-Demand cluster'
                     },
-                    'MinSize': {
-                        'default': 'Min. no. of instances in cluster'
+                    'OnDemandMaxSize': {
+                        'default': 'Max. no. of instances in On-Demand cluster'
                     },
                     'NotificationSnsArn': {
                         'default': 'The SNS topic to which notifications has to be triggered'
                     },
                     'Subnet1': {
                         'default': 'Enter the ID of the 1st subnet'
                     },
```

### Comparing `cloudlift-1.5.7/cloudlift/deployment/deployer.py` & `cloudlift-2.0.0/cloudlift/deployment/deployer.py`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/cloudlift/deployment/ecr_client.py` & `cloudlift-2.0.0/cloudlift/deployment/ecr_client.py`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/cloudlift/deployment/ecs.py` & `cloudlift-2.0.0/cloudlift/deployment/ecs.py`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/cloudlift/deployment/editor.py` & `cloudlift-2.0.0/cloudlift/deployment/editor.py`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/cloudlift/deployment/environment_creator.py` & `cloudlift-2.0.0/cloudlift/deployment/environment_creator.py`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/cloudlift/deployment/progress.py` & `cloudlift-2.0.0/cloudlift/deployment/progress.py`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/cloudlift/deployment/service_creator.py` & `cloudlift-2.0.0/cloudlift/deployment/service_creator.py`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/cloudlift/deployment/service_information_fetcher.py` & `cloudlift-2.0.0/cloudlift/deployment/service_information_fetcher.py`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/cloudlift/deployment/service_template_generator.py` & `cloudlift-2.0.0/cloudlift/deployment/service_template_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,23 +14,24 @@
 from troposphere import GetAtt, Output, Parameter, Ref, Sub, ImportValue, Tags
 from troposphere.cloudwatch import Alarm, MetricDimension
 from troposphere.ec2 import SecurityGroup
 from troposphere.ecs import (AwsvpcConfiguration, ContainerDefinition,
                              DeploymentConfiguration, Secret, MountPoint,
                              LoadBalancer, LogConfiguration, Volume, EFSVolumeConfiguration,
                              NetworkConfiguration, PlacementStrategy,
-                             PortMapping, Service, TaskDefinition, ServiceRegistry)
+                             PortMapping, Service, TaskDefinition, ServiceRegistry, PlacementConstraint)
 from troposphere.elasticloadbalancingv2 import Action, Certificate, Listener
 from troposphere.elasticloadbalancingv2 import LoadBalancer as ALBLoadBalancer
 from troposphere.elasticloadbalancingv2 import (Matcher, RedirectConfig,
                                                 TargetGroup,
                                                 TargetGroupAttribute)
 from troposphere.iam import Role
 from troposphere.servicediscovery import Service as SD
 from troposphere.servicediscovery import DnsConfig, DnsRecord
+from troposphere.events import Rule, Target
 
 from cloudlift.config import region as region_service
 from cloudlift.config import get_account_id
 from cloudlift.config import DecimalEncoder, VERSION
 from cloudlift.config import get_service_stack_name
 from cloudlift.deployment.deployer import build_config
 from cloudlift.deployment.ecs import DeployAction, EcsClient
@@ -97,14 +98,44 @@
             return to_yaml(self.template.to_json()), 'TemplateBody', ''
 
     def _add_cluster_services(self):
         for ecs_service_name, config in self.configuration['services'].items():
             self._add_service(ecs_service_name, config)
 
     def _add_service_alarms(self, svc):
+        oom_event_rule = Rule(
+            'EcsOOM' + str(svc.name),
+            Description="Triggered when an Amazon ECS Task is stopped",
+            EventPattern={
+                "detail-type": ["ECS Task State Change"],
+                "source": ["aws.ecs"],
+                "detail": {
+                    "clusterArn": [{"anything-but": [str(self.cluster_name)]}],
+                    "containers": {
+                        "reason": [{
+                            "prefix": "OutOfMemory"
+                        }]
+                    },
+                    "desiredStatus": ["STOPPED"],
+                    "lastStatus": ["STOPPED"],
+                    "taskDefinitionArn": [{
+                        "anything-but": [str(svc.name) + "Family"]
+                    }]
+                }
+            },
+            State="ENABLED",
+            Targets=[Target(
+                    Arn=Ref(self.notification_sns_arn),
+                    Id="ECSOOMStoppedTasks",
+                    InputPath="$.detail.containers[0]"
+                )
+            ]
+        )
+        self.template.add_resource(oom_event_rule)
+
         ecs_high_cpu_alarm = Alarm(
             'EcsHighCPUAlarm' + str(svc.name),
             EvaluationPeriods=1,
             Dimensions=[
                 MetricDimension(
                     Name='ClusterName',
                     Value=self.cluster_name
@@ -189,38 +220,57 @@
         container_definition_arguments = {
             "Secrets": [
                 Secret(Name=k, ValueFrom=v) for (k, v) in env_config
             ],
             "Name": service_name + "Container",
             "Image": self.ecr_image_uri + ':' + self.current_version,
             "Essential": 'true',
-            "Memory": int(config['memory_reservation']) + -(-(int(config['memory_reservation']) * 50 )//100), # Celling the value
-            "MemoryReservation": int(config['memory_reservation']),
             "Cpu": 0
         }
+        placement_constraint = {}
+        for key in self.environment_stack["Outputs"]:
+            if key["OutputKey"] == 'ECSClusterDefaultInstanceLifecycle':
+                spot_deployment = False if ImportValue("{self.env}ECSClusterDefaultInstanceLifecycle".format(**locals())) == 'ondemand' else True
+                placement_constraint = {
+                    "PlacementConstraints": [PlacementConstraint(
+                        Type='memberOf',
+                        Expression='attribute:deployment_type == spot' if spot_deployment else 'attribute:deployment_type == ondemand'
+                    )],
+                }
+        if 'spot_deployment' in config:
+            spot_deployment = config["spot_deployment"]
+            placement_constraint = {
+                "PlacementConstraints" : [PlacementConstraint(
+                    Type='memberOf',
+                    Expression='attribute:deployment_type == spot' if spot_deployment else 'attribute:deployment_type == ondemand'
+                )],
+            }
 
         if 'http_interface' in config:
             container_definition_arguments['PortMappings'] = [
                 PortMapping(
                     ContainerPort=int(
                         config['http_interface']['container_port']
                     )
                 )
             ]
-        if 'logging' not in config or 'logging' in config and config['logging']:
-            container_definition_arguments['LogConfiguration'] = self._gen_log_config(service_name)
+        if 'logging' not in config or 'logging' in config and config['logging'] is not None:
+            container_definition_arguments['LogConfiguration'] = self._gen_log_config(service_name, "awslogs" if 'logging' not in config else config['logging'])
 
         if config['command'] is not None:
             container_definition_arguments['Command'] = [config['command']]
 
         if 'volume' in config:
             container_definition_arguments['MountPoints'] = [MountPoint(
                 SourceVolume=service_name + '-efs-volume',
                 ContainerPath=config['volume']['container_path']
             )]
+        if launch_type == self.LAUNCH_TYPE_EC2:
+            container_definition_arguments['MemoryReservation'] = int(config['memory_reservation'])
+            container_definition_arguments['Memory'] = int(config['memory_reservation']) + -(-(int(config['memory_reservation']) * 50 )//100) # Celling the value
 
         cd = ContainerDefinition(**container_definition_arguments)
 
         task_role = self.template.add_resource(Role(
             service_name + "Role",
             AssumeRolePolicyDocument=PolicyDocument(
                 Statement=[
@@ -233,15 +283,14 @@
             )
         ))
 
         launch_type_td = {}
         if launch_type == self.LAUNCH_TYPE_FARGATE:
             launch_type_td = {
                 'RequiresCompatibilities': ['FARGATE'],
-                'ExecutionRoleArn': boto3.resource('iam').Role('ecsTaskExecutionRole').arn,
                 'NetworkMode': 'awsvpc',
                 'Cpu': str(config['fargate']['cpu']),
                 'Memory': str(config['fargate']['memory'])
             }
 
         if 'custom_metrics' in config:
             launch_type_td['NetworkMode'] = 'awsvpc'
@@ -364,15 +413,16 @@
                 LoadBalancers=[lb],
                 Cluster=self.cluster_name,
                 TaskDefinition=Ref(td),
                 DesiredCount=desired_count,
                 DependsOn=service_listener.title,
                 LaunchType=launch_type,
                 **launch_type_svc,
-                Tags=Tags(Team=self.team_name, environment=self.env)
+                Tags=Tags(Team=self.team_name, environment=self.env),
+                **placement_constraint
             )
             self.template.add_output(
                 Output(
                     service_name + 'EcsServiceName',
                     Description='The ECS name which needs to be entered',
                     Value=GetAtt(svc, 'Name')
                 )
@@ -463,35 +513,50 @@
                 service_name,
                 Cluster=self.cluster_name,
                 TaskDefinition=Ref(td),
                 DesiredCount=desired_count,
                 DeploymentConfiguration=deployment_configuration,
                 LaunchType=launch_type,
                 **launch_type_svc,
-                Tags=Tags(Team=self.team_name, environment=self.env)
+                Tags=Tags(Team=self.team_name, environment=self.env),
+                **placement_constraint
             )
             self.template.add_output(
                 Output(
                     service_name + 'EcsServiceName',
                     Description='The ECS name which needs to be entered',
                     Value=GetAtt(svc, 'Name')
                 )
             )
             self.template.add_resource(svc)
         self._add_service_alarms(svc)
 
-    def _gen_log_config(self, service_name):
-        return LogConfiguration(
-            LogDriver="awslogs",
-            Options={
-                'awslogs-stream-prefix': service_name,
-                'awslogs-group': '-'.join([self.env, 'logs']),
-                'awslogs-region': self.region
-            }
-        )
+    def _gen_log_config(self, service_name, config):
+        if config == 'awslogs':
+            return LogConfiguration(
+                LogDriver="awslogs",
+                Options={
+                    'awslogs-stream-prefix': service_name,
+                    'awslogs-group': '-'.join([self.env, 'logs']),
+                    'awslogs-region': self.region
+                }
+            )
+        elif config == 'fluentd':
+            return LogConfiguration(
+                LogDriver="fluentd",
+                Options={
+                    'fluentd-address': 'unix:///var/run/fluent.sock',
+                    'labels': 'com.amazonaws.ecs.cluster,com.amazonaws.ecs.container-name,com.amazonaws.ecs.task-arn,com.amazonaws.ecs.task-definition-family,com.amazonaws.ecs.task-definition-version',
+                    'fluentd-async': 'true'
+                }
+            )
+        elif config == 'null':
+            return LogConfiguration(
+                LogDriver="none"
+            )
 
     def _add_alb(self, cd, service_name, config, launch_type):
         sg_name = 'SG' + self.env + service_name
         svc_alb_sg = SecurityGroup(
             re.sub(r'\W+', '', sg_name),
             GroupName=self.env + '-' + service_name,
             SecurityGroupIngress=self._generate_alb_security_group_ingress(
```

### Comparing `cloudlift-1.5.7/cloudlift/deployment/service_updater.py` & `cloudlift-2.0.0/cloudlift/deployment/service_updater.py`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/cloudlift/deployment/task_definition_creator.py` & `cloudlift-2.0.0/cloudlift/deployment/task_definition_creator.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
                              TaskDefinition)
 from troposphere.iam import Role
 from botocore.exceptions import ClientError
 
 from cloudlift.config.logging import log_bold, log_intent, log_warning
 from cloudlift.deployment import EcrClient, UnrecoverableException, EcsClient, DeployAction, EcsTaskDefinition
 from cloudlift.deployment.deployer import build_config, print_task_diff
-from cloudlift.config import get_client_for
+from cloudlift.config import get_client_for, get_resource_for
 from cloudlift.exceptions import UnrecoverableException
 
 
 def _complete_image_url(ecr_client: EcrClient):
     return ecr_client.ecr_image_uri + ':' + ecr_client.version
 
 
@@ -24,14 +24,15 @@
     def __init__(self, name, environment, version, build_args, region='ap-south-1'):
         self.name = name
         self.environment = environment
         self.build_args = build_args
         self.region = region
         self.version = version
         self.client = get_client_for('iam', self.environment)
+        self.resource = get_resource_for('iam', self.environment)
         self.env_sample_file = './env.sample'
         self.cluster_name = f'cluster-{self.environment}'
         self.name_with_env = f"{pascalcase(self.name)}{pascalcase(self.environment)}"
 
     def create(self):
         log_warning("Create task definition to {self.region}".format(**locals()))
         if not os.path.exists(self.env_sample_file):
@@ -53,36 +54,18 @@
             ],
             "name": pascalcase(self.name) + "Container",
             "image": _complete_image_url(ecr_client),
             "essential": True,
             "logConfiguration": self._gen_log_config(pascalcase(self.name)),
             "memoryReservation": 1024
         }
-
-        task_role = dumps({
-            "Version": "2012-10-17",
-            "Statement": {
-                "Effect": "Allow",
-                "Principal": {
-                    "Service": "ecs-tasks.amazonaws.com"
-                },
-                "Action": "sts:AssumeRole"
-            }
-        })
-        try:
-            create_task_role = self.client.create_role(RoleName=self.name_with_env + "Role", AssumeRolePolicyDocument=task_role)
-            task_role_arn = create_task_role["Role"]["Arn"]
-        except ClientError as boto_client_error:
-            error_code = boto_client_error.response['Error']['Code']
-            if error_code == 'EntityAlreadyExists':
-                task_role_arn = self.name_with_env + "Role"
-            else:
-                raise boto_client_error
+        task_role_arn = self._task_role()
         ecs_client = EcsClient(region=self.region)
-        ecs_client.register_task_definition(self._task_defn_family(), [container_definition_arguments], [], task_role_arn, None)
+        execution_role_arn = self.resource.Role('ecsTaskExecutionRole').arn
+        ecs_client.register_task_definition(self._task_defn_family(), [container_definition_arguments], [], task_role_arn, False, False, execution_role_arn)
         log_bold("Task definition successfully created\n")
 
     def update(self):
         log_warning("Update task definition to {self.region}".format(**locals()))
         if not os.path.exists(self.env_sample_file):
             raise UnrecoverableException('env.sample not found. Exiting.')
         ecr_client = EcrClient(self.name, self.region, self.build_args)
@@ -110,22 +93,45 @@
                                               deployment: DeployAction):
         current_task_defn = self._current_task_defn(ecs_client, deployment)
         container_name = current_task_defn['containerDefinitions'][0]['name']
         current_task_defn.set_images(
             ecr_client.version,
             **{container_name: _complete_image_url(ecr_client)}
         )
+        if "taskRoleArn" not in current_task_defn:
+            current_task_defn["taskRoleArn"] = self._task_role()
         for container in current_task_defn.containers:
             current_task_defn.apply_container_environment(container, env_config)
         print_task_diff(self.name, current_task_defn.diff, 'white')
         return current_task_defn
 
     def _task_defn_family(self):
         return f"{self.name_with_env}Family"
 
+    def _task_role(self):
+        task_role = dumps({
+            "Version": "2012-10-17",
+            "Statement": {
+                "Effect": "Allow",
+                "Principal": {
+                    "Service": "ecs-tasks.amazonaws.com"
+                },
+                "Action": "sts:AssumeRole"
+            }
+        })
+        try:
+            create_task_role = self.client.create_role(RoleName=self.name_with_env + "Role", AssumeRolePolicyDocument=task_role)
+            return create_task_role["Role"]["Arn"]
+        except ClientError as boto_client_error:
+            error_code = boto_client_error.response['Error']['Code']
+            if error_code == 'EntityAlreadyExists':
+                return self.name_with_env + "Role"
+            else:
+                raise boto_client_error
+
     def _gen_log_config(self, stream_prefix):
         return {
             'logDriver': 'awslogs',
             'options': {
                 'awslogs-stream-prefix': stream_prefix,
                 'awslogs-group': '-'.join([self.environment, 'logs']),
                 'awslogs-region': self.region
```

### Comparing `cloudlift-1.5.7/cloudlift/deployment/template_generator.py` & `cloudlift-2.0.0/cloudlift/deployment/template_generator.py`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/cloudlift/session/session_creator.py` & `cloudlift-2.0.0/cloudlift/session/session_creator.py`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/cloudlift.egg-info/SOURCES.txt` & `cloudlift-2.0.0/cloudlift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/setup.py` & `cloudlift-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `cloudlift-1.5.7/test/test_cloudlift.py` & `cloudlift-2.0.0/test/test_cloudlift.py`

 * *Files identical despite different names*

