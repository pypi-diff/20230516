# Comparing `tmp/hsfs-3.2.0rc1.tar.gz` & `tmp/hsfs-3.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsfs-3.2.0rc1.tar", last modified: Wed May  3 08:10:55 2023, max compression
+gzip compressed data, was "hsfs-3.2.0rc2.tar", last modified: Tue May 16 16:17:35 2023, max compression
```

## Comparing `hsfs-3.2.0rc1.tar` & `hsfs-3.2.0rc2.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0     1006     1006        0 2023-05-03 08:10:55.312981 hsfs-3.2.0rc1/
--rw-r--r--   0     1006     1006       40 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/MANIFEST.in
--rw-r--r--   0     1006     1006     7714 2023-05-03 08:10:55.312981 hsfs-3.2.0rc1/PKG-INFO
--rw-r--r--   0     1006     1006     5539 2023-05-03 08:10:53.000000 hsfs-3.2.0rc1/README.md
-drwxr-xr-x   0     1006     1006        0 2023-05-03 08:10:55.292981 hsfs-3.2.0rc1/hsfs/
--rw-r--r--   0     1006     1006     1182 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/__init__.py
-drwxr-xr-x   0     1006     1006        0 2023-05-03 08:10:55.296981 hsfs-3.2.0rc1/hsfs/client/
--rw-r--r--   0     1006     1006     1694 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/client/__init__.py
--rw-r--r--   0     1006     1006     1132 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/client/auth.py
--rw-r--r--   0     1006     1006     6622 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/client/base.py
--rw-r--r--   0     1006     1006     2090 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/client/exceptions.py
--rw-r--r--   0     1006     1006    11621 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/client/external.py
--rw-r--r--   0     1006     1006     7924 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/client/hopsworks.py
--rw-r--r--   0     1006     1006     1536 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/code.py
--rw-r--r--   0     1006     1006    18899 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/connection.py
-drwxr-xr-x   0     1006     1006        0 2023-05-03 08:10:55.300981 hsfs-3.2.0rc1/hsfs/constructor/
--rw-r--r--   0     1006     1006      605 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/constructor/__init__.py
--rw-r--r--   0     1006     1006     1261 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/constructor/external_feature_group_alias.py
--rw-r--r--   0     1006     1006     5106 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/constructor/filter.py
--rw-r--r--   0     1006     1006     2981 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/constructor/fs_query.py
--rw-r--r--   0     1006     1006     1731 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/constructor/hudi_feature_group_alias.py
--rw-r--r--   0     1006     1006     2157 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/constructor/join.py
--rw-r--r--   0     1006     1006     1577 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/constructor/prepared_statement_parameter.py
--rw-r--r--   0     1006     1006    20138 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/constructor/query.py
--rw-r--r--   0     1006     1006     3331 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/constructor/serving_prepared_statement.py
-drwxr-xr-x   0     1006     1006        0 2023-05-03 08:10:55.312981 hsfs-3.2.0rc1/hsfs/core/
--rw-r--r--   0     1006     1006      605 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/__init__.py
--rw-r--r--   0     1006     1006     3688 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/builtin_transformation_function.py
--rw-r--r--   0     1006     1006     1853 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/code_api.py
--rw-r--r--   0     1006     1006     3292 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/code_engine.py
--rw-r--r--   0     1006     1006     3509 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/dataset_api.py
--rw-r--r--   0     1006     1006     1030 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/deltastreamer_jobconf.py
--rw-r--r--   0     1006     1006     1609 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/execution.py
--rw-r--r--   0     1006     1006     5396 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/expectation_api.py
--rw-r--r--   0     1006     1006     2632 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/expectation_engine.py
--rw-r--r--   0     1006     1006     6356 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/expectation_suite_api.py
--rw-r--r--   0     1006     1006     4002 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/expectation_suite_engine.py
--rw-r--r--   0     1006     1006     9792 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/explicit_provenance.py
--rw-r--r--   0     1006     1006     5418 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/core/external_feature_group_engine.py
--rw-r--r--   0     1006     1006    13334 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/feature_group_api.py
--rw-r--r--   0     1006     1006     6610 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/core/feature_group_base_engine.py
--rw-r--r--   0     1006     1006    13164 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/core/feature_group_engine.py
--rw-r--r--   0     1006     1006     1238 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/feature_store_api.py
--rw-r--r--   0     1006     1006     9739 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/feature_view_api.py
--rw-r--r--   0     1006     1006    24896 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/core/feature_view_engine.py
--rw-r--r--   0     1006     1006     5024 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/core/great_expectation_engine.py
--rw-r--r--   0     1006     1006      828 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/hosts_api.py
--rw-r--r--   0     1006     1006    11546 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/hudi_engine.py
--rw-r--r--   0     1006     1006     1211 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/ingestion_job.py
--rw-r--r--   0     1006     1006     2262 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/ingestion_job_conf.py
--rw-r--r--   0     1006     1006     1077 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/inode.py
--rw-r--r--   0     1006     1006     2906 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/core/job.py
--rw-r--r--   0     1006     1006     2004 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/core/job_api.py
--rw-r--r--   0     1006     1006     2048 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/job_configuration.py
--rw-r--r--   0     1006     1006     1530 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/kafka_api.py
--rw-r--r--   0     1006     1006      898 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/project_api.py
--rw-r--r--   0     1006     1006     1093 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/query_constructor_api.py
--rw-r--r--   0     1006     1006      875 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/services_api.py
--rw-r--r--   0     1006     1006     4204 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/statistics_api.py
--rw-r--r--   0     1006     1006     8159 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/statistics_engine.py
--rw-r--r--   0     1006     1006     2325 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/storage_connector_api.py
--rw-r--r--   0     1006     1006     4696 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/tags_api.py
--rw-r--r--   0     1006     1006     6685 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/training_dataset_api.py
--rw-r--r--   0     1006     1006     6357 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/training_dataset_engine.py
--rw-r--r--   0     1006     1006     2148 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/training_dataset_job_conf.py
--rw-r--r--   0     1006     1006     4161 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/core/transformation_function_api.py
--rw-r--r--   0     1006     1006    14792 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/transformation_function_engine.py
--rw-r--r--   0     1006     1006     4773 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/validation_report_api.py
--rw-r--r--   0     1006     1006     3640 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/validation_report_engine.py
--rw-r--r--   0     1006     1006     2158 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/validation_result_api.py
--rw-r--r--   0     1006     1006     5469 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/validation_result_engine.py
--rw-r--r--   0     1006     1006     1261 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/core/variable_api.py
--rw-r--r--   0     1006     1006    18519 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/core/vector_server.py
--rw-r--r--   0     1006     1006     1655 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/decorators.py
-drwxr-xr-x   0     1006     1006        0 2023-05-03 08:10:55.312981 hsfs-3.2.0rc1/hsfs/engine/
--rw-r--r--   0     1006     1006     2244 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/engine/__init__.py
--rw-r--r--   0     1006     1006    46808 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/engine/python.py
--rw-r--r--   0     1006     1006    42820 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/engine/spark.py
--rw-r--r--   0     1006     1006    21585 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/expectation_suite.py
--rw-r--r--   0     1006     1006     6857 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/feature.py
--rw-r--r--   0     1006     1006   110708 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/feature_group.py
--rw-r--r--   0     1006     1006     3424 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/feature_group_commit.py
--rw-r--r--   0     1006     1006     1986 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/feature_group_writer.py
--rw-r--r--   0     1006     1006    62935 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/feature_store.py
--rw-r--r--   0     1006     1006    95713 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/feature_view.py
--rw-r--r--   0     1006     1006     4822 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/ge_expectation.py
--rw-r--r--   0     1006     1006     8633 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/ge_validation_result.py
--rw-r--r--   0     1006     1006     1450 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/split_statistics.py
--rw-r--r--   0     1006     1006     2893 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/statistics.py
--rw-r--r--   0     1006     1006     3313 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/statistics_config.py
--rw-r--r--   0     1006     1006    39092 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/storage_connector.py
--rw-r--r--   0     1006     1006     1850 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/tag.py
--rw-r--r--   0     1006     1006    35625 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/training_dataset.py
--rw-r--r--   0     1006     1006     3542 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/training_dataset_feature.py
--rw-r--r--   0     1006     1006     2759 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/training_dataset_split.py
--rw-r--r--   0     1006     1006     8929 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/transformation_function.py
--rw-r--r--   0     1006     1006     2179 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/transformation_function_attached.py
--rw-r--r--   0     1006     1006     3491 2023-03-13 10:42:53.000000 hsfs-3.2.0rc1/hsfs/user.py
--rw-r--r--   0     1006     1006    11410 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/util.py
--rw-r--r--   0     1006     1006     7519 2023-05-03 07:54:47.000000 hsfs-3.2.0rc1/hsfs/validation_report.py
--rw-r--r--   0     1006     1006      631 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/hsfs/version.py
-drwxr-xr-x   0     1006     1006        0 2023-05-03 08:10:55.296981 hsfs-3.2.0rc1/hsfs.egg-info/
--rw-r--r--   0     1006     1006     7714 2023-05-03 08:10:54.000000 hsfs-3.2.0rc1/hsfs.egg-info/PKG-INFO
--rw-r--r--   0     1006     1006     2805 2023-05-03 08:10:55.000000 hsfs-3.2.0rc1/hsfs.egg-info/SOURCES.txt
--rw-r--r--   0     1006     1006        1 2023-05-03 08:10:54.000000 hsfs-3.2.0rc1/hsfs.egg-info/dependency_links.txt
--rw-r--r--   0     1006     1006      679 2023-05-03 08:10:54.000000 hsfs-3.2.0rc1/hsfs.egg-info/requires.txt
--rw-r--r--   0     1006     1006        5 2023-05-03 08:10:54.000000 hsfs-3.2.0rc1/hsfs.egg-info/top_level.txt
--rw-r--r--   0     1006     1006       38 2023-05-03 08:10:55.312981 hsfs-3.2.0rc1/setup.cfg
--rw-r--r--   0     1006     1006     2756 2023-05-03 08:10:49.000000 hsfs-3.2.0rc1/setup.py
+drwxr-xr-x   0     1006     1006        0 2023-05-16 16:17:35.309980 hsfs-3.2.0rc2/
+-rw-r--r--   0     1006     1006       40 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/MANIFEST.in
+-rw-r--r--   0     1006     1006     7714 2023-05-16 16:17:35.305980 hsfs-3.2.0rc2/PKG-INFO
+-rw-r--r--   0     1006     1006     5539 2023-05-16 16:17:34.000000 hsfs-3.2.0rc2/README.md
+drwxr-xr-x   0     1006     1006        0 2023-05-16 16:17:35.277980 hsfs-3.2.0rc2/hsfs/
+-rw-r--r--   0     1006     1006     1182 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/__init__.py
+drwxr-xr-x   0     1006     1006        0 2023-05-16 16:17:35.281980 hsfs-3.2.0rc2/hsfs/client/
+-rw-r--r--   0     1006     1006     1694 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/client/__init__.py
+-rw-r--r--   0     1006     1006     1132 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/client/auth.py
+-rw-r--r--   0     1006     1006     6622 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/client/base.py
+-rw-r--r--   0     1006     1006     2090 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/client/exceptions.py
+-rw-r--r--   0     1006     1006    11621 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/client/external.py
+-rw-r--r--   0     1006     1006     7924 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/client/hopsworks.py
+-rw-r--r--   0     1006     1006     1536 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/code.py
+-rw-r--r--   0     1006     1006    18899 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/connection.py
+drwxr-xr-x   0     1006     1006        0 2023-05-16 16:17:35.285980 hsfs-3.2.0rc2/hsfs/constructor/
+-rw-r--r--   0     1006     1006      605 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/constructor/__init__.py
+-rw-r--r--   0     1006     1006     1261 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/constructor/external_feature_group_alias.py
+-rw-r--r--   0     1006     1006     5106 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/constructor/filter.py
+-rw-r--r--   0     1006     1006     2981 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/constructor/fs_query.py
+-rw-r--r--   0     1006     1006     1731 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/constructor/hudi_feature_group_alias.py
+-rw-r--r--   0     1006     1006     2157 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/constructor/join.py
+-rw-r--r--   0     1006     1006     1577 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/constructor/prepared_statement_parameter.py
+-rw-r--r--   0     1006     1006    20138 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/constructor/query.py
+-rw-r--r--   0     1006     1006     3331 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/constructor/serving_prepared_statement.py
+drwxr-xr-x   0     1006     1006        0 2023-05-16 16:17:35.305980 hsfs-3.2.0rc2/hsfs/core/
+-rw-r--r--   0     1006     1006      605 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/core/__init__.py
+-rw-r--r--   0     1006     1006     3688 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/core/builtin_transformation_function.py
+-rw-r--r--   0     1006     1006     1853 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/core/code_api.py
+-rw-r--r--   0     1006     1006     3292 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/core/code_engine.py
+-rw-r--r--   0     1006     1006     3509 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/core/dataset_api.py
+-rw-r--r--   0     1006     1006     1030 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/core/deltastreamer_jobconf.py
+-rw-r--r--   0     1006     1006     1609 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/core/execution.py
+-rw-r--r--   0     1006     1006     5396 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/core/expectation_api.py
+-rw-r--r--   0     1006     1006     2632 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/core/expectation_engine.py
+-rw-r--r--   0     1006     1006     6356 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/core/expectation_suite_api.py
+-rw-r--r--   0     1006     1006     4002 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/core/expectation_suite_engine.py
+-rw-r--r--   0     1006     1006     9792 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/core/explicit_provenance.py
+-rw-r--r--   0     1006     1006     5418 2023-05-05 15:55:12.000000 hsfs-3.2.0rc2/hsfs/core/external_feature_group_engine.py
+-rw-r--r--   0     1006     1006    13334 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/core/feature_group_api.py
+-rw-r--r--   0     1006     1006     6610 2023-05-05 15:55:12.000000 hsfs-3.2.0rc2/hsfs/core/feature_group_base_engine.py
+-rw-r--r--   0     1006     1006    13164 2023-05-05 15:55:12.000000 hsfs-3.2.0rc2/hsfs/core/feature_group_engine.py
+-rw-r--r--   0     1006     1006     1238 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/core/feature_store_api.py
+-rw-r--r--   0     1006     1006     9739 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/core/feature_view_api.py
+-rw-r--r--   0     1006     1006    24896 2023-05-05 15:55:12.000000 hsfs-3.2.0rc2/hsfs/core/feature_view_engine.py
+-rw-r--r--   0     1006     1006     5024 2023-05-05 15:55:12.000000 hsfs-3.2.0rc2/hsfs/core/great_expectation_engine.py
+-rw-r--r--   0     1006     1006      828 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/core/hosts_api.py
+-rw-r--r--   0     1006     1006    11546 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/core/hudi_engine.py
+-rw-r--r--   0     1006     1006     1211 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/core/ingestion_job.py
+-rw-r--r--   0     1006     1006     2262 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/core/ingestion_job_conf.py
+-rw-r--r--   0     1006     1006     1077 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/core/inode.py
+-rw-r--r--   0     1006     1006     2906 2023-05-05 15:55:12.000000 hsfs-3.2.0rc2/hsfs/core/job.py
+-rw-r--r--   0     1006     1006     2004 2023-05-05 15:55:12.000000 hsfs-3.2.0rc2/hsfs/core/job_api.py
+-rw-r--r--   0     1006     1006     2048 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/core/job_configuration.py
+-rw-r--r--   0     1006     1006     1530 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/core/kafka_api.py
+-rw-r--r--   0     1006     1006      898 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/core/project_api.py
+-rw-r--r--   0     1006     1006     1093 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/core/query_constructor_api.py
+-rw-r--r--   0     1006     1006      875 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/core/services_api.py
+-rw-r--r--   0     1006     1006     4204 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/core/statistics_api.py
+-rw-r--r--   0     1006     1006     8159 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/core/statistics_engine.py
+-rw-r--r--   0     1006     1006     2325 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/core/storage_connector_api.py
+-rw-r--r--   0     1006     1006     4696 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/core/tags_api.py
+-rw-r--r--   0     1006     1006     6685 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/core/training_dataset_api.py
+-rw-r--r--   0     1006     1006     6357 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/core/training_dataset_engine.py
+-rw-r--r--   0     1006     1006     2148 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/core/training_dataset_job_conf.py
+-rw-r--r--   0     1006     1006     4161 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/core/transformation_function_api.py
+-rw-r--r--   0     1006     1006    14792 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/core/transformation_function_engine.py
+-rw-r--r--   0     1006     1006     4773 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/core/validation_report_api.py
+-rw-r--r--   0     1006     1006     3640 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/core/validation_report_engine.py
+-rw-r--r--   0     1006     1006     2158 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/core/validation_result_api.py
+-rw-r--r--   0     1006     1006     5469 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/core/validation_result_engine.py
+-rw-r--r--   0     1006     1006     1261 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/core/variable_api.py
+-rw-r--r--   0     1006     1006    18519 2023-05-05 15:55:12.000000 hsfs-3.2.0rc2/hsfs/core/vector_server.py
+-rw-r--r--   0     1006     1006     1655 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/decorators.py
+drwxr-xr-x   0     1006     1006        0 2023-05-16 16:17:35.305980 hsfs-3.2.0rc2/hsfs/engine/
+-rw-r--r--   0     1006     1006     2244 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/engine/__init__.py
+-rw-r--r--   0     1006     1006    46890 2023-05-10 15:22:58.000000 hsfs-3.2.0rc2/hsfs/engine/python.py
+-rw-r--r--   0     1006     1006    43466 2023-05-16 16:17:30.000000 hsfs-3.2.0rc2/hsfs/engine/spark.py
+-rw-r--r--   0     1006     1006    21585 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/expectation_suite.py
+-rw-r--r--   0     1006     1006     6857 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/feature.py
+-rw-r--r--   0     1006     1006   110697 2023-05-05 15:55:12.000000 hsfs-3.2.0rc2/hsfs/feature_group.py
+-rw-r--r--   0     1006     1006     3424 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/feature_group_commit.py
+-rw-r--r--   0     1006     1006     1986 2023-05-05 15:55:12.000000 hsfs-3.2.0rc2/hsfs/feature_group_writer.py
+-rw-r--r--   0     1006     1006    62935 2023-05-05 15:55:12.000000 hsfs-3.2.0rc2/hsfs/feature_store.py
+-rw-r--r--   0     1006     1006    95713 2023-05-05 15:55:12.000000 hsfs-3.2.0rc2/hsfs/feature_view.py
+-rw-r--r--   0     1006     1006     4822 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/ge_expectation.py
+-rw-r--r--   0     1006     1006     8633 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/ge_validation_result.py
+-rw-r--r--   0     1006     1006     1450 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/split_statistics.py
+-rw-r--r--   0     1006     1006     2893 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/statistics.py
+-rw-r--r--   0     1006     1006     3313 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/statistics_config.py
+-rw-r--r--   0     1006     1006    39092 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/storage_connector.py
+-rw-r--r--   0     1006     1006     1850 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/tag.py
+-rw-r--r--   0     1006     1006    35625 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/training_dataset.py
+-rw-r--r--   0     1006     1006     3542 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/training_dataset_feature.py
+-rw-r--r--   0     1006     1006     2759 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/training_dataset_split.py
+-rw-r--r--   0     1006     1006     8929 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/transformation_function.py
+-rw-r--r--   0     1006     1006     2179 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/transformation_function_attached.py
+-rw-r--r--   0     1006     1006     3491 2023-03-13 10:42:53.000000 hsfs-3.2.0rc2/hsfs/user.py
+-rw-r--r--   0     1006     1006    11410 2023-05-05 15:55:12.000000 hsfs-3.2.0rc2/hsfs/util.py
+-rw-r--r--   0     1006     1006     7519 2023-05-03 07:54:47.000000 hsfs-3.2.0rc2/hsfs/validation_report.py
+-rw-r--r--   0     1006     1006      631 2023-05-16 16:17:30.000000 hsfs-3.2.0rc2/hsfs/version.py
+drwxr-xr-x   0     1006     1006        0 2023-05-16 16:17:35.277980 hsfs-3.2.0rc2/hsfs.egg-info/
+-rw-r--r--   0     1006     1006     7714 2023-05-16 16:17:35.000000 hsfs-3.2.0rc2/hsfs.egg-info/PKG-INFO
+-rw-r--r--   0     1006     1006     2805 2023-05-16 16:17:35.000000 hsfs-3.2.0rc2/hsfs.egg-info/SOURCES.txt
+-rw-r--r--   0     1006     1006        1 2023-05-16 16:17:35.000000 hsfs-3.2.0rc2/hsfs.egg-info/dependency_links.txt
+-rw-r--r--   0     1006     1006      679 2023-05-16 16:17:35.000000 hsfs-3.2.0rc2/hsfs.egg-info/requires.txt
+-rw-r--r--   0     1006     1006        5 2023-05-16 16:17:35.000000 hsfs-3.2.0rc2/hsfs.egg-info/top_level.txt
+-rw-r--r--   0     1006     1006       38 2023-05-16 16:17:35.309980 hsfs-3.2.0rc2/setup.cfg
+-rw-r--r--   0     1006     1006     2756 2023-05-05 15:55:12.000000 hsfs-3.2.0rc2/setup.py
```

### Comparing `hsfs-3.2.0rc1/PKG-INFO` & `hsfs-3.2.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsfs
-Version: 3.2.0rc1
+Version: 3.2.0rc2
 Summary: HSFS: An environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api
 Author: Hopsworks AB
 Author-email: moritz@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc1
+Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc2
 Description: # Hopsworks Feature Store
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: hsfs Version: 3.2.0rc1 Summary: HSFS: An
+Metadata-Version: 2.1 Name: hsfs Version: 3.2.0rc2 Summary: HSFS: An
 environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api Author: Hopsworks
 AB Author-email: moritz@logicalclocks.com License: Apache License 2.0 Download-
-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc1
+URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc2
 Description: # Hopsworks Feature Store
   [Hopsworks_Community] [Hopsworks_Feature_Store_Documentation] [PyPiStatus]
            [Scala/Java_Artifacts] [Downloads] [CodeStyle] [License]
 HSFS is the library to interact with the Hopsworks Feature Store. The library
 makes creating new features, feature groups and training datasets easy. The
 library is environment independent and can be used in two modes: - Spark mode:
 For data engineering jobs that create and write features into the feature store
```

### Comparing `hsfs-3.2.0rc1/README.md` & `hsfs-3.2.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/__init__.py` & `hsfs-3.2.0rc2/hsfs/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/client/__init__.py` & `hsfs-3.2.0rc2/hsfs/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/client/auth.py` & `hsfs-3.2.0rc2/hsfs/client/auth.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/client/base.py` & `hsfs-3.2.0rc2/hsfs/client/base.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/client/exceptions.py` & `hsfs-3.2.0rc2/hsfs/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/client/external.py` & `hsfs-3.2.0rc2/hsfs/client/external.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/client/hopsworks.py` & `hsfs-3.2.0rc2/hsfs/client/hopsworks.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/code.py` & `hsfs-3.2.0rc2/hsfs/code.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/connection.py` & `hsfs-3.2.0rc2/hsfs/connection.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/constructor/__init__.py` & `hsfs-3.2.0rc2/hsfs/constructor/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/constructor/external_feature_group_alias.py` & `hsfs-3.2.0rc2/hsfs/constructor/external_feature_group_alias.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/constructor/filter.py` & `hsfs-3.2.0rc2/hsfs/constructor/filter.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/constructor/fs_query.py` & `hsfs-3.2.0rc2/hsfs/constructor/fs_query.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/constructor/hudi_feature_group_alias.py` & `hsfs-3.2.0rc2/hsfs/constructor/hudi_feature_group_alias.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/constructor/join.py` & `hsfs-3.2.0rc2/hsfs/constructor/join.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/constructor/prepared_statement_parameter.py` & `hsfs-3.2.0rc2/hsfs/constructor/prepared_statement_parameter.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/constructor/query.py` & `hsfs-3.2.0rc2/hsfs/constructor/query.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/constructor/serving_prepared_statement.py` & `hsfs-3.2.0rc2/hsfs/constructor/serving_prepared_statement.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/__init__.py` & `hsfs-3.2.0rc2/hsfs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/builtin_transformation_function.py` & `hsfs-3.2.0rc2/hsfs/core/builtin_transformation_function.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/code_api.py` & `hsfs-3.2.0rc2/hsfs/core/code_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/code_engine.py` & `hsfs-3.2.0rc2/hsfs/core/code_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/dataset_api.py` & `hsfs-3.2.0rc2/hsfs/core/dataset_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/deltastreamer_jobconf.py` & `hsfs-3.2.0rc2/hsfs/core/deltastreamer_jobconf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/execution.py` & `hsfs-3.2.0rc2/hsfs/core/execution.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/expectation_api.py` & `hsfs-3.2.0rc2/hsfs/core/expectation_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/expectation_engine.py` & `hsfs-3.2.0rc2/hsfs/core/expectation_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/expectation_suite_api.py` & `hsfs-3.2.0rc2/hsfs/core/expectation_suite_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/expectation_suite_engine.py` & `hsfs-3.2.0rc2/hsfs/core/expectation_suite_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/explicit_provenance.py` & `hsfs-3.2.0rc2/hsfs/core/explicit_provenance.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/external_feature_group_engine.py` & `hsfs-3.2.0rc2/hsfs/core/external_feature_group_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/feature_group_api.py` & `hsfs-3.2.0rc2/hsfs/core/feature_group_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/feature_group_base_engine.py` & `hsfs-3.2.0rc2/hsfs/core/feature_group_base_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/feature_group_engine.py` & `hsfs-3.2.0rc2/hsfs/core/feature_group_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/feature_store_api.py` & `hsfs-3.2.0rc2/hsfs/core/feature_store_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/feature_view_api.py` & `hsfs-3.2.0rc2/hsfs/core/feature_view_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/feature_view_engine.py` & `hsfs-3.2.0rc2/hsfs/core/feature_view_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/great_expectation_engine.py` & `hsfs-3.2.0rc2/hsfs/core/great_expectation_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/hosts_api.py` & `hsfs-3.2.0rc2/hsfs/core/hosts_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/hudi_engine.py` & `hsfs-3.2.0rc2/hsfs/core/hudi_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/ingestion_job.py` & `hsfs-3.2.0rc2/hsfs/core/ingestion_job.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/ingestion_job_conf.py` & `hsfs-3.2.0rc2/hsfs/core/ingestion_job_conf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/inode.py` & `hsfs-3.2.0rc2/hsfs/core/inode.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/job.py` & `hsfs-3.2.0rc2/hsfs/core/job.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/job_api.py` & `hsfs-3.2.0rc2/hsfs/core/job_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/job_configuration.py` & `hsfs-3.2.0rc2/hsfs/core/job_configuration.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/kafka_api.py` & `hsfs-3.2.0rc2/hsfs/core/kafka_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/project_api.py` & `hsfs-3.2.0rc2/hsfs/core/project_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/query_constructor_api.py` & `hsfs-3.2.0rc2/hsfs/core/query_constructor_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/services_api.py` & `hsfs-3.2.0rc2/hsfs/core/services_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/statistics_api.py` & `hsfs-3.2.0rc2/hsfs/core/statistics_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/statistics_engine.py` & `hsfs-3.2.0rc2/hsfs/core/statistics_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/storage_connector_api.py` & `hsfs-3.2.0rc2/hsfs/core/storage_connector_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/tags_api.py` & `hsfs-3.2.0rc2/hsfs/core/tags_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/training_dataset_api.py` & `hsfs-3.2.0rc2/hsfs/core/training_dataset_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/training_dataset_engine.py` & `hsfs-3.2.0rc2/hsfs/core/training_dataset_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/training_dataset_job_conf.py` & `hsfs-3.2.0rc2/hsfs/core/training_dataset_job_conf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/transformation_function_api.py` & `hsfs-3.2.0rc2/hsfs/core/transformation_function_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/transformation_function_engine.py` & `hsfs-3.2.0rc2/hsfs/core/transformation_function_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/validation_report_api.py` & `hsfs-3.2.0rc2/hsfs/core/validation_report_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/validation_report_engine.py` & `hsfs-3.2.0rc2/hsfs/core/validation_report_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/validation_result_api.py` & `hsfs-3.2.0rc2/hsfs/core/validation_result_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/validation_result_engine.py` & `hsfs-3.2.0rc2/hsfs/core/validation_result_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/variable_api.py` & `hsfs-3.2.0rc2/hsfs/core/variable_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/core/vector_server.py` & `hsfs-3.2.0rc2/hsfs/core/vector_server.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/decorators.py` & `hsfs-3.2.0rc2/hsfs/decorators.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/engine/__init__.py` & `hsfs-3.2.0rc2/hsfs/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/engine/python.py` & `hsfs-3.2.0rc2/hsfs/engine/python.py`

 * *Files 0% similar despite different names*

```diff
@@ -845,15 +845,17 @@
                 "Elapsed Time: {elapsed} | Remaining Time: {remaining}",
                 desc="Uploading Dataframe",
                 mininterval=1,
             )
 
             reset_offsets = (
                 feature_group._online_topic_name
-                not in producer.list_topics(timeout=1).topics.keys()
+                not in producer.list_topics(
+                    timeout=offline_write_options.get("kafka_timeout", 6)
+                ).topics.keys()
                 and len(feature_group.commit_details(limit=1)) == 1
             )
 
         def acked(err, msg):
             if err is not None:
                 if offline_write_options.get("debug_kafka", False):
                     print("Failed to deliver message: %s: %s" % (str(msg), str(err)))
```

### Comparing `hsfs-3.2.0rc1/hsfs/engine/spark.py` & `hsfs-3.2.0rc2/hsfs/engine/spark.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 except ImportError:
     pass
 
 from hsfs import feature, training_dataset_feature, client, util
 from hsfs.feature_group import ExternalFeatureGroup
 from hsfs.storage_connector import StorageConnector
 from hsfs.client.exceptions import FeatureStoreException
+from hsfs.client import hopsworks
 from hsfs.core import hudi_engine, transformation_function_engine, kafka_api
 from hsfs.constructor import query
 from hsfs.training_dataset_split import TrainingDatasetSplit
 
 from great_expectations.core.batch import RuntimeBatchRequest
 from great_expectations.data_context import BaseDataContext
 from great_expectations.data_context.types.base import (
@@ -1103,27 +1104,43 @@
         )
         for _feat in pyspark_schema:
             df = df.withColumn(_feat, col(_feat).cast(pyspark_schema[_feat]))
         return df
 
     def _get_kafka_config(self, write_options: dict = {}) -> dict:
         if self._kafka_config is None:
+
             self._kafka_config = {
-                "kafka.bootstrap.servers": ",".join(
-                    [
-                        endpoint.replace("INTERNAL://", "")
-                        for endpoint in self._kafka_api.get_broker_endpoints()
-                    ]
-                ),
                 "kafka.security.protocol": "SSL",
                 "kafka.ssl.truststore.location": client.get_instance()._get_jks_trust_store_path(),
                 "kafka.ssl.truststore.password": client.get_instance()._cert_key,
                 "kafka.ssl.keystore.location": client.get_instance()._get_jks_key_store_path(),
                 "kafka.ssl.keystore.password": client.get_instance()._cert_key,
                 "kafka.ssl.key.password": client.get_instance()._cert_key,
                 "kafka.ssl.endpoint.identification.algorithm": "",
             }
+            if isinstance(client.get_instance(), hopsworks.Client) or write_options.get(
+                "internal_kafka", False
+            ):
+                self._kafka_config["kafka.bootstrap.servers"] = ",".join(
+                    [
+                        endpoint.replace("INTERNAL://", "")
+                        for endpoint in self._kafka_api.get_broker_endpoints(
+                            externalListeners=False
+                        )
+                    ]
+                )
+            else:
+                self._kafka_config["kafka.bootstrap.servers"] = ",".join(
+                    [
+                        endpoint.replace("EXTERNAL://", "")
+                        for endpoint in self._kafka_api.get_broker_endpoints(
+                            externalListeners=True
+                        )
+                    ]
+                )
+
         return {**write_options, **self._kafka_config}
 
 
 class SchemaError(Exception):
     """Thrown when schemas don't match"""
```

### Comparing `hsfs-3.2.0rc1/hsfs/expectation_suite.py` & `hsfs-3.2.0rc2/hsfs/expectation_suite.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/feature.py` & `hsfs-3.2.0rc2/hsfs/feature.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/feature_group.py` & `hsfs-3.2.0rc2/hsfs/feature_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -4638,2283 +4638,2282 @@
 000121d0: 756e 2069 6e73 6572 7473 2069 6e20 6120  un inserts in a 
 000121e0: 6c6f 6f70 3a0a 2020 2020 2020 2020 2020  loop:.          
 000121f0: 2020 2020 2020 7768 696c 6520 6c6f 6f70        while loop
 00012200: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
 00012210: 2020 2020 2020 736d 616c 6c5f 6261 7463        small_batc
 00012220: 685f 6466 203d 202e 2e2e 0a20 2020 2020  h_df = ....     
 00012230: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00012240: 7269 7465 722e 6d75 6c74 695f 7061 7274  riter.multi_part
-00012250: 5f69 6e73 6572 7428 736d 616c 6c5f 6261  _insert(small_ba
-00012260: 7463 685f 6466 290a 2020 2020 2020 2020  tch_df).        
-00012270: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
-00012280: 2020 2020 5468 6520 7772 6974 6572 2062      The writer b
-00012290: 6174 6368 6573 2074 6865 2073 6d61 6c6c  atches the small
-000122a0: 2044 6174 6166 7261 6d65 7320 616e 6420   Dataframes and 
-000122b0: 7472 616e 736d 6974 7320 7468 656d 2074  transmits them t
-000122c0: 6f20 486f 7073 776f 726b 730a 2020 2020  o Hopsworks.    
-000122d0: 2020 2020 2020 2020 6566 6669 6369 656e          efficien
-000122e0: 746c 792e 0a20 2020 2020 2020 2020 2020  tly..           
-000122f0: 2057 6865 6e20 6578 6974 696e 6720 7468   When exiting th
-00012300: 6520 636f 6e74 6578 742c 2074 6865 2066  e context, the f
-00012310: 6561 7475 7265 2067 726f 7570 2077 7269  eature group wri
-00012320: 7465 7220 6973 2073 7572 6520 746f 2065  ter is sure to e
-00012330: 7869 740a 2020 2020 2020 2020 2020 2020  xit.            
-00012340: 6f6e 6c79 206f 6e63 6520 616c 6c20 7468  only once all th
-00012350: 6520 726f 7773 2068 6176 6520 6265 656e  e rows have been
-00012360: 2074 7261 6e73 6d69 7474 6564 2e0a 0a20   transmitted... 
-00012370: 2020 2020 2020 2021 2121 2065 7861 6d70         !!! examp
-00012380: 6c65 2022 4d75 6c74 6920 7061 7274 2069  le "Multi part i
-00012390: 6e73 6572 7420 7769 7468 206d 616e 7561  nsert with manua
-000123a0: 6c20 636f 6e74 6578 7420 6d61 6e61 6765  l context manage
-000123b0: 6d65 6e74 220a 2020 2020 2020 2020 2020  ment".          
-000123c0: 2020 496e 7374 6561 6420 6f66 206c 6574    Instead of let
-000123d0: 7469 6e67 2050 7974 686f 6e20 6861 6e64  ting Python hand
-000123e0: 6c65 2074 6865 2065 6e74 6572 696e 6720  le the entering 
-000123f0: 616e 6420 6578 6974 696e 6720 6f66 2074  and exiting of t
-00012400: 6865 0a20 2020 2020 2020 2020 2020 206d  he.            m
-00012410: 756c 7469 2070 6172 7420 696e 7365 7274  ulti part insert
-00012420: 2063 6f6e 7465 7874 2c20 796f 7520 6361   context, you ca
-00012430: 6e20 7374 6172 7420 616e 6420 6669 6e61  n start and fina
-00012440: 6c69 7a65 2074 6865 2063 6f6e 7465 7874  lize the context
-00012450: 0a20 2020 2020 2020 2020 2020 206d 616e  .            man
-00012460: 7561 6c6c 792e 0a20 2020 2020 2020 2020  ually..         
-00012470: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
-00012480: 2020 2020 2020 2020 2066 6561 7475 7265           feature
-00012490: 5f67 726f 7570 203d 2066 732e 6765 745f  _group = fs.get_
-000124a0: 6f72 5f63 7265 6174 655f 6665 6174 7572  or_create_featur
-000124b0: 655f 6772 6f75 7028 2266 675f 6e61 6d65  e_group("fg_name
-000124c0: 222c 2076 6572 7369 6f6e 3d31 290a 0a20  ", version=1).. 
-000124d0: 2020 2020 2020 2020 2020 2077 6869 6c65             while
-000124e0: 206c 6f6f 703a 0a20 2020 2020 2020 2020   loop:.         
-000124f0: 2020 2020 2020 2073 6d61 6c6c 5f62 6174         small_bat
-00012500: 6368 5f64 6620 3d20 2e2e 2e0a 2020 2020  ch_df = ....    
-00012510: 2020 2020 2020 2020 2020 2020 6665 6174              feat
-00012520: 7572 655f 6772 6f75 702e 6d75 6c74 695f  ure_group.multi_
-00012530: 7061 7274 5f69 6e73 6572 7428 736d 616c  part_insert(smal
-00012540: 6c5f 6261 7463 685f 6466 290a 0a20 2020  l_batch_df)..   
-00012550: 2020 2020 2020 2020 2023 2049 4d50 4f52           # IMPOR
-00012560: 5441 4e54 3a20 6669 6e61 6c69 7a65 2074  TANT: finalize t
-00012570: 6865 206d 756c 7469 2070 6172 7420 696e  he multi part in
-00012580: 7365 7274 2074 6f20 6d61 6b65 2073 7572  sert to make sur
-00012590: 6520 616c 6c20 726f 7773 0a20 2020 2020  e all rows.     
-000125a0: 2020 2020 2020 2023 2068 6176 6520 6265         # have be
-000125b0: 656e 2074 7261 6e73 6d69 7474 6564 0a20  en transmitted. 
-000125c0: 2020 2020 2020 2020 2020 2066 6561 7475             featu
-000125d0: 7265 5f67 726f 7570 2e66 696e 616c 697a  re_group.finaliz
-000125e0: 655f 6d75 6c74 695f 7061 7274 5f69 6e73  e_multi_part_ins
-000125f0: 6572 7428 290a 2020 2020 2020 2020 2020  ert().          
-00012600: 2020 6060 600a 2020 2020 2020 2020 2020    ```.          
-00012610: 2020 4e6f 7465 2074 6861 7420 7468 6520    Note that the 
-00012620: 6669 7273 7420 6361 6c6c 2074 6f20 606d  first call to `m
-00012630: 756c 7469 5f70 6172 745f 696e 7365 7274  ulti_part_insert
-00012640: 6020 696e 6974 6961 7465 7320 7468 6520  ` initiates the 
-00012650: 636f 6e74 6578 740a 2020 2020 2020 2020  context.        
-00012660: 2020 2020 616e 6420 6265 2073 7572 6520      and be sure 
-00012670: 746f 2066 696e 616c 697a 6520 6974 2e20  to finalize it. 
-00012680: 5468 6520 6066 696e 616c 697a 655f 6d75  The `finalize_mu
-00012690: 6c74 695f 7061 7274 5f69 6e73 6572 7460  lti_part_insert`
-000126a0: 2069 7320 610a 2020 2020 2020 2020 2020   is a.          
-000126b0: 2020 626c 6f63 6b69 6e67 2063 616c 6c20    blocking call 
-000126c0: 7468 6174 2072 6574 7572 6e73 206f 6e63  that returns onc
-000126d0: 6520 616c 6c20 726f 7773 2068 6176 6520  e all rows have 
-000126e0: 6265 656e 2074 7261 6e73 6d69 7474 6564  been transmitted
-000126f0: 2e0a 0a20 2020 2020 2020 2020 2020 204f  ...            O
-00012700: 6e63 6520 796f 7520 6172 6520 646f 6e65  nce you are done
-00012710: 2077 6974 6820 7468 6520 6d75 6c74 6920   with the multi 
-00012720: 7061 7274 2069 6e73 6572 742c 2069 7420  part insert, it 
-00012730: 6973 2067 6f6f 6420 7072 6163 7469 6365  is good practice
-00012740: 2074 6f0a 2020 2020 2020 2020 2020 2020   to.            
-00012750: 7374 6172 7420 7468 6520 6261 636b 6669  start the backfi
-00012760: 6c6c 206a 6f62 2069 6e20 6f72 6465 7220  ll job in order 
-00012770: 746f 2077 7269 7465 2074 6865 2064 6174  to write the dat
-00012780: 6120 746f 2074 6865 206f 6666 6c69 6e65  a to the offline
-00012790: 0a20 2020 2020 2020 2020 2020 2073 746f  .            sto
-000127a0: 7261 6765 3a0a 2020 2020 2020 2020 2020  rage:.          
-000127b0: 2020 6060 6070 7974 686f 6e0a 2020 2020    ```python.    
-000127c0: 2020 2020 2020 2020 6665 6174 7572 655f          feature_
-000127d0: 6772 6f75 702e 6261 636b 6669 6c6c 5f6a  group.backfill_j
-000127e0: 6f62 2e72 756e 2861 7761 6974 5f74 6572  ob.run(await_ter
-000127f0: 6d69 6e61 7469 6f6e 3d54 7275 6529 0a20  mination=True). 
-00012800: 2020 2020 2020 2020 2020 2060 6060 0a0a             ```..
-00012810: 2020 2020 2020 2020 2320 4172 6775 6d65          # Argume
-00012820: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
-00012830: 6665 6174 7572 6573 3a20 4461 7461 4672  features: DataFr
-00012840: 616d 652c 2052 4444 2c20 4e64 6172 7261  ame, RDD, Ndarra
-00012850: 792c 206c 6973 742e 2046 6561 7475 7265  y, list. Feature
-00012860: 7320 746f 2062 6520 7361 7665 642e 0a20  s to be saved.. 
-00012870: 2020 2020 2020 2020 2020 206f 7665 7277             overw
-00012880: 7269 7465 3a20 4472 6f70 2061 6c6c 2064  rite: Drop all d
-00012890: 6174 6120 696e 2074 6865 2066 6561 7475  ata in the featu
-000128a0: 7265 2067 726f 7570 2062 6566 6f72 650a  re group before.
-000128b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128c0: 696e 7365 7274 696e 6720 6e65 7720 6461  inserting new da
-000128d0: 7461 2e20 5468 6973 2064 6f65 7320 6e6f  ta. This does no
-000128e0: 7420 6166 6665 6374 206d 6574 6164 6174  t affect metadat
-000128f0: 612c 2064 6566 6175 6c74 7320 746f 2046  a, defaults to F
-00012900: 616c 7365 2e0a 2020 2020 2020 2020 2020  alse..          
-00012910: 2020 6f70 6572 6174 696f 6e3a 2041 7061    operation: Apa
-00012920: 6368 6520 4875 6469 206f 7065 7261 7469  che Hudi operati
-00012930: 6f6e 2074 7970 6520 6022 696e 7365 7274  on type `"insert
-00012940: 2260 206f 7220 6022 7570 7365 7274 2260  "` or `"upsert"`
-00012950: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012960: 2020 4465 6661 756c 7473 2074 6f20 6022    Defaults to `"
-00012970: 7570 7365 7274 2260 2e0a 2020 2020 2020  upsert"`..      
-00012980: 2020 2020 2020 7374 6f72 6167 653a 204f        storage: O
-00012990: 7665 7277 7269 7465 2064 6566 6175 6c74  verwrite default
-000129a0: 2062 6568 6176 696f 7572 2c20 7772 6974   behaviour, writ
-000129b0: 6520 746f 206f 6666 6c69 6e65 0a20 2020  e to offline.   
-000129c0: 2020 2020 2020 2020 2020 2020 2073 746f               sto
-000129d0: 7261 6765 206f 6e6c 7920 7769 7468 2060  rage only with `
-000129e0: 226f 6666 6c69 6e65 2260 206f 7220 6f6e  "offline"` or on
-000129f0: 6c69 6e65 206f 6e6c 7920 7769 7468 2060  line only with `
-00012a00: 226f 6e6c 696e 6522 602c 2064 6566 6175  "online"`, defau
-00012a10: 6c74 730a 2020 2020 2020 2020 2020 2020  lts.            
-00012a20: 2020 2020 746f 2060 4e6f 6e65 602e 0a20      to `None`.. 
-00012a30: 2020 2020 2020 2020 2020 2077 7269 7465             write
-00012a40: 5f6f 7074 696f 6e73 3a20 4164 6469 7469  _options: Additi
-00012a50: 6f6e 616c 2077 7269 7465 206f 7074 696f  onal write optio
-00012a60: 6e73 2061 7320 6b65 792d 7661 6c75 6520  ns as key-value 
-00012a70: 7061 6972 732c 2064 6566 6175 6c74 7320  pairs, defaults 
-00012a80: 746f 2060 7b7d 602e 0a20 2020 2020 2020  to `{}`..       
-00012a90: 2020 2020 2020 2020 2057 6865 6e20 7573           When us
-00012aa0: 696e 6720 7468 6520 6070 7974 686f 6e60  ing the `python`
-00012ab0: 2065 6e67 696e 652c 2077 7269 7465 5f6f   engine, write_o
-00012ac0: 7074 696f 6e73 2063 616e 2063 6f6e 7461  ptions can conta
-00012ad0: 696e 2074 6865 0a20 2020 2020 2020 2020  in the.         
-00012ae0: 2020 2020 2020 2066 6f6c 6c6f 7769 6e67         following
-00012af0: 2065 6e74 7269 6573 3a0a 2020 2020 2020   entries:.      
-00012b00: 2020 2020 2020 2020 2020 2a20 6b65 7920            * key 
-00012b10: 6073 7061 726b 6020 616e 6420 7661 6c75  `spark` and valu
-00012b20: 6520 616e 206f 626a 6563 7420 6f66 2074  e an object of t
-00012b30: 7970 650a 2020 2020 2020 2020 2020 2020  ype.            
-00012b40: 2020 2020 5b68 7366 732e 636f 7265 2e6a      [hsfs.core.j
-00012b50: 6f62 5f63 6f6e 6669 6775 7261 7469 6f6e  ob_configuration
-00012b60: 2e4a 6f62 436f 6e66 6967 7572 6174 696f  .JobConfiguratio
-00012b70: 6e5d 282e 2e2f 6a6f 625f 636f 6e66 6967  n](../job_config
-00012b80: 7572 6174 696f 6e29 0a20 2020 2020 2020  uration).       
-00012b90: 2020 2020 2020 2020 2020 2074 6f20 636f             to co
-00012ba0: 6e66 6967 7572 6520 7468 6520 486f 7073  nfigure the Hops
-00012bb0: 776f 726b 7320 4a6f 6220 7573 6564 2074  works Job used t
-00012bc0: 6f20 7772 6974 6520 6461 7461 2069 6e74  o write data int
-00012bd0: 6f20 7468 650a 2020 2020 2020 2020 2020  o the.          
-00012be0: 2020 2020 2020 2020 6665 6174 7572 6520          feature 
-00012bf0: 6772 6f75 702e 0a20 2020 2020 2020 2020  group..         
-00012c00: 2020 2020 2020 202a 206b 6579 2060 7761         * key `wa
-00012c10: 6974 5f66 6f72 5f6a 6f62 6020 616e 6420  it_for_job` and 
-00012c20: 7661 6c75 6520 6054 7275 6560 206f 7220  value `True` or 
-00012c30: 6046 616c 7365 6020 746f 2063 6f6e 6669  `False` to confi
-00012c40: 6775 7265 0a20 2020 2020 2020 2020 2020  gure.           
-00012c50: 2020 2020 2020 2077 6865 7468 6572 206f         whether o
-00012c60: 7220 6e6f 7420 746f 2074 6865 2069 6e73  r not to the ins
-00012c70: 6572 7420 6361 6c6c 2073 686f 756c 6420  ert call should 
-00012c80: 7265 7475 726e 206f 6e6c 790a 2020 2020  return only.    
-00012c90: 2020 2020 2020 2020 2020 2020 2020 6166                af
-00012ca0: 7465 7220 7468 6520 486f 7073 776f 726b  ter the Hopswork
-00012cb0: 7320 4a6f 6220 6861 7320 6669 6e69 7368  s Job has finish
-00012cc0: 6564 2e20 4279 2064 6566 6175 6c74 2069  ed. By default i
-00012cd0: 7420 7761 6974 732e 0a20 2020 2020 2020  t waits..       
-00012ce0: 2020 2020 2020 2020 202a 206b 6579 2060           * key `
-00012cf0: 7374 6172 745f 6f66 666c 696e 655f 6261  start_offline_ba
-00012d00: 636b 6669 6c6c 6020 616e 6420 7661 6c75  ckfill` and valu
-00012d10: 6520 6054 7275 6560 206f 7220 6046 616c  e `True` or `Fal
-00012d20: 7365 6020 746f 2063 6f6e 6669 6775 7265  se` to configure
-00012d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012d40: 2020 2077 6865 7468 6572 206f 7220 6e6f     whether or no
-00012d50: 7420 746f 2073 7461 7274 2074 6865 2062  t to start the b
-00012d60: 6163 6b66 696c 6c20 6a6f 6220 746f 2077  ackfill job to w
-00012d70: 7269 7465 2064 6174 6120 746f 2074 6865  rite data to the
-00012d80: 206f 6666 6c69 6e65 0a20 2020 2020 2020   offline.       
-00012d90: 2020 2020 2020 2020 2020 2073 746f 7261             stora
-00012da0: 6765 2e20 4279 2064 6566 6175 6c74 2074  ge. By default t
-00012db0: 6865 2062 6163 6b66 696c 6c20 6a6f 6220  he backfill job 
-00012dc0: 646f 6573 206e 6f74 2067 6574 2073 7461  does not get sta
-00012dd0: 7274 6564 2061 7574 6f6d 6174 6963 616c  rted automatical
-00012de0: 6c79 0a20 2020 2020 2020 2020 2020 2020  ly.             
-00012df0: 2020 2020 2066 6f72 206d 756c 7469 2070       for multi p
-00012e00: 6172 7420 696e 7365 7274 732e 0a20 2020  art inserts..   
-00012e10: 2020 2020 2020 2020 2020 2020 202a 206b               * k
-00012e20: 6579 2060 696e 7465 726e 616c 5f6b 6166  ey `internal_kaf
-00012e30: 6b61 6020 616e 6420 7661 6c75 6520 6054  ka` and value `T
-00012e40: 7275 6560 206f 7220 6046 616c 7365 6020  rue` or `False` 
-00012e50: 696e 2063 6173 6520 796f 7520 6573 7461  in case you esta
-00012e60: 626c 6973 6865 640a 2020 2020 2020 2020  blished.        
-00012e70: 2020 2020 2020 2020 2020 636f 6e6e 6563            connec
-00012e80: 7469 7669 7479 2066 726f 6d20 796f 7520  tivity from you 
-00012e90: 5079 7468 6f6e 2065 6e76 6972 6f6e 6d65  Python environme
-00012ea0: 6e74 2074 6f20 7468 6520 696e 7465 726e  nt to the intern
-00012eb0: 616c 2061 6476 6572 7469 7365 640a 2020  al advertised.  
-00012ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ed0: 6c69 7374 656e 6572 7320 6f66 2074 6865  listeners of the
-00012ee0: 2048 6f70 7377 6f72 6b73 204b 6166 6b61   Hopsworks Kafka
-00012ef0: 2043 6c75 7374 6572 2e20 4465 6661 756c   Cluster. Defaul
-00012f00: 7473 2074 6f20 6046 616c 7365 6020 616e  ts to `False` an
-00012f10: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-00012f20: 2020 2020 7769 6c6c 2075 7365 2065 7874      will use ext
-00012f30: 6572 6e61 6c20 6c69 7374 656e 6572 7320  ernal listeners 
-00012f40: 7768 656e 2063 6f6e 6e65 6374 696e 6720  when connecting 
-00012f50: 6672 6f6d 206f 7574 7369 6465 206f 6620  from outside of 
-00012f60: 486f 7073 776f 726b 732e 0a20 2020 2020  Hopsworks..     
-00012f70: 2020 2020 2020 2076 616c 6964 6174 696f         validatio
-00012f80: 6e5f 6f70 7469 6f6e 733a 2041 6464 6974  n_options: Addit
-00012f90: 696f 6e61 6c20 7661 6c69 6461 7469 6f6e  ional validation
-00012fa0: 206f 7074 696f 6e73 2061 7320 6b65 792d   options as key-
-00012fb0: 7661 6c75 6520 7061 6972 732c 2064 6566  value pairs, def
-00012fc0: 6175 6c74 7320 746f 2060 7b7d 602e 0a20  aults to `{}`.. 
-00012fd0: 2020 2020 2020 2020 2020 2020 2020 202a                 *
-00012fe0: 206b 6579 2060 7275 6e5f 7661 6c69 6461   key `run_valida
-00012ff0: 7469 6f6e 6020 626f 6f6c 6561 6e20 7661  tion` boolean va
-00013000: 6c75 652c 2073 6574 2074 6f20 6046 616c  lue, set to `Fal
-00013010: 7365 6020 746f 2073 6b69 7020 7661 6c69  se` to skip vali
-00013020: 6461 7469 6f6e 2074 656d 706f 7261 7269  dation temporari
-00013030: 6c79 206f 6e20 696e 6765 7374 696f 6e2e  ly on ingestion.
-00013040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013050: 202a 206b 6579 2060 7361 7665 5f72 6570   * key `save_rep
-00013060: 6f72 7460 2062 6f6f 6c65 616e 2076 616c  ort` boolean val
-00013070: 7565 2c20 7365 7420 746f 2060 4661 6c73  ue, set to `Fals
-00013080: 6560 2074 6f20 736b 6970 2075 706c 6f61  e` to skip uploa
-00013090: 6420 6f66 2074 6865 2076 616c 6964 6174  d of the validat
-000130a0: 696f 6e20 7265 706f 7274 2074 6f20 486f  ion report to Ho
-000130b0: 7073 776f 726b 732e 0a20 2020 2020 2020  psworks..       
-000130c0: 2020 2020 2020 2020 202a 206b 6579 2060           * key `
-000130d0: 6765 5f76 616c 6964 6174 655f 6b77 6172  ge_validate_kwar
-000130e0: 6773 6020 6120 6469 6374 696f 6e61 7279  gs` a dictionary
-000130f0: 2063 6f6e 7461 696e 696e 6720 6b77 6172   containing kwar
-00013100: 6773 2066 6f72 2074 6865 2076 616c 6964  gs for the valid
-00013110: 6174 6520 6d65 7468 6f64 206f 6620 4772  ate method of Gr
-00013120: 6561 7420 4578 7065 6374 6174 696f 6e73  eat Expectations
-00013130: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013140: 2020 2a20 6b65 7920 6066 6574 6368 5f65    * key `fetch_e
-00013150: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
-00013160: 6020 6120 626f 6f6c 6561 6e20 7661 6c75  ` a boolean valu
-00013170: 652c 2062 7920 6465 6661 756c 7420 6046  e, by default `F
-00013180: 616c 7365 6020 666f 7220 6d75 6c74 6920  alse` for multi 
-00013190: 7061 7274 2069 6e73 6572 7473 2c0a 2020  part inserts,.  
-000131a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131b0: 2074 6f20 636f 6e74 726f 6c20 7768 6574   to control whet
-000131c0: 6865 7220 7468 6520 6578 7065 6374 6174  her the expectat
-000131d0: 696f 6e20 7375 6974 6520 6f66 2074 6865  ion suite of the
-000131e0: 2066 6561 7475 7265 2067 726f 7570 2073   feature group s
-000131f0: 686f 756c 6420 6265 2066 6574 6368 6564  hould be fetched
-00013200: 2062 6566 6f72 6520 6576 6572 7920 696e   before every in
-00013210: 7365 7274 2e0a 0a20 2020 2020 2020 2023  sert...        #
-00013220: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-00013230: 2020 2020 2028 604a 6f62 602c 2060 5661       (`Job`, `Va
-00013240: 6c69 6461 7469 6f6e 5265 706f 7274 6029  lidationReport`)
-00013250: 2041 2074 7570 6c65 2077 6974 6820 6a6f   A tuple with jo
-00013260: 6220 696e 666f 726d 6174 696f 6e20 6966  b information if
-00013270: 2070 7974 686f 6e20 656e 6769 6e65 2069   python engine i
-00013280: 7320 7573 6564 2061 6e64 2074 6865 2076  s used and the v
-00013290: 616c 6964 6174 696f 6e20 7265 706f 7274  alidation report
-000132a0: 2069 6620 7661 6c69 6461 7469 6f6e 2069   if validation i
-000132b0: 7320 656e 6162 6c65 642e 0a20 2020 2020  s enabled..     
-000132c0: 2020 2020 2020 2060 4665 6174 7572 6547         `FeatureG
-000132d0: 726f 7570 5772 6974 6572 6020 5768 656e  roupWriter` When
-000132e0: 2075 7365 6420 6173 2061 2063 6f6e 7465   used as a conte
-000132f0: 7874 206d 616e 6167 6572 2077 6974 6820  xt manager with 
-00013300: 5079 7468 6f6e 2060 7769 7468 6020 7374  Python `with` st
-00013310: 6174 656d 656e 742e 0a20 2020 2020 2020  atement..       
-00013320: 2022 2222 0a20 2020 2020 2020 2073 656c   """.        sel
-00013330: 662e 5f6d 756c 7469 5f70 6172 745f 696e  f._multi_part_in
-00013340: 7365 7274 203d 2054 7275 650a 2020 2020  sert = True.    
-00013350: 2020 2020 6d75 6c74 695f 7061 7274 5f77      multi_part_w
-00013360: 7269 7465 7220 3d20 6665 6174 7572 655f  riter = feature_
-00013370: 6772 6f75 705f 7772 6974 6572 2e46 6561  group_writer.Fea
-00013380: 7475 7265 4772 6f75 7057 7269 7465 7228  tureGroupWriter(
-00013390: 7365 6c66 290a 2020 2020 2020 2020 6966  self).        if
-000133a0: 2066 6561 7475 7265 7320 6973 204e 6f6e   features is Non
-000133b0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000133c0: 6574 7572 6e20 6d75 6c74 695f 7061 7274  eturn multi_part
-000133d0: 5f77 7269 7465 720a 2020 2020 2020 2020  _writer.        
-000133e0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000133f0: 2020 2320 676f 2074 6872 6f75 6768 2077    # go through w
-00013400: 7269 7465 7220 746f 2061 766f 6964 2073  riter to avoid s
-00013410: 6574 7469 6e67 206d 756c 7469 2069 6e73  etting multi ins
-00013420: 6572 7420 6465 6661 756c 7473 2061 6761  ert defaults aga
-00013430: 696e 0a20 2020 2020 2020 2020 2020 2072  in.            r
-00013440: 6574 7572 6e20 6d75 6c74 695f 7061 7274  eturn multi_part
-00013450: 5f77 7269 7465 722e 696e 7365 7274 280a  _writer.insert(.
-00013460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013470: 6665 6174 7572 6573 2c0a 2020 2020 2020  features,.      
-00013480: 2020 2020 2020 2020 2020 6f76 6572 7772            overwr
-00013490: 6974 652c 0a20 2020 2020 2020 2020 2020  ite,.           
-000134a0: 2020 2020 206f 7065 7261 7469 6f6e 2c0a       operation,.
-000134b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134c0: 7374 6f72 6167 652c 0a20 2020 2020 2020  storage,.       
-000134d0: 2020 2020 2020 2020 2077 7269 7465 5f6f           write_o
-000134e0: 7074 696f 6e73 2c0a 2020 2020 2020 2020  ptions,.        
-000134f0: 2020 2020 2020 2020 7661 6c69 6461 7469          validati
-00013500: 6f6e 5f6f 7074 696f 6e73 2c0a 2020 2020  on_options,.    
-00013510: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-00013520: 6566 2066 696e 616c 697a 655f 6d75 6c74  ef finalize_mult
-00013530: 695f 7061 7274 5f69 6e73 6572 7428 7365  i_part_insert(se
-00013540: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00013550: 4669 6e61 6c69 7a65 7320 616e 6420 6578  Finalizes and ex
-00013560: 6974 7320 7468 6520 6d75 6c74 6920 7061  its the multi pa
-00013570: 7274 2069 6e73 6572 7420 636f 6e74 6578  rt insert contex
-00013580: 7420 6f70 656e 6564 2062 7920 606d 756c  t opened by `mul
-00013590: 7469 5f70 6172 745f 696e 7365 7274 600a  ti_part_insert`.
-000135a0: 2020 2020 2020 2020 696e 2061 2062 6c6f          in a blo
-000135b0: 636b 696e 6720 6661 7368 696f 6e20 6f6e  cking fashion on
-000135c0: 6365 2061 6c6c 2072 6f77 7320 6861 7665  ce all rows have
-000135d0: 2062 6565 6e20 7472 616e 736d 6974 7465   been transmitte
-000135e0: 642e 0a0a 2020 2020 2020 2020 2121 2120  d...        !!! 
-000135f0: 6578 616d 706c 6520 224d 756c 7469 2070  example "Multi p
-00013600: 6172 7420 696e 7365 7274 2077 6974 6820  art insert with 
-00013610: 6d61 6e75 616c 2063 6f6e 7465 7874 206d  manual context m
-00013620: 616e 6167 656d 656e 7422 0a20 2020 2020  anagement".     
-00013630: 2020 2020 2020 2049 6e73 7465 6164 206f         Instead o
-00013640: 6620 6c65 7474 696e 6720 5079 7468 6f6e  f letting Python
-00013650: 2068 616e 646c 6520 7468 6520 656e 7465   handle the ente
-00013660: 7269 6e67 2061 6e64 2065 7869 7469 6e67  ring and exiting
-00013670: 206f 6620 7468 650a 2020 2020 2020 2020   of the.        
-00013680: 2020 2020 6d75 6c74 6920 7061 7274 2069      multi part i
-00013690: 6e73 6572 7420 636f 6e74 6578 742c 2079  nsert context, y
-000136a0: 6f75 2063 616e 2073 7461 7274 2061 6e64  ou can start and
-000136b0: 2066 696e 616c 697a 6520 7468 6520 636f   finalize the co
-000136c0: 6e74 6578 740a 2020 2020 2020 2020 2020  ntext.          
-000136d0: 2020 6d61 6e75 616c 6c79 2e0a 2020 2020    manually..    
-000136e0: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
-000136f0: 6e0a 2020 2020 2020 2020 2020 2020 6665  n.            fe
-00013700: 6174 7572 655f 6772 6f75 7020 3d20 6673  ature_group = fs
-00013710: 2e67 6574 5f6f 725f 6372 6561 7465 5f66  .get_or_create_f
-00013720: 6561 7475 7265 5f67 726f 7570 2822 6667  eature_group("fg
-00013730: 5f6e 616d 6522 2c20 7665 7273 696f 6e3d  _name", version=
-00013740: 3129 0a0a 2020 2020 2020 2020 2020 2020  1)..            
-00013750: 7768 696c 6520 6c6f 6f70 3a0a 2020 2020  while loop:.    
-00013760: 2020 2020 2020 2020 2020 2020 736d 616c              smal
-00013770: 6c5f 6261 7463 685f 6466 203d 202e 2e2e  l_batch_df = ...
-00013780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013790: 2066 6561 7475 7265 5f67 726f 7570 2e6d   feature_group.m
-000137a0: 756c 7469 5f70 6172 745f 696e 7365 7274  ulti_part_insert
-000137b0: 2873 6d61 6c6c 5f62 6174 6368 5f64 6629  (small_batch_df)
-000137c0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-000137d0: 494d 504f 5254 414e 543a 2066 696e 616c  IMPORTANT: final
-000137e0: 697a 6520 7468 6520 6d75 6c74 6920 7061  ize the multi pa
-000137f0: 7274 2069 6e73 6572 7420 746f 206d 616b  rt insert to mak
-00013800: 6520 7375 7265 2061 6c6c 2072 6f77 730a  e sure all rows.
-00013810: 2020 2020 2020 2020 2020 2020 2320 6861              # ha
-00013820: 7665 2062 6565 6e20 7472 616e 736d 6974  ve been transmit
-00013830: 7465 640a 2020 2020 2020 2020 2020 2020  ted.            
-00013840: 6665 6174 7572 655f 6772 6f75 702e 6669  feature_group.fi
-00013850: 6e61 6c69 7a65 5f6d 756c 7469 5f70 6172  nalize_multi_par
-00013860: 745f 696e 7365 7274 2829 0a20 2020 2020  t_insert().     
-00013870: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-00013880: 2020 2020 2020 204e 6f74 6520 7468 6174         Note that
-00013890: 2074 6865 2066 6972 7374 2063 616c 6c20   the first call 
-000138a0: 746f 2060 6d75 6c74 695f 7061 7274 5f69  to `multi_part_i
-000138b0: 6e73 6572 7460 2069 6e69 7469 6174 6573  nsert` initiates
-000138c0: 2074 6865 2063 6f6e 7465 7874 0a20 2020   the context.   
-000138d0: 2020 2020 2020 2020 2061 6e64 2062 6520           and be 
-000138e0: 7375 7265 2074 6f20 6669 6e61 6c69 7a65  sure to finalize
-000138f0: 2069 742e 2054 6865 2060 6669 6e61 6c69   it. The `finali
-00013900: 7a65 5f6d 756c 7469 5f70 6172 745f 696e  ze_multi_part_in
-00013910: 7365 7274 6020 6973 2061 0a20 2020 2020  sert` is a.     
-00013920: 2020 2020 2020 2062 6c6f 636b 696e 6720         blocking 
-00013930: 6361 6c6c 2074 6861 7420 7265 7475 726e  call that return
-00013940: 7320 6f6e 6365 2061 6c6c 2072 6f77 7320  s once all rows 
-00013950: 6861 7665 2062 6565 6e20 7472 616e 736d  have been transm
-00013960: 6974 7465 642e 0a20 2020 2020 2020 2022  itted..        "
-00013970: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
-00013980: 6c66 2e5f 6b61 666b 615f 7072 6f64 7563  lf._kafka_produc
-00013990: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
-000139a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000139b0: 2e5f 6b61 666b 615f 7072 6f64 7563 6572  ._kafka_producer
-000139c0: 2e66 6c75 7368 2829 0a20 2020 2020 2020  .flush().       
-000139d0: 2020 2020 2073 656c 662e 5f6b 6166 6b61       self._kafka
-000139e0: 5f70 726f 6475 6365 7220 3d20 4e6f 6e65  _producer = None
-000139f0: 0a20 2020 2020 2020 2073 656c 662e 5f66  .        self._f
-00013a00: 6561 7475 7265 5f77 7269 7465 7273 203d  eature_writers =
-00013a10: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
-00013a20: 6c66 2e5f 7772 6974 6572 203d 204e 6f6e  lf._writer = Non
-00013a30: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
-00013a40: 6d75 6c74 695f 7061 7274 5f69 6e73 6572  multi_part_inser
-00013a50: 7420 3d20 4661 6c73 650a 0a20 2020 2064  t = False..    d
-00013a60: 6566 2069 6e73 6572 745f 7374 7265 616d  ef insert_stream
-00013a70: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00013a80: 2020 2020 2020 2020 6665 6174 7572 6573          features
-00013a90: 3a20 5479 7065 5661 7228 2270 7973 7061  : TypeVar("pyspa
-00013aa0: 726b 2e73 716c 2e44 6174 6146 7261 6d65  rk.sql.DataFrame
-00013ab0: 2229 2c20 2023 206e 6f71 613a 2046 3832  "),  # noqa: F82
-00013ac0: 310a 2020 2020 2020 2020 7175 6572 795f  1.        query_
-00013ad0: 6e61 6d65 3a20 4f70 7469 6f6e 616c 5b73  name: Optional[s
-00013ae0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-00013af0: 2020 2020 6f75 7470 7574 5f6d 6f64 653a      output_mode:
-00013b00: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-00013b10: 2022 6170 7065 6e64 222c 0a20 2020 2020   "append",.     
-00013b20: 2020 2061 7761 6974 5f74 6572 6d69 6e61     await_termina
-00013b30: 7469 6f6e 3a20 4f70 7469 6f6e 616c 5b62  tion: Optional[b
-00013b40: 6f6f 6c5d 203d 2046 616c 7365 2c0a 2020  ool] = False,.  
-00013b50: 2020 2020 2020 7469 6d65 6f75 743a 204f        timeout: O
-00013b60: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-00013b70: 6f6e 652c 0a20 2020 2020 2020 2063 6865  one,.        che
-00013b80: 636b 706f 696e 745f 6469 723a 204f 7074  ckpoint_dir: Opt
-00013b90: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00013ba0: 652c 0a20 2020 2020 2020 2077 7269 7465  e,.        write
-00013bb0: 5f6f 7074 696f 6e73 3a20 4f70 7469 6f6e  _options: Option
-00013bc0: 616c 5b44 6963 745b 416e 792c 2041 6e79  al[Dict[Any, Any
-00013bd0: 5d5d 203d 207b 7d2c 0a20 2020 2029 3a0a  ]] = {},.    ):.
-00013be0: 2020 2020 2020 2020 2222 2249 6e67 6573          """Inges
-00013bf0: 7420 6120 5370 6172 6b20 5374 7275 6374  t a Spark Struct
-00013c00: 7572 6564 2053 7472 6561 6d69 6e67 2044  ured Streaming D
-00013c10: 6174 6166 7261 6d65 2074 6f20 7468 6520  ataframe to the 
-00013c20: 6f6e 6c69 6e65 2066 6561 7475 7265 2073  online feature s
-00013c30: 746f 7265 2e0a 0a20 2020 2020 2020 2054  tore...        T
-00013c40: 6869 7320 6d65 7468 6f64 2063 7265 6174  his method creat
-00013c50: 6573 2061 206c 6f6e 6720 7275 6e6e 696e  es a long runnin
-00013c60: 6720 5370 6172 6b20 5374 7265 616d 696e  g Spark Streamin
-00013c70: 6720 5175 6572 792c 2079 6f75 2063 616e  g Query, you can
-00013c80: 2063 6f6e 7472 6f6c 2074 6865 0a20 2020   control the.   
-00013c90: 2020 2020 2074 6572 6d69 6e61 7469 6f6e       termination
-00013ca0: 206f 6620 7468 6520 7175 6572 7920 7468   of the query th
-00013cb0: 726f 7567 6820 7468 6520 6172 6775 6d65  rough the argume
-00013cc0: 6e74 732e 0a0a 2020 2020 2020 2020 4974  nts...        It
-00013cd0: 2069 7320 706f 7373 6962 6c65 2074 6f20   is possible to 
-00013ce0: 7374 6f70 2074 6865 2072 6574 7572 6e65  stop the returne
-00013cf0: 6420 7175 6572 7920 7769 7468 2074 6865  d query with the
-00013d00: 2060 2e73 746f 7028 2960 2061 6e64 2063   `.stop()` and c
-00013d10: 6865 636b 2069 7473 0a20 2020 2020 2020  heck its.       
-00013d20: 2073 7461 7475 7320 7769 7468 2060 2e69   status with `.i
-00013d30: 7341 6374 6976 6560 2e0a 0a20 2020 2020  sActive`...     
-00013d40: 2020 2054 6f20 6765 7420 6120 6c69 7374     To get a list
-00013d50: 206f 6620 616c 6c20 6163 7469 7665 2071   of all active q
-00013d60: 7565 7269 6573 2c20 7573 653a 0a0a 2020  ueries, use:..  
-00013d70: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
-00013d80: 2020 2020 2020 2020 7371 6d20 3d20 7370          sqm = sp
-00013d90: 6172 6b2e 7374 7265 616d 730a 0a20 2020  ark.streams..   
-00013da0: 2020 2020 2023 2067 6574 2074 6865 206c       # get the l
-00013db0: 6973 7420 6f66 2061 6374 6976 6520 7374  ist of active st
-00013dc0: 7265 616d 696e 6720 7175 6572 6965 730a  reaming queries.
-00013dd0: 2020 2020 2020 2020 5b71 2e6e 616d 6520          [q.name 
-00013de0: 666f 7220 7120 696e 2073 716d 2e61 6374  for q in sqm.act
-00013df0: 6976 655d 0a20 2020 2020 2020 2060 6060  ive].        ```
-00013e00: 0a0a 2020 2020 2020 2020 2121 2120 7761  ..        !!! wa
-00013e10: 726e 696e 6720 2245 6e67 696e 6520 5375  rning "Engine Su
-00013e20: 7070 6f72 7422 0a20 2020 2020 2020 2020  pport".         
-00013e30: 2020 202a 2a53 7061 726b 206f 6e6c 792a     **Spark only*
-00013e40: 2a0a 0a20 2020 2020 2020 2020 2020 2053  *..            S
-00013e50: 7472 6561 6d20 696e 6765 7374 696f 6e20  tream ingestion 
-00013e60: 7573 696e 6720 5061 6e64 6173 2f50 7974  using Pandas/Pyt
-00013e70: 686f 6e20 6173 2065 6e67 696e 6520 6973  hon as engine is
-00013e80: 2063 7572 7265 6e74 6c79 206e 6f74 2073   currently not s
-00013e90: 7570 706f 7274 6564 2e0a 2020 2020 2020  upported..      
-00013ea0: 2020 2020 2020 5079 7468 6f6e 2f50 616e        Python/Pan
-00013eb0: 6461 7320 6861 7320 6e6f 206e 6f74 696f  das has no notio
-00013ec0: 6e20 6f66 2073 7472 6561 6d69 6e67 2e0a  n of streaming..
-00013ed0: 0a20 2020 2020 2020 2021 2121 2077 6172  .        !!! war
-00013ee0: 6e69 6e67 2022 4461 7461 2056 616c 6964  ning "Data Valid
-00013ef0: 6174 696f 6e20 5375 7070 6f72 7422 0a20  ation Support". 
-00013f00: 2020 2020 2020 2020 2020 2060 696e 7365             `inse
-00013f10: 7274 5f73 7472 6561 6d60 2064 6f65 7320  rt_stream` does 
-00013f20: 6e6f 7420 7065 7266 6f72 6d20 616e 7920  not perform any 
-00013f30: 6461 7461 2076 616c 6964 6174 696f 6e20  data validation 
-00013f40: 7573 696e 6720 4772 6561 7420 4578 7065  using Great Expe
-00013f50: 6374 6174 696f 6e73 0a20 2020 2020 2020  ctations.       
-00013f60: 2020 2020 2065 7665 6e20 7768 656e 2061       even when a
-00013f70: 2065 7870 6563 7461 7469 6f6e 2073 7569   expectation sui
-00013f80: 7465 2069 7320 6174 7461 6368 6564 2e0a  te is attached..
-00013f90: 0a20 2020 2020 2020 2023 2041 7267 756d  .        # Argum
-00013fa0: 656e 7473 0a20 2020 2020 2020 2020 2020  ents.           
-00013fb0: 2066 6561 7475 7265 733a 2046 6561 7475   features: Featu
-00013fc0: 7265 7320 696e 2053 7472 6561 6d69 6e67  res in Streaming
-00013fd0: 2044 6174 6166 7261 6d65 2074 6f20 6265   Dataframe to be
-00013fe0: 2073 6176 6564 2e0a 2020 2020 2020 2020   saved..        
-00013ff0: 2020 2020 7175 6572 795f 6e61 6d65 3a20      query_name: 
-00014000: 4974 2069 7320 706f 7373 6962 6c65 2074  It is possible t
-00014010: 6f20 6f70 7469 6f6e 616c 6c79 2073 7065  o optionally spe
-00014020: 6369 6679 2061 206e 616d 6520 666f 7220  cify a name for 
-00014030: 7468 6520 7175 6572 7920 746f 0a20 2020  the query to.   
-00014040: 2020 2020 2020 2020 2020 2020 206d 616b               mak
-00014050: 6520 6974 2065 6173 6965 7220 746f 2072  e it easier to r
-00014060: 6563 6f67 6e69 7365 2069 6e20 7468 6520  ecognise in the 
-00014070: 5370 6172 6b20 5549 2e20 4465 6661 756c  Spark UI. Defaul
-00014080: 7473 2074 6f20 604e 6f6e 6560 2e0a 2020  ts to `None`..  
-00014090: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-000140a0: 5f6d 6f64 653a 2053 7065 6369 6669 6573  _mode: Specifies
-000140b0: 2068 6f77 2064 6174 6120 6f66 2061 2073   how data of a s
-000140c0: 7472 6561 6d69 6e67 2044 6174 6146 7261  treaming DataFra
-000140d0: 6d65 2f44 6174 6173 6574 2069 730a 2020  me/Dataset is.  
-000140e0: 2020 2020 2020 2020 2020 2020 2020 7772                wr
-000140f0: 6974 7465 6e20 746f 2061 2073 7472 6561  itten to a strea
-00014100: 6d69 6e67 2073 696e 6b2e 2028 3129 2060  ming sink. (1) `
-00014110: 2261 7070 656e 6422 603a 204f 6e6c 7920  "append"`: Only 
-00014120: 7468 6520 6e65 7720 726f 7773 2069 6e20  the new rows in 
-00014130: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
-00014140: 2020 2020 7374 7265 616d 696e 6720 4461      streaming Da
-00014150: 7461 4672 616d 652f 4461 7461 7365 7420  taFrame/Dataset 
-00014160: 7769 6c6c 2062 6520 7772 6974 7465 6e20  will be written 
-00014170: 746f 2074 6865 2073 696e 6b2e 2028 3229  to the sink. (2)
-00014180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014190: 2060 2263 6f6d 706c 6574 6522 603a 2041   `"complete"`: A
-000141a0: 6c6c 2074 6865 2072 6f77 7320 696e 2074  ll the rows in t
-000141b0: 6865 2073 7472 6561 6d69 6e67 2044 6174  he streaming Dat
-000141c0: 6146 7261 6d65 2f44 6174 6173 6574 2077  aFrame/Dataset w
-000141d0: 696c 6c20 6265 0a20 2020 2020 2020 2020  ill be.         
-000141e0: 2020 2020 2020 2077 7269 7474 656e 2074         written t
-000141f0: 6f20 7468 6520 7369 6e6b 2065 7665 7279  o the sink every
-00014200: 2074 696d 6520 7468 6572 6520 6973 2073   time there is s
-00014210: 6f6d 6520 7570 6461 7465 2e20 2833 2920  ome update. (3) 
-00014220: 6022 7570 6461 7465 2260 3a0a 2020 2020  `"update"`:.    
-00014230: 2020 2020 2020 2020 2020 2020 6f6e 6c79              only
-00014240: 2074 6865 2072 6f77 7320 7468 6174 2077   the rows that w
-00014250: 6572 6520 7570 6461 7465 6420 696e 2074  ere updated in t
-00014260: 6865 2073 7472 6561 6d69 6e67 2044 6174  he streaming Dat
-00014270: 6146 7261 6d65 2f44 6174 6173 6574 2077  aFrame/Dataset w
-00014280: 696c 6c0a 2020 2020 2020 2020 2020 2020  ill.            
-00014290: 2020 2020 6265 2077 7269 7474 656e 2074      be written t
-000142a0: 6f20 7468 6520 7369 6e6b 2065 7665 7279  o the sink every
-000142b0: 2074 696d 6520 7468 6572 6520 6172 6520   time there are 
-000142c0: 736f 6d65 2075 7064 6174 6573 2e0a 2020  some updates..  
-000142d0: 2020 2020 2020 2020 2020 2020 2020 4966                If
-000142e0: 2074 6865 2071 7565 7279 2064 6f65 736e   the query doesn
-000142f0: e280 9974 2063 6f6e 7461 696e 2061 6767  ...t contain agg
-00014300: 7265 6761 7469 6f6e 732c 2069 7420 7769  regations, it wi
-00014310: 6c6c 2062 6520 6571 7569 7661 6c65 6e74  ll be equivalent
-00014320: 2074 6f0a 2020 2020 2020 2020 2020 2020   to.            
-00014330: 2020 2020 6170 7065 6e64 206d 6f64 652e      append mode.
-00014340: 2044 6566 6175 6c74 7320 746f 2060 2261   Defaults to `"a
-00014350: 7070 656e 6422 602e 0a20 2020 2020 2020  ppend"`..       
-00014360: 2020 2020 2061 7761 6974 5f74 6572 6d69       await_termi
-00014370: 6e61 7469 6f6e 3a20 5761 6974 7320 666f  nation: Waits fo
-00014380: 7220 7468 6520 7465 726d 696e 6174 696f  r the terminatio
-00014390: 6e20 6f66 2074 6869 7320 7175 6572 792c  n of this query,
-000143a0: 2065 6974 6865 7220 6279 0a20 2020 2020   either by.     
-000143b0: 2020 2020 2020 2020 2020 2071 7565 7279             query
-000143c0: 2e73 746f 7028 2920 6f72 2062 7920 616e  .stop() or by an
-000143d0: 2065 7863 6570 7469 6f6e 2e20 4966 2074   exception. If t
-000143e0: 6865 2071 7565 7279 2068 6173 2074 6572  he query has ter
-000143f0: 6d69 6e61 7465 6420 7769 7468 2061 6e0a  minated with an.
-00014400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014410: 6578 6365 7074 696f 6e2c 2074 6865 6e20  exception, then 
-00014420: 7468 6520 6578 6365 7074 696f 6e20 7769  the exception wi
-00014430: 6c6c 2062 6520 7468 726f 776e 2e20 4966  ll be thrown. If
-00014440: 2074 696d 656f 7574 2069 7320 7365 742c   timeout is set,
-00014450: 2069 740a 2020 2020 2020 2020 2020 2020   it.            
-00014460: 2020 2020 7265 7475 726e 7320 7768 6574      returns whet
-00014470: 6865 7220 7468 6520 7175 6572 7920 6861  her the query ha
-00014480: 7320 7465 726d 696e 6174 6564 206f 7220  s terminated or 
-00014490: 6e6f 7420 7769 7468 696e 2074 6865 2074  not within the t
-000144a0: 696d 656f 7574 0a20 2020 2020 2020 2020  imeout.         
-000144b0: 2020 2020 2020 2073 6563 6f6e 6473 2e20         seconds. 
-000144c0: 4465 6661 756c 7473 2074 6f20 6046 616c  Defaults to `Fal
-000144d0: 7365 602e 0a20 2020 2020 2020 2020 2020  se`..           
-000144e0: 2074 696d 656f 7574 3a20 4f6e 6c79 2072   timeout: Only r
-000144f0: 656c 6576 616e 7420 696e 2063 6f6d 6269  elevant in combi
-00014500: 6e61 7469 6f6e 2077 6974 6820 6061 7761  nation with `awa
-00014510: 6974 5f74 6572 6d69 6e61 7469 6f6e 3d54  it_termination=T
-00014520: 7275 6560 2e0a 2020 2020 2020 2020 2020  rue`..          
-00014530: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
-00014540: 6f20 604e 6f6e 6560 2e0a 2020 2020 2020  o `None`..      
-00014550: 2020 2020 2020 6368 6563 6b70 6f69 6e74        checkpoint
-00014560: 5f64 6972 3a20 4368 6563 6b70 6f69 6e74  _dir: Checkpoint
-00014570: 2064 6972 6563 746f 7279 206c 6f63 6174   directory locat
-00014580: 696f 6e2e 2054 6869 7320 7769 6c6c 2062  ion. This will b
-00014590: 6520 7573 6564 2074 6f20 6173 2061 2072  e used to as a r
-000145a0: 6566 6572 656e 6365 2074 6f0a 2020 2020  eference to.    
-000145b0: 2020 2020 2020 2020 2020 2020 6672 6f6d              from
-000145c0: 2077 6865 7265 2074 6f20 7265 7375 6d65   where to resume
-000145d0: 2074 6865 2073 7472 6561 6d69 6e67 206a   the streaming j
-000145e0: 6f62 2e20 4966 2060 4e6f 6e65 6020 7468  ob. If `None` th
-000145f0: 656e 2068 7366 7320 7769 6c6c 2063 6f6e  en hsfs will con
-00014600: 7374 7275 6374 2061 730a 2020 2020 2020  struct as.      
-00014610: 2020 2020 2020 2020 2020 2269 6e73 6572            "inser
-00014620: 745f 7374 7265 616d 5f22 202b 206f 6e6c  t_stream_" + onl
-00014630: 696e 655f 746f 7069 635f 6e61 6d65 2e20  ine_topic_name. 
-00014640: 4465 6661 756c 7473 2074 6f20 604e 6f6e  Defaults to `Non
-00014650: 6560 2e0a 2020 2020 2020 2020 2020 2020  e`..            
-00014660: 2020 2020 7772 6974 655f 6f70 7469 6f6e      write_option
-00014670: 733a 2041 6464 6974 696f 6e61 6c20 7772  s: Additional wr
-00014680: 6974 6520 6f70 7469 6f6e 7320 666f 7220  ite options for 
-00014690: 5370 6172 6b20 6173 206b 6579 2d76 616c  Spark as key-val
-000146a0: 7565 2070 6169 7273 2e0a 2020 2020 2020  ue pairs..      
-000146b0: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-000146c0: 7473 2074 6f20 607b 7d60 2e0a 0a20 2020  ts to `{}`...   
-000146d0: 2020 2020 2023 2052 6574 7572 6e73 0a20       # Returns. 
-000146e0: 2020 2020 2020 2020 2020 2060 5374 7265             `Stre
-000146f0: 616d 696e 6751 7565 7279 603a 2053 7061  amingQuery`: Spa
-00014700: 726b 2053 7472 7563 7475 7265 6420 5374  rk Structured St
-00014710: 7265 616d 696e 6720 5175 6572 7920 6f62  reaming Query ob
-00014720: 6a65 6374 2e0a 2020 2020 2020 2020 2222  ject..        ""
-00014730: 220a 2020 2020 2020 2020 6966 2028 0a20  ".        if (. 
-00014740: 2020 2020 2020 2020 2020 206e 6f74 2065             not e
-00014750: 6e67 696e 652e 6765 745f 696e 7374 616e  ngine.get_instan
-00014760: 6365 2829 2e69 735f 7370 6172 6b5f 6461  ce().is_spark_da
-00014770: 7461 6672 616d 6528 6665 6174 7572 6573  taframe(features
-00014780: 290a 2020 2020 2020 2020 2020 2020 6f72  ).            or
-00014790: 206e 6f74 2066 6561 7475 7265 732e 6973   not features.is
-000147a0: 5374 7265 616d 696e 670a 2020 2020 2020  Streaming.      
-000147b0: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
-000147c0: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
-000147d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000147e0: 2020 2246 6561 7475 7265 7320 6861 7665    "Features have
-000147f0: 2074 6f20 6265 2061 2073 7472 6561 6d69   to be a streami
-00014800: 6e67 2074 7970 6520 7370 6172 6b20 6461  ng type spark da
-00014810: 7461 6672 616d 652e 2055 7365 2060 696e  taframe. Use `in
-00014820: 7365 7274 2829 6020 6d65 7468 6f64 2069  sert()` method i
-00014830: 6e73 7465 6164 2e22 0a20 2020 2020 2020  nstead.".       
-00014840: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
-00014850: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00014860: 2023 206c 6f77 6572 2063 6173 696e 6720   # lower casing 
-00014870: 6665 6174 7572 6520 6e61 6d65 730a 2020  feature names.  
-00014880: 2020 2020 2020 2020 2020 6665 6174 7572            featur
-00014890: 655f 6461 7461 6672 616d 6520 3d20 656e  e_dataframe = en
-000148a0: 6769 6e65 2e67 6574 5f69 6e73 7461 6e63  gine.get_instanc
-000148b0: 6528 292e 636f 6e76 6572 745f 746f 5f64  e().convert_to_d
-000148c0: 6566 6175 6c74 5f64 6174 6166 7261 6d65  efault_dataframe
-000148d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000148e0: 2020 6665 6174 7572 6573 0a20 2020 2020    features.     
-000148f0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00014900: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
-00014910: 726e 280a 2020 2020 2020 2020 2020 2020  rn(.            
-00014920: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
-00014930: 2020 2020 2020 2020 2020 2253 7472 6561            "Strea
-00014940: 6d20 696e 6765 7374 696f 6e20 666f 7220  m ingestion for 
-00014950: 6665 6174 7572 6520 6772 6f75 7020 607b  feature group `{
-00014960: 7d60 2c20 7769 7468 2076 6572 7369 6f6e  }`, with version
-00014970: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00014980: 2020 2020 2020 2220 607b 7d60 2077 696c        " `{}` wil
-00014990: 6c20 6e6f 7420 636f 6d70 7574 6520 7374  l not compute st
-000149a0: 6174 6973 7469 6373 2e22 0a20 2020 2020  atistics.".     
-000149b0: 2020 2020 2020 2020 2020 2029 2e66 6f72             ).for
-000149c0: 6d61 7428 7365 6c66 2e5f 6e61 6d65 2c20  mat(self._name, 
-000149d0: 7365 6c66 2e5f 7665 7273 696f 6e29 2c0a  self._version),.
-000149e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149f0: 7574 696c 2e53 7461 7469 7374 6963 7357  util.StatisticsW
-00014a00: 6172 6e69 6e67 2c0a 2020 2020 2020 2020  arning,.        
-00014a10: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-00014a20: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00014a30: 6665 6174 7572 655f 6772 6f75 705f 656e  feature_group_en
-00014a40: 6769 6e65 2e69 6e73 6572 745f 7374 7265  gine.insert_stre
-00014a50: 616d 280a 2020 2020 2020 2020 2020 2020  am(.            
-00014a60: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00014a70: 2020 2020 2020 2020 2020 6665 6174 7572            featur
-00014a80: 655f 6461 7461 6672 616d 652c 0a20 2020  e_dataframe,.   
-00014a90: 2020 2020 2020 2020 2020 2020 2071 7565               que
-00014aa0: 7279 5f6e 616d 652c 0a20 2020 2020 2020  ry_name,.       
-00014ab0: 2020 2020 2020 2020 206f 7574 7075 745f           output_
-00014ac0: 6d6f 6465 2c0a 2020 2020 2020 2020 2020  mode,.          
-00014ad0: 2020 2020 2020 6177 6169 745f 7465 726d        await_term
-00014ae0: 696e 6174 696f 6e2c 0a20 2020 2020 2020  ination,.       
-00014af0: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
-00014b00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00014b10: 2020 6368 6563 6b70 6f69 6e74 5f64 6972    checkpoint_dir
-00014b20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00014b30: 2020 7772 6974 655f 6f70 7469 6f6e 732c    write_options,
-00014b40: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00014b50: 2020 2020 6465 6620 636f 6d6d 6974 5f64      def commit_d
-00014b60: 6574 6169 6c73 280a 2020 2020 2020 2020  etails(.        
-00014b70: 7365 6c66 2c0a 2020 2020 2020 2020 7761  self,.        wa
-00014b80: 6c6c 636c 6f63 6b5f 7469 6d65 3a20 4f70  llclock_time: Op
-00014b90: 7469 6f6e 616c 5b55 6e69 6f6e 5b73 7472  tional[Union[str
-00014ba0: 2c20 696e 742c 2064 6174 6574 696d 652c  , int, datetime,
-00014bb0: 2064 6174 655d 5d20 3d20 4e6f 6e65 2c0a   date]] = None,.
-00014bc0: 2020 2020 2020 2020 6c69 6d69 743a 204f          limit: O
-00014bd0: 7074 696f 6e61 6c5b 696e 745d 203d 204e  ptional[int] = N
-00014be0: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-00014bf0: 2020 2020 2222 2252 6574 7269 6576 6573      """Retrieves
-00014c00: 2063 6f6d 6d69 7420 7469 6d65 6c69 6e65   commit timeline
-00014c10: 2066 6f72 2074 6869 7320 6665 6174 7572   for this featur
-00014c20: 6520 6772 6f75 702e 2054 6869 7320 6d65  e group. This me
-00014c30: 7468 6f64 2063 616e 206f 6e6c 7920 6265  thod can only be
-00014c40: 2075 7365 640a 2020 2020 2020 2020 6f6e   used.        on
-00014c50: 2074 696d 6520 7472 6176 656c 2065 6e61   time travel ena
-00014c60: 626c 6564 2066 6561 7475 7265 2067 726f  bled feature gro
-00014c70: 7570 730a 0a20 2020 2020 2020 2021 2121  ups..        !!!
-00014c80: 2065 7861 6d70 6c65 0a20 2020 2020 2020   example.       
-00014c90: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
-00014ca0: 2020 2020 2020 2020 2020 2023 2063 6f6e             # con
-00014cb0: 6e65 6374 2074 6f20 7468 6520 4665 6174  nect to the Feat
-00014cc0: 7572 6520 5374 6f72 650a 2020 2020 2020  ure Store.      
-00014cd0: 2020 2020 2020 6673 203d 202e 2e2e 0a0a        fs = .....
-00014ce0: 2020 2020 2020 2020 2020 2020 2320 6765              # ge
-00014cf0: 7420 7468 6520 4665 6174 7572 6520 4772  t the Feature Gr
-00014d00: 6f75 7020 696e 7374 616e 6365 0a20 2020  oup instance.   
-00014d10: 2020 2020 2020 2020 2066 6720 3d20 6673           fg = fs
-00014d20: 2e67 6574 5f6f 725f 6372 6561 7465 5f66  .get_or_create_f
-00014d30: 6561 7475 7265 5f67 726f 7570 282e 2e2e  eature_group(...
-00014d40: 290a 0a20 2020 2020 2020 2020 2020 2063  )..            c
-00014d50: 6f6d 6d69 745f 6465 7461 696c 7320 3d20  ommit_details = 
-00014d60: 6667 2e63 6f6d 6d69 745f 6465 7461 696c  fg.commit_detail
-00014d70: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-00014d80: 6060 600a 0a20 2020 2020 2020 2023 2041  ```..        # A
-00014d90: 7267 756d 656e 7473 0a20 2020 2020 2020  rguments.       
-00014da0: 2020 2020 2077 616c 6c63 6c6f 636b 5f74       wallclock_t
-00014db0: 696d 653a 2043 6f6d 6d69 7420 6465 7461  ime: Commit deta
-00014dc0: 696c 7320 6173 206f 6620 7370 6563 6966  ils as of specif
-00014dd0: 6963 2070 6f69 6e74 2069 6e20 7469 6d65  ic point in time
-00014de0: 2e20 4465 6661 756c 7473 2074 6f20 604e  . Defaults to `N
-00014df0: 6f6e 6560 2e0a 2020 2020 2020 2020 2020  one`..          
-00014e00: 2020 2020 2020 2053 7472 696e 6773 2073         Strings s
-00014e10: 686f 756c 6420 6265 2066 6f72 6d61 7474  hould be formatt
-00014e20: 6564 2069 6e20 6f6e 6520 6f66 2074 6865  ed in one of the
-00014e30: 2066 6f6c 6c6f 7769 6e67 2066 6f72 6d61   following forma
-00014e40: 7473 2060 2559 2d25 6d2d 2564 602c 2060  ts `%Y-%m-%d`, `
-00014e50: 2559 2d25 6d2d 2564 2025 4860 2c20 6025  %Y-%m-%d %H`, `%
-00014e60: 592d 256d 2d25 6420 2548 3a25 4d60 2c0a  Y-%m-%d %H:%M`,.
-00014e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e80: 6025 592d 256d 2d25 6420 2548 3a25 4d3a  `%Y-%m-%d %H:%M:
-00014e90: 2553 602c 206f 7220 6025 592d 256d 2d25  %S`, or `%Y-%m-%
-00014ea0: 6420 2548 3a25 4d3a 2553 2e25 6660 2e0a  d %H:%M:%S.%f`..
-00014eb0: 2020 2020 2020 2020 2020 2020 6c69 6d69              limi
-00014ec0: 743a 204e 756d 6265 7220 6f66 2063 6f6d  t: Number of com
-00014ed0: 6d69 7473 2074 6f20 7265 7472 6965 7665  mits to retrieve
-00014ee0: 2e20 4465 6661 756c 7473 2074 6f20 604e  . Defaults to `N
-00014ef0: 6f6e 6560 2e0a 0a20 2020 2020 2020 2023  one`...        #
-00014f00: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-00014f10: 2020 2020 2060 4469 6374 5b73 7472 2c20       `Dict[str, 
-00014f20: 4469 6374 5b73 7472 2c20 7374 725d 5d60  Dict[str, str]]`
-00014f30: 2e20 4469 6374 696f 6e61 7279 206f 626a  . Dictionary obj
-00014f40: 6563 7420 6f66 2063 6f6d 6d69 7420 6d65  ect of commit me
-00014f50: 7461 6461 7461 2074 696d 656c 696e 652c  tadata timeline,
-00014f60: 2077 6865 7265 204b 6579 2069 7320 636f   where Key is co
-00014f70: 6d6d 6974 2069 6420 616e 6420 7661 6c75  mmit id and valu
-00014f80: 650a 2020 2020 2020 2020 2020 2020 6973  e.            is
-00014f90: 2060 4469 6374 5b73 7472 2c20 7374 725d   `Dict[str, str]
-00014fa0: 6020 7769 7468 206b 6579 2076 616c 7565  ` with key value
-00014fb0: 2070 6169 7273 206f 6620 6461 7465 2063   pairs of date c
-00014fc0: 6f6d 6d69 7474 6564 206f 6e2c 206e 756d  ommitted on, num
-00014fd0: 6265 7220 6f66 2072 6f77 7320 7570 6461  ber of rows upda
-00014fe0: 7465 642c 2069 6e73 6572 7465 6420 616e  ted, inserted an
-00014ff0: 6420 6465 6c65 7465 642e 0a0a 2020 2020  d deleted...    
-00015000: 2020 2020 2320 5261 6973 6573 0a20 2020      # Raises.   
-00015010: 2020 2020 2020 2020 2060 6873 6673 2e63           `hsfs.c
-00015020: 6c69 656e 742e 6578 6365 7074 696f 6e73  lient.exceptions
-00015030: 2e52 6573 7441 5049 4572 726f 7260 2e0a  .RestAPIError`..
-00015040: 2020 2020 2020 2020 2020 2020 6068 7366              `hsf
-00015050: 732e 636c 6965 6e74 2e65 7863 6570 7469  s.client.excepti
-00015060: 6f6e 732e 4665 6174 7572 6553 746f 7265  ons.FeatureStore
-00015070: 4578 6365 7074 696f 6e60 2e20 4966 2074  Exception`. If t
-00015080: 6865 2066 6561 7475 7265 2067 726f 7570  he feature group
-00015090: 2064 6f65 7320 6e6f 7420 6861 7665 2060   does not have `
-000150a0: 4855 4449 6020 7469 6d65 2074 7261 7665  HUDI` time trave
-000150b0: 6c20 666f 726d 6174 0a20 2020 2020 2020  l format.       
-000150c0: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-000150d0: 7572 6e20 7365 6c66 2e5f 6665 6174 7572  urn self._featur
-000150e0: 655f 6772 6f75 705f 656e 6769 6e65 2e63  e_group_engine.c
-000150f0: 6f6d 6d69 745f 6465 7461 696c 7328 7365  ommit_details(se
-00015100: 6c66 2c20 7761 6c6c 636c 6f63 6b5f 7469  lf, wallclock_ti
-00015110: 6d65 2c20 6c69 6d69 7429 0a0a 2020 2020  me, limit)..    
-00015120: 6465 6620 636f 6d6d 6974 5f64 656c 6574  def commit_delet
-00015130: 655f 7265 636f 7264 280a 2020 2020 2020  e_record(.      
-00015140: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00015150: 6465 6c65 7465 5f64 663a 2054 7970 6556  delete_df: TypeV
-00015160: 6172 2822 7079 7370 6172 6b2e 7371 6c2e  ar("pyspark.sql.
-00015170: 4461 7461 4672 616d 6522 292c 2020 2320  DataFrame"),  # 
-00015180: 6e6f 7161 3a20 4638 3231 0a20 2020 2020  noqa: F821.     
-00015190: 2020 2077 7269 7465 5f6f 7074 696f 6e73     write_options
-000151a0: 3a20 4f70 7469 6f6e 616c 5b44 6963 745b  : Optional[Dict[
-000151b0: 416e 792c 2041 6e79 5d5d 203d 207b 7d2c  Any, Any]] = {},
-000151c0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-000151d0: 2222 2244 726f 7073 2072 6563 6f72 6473  """Drops records
-000151e0: 2070 7265 7365 6e74 2069 6e20 7468 6520   present in the 
-000151f0: 7072 6f76 6964 6564 2044 6174 6146 7261  provided DataFra
-00015200: 6d65 2061 6e64 2063 6f6d 6d69 7473 2069  me and commits i
-00015210: 7420 6173 2075 7064 6174 6520 746f 2074  t as update to t
-00015220: 6869 730a 2020 2020 2020 2020 4665 6174  his.        Feat
-00015230: 7572 6520 6772 6f75 702e 2054 6869 7320  ure group. This 
-00015240: 6d65 7468 6f64 2063 616e 206f 6e6c 7920  method can only 
-00015250: 6265 2075 7365 6420 6f6e 2074 696d 6520  be used on time 
-00015260: 7472 6176 656c 2065 6e61 626c 6564 2066  travel enabled f
-00015270: 6561 7475 7265 2067 726f 7570 732e 0a0a  eature groups...
-00015280: 2020 2020 2020 2020 2320 4172 6775 6d65          # Argume
-00015290: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
-000152a0: 6465 6c65 7465 5f64 663a 2064 6174 6146  delete_df: dataF
-000152b0: 7261 6d65 2063 6f6e 7461 696e 696e 6720  rame containing 
-000152c0: 7265 636f 7264 7320 746f 2062 6520 6465  records to be de
-000152d0: 6c65 7465 642e 0a20 2020 2020 2020 2020  leted..         
-000152e0: 2020 2077 7269 7465 5f6f 7074 696f 6e73     write_options
-000152f0: 3a20 5573 6572 2070 726f 7669 6465 6420  : User provided 
-00015300: 7772 6974 6520 6f70 7469 6f6e 732e 2044  write options. D
-00015310: 6566 6175 6c74 7320 746f 2060 7b7d 602e  efaults to `{}`.
-00015320: 0a0a 2020 2020 2020 2020 2320 5261 6973  ..        # Rais
-00015330: 6573 0a20 2020 2020 2020 2020 2020 2060  es.            `
-00015340: 6873 6673 2e63 6c69 656e 742e 6578 6365  hsfs.client.exce
-00015350: 7074 696f 6e73 2e52 6573 7441 5049 4572  ptions.RestAPIEr
-00015360: 726f 7260 2e0a 2020 2020 2020 2020 2222  ror`..        ""
-00015370: 220a 2020 2020 2020 2020 7365 6c66 2e5f  ".        self._
-00015380: 6665 6174 7572 655f 6772 6f75 705f 656e  feature_group_en
-00015390: 6769 6e65 2e63 6f6d 6d69 745f 6465 6c65  gine.commit_dele
-000153a0: 7465 2873 656c 662c 2064 656c 6574 655f  te(self, delete_
-000153b0: 6466 2c20 7772 6974 655f 6f70 7469 6f6e  df, write_option
-000153c0: 7329 0a0a 2020 2020 6465 6620 6173 5f6f  s)..    def as_o
-000153d0: 6628 0a20 2020 2020 2020 2073 656c 662c  f(.        self,
-000153e0: 0a20 2020 2020 2020 2077 616c 6c63 6c6f  .        wallclo
-000153f0: 636b 5f74 696d 653a 204f 7074 696f 6e61  ck_time: Optiona
-00015400: 6c5b 556e 696f 6e5b 7374 722c 2069 6e74  l[Union[str, int
-00015410: 2c20 6461 7465 7469 6d65 2c20 6461 7465  , datetime, date
-00015420: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
-00015430: 2020 2065 7863 6c75 6465 5f75 6e74 696c     exclude_until
-00015440: 3a20 4f70 7469 6f6e 616c 5b55 6e69 6f6e  : Optional[Union
-00015450: 5b73 7472 2c20 696e 742c 2064 6174 6574  [str, int, datet
-00015460: 696d 652c 2064 6174 655d 5d20 3d20 4e6f  ime, date]] = No
-00015470: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-00015480: 2020 2022 2222 4765 7420 5175 6572 7920     """Get Query 
-00015490: 6f62 6a65 6374 2074 6f20 7265 7472 6965  object to retrie
-000154a0: 7665 2061 6c6c 2066 6561 7475 7265 7320  ve all features 
-000154b0: 6f66 2074 6865 2067 726f 7570 2061 7420  of the group at 
-000154c0: 6120 706f 696e 7420 696e 2074 6865 2070  a point in the p
-000154d0: 6173 742e 0a0a 2020 2020 2020 2020 5468  ast...        Th
-000154e0: 6973 206d 6574 686f 6420 7365 6c65 6374  is method select
-000154f0: 7320 616c 6c20 6665 6174 7572 6573 2069  s all features i
-00015500: 6e20 7468 6520 6665 6174 7572 6520 6772  n the feature gr
-00015510: 6f75 7020 616e 6420 7265 7475 726e 7320  oup and returns 
-00015520: 6120 5175 6572 7920 6f62 6a65 6374 0a20  a Query object. 
-00015530: 2020 2020 2020 2061 7420 7468 6520 7370         at the sp
-00015540: 6563 6966 6965 6420 706f 696e 7420 696e  ecified point in
-00015550: 2074 696d 652e 204f 7074 696f 6e61 6c6c   time. Optionall
-00015560: 792c 2063 6f6d 6d69 7473 2062 6566 6f72  y, commits befor
-00015570: 6520 6120 7370 6563 6966 6965 6420 706f  e a specified po
-00015580: 696e 7420 696e 2074 696d 6520 6361 6e20  int in time can 
-00015590: 6265 0a20 2020 2020 2020 2065 7863 6c75  be.        exclu
-000155a0: 6465 6420 6672 6f6d 2074 6865 2071 7565  ded from the que
-000155b0: 7279 2e20 5468 6520 5175 6572 7920 6361  ry. The Query ca
-000155c0: 6e20 7468 656e 2065 6974 6865 7220 6265  n then either be
-000155d0: 2072 6561 6420 696e 746f 2061 2044 6174   read into a Dat
-000155e0: 6166 7261 6d65 0a20 2020 2020 2020 206f  aframe.        o
-000155f0: 7220 7573 6564 2066 7572 7468 6572 2074  r used further t
-00015600: 6f20 7065 7266 6f72 6d20 6a6f 696e 7320  o perform joins 
-00015610: 6f72 2063 6f6e 7374 7275 6374 2061 2074  or construct a t
-00015620: 7261 696e 696e 6720 6461 7461 7365 742e  raining dataset.
-00015630: 0a0a 2020 2020 2020 2020 2121 2120 6578  ..        !!! ex
-00015640: 616d 706c 6520 2252 6561 6469 6e67 2066  ample "Reading f
-00015650: 6561 7475 7265 7320 6174 2061 2073 7065  eatures at a spe
-00015660: 6369 6669 6320 706f 696e 7420 696e 2074  cific point in t
-00015670: 696d 653a 220a 2020 2020 2020 2020 2020  ime:".          
-00015680: 2020 6060 6070 7974 686f 6e0a 2020 2020    ```python.    
-00015690: 2020 2020 2020 2020 2320 636f 6e6e 6563          # connec
-000156a0: 7420 746f 2074 6865 2046 6561 7475 7265  t to the Feature
-000156b0: 2053 746f 7265 0a20 2020 2020 2020 2020   Store.         
-000156c0: 2020 2066 7320 3d20 2e2e 2e0a 0a20 2020     fs = .....   
-000156d0: 2020 2020 2020 2020 2023 2067 6574 2074           # get t
-000156e0: 6865 2046 6561 7475 7265 2047 726f 7570  he Feature Group
-000156f0: 2069 6e73 7461 6e63 650a 2020 2020 2020   instance.      
-00015700: 2020 2020 2020 6667 203d 2066 732e 6765        fg = fs.ge
-00015710: 745f 6f72 5f63 7265 6174 655f 6665 6174  t_or_create_feat
-00015720: 7572 655f 6772 6f75 7028 2e2e 2e29 0a0a  ure_group(...)..
-00015730: 2020 2020 2020 2020 2020 2020 2320 6765              # ge
-00015740: 7420 6461 7461 2061 7420 6120 7370 6563  t data at a spec
-00015750: 6966 6963 2070 6f69 6e74 2069 6e20 7469  ific point in ti
-00015760: 6d65 2061 6e64 2073 686f 7720 6974 0a20  me and show it. 
-00015770: 2020 2020 2020 2020 2020 2066 672e 6173             fg.as
-00015780: 5f6f 6628 2232 3032 302d 3130 2d32 3020  _of("2020-10-20 
-00015790: 3037 3a33 343a 3131 2229 2e72 6561 6428  07:34:11").read(
-000157a0: 292e 7368 6f77 2829 0a20 2020 2020 2020  ).show().       
-000157b0: 2020 2020 2060 6060 0a0a 2020 2020 2020       ```..      
-000157c0: 2020 2121 2120 6578 616d 706c 6520 2252    !!! example "R
-000157d0: 6561 6469 6e67 2063 6f6d 6d69 7473 2069  eading commits i
-000157e0: 6e63 7265 6d65 6e74 616c 6c79 2062 6574  ncrementally bet
-000157f0: 7765 656e 2073 7065 6369 6669 6564 2070  ween specified p
-00015800: 6f69 6e74 7320 696e 2074 696d 653a 220a  oints in time:".
-00015810: 2020 2020 2020 2020 2020 2020 6060 6070              ```p
-00015820: 7974 686f 6e0a 2020 2020 2020 2020 2020  ython.          
-00015830: 2020 6667 2e61 735f 6f66 2822 3230 3230    fg.as_of("2020
-00015840: 2d31 302d 3230 2030 373a 3334 3a31 3122  -10-20 07:34:11"
-00015850: 2c20 6578 636c 7564 655f 756e 7469 6c3d  , exclude_until=
-00015860: 2232 3032 302d 3130 2d31 3920 3037 3a33  "2020-10-19 07:3
-00015870: 343a 3131 2229 2e72 6561 6428 292e 7368  4:11").read().sh
-00015880: 6f77 2829 0a20 2020 2020 2020 2020 2020  ow().           
-00015890: 2060 6060 0a0a 2020 2020 2020 2020 5468   ```..        Th
-000158a0: 6520 6669 7273 7420 7061 7261 6d65 7465  e first paramete
-000158b0: 7220 6973 2069 6e63 6c75 7369 7665 2077  r is inclusive w
-000158c0: 6869 6c65 2074 6865 206c 6174 7465 7220  hile the latter 
-000158d0: 6973 2065 7863 6c75 7369 7665 2e0a 2020  is exclusive..  
-000158e0: 2020 2020 2020 5468 6174 206d 6561 6e73        That means
-000158f0: 2c20 696e 206f 7264 6572 2074 6f20 7175  , in order to qu
-00015900: 6572 7920 6120 7369 6e67 6c65 2063 6f6d  ery a single com
-00015910: 6d69 742c 2079 6f75 206e 6565 6420 746f  mit, you need to
-00015920: 2071 7565 7279 2074 6861 7420 636f 6d6d   query that comm
-00015930: 6974 2074 696d 650a 2020 2020 2020 2020  it time.        
-00015940: 616e 6420 6578 636c 7564 6520 6576 6572  and exclude ever
-00015950: 7974 6869 6e67 206a 7573 7420 6265 666f  ything just befo
-00015960: 7265 2074 6865 2063 6f6d 6d69 742e 0a0a  re the commit...
-00015970: 2020 2020 2020 2020 2121 2120 6578 616d          !!! exam
-00015980: 706c 6520 2252 6561 6469 6e67 206f 6e6c  ple "Reading onl
-00015990: 7920 7468 6520 6368 616e 6765 7320 6672  y the changes fr
-000159a0: 6f6d 2061 2073 696e 676c 6520 636f 6d6d  om a single comm
-000159b0: 6974 220a 2020 2020 2020 2020 2020 2020  it".            
-000159c0: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
-000159d0: 2020 2020 2020 6667 2e61 735f 6f66 2822        fg.as_of("
-000159e0: 3230 3230 2d31 302d 3230 2030 373a 3331  2020-10-20 07:31
-000159f0: 3a33 3822 2c20 6578 636c 7564 655f 756e  :38", exclude_un
-00015a00: 7469 6c3d 2232 3032 302d 3130 2d32 3020  til="2020-10-20 
-00015a10: 3037 3a33 313a 3337 2229 2e72 6561 6428  07:31:37").read(
-00015a20: 292e 7368 6f77 2829 0a20 2020 2020 2020  ).show().       
-00015a30: 2020 2020 2060 6060 0a0a 2020 2020 2020       ```..      
-00015a40: 2020 5768 656e 206e 6f20 7761 6c6c 636c    When no wallcl
-00015a50: 6f63 6b5f 7469 6d65 2069 7320 6769 7665  ock_time is give
-00015a60: 6e2c 2074 6865 206c 6174 6573 7420 7374  n, the latest st
-00015a70: 6174 6520 6f66 2066 6561 7475 7265 7320  ate of features 
-00015a80: 6973 2072 6574 7572 6e65 642e 204f 7074  is returned. Opt
-00015a90: 696f 6e61 6c6c 792c 2063 6f6d 6d69 7473  ionally, commits
-00015aa0: 2062 6566 6f72 650a 2020 2020 2020 2020   before.        
-00015ab0: 6120 7370 6563 6966 6965 6420 706f 696e  a specified poin
-00015ac0: 7420 696e 2074 696d 6520 6361 6e20 7374  t in time can st
-00015ad0: 696c 6c20 6265 2065 7863 6c75 6465 642e  ill be excluded.
-00015ae0: 0a0a 2020 2020 2020 2020 2121 2120 6578  ..        !!! ex
-00015af0: 616d 706c 6520 2252 6561 6469 6e67 2074  ample "Reading t
-00015b00: 6865 206c 6174 6573 7420 7374 6174 6520  he latest state 
-00015b10: 6f66 2066 6561 7475 7265 732c 2065 7863  of features, exc
-00015b20: 6c75 6469 6e67 2063 6f6d 6d69 7473 2062  luding commits b
-00015b30: 6566 6f72 6520 6120 7370 6563 6966 6965  efore a specifie
-00015b40: 6420 706f 696e 7420 696e 2074 696d 653a  d point in time:
-00015b50: 220a 2020 2020 2020 2020 2020 2020 6060  ".            ``
-00015b60: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
-00015b70: 2020 2020 6667 2e61 735f 6f66 284e 6f6e      fg.as_of(Non
-00015b80: 652c 2065 7863 6c75 6465 5f75 6e74 696c  e, exclude_until
-00015b90: 3d22 3230 3230 2d31 302d 3230 2030 373a  ="2020-10-20 07:
-00015ba0: 3331 3a33 3822 292e 7265 6164 2829 2e73  31:38").read().s
-00015bb0: 686f 7728 290a 2020 2020 2020 2020 2020  how().          
-00015bc0: 2020 6060 600a 0a20 2020 2020 2020 204e    ```..        N
-00015bd0: 6f74 6520 7468 6174 2074 6865 2069 6e74  ote that the int
-00015be0: 6572 7661 6c20 7769 6c6c 2062 6520 6170  erval will be ap
-00015bf0: 706c 6965 6420 746f 2061 6c6c 206a 6f69  plied to all joi
-00015c00: 6e73 2069 6e20 7468 6520 7175 6572 792e  ns in the query.
-00015c10: 0a20 2020 2020 2020 2049 6620 796f 7520  .        If you 
-00015c20: 7761 6e74 2074 6f20 7175 6572 7920 6469  want to query di
-00015c30: 6666 6572 656e 7420 696e 7465 7276 616c  fferent interval
-00015c40: 7320 666f 7220 6469 6666 6572 656e 7420  s for different 
-00015c50: 6665 6174 7572 6520 6772 6f75 7073 2069  feature groups i
-00015c60: 6e0a 2020 2020 2020 2020 7468 6520 7175  n.        the qu
-00015c70: 6572 792c 2079 6f75 2068 6176 6520 746f  ery, you have to
-00015c80: 2061 7070 6c79 2074 6865 6d20 696e 2061   apply them in a
-00015c90: 206e 6573 7465 6420 6661 7368 696f 6e3a   nested fashion:
-00015ca0: 0a20 2020 2020 2020 2021 2121 2065 7861  .        !!! exa
-00015cb0: 6d70 6c65 0a20 2020 2020 2020 2020 2020  mple.           
-00015cc0: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
-00015cd0: 2020 2020 2020 2023 2063 6f6e 6e65 6374         # connect
-00015ce0: 2074 6f20 7468 6520 4665 6174 7572 6520   to the Feature 
-00015cf0: 5374 6f72 650a 2020 2020 2020 2020 2020  Store.          
-00015d00: 2020 6673 203d 202e 2e2e 0a0a 2020 2020    fs = .....    
-00015d10: 2020 2020 2020 2020 2320 6765 7420 7468          # get th
-00015d20: 6520 4665 6174 7572 6520 4772 6f75 7020  e Feature Group 
-00015d30: 696e 7374 616e 6365 0a20 2020 2020 2020  instance.       
-00015d40: 2020 2020 2066 6731 203d 2066 732e 6765       fg1 = fs.ge
-00015d50: 745f 6f72 5f63 7265 6174 655f 6665 6174  t_or_create_feat
-00015d60: 7572 655f 6772 6f75 7028 2e2e 2e29 0a20  ure_group(...). 
-00015d70: 2020 2020 2020 2020 2020 2066 6732 203d             fg2 =
-00015d80: 2066 732e 6765 745f 6f72 5f63 7265 6174   fs.get_or_creat
-00015d90: 655f 6665 6174 7572 655f 6772 6f75 7028  e_feature_group(
-00015da0: 2e2e 2e29 0a0a 2020 2020 2020 2020 2020  ...)..          
-00015db0: 2020 6667 312e 7365 6c65 6374 5f61 6c6c    fg1.select_all
-00015dc0: 2829 2e61 735f 6f66 2822 3230 3230 2d31  ().as_of("2020-1
-00015dd0: 302d 3230 222c 2065 7863 6c75 6465 5f75  0-20", exclude_u
-00015de0: 6e74 696c 3d22 3230 3230 2d31 302d 3139  ntil="2020-10-19
-00015df0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00015e00: 2020 202e 6a6f 696e 2866 6732 2e73 656c     .join(fg2.sel
-00015e10: 6563 745f 616c 6c28 292e 6173 5f6f 6628  ect_all().as_of(
-00015e20: 2232 3032 302d 3130 2d32 3022 2c20 6578  "2020-10-20", ex
-00015e30: 636c 7564 655f 756e 7469 6c3d 2232 3032  clude_until="202
-00015e40: 302d 3130 2d31 3922 2929 0a20 2020 2020  0-10-19")).     
-00015e50: 2020 2020 2020 2060 6060 0a0a 2020 2020         ```..    
-00015e60: 2020 2020 4966 2069 6e73 7465 6164 2079      If instead y
-00015e70: 6f75 2061 7070 6c79 2061 6e6f 7468 6572  ou apply another
-00015e80: 2060 6173 5f6f 6660 2073 656c 6563 7469   `as_of` selecti
-00015e90: 6f6e 2061 6674 6572 2074 6865 206a 6f69  on after the joi
-00015ea0: 6e2c 2061 6c6c 0a20 2020 2020 2020 206a  n, all.        j
-00015eb0: 6f69 6e65 6420 6665 6174 7572 6520 6772  oined feature gr
-00015ec0: 6f75 7073 2077 696c 6c20 6265 2071 7565  oups will be que
-00015ed0: 7269 6564 2077 6974 6820 7468 6973 2069  ried with this i
-00015ee0: 6e74 6572 7661 6c3a 0a20 2020 2020 2020  nterval:.       
-00015ef0: 2021 2121 2065 7861 6d70 6c65 0a20 2020   !!! example.   
-00015f00: 2020 2020 2020 2020 2060 6060 7079 7468           ```pyth
-00015f10: 6f6e 0a20 2020 2020 2020 2020 2020 2066  on.            f
-00015f20: 6731 2e73 656c 6563 745f 616c 6c28 292e  g1.select_all().
-00015f30: 6173 5f6f 6628 2232 3032 302d 3130 2d32  as_of("2020-10-2
-00015f40: 3022 2c20 6578 636c 7564 655f 756e 7469  0", exclude_unti
-00015f50: 6c3d 2232 3032 302d 3130 2d31 3922 2920  l="2020-10-19") 
-00015f60: 2023 2061 735f 6f66 2069 7320 6e6f 7420   # as_of is not 
-00015f70: 6170 706c 6965 640a 2020 2020 2020 2020  applied.        
-00015f80: 2020 2020 2020 2020 2e6a 6f69 6e28 6667          .join(fg
-00015f90: 322e 7365 6c65 6374 5f61 6c6c 2829 2e61  2.select_all().a
-00015fa0: 735f 6f66 2822 3230 3230 2d31 302d 3230  s_of("2020-10-20
-00015fb0: 222c 2065 7863 6c75 6465 5f75 6e74 696c  ", exclude_until
-00015fc0: 3d22 3230 3230 2d31 302d 3135 2229 2920  ="2020-10-15")) 
-00015fd0: 2023 2061 735f 6f66 2069 7320 6e6f 7420   # as_of is not 
-00015fe0: 6170 706c 6965 640a 2020 2020 2020 2020  applied.        
-00015ff0: 2020 2020 2020 2020 2e61 735f 6f66 2822          .as_of("
-00016000: 3230 3230 2d31 302d 3230 222c 2065 7863  2020-10-20", exc
-00016010: 6c75 6465 5f75 6e74 696c 3d22 3230 3230  lude_until="2020
-00016020: 2d31 302d 3139 2229 0a20 2020 2020 2020  -10-19").       
-00016030: 2020 2020 2060 6060 0a0a 2020 2020 2020       ```..      
-00016040: 2020 2121 2120 7761 726e 696e 670a 2020    !!! warning.  
-00016050: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-00016060: 756e 6374 696f 6e20 6f6e 6c79 2077 6f72  unction only wor
-00016070: 6b73 2066 6f72 2066 6561 7475 7265 2067  ks for feature g
-00016080: 726f 7570 7320 7769 7468 2074 696d 655f  roups with time_
-00016090: 7472 6176 656c 5f66 6f72 6d61 743d 2748  travel_format='H
-000160a0: 5544 4927 2e0a 0a20 2020 2020 2020 2021  UDI'...        !
-000160b0: 2121 2077 6172 6e69 6e67 0a20 2020 2020  !! warning.     
-000160c0: 2020 2020 2020 2045 7863 6c75 6469 6e67         Excluding
-000160d0: 2063 6f6d 6d69 7473 2076 6961 2065 7863   commits via exc
-000160e0: 6c75 6465 5f75 6e74 696c 2069 7320 6f6e  lude_until is on
-000160f0: 6c79 2070 6f73 7369 626c 6520 7769 7468  ly possible with
-00016100: 696e 2074 6865 2072 616e 6765 206f 6620  in the range of 
-00016110: 7468 6520 4875 6469 2061 6374 6976 6520  the Hudi active 
-00016120: 7469 6d65 6c69 6e65 2e0a 2020 2020 2020  timeline..      
-00016130: 2020 2020 2020 4279 2064 6566 6175 6c74        By default
-00016140: 2c20 4875 6469 206b 6565 7073 2074 6865  , Hudi keeps the
-00016150: 206c 6173 7420 3230 2074 6f20 3330 2063   last 20 to 30 c
-00016160: 6f6d 6d69 7473 2069 6e20 7468 6520 6163  ommits in the ac
-00016170: 7469 7665 2074 696d 656c 696e 652e 0a20  tive timeline.. 
-00016180: 2020 2020 2020 2020 2020 2049 6620 796f             If yo
-00016190: 7520 6e65 6564 2074 6f20 6b65 6570 2061  u need to keep a
-000161a0: 206c 6f6e 6765 7220 6163 7469 7665 2074   longer active t
-000161b0: 696d 656c 696e 652c 2079 6f75 2063 616e  imeline, you can
-000161c0: 206f 7665 7277 7269 7465 2074 6865 206f   overwrite the o
-000161d0: 7074 696f 6e73 3a0a 2020 2020 2020 2020  ptions:.        
-000161e0: 2020 2020 6068 6f6f 6469 652e 6b65 6570      `hoodie.keep
-000161f0: 2e6d 696e 2e63 6f6d 6d69 7473 6020 616e  .min.commits` an
-00016200: 6420 6068 6f6f 6469 652e 6b65 6570 2e6d  d `hoodie.keep.m
-00016210: 6178 2e63 6f6d 6d69 7473 600a 2020 2020  ax.commits`.    
-00016220: 2020 2020 2020 2020 7768 656e 2063 616c          when cal
-00016230: 6c69 6e67 2074 6865 2060 696e 7365 7274  ling the `insert
-00016240: 2829 6020 6d65 7468 6f64 2e0a 0a20 2020  ()` method...   
-00016250: 2020 2020 2023 2041 7267 756d 656e 7473       # Arguments
-00016260: 0a20 2020 2020 2020 2020 2020 2077 616c  .            wal
-00016270: 6c63 6c6f 636b 5f74 696d 653a 2052 6561  lclock_time: Rea
-00016280: 6420 6461 7461 2061 7320 6f66 2074 6869  d data as of thi
-00016290: 7320 706f 696e 7420 696e 2074 696d 652e  s point in time.
-000162a0: 2053 7472 696e 6773 2073 686f 756c 6420   Strings should 
-000162b0: 6265 2066 6f72 6d61 7474 6564 2069 6e20  be formatted in 
-000162c0: 6f6e 6520 6f66 2074 6865 0a20 2020 2020  one of the.     
-000162d0: 2020 2020 2020 2020 2020 2066 6f6c 6c6f             follo
-000162e0: 7769 6e67 2066 6f72 6d61 7473 2060 2559  wing formats `%Y
-000162f0: 2d25 6d2d 2564 602c 2060 2559 2d25 6d2d  -%m-%d`, `%Y-%m-
-00016300: 2564 2025 4860 2c20 6025 592d 256d 2d25  %d %H`, `%Y-%m-%
-00016310: 6420 2548 3a25 4d60 2c20 6f72 2060 2559  d %H:%M`, or `%Y
-00016320: 2d25 6d2d 2564 2025 483a 254d 3a25 5360  -%m-%d %H:%M:%S`
-00016330: 2e0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
-00016340: 636c 7564 655f 756e 7469 6c3a 2045 7863  clude_until: Exc
-00016350: 6c75 6465 2063 6f6d 6d69 7473 2075 6e74  lude commits unt
-00016360: 696c 2074 6869 7320 706f 696e 7420 696e  il this point in
-00016370: 2074 696d 652e 2053 7472 696e 6720 7368   time. String sh
-00016380: 6f75 6c64 2062 6520 666f 726d 6174 7465  ould be formatte
-00016390: 6420 696e 206f 6e65 206f 6620 7468 650a  d in one of the.
-000163a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000163b0: 666f 6c6c 6f77 696e 6720 666f 726d 6174  following format
-000163c0: 7320 6025 592d 256d 2d25 6460 2c20 6025  s `%Y-%m-%d`, `%
-000163d0: 592d 256d 2d25 6420 2548 602c 2060 2559  Y-%m-%d %H`, `%Y
-000163e0: 2d25 6d2d 2564 2025 483a 254d 602c 206f  -%m-%d %H:%M`, o
-000163f0: 7220 6025 592d 256d 2d25 6420 2548 3a25  r `%Y-%m-%d %H:%
-00016400: 4d3a 2553 602e 0a0a 2020 2020 2020 2020  M:%S`...        
-00016410: 2320 5265 7475 726e 730a 2020 2020 2020  # Returns.      
-00016420: 2020 2020 2020 6051 7565 7279 602e 2054        `Query`. T
-00016430: 6865 2071 7565 7279 206f 626a 6563 7420  he query object 
-00016440: 7769 7468 2074 6865 2061 7070 6c69 6564  with the applied
-00016450: 2074 696d 6520 7472 6176 656c 2063 6f6e   time travel con
-00016460: 6469 7469 6f6e 2e0a 2020 2020 2020 2020  dition..        
-00016470: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-00016480: 726e 2073 656c 662e 7365 6c65 6374 5f61  rn self.select_a
-00016490: 6c6c 2829 2e61 735f 6f66 2877 616c 6c63  ll().as_of(wallc
-000164a0: 6c6f 636b 5f74 696d 652c 2065 7863 6c75  lock_time, exclu
-000164b0: 6465 5f75 6e74 696c 290a 0a20 2020 2064  de_until)..    d
-000164c0: 6566 2063 6f6d 7075 7465 5f73 7461 7469  ef compute_stati
-000164d0: 7374 6963 7328 0a20 2020 2020 2020 2073  stics(.        s
-000164e0: 656c 662c 2077 616c 6c63 6c6f 636b 5f74  elf, wallclock_t
-000164f0: 696d 653a 204f 7074 696f 6e61 6c5b 556e  ime: Optional[Un
-00016500: 696f 6e5b 7374 722c 2069 6e74 2c20 6461  ion[str, int, da
-00016510: 7465 7469 6d65 2c20 6461 7465 5d5d 203d  tetime, date]] =
-00016520: 204e 6f6e 650a 2020 2020 293a 0a20 2020   None.    ):.   
-00016530: 2020 2020 2022 2222 5265 636f 6d70 7574       """Recomput
-00016540: 6520 7468 6520 7374 6174 6973 7469 6373  e the statistics
-00016550: 2066 6f72 2074 6865 2066 6561 7475 7265   for the feature
-00016560: 2067 726f 7570 2061 6e64 2073 6176 6520   group and save 
-00016570: 7468 656d 2074 6f20 7468 650a 2020 2020  them to the.    
-00016580: 2020 2020 6665 6174 7572 6520 7374 6f72      feature stor
-00016590: 652e 0a0a 2020 2020 2020 2020 5374 6174  e...        Stat
-000165a0: 6973 7469 6373 2061 7265 206f 6e6c 7920  istics are only 
-000165b0: 636f 6d70 7574 6564 2066 6f72 2064 6174  computed for dat
-000165c0: 6120 696e 2074 6865 206f 6666 6c69 6e65  a in the offline
-000165d0: 2073 746f 7261 6765 206f 6620 7468 6520   storage of the 
-000165e0: 6665 6174 7572 650a 2020 2020 2020 2020  feature.        
-000165f0: 6772 6f75 702e 0a0a 2020 2020 2020 2020  group...        
-00016600: 2320 4172 6775 6d65 6e74 730a 2020 2020  # Arguments.    
-00016610: 2020 2020 2020 2020 7761 6c6c 636c 6f63          wallcloc
-00016620: 6b5f 7469 6d65 3a20 4966 2073 7065 6369  k_time: If speci
-00016630: 6669 6564 2077 696c 6c20 7265 636f 6d70  fied will recomp
-00016640: 7574 6520 7374 6174 6973 7469 6373 206f  ute statistics o
-00016650: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00016660: 2020 6665 6174 7572 6520 6772 6f75 7020    feature group 
-00016670: 6173 206f 6620 7370 6563 6966 6963 2070  as of specific p
-00016680: 6f69 6e74 2069 6e20 7469 6d65 2e20 4966  oint in time. If
-00016690: 206e 6f74 2073 7065 6369 6669 6564 2074   not specified t
-000166a0: 6865 6e20 7769 6c6c 2063 6f6d 7075 7465  hen will compute
-000166b0: 2073 7461 7469 7374 6963 730a 2020 2020   statistics.    
-000166c0: 2020 2020 2020 2020 2020 2020 6173 206f              as o
-000166d0: 6620 6d6f 7374 2072 6563 656e 7420 7469  f most recent ti
-000166e0: 6d65 206f 6620 7468 6973 2066 6561 7475  me of this featu
-000166f0: 7265 2067 726f 7570 2e20 4465 6661 756c  re group. Defaul
-00016700: 7473 2074 6f20 604e 6f6e 6560 2e20 5374  ts to `None`. St
-00016710: 7269 6e67 7320 7368 6f75 6c64 0a20 2020  rings should.   
-00016720: 2020 2020 2020 2020 2020 2020 2062 6520               be 
-00016730: 666f 726d 6174 7465 6420 696e 206f 6e65  formatted in one
-00016740: 206f 6620 7468 6520 666f 6c6c 6f77 696e   of the followin
-00016750: 6720 666f 726d 6174 7320 6025 592d 256d  g formats `%Y-%m
-00016760: 2d25 6460 2c20 6025 592d 256d 2d25 6420  -%d`, `%Y-%m-%d 
-00016770: 2548 602c 2060 2559 2d25 6d2d 2564 2025  %H`, `%Y-%m-%d %
-00016780: 483a 254d 602c 2060 2559 2d25 6d2d 2564  H:%M`, `%Y-%m-%d
-00016790: 2025 483a 254d 3a25 5360 2c0a 2020 2020   %H:%M:%S`,.    
-000167a0: 2020 2020 2020 2020 2020 2020 6f72 2060              or `
-000167b0: 2559 2d25 6d2d 2564 2025 483a 254d 3a25  %Y-%m-%d %H:%M:%
-000167c0: 532e 2566 602e 0a0a 2020 2020 2020 2020  S.%f`...        
-000167d0: 2320 5265 7475 726e 730a 2020 2020 2020  # Returns.      
-000167e0: 2020 2020 2020 6053 7461 7469 7374 6963        `Statistic
-000167f0: 7360 2e20 5468 6520 7374 6174 6973 7469  s`. The statisti
-00016800: 6373 206d 6574 6164 6174 6120 6f62 6a65  cs metadata obje
-00016810: 6374 2e0a 0a20 2020 2020 2020 2023 2052  ct...        # R
-00016820: 6169 7365 730a 2020 2020 2020 2020 2020  aises.          
-00016830: 2020 6068 7366 732e 636c 6965 6e74 2e65    `hsfs.client.e
-00016840: 7863 6570 7469 6f6e 732e 5265 7374 4150  xceptions.RestAP
-00016850: 4945 7272 6f72 602e 2055 6e61 626c 6520  IError`. Unable 
-00016860: 746f 2070 6572 7369 7374 2074 6865 2073  to persist the s
-00016870: 7461 7469 7374 6963 732e 0a20 2020 2020  tatistics..     
-00016880: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00016890: 6620 7365 6c66 2e73 7461 7469 7374 6963  f self.statistic
-000168a0: 735f 636f 6e66 6967 2e65 6e61 626c 6564  s_config.enabled
-000168b0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-000168c0: 446f 6e27 7420 7265 6164 2074 6865 2064  Don't read the d
-000168d0: 6174 6166 7261 6d65 2068 6572 652c 2074  ataframe here, t
-000168e0: 6f20 6176 6f69 6420 7472 6967 6765 7269  o avoid triggeri
-000168f0: 6e67 2061 2072 6561 6420 6f70 6572 6174  ng a read operat
-00016900: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-00016910: 2320 666f 7220 7468 6520 5079 7468 6f6e  # for the Python
-00016920: 2065 6e67 696e 652e 2054 6865 2050 7974   engine. The Pyt
-00016930: 686f 6e20 656e 6769 6e65 2069 7320 676f  hon engine is go
-00016940: 696e 6720 746f 2073 6574 7570 2061 2053  ing to setup a S
-00016950: 7061 726b 204a 6f62 0a20 2020 2020 2020  park Job.       
-00016960: 2020 2020 2023 2074 6f20 7570 6461 7465       # to update
-00016970: 2074 6865 2073 7461 7469 7374 6963 732e   the statistics.
-00016980: 0a0a 2020 2020 2020 2020 2020 2020 6667  ..            fg
-00016990: 5f63 6f6d 6d69 745f 6964 203d 204e 6f6e  _commit_id = Non
-000169a0: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
-000169b0: 2077 616c 6c63 6c6f 636b 5f74 696d 6520   wallclock_time 
-000169c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000169d0: 2020 2020 2020 2020 2020 2020 2023 2052               # R
-000169e0: 6574 7269 6576 6520 6667 2063 6f6d 6d69  etrieve fg commi
-000169f0: 7420 6964 2072 656c 6174 6564 2074 6f20  t id related to 
-00016a00: 7468 6973 2077 616c 6c20 636c 6f63 6b20  this wall clock 
-00016a10: 7469 6d65 2061 6e64 2072 6563 6f6d 7075  time and recompu
-00016a20: 7465 2073 7461 7469 7374 6963 732e 2049  te statistics. I
-00016a30: 7420 7769 6c6c 2074 6872 6f77 0a20 2020  t will throw.   
-00016a40: 2020 2020 2020 2020 2020 2020 2023 2065               # e
-00016a50: 7863 6570 7469 6f6e 2069 6620 6974 7320  xception if its 
-00016a60: 6e6f 7420 7469 6d65 2074 7261 7665 6c20  not time travel 
-00016a70: 656e 6162 6c65 6420 6665 6174 7572 6520  enabled feature 
-00016a80: 6772 6f75 702e 0a20 2020 2020 2020 2020  group..         
-00016a90: 2020 2020 2020 2066 675f 636f 6d6d 6974         fg_commit
-00016aa0: 5f69 6420 3d20 5b0a 2020 2020 2020 2020  _id = [.        
-00016ab0: 2020 2020 2020 2020 2020 2020 636f 6d6d              comm
-00016ac0: 6974 5f69 640a 2020 2020 2020 2020 2020  it_id.          
-00016ad0: 2020 2020 2020 2020 2020 666f 7220 636f            for co
-00016ae0: 6d6d 6974 5f69 6420 696e 2073 656c 662e  mmit_id in self.
-00016af0: 5f66 6561 7475 7265 5f67 726f 7570 5f65  _feature_group_e
-00016b00: 6e67 696e 652e 636f 6d6d 6974 5f64 6574  ngine.commit_det
-00016b10: 6169 6c73 280a 2020 2020 2020 2020 2020  ails(.          
-00016b20: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016b30: 6c66 2c20 7761 6c6c 636c 6f63 6b5f 7469  lf, wallclock_ti
-00016b40: 6d65 2c20 310a 2020 2020 2020 2020 2020  me, 1.          
-00016b50: 2020 2020 2020 2020 2020 292e 6b65 7973            ).keys
-00016b60: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00016b70: 2020 205d 5b30 5d0a 0a20 2020 2020 2020     ][0]..       
-00016b80: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00016b90: 2e5f 7374 6174 6973 7469 6373 5f65 6e67  ._statistics_eng
-00016ba0: 696e 652e 636f 6d70 7574 655f 7374 6174  ine.compute_stat
-00016bb0: 6973 7469 6373 280a 2020 2020 2020 2020  istics(.        
-00016bc0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00016bd0: 2020 2020 2020 2020 2020 2020 2020 6665                fe
-00016be0: 6174 7572 655f 6772 6f75 705f 636f 6d6d  ature_group_comm
-00016bf0: 6974 5f69 643d 6667 5f63 6f6d 6d69 745f  it_id=fg_commit_
-00016c00: 6964 0a20 2020 2020 2020 2020 2020 2020  id.             
-00016c10: 2020 2069 6620 6667 5f63 6f6d 6d69 745f     if fg_commit_
-00016c20: 6964 2069 7320 6e6f 7420 4e6f 6e65 0a20  id is not None. 
-00016c30: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00016c40: 6c73 6520 4e6f 6e65 2c0a 2020 2020 2020  lse None,.      
-00016c50: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00016c60: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00016c70: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
-00016c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016c90: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-00016ca0: 2020 2020 2020 2022 5468 6520 7374 6174         "The stat
-00016cb0: 6973 7469 6373 2061 7265 206e 6f74 2065  istics are not e
-00016cc0: 6e61 626c 6564 206f 6620 6665 6174 7572  nabled of featur
-00016cd0: 6520 6772 6f75 7020 607b 7d60 2c20 7769  e group `{}`, wi
-00016ce0: 7468 2076 6572 7369 6f6e 220a 2020 2020  th version".    
-00016cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d00: 2220 607b 7d60 2e20 4e6f 2073 7461 7469  " `{}`. No stati
-00016d10: 7374 6963 7320 636f 6d70 7574 6564 2e22  stics computed."
-00016d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016d30: 2029 2e66 6f72 6d61 7428 7365 6c66 2e5f   ).format(self._
-00016d40: 6e61 6d65 2c20 7365 6c66 2e5f 7665 7273  name, self._vers
-00016d50: 696f 6e29 2c0a 2020 2020 2020 2020 2020  ion),.          
-00016d60: 2020 2020 2020 7574 696c 2e53 746f 7261        util.Stora
-00016d70: 6765 5761 726e 696e 672c 0a20 2020 2020  geWarning,.     
-00016d80: 2020 2020 2020 2029 0a0a 2020 2020 4063         )..    @c
-00016d90: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
-00016da0: 6566 2066 726f 6d5f 7265 7370 6f6e 7365  ef from_response
-00016db0: 5f6a 736f 6e28 636c 732c 206a 736f 6e5f  _json(cls, json_
-00016dc0: 6469 6374 293a 0a20 2020 2020 2020 206a  dict):.        j
-00016dd0: 736f 6e5f 6465 6361 6d65 6c69 7a65 6420  son_decamelized 
-00016de0: 3d20 6875 6d70 732e 6465 6361 6d65 6c69  = humps.decameli
-00016df0: 7a65 286a 736f 6e5f 6469 6374 290a 2020  ze(json_dict).  
-00016e00: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00016e10: 6e63 6528 6a73 6f6e 5f64 6563 616d 656c  nce(json_decamel
-00016e20: 697a 6564 2c20 6469 6374 293a 0a20 2020  ized, dict):.   
-00016e30: 2020 2020 2020 2020 2069 6620 2274 7970           if "typ
-00016e40: 6522 2069 6e20 6a73 6f6e 5f64 6563 616d  e" in json_decam
-00016e50: 656c 697a 6564 3a0a 2020 2020 2020 2020  elized:.        
-00016e60: 2020 2020 2020 2020 6a73 6f6e 5f64 6563          json_dec
-00016e70: 616d 656c 697a 6564 5b22 7374 7265 616d  amelized["stream
-00016e80: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
-00016e90: 2020 2020 2020 2020 2020 206a 736f 6e5f             json_
-00016ea0: 6465 6361 6d65 6c69 7a65 645b 2274 7970  decamelized["typ
-00016eb0: 6522 5d20 3d3d 2022 7374 7265 616d 4665  e"] == "streamFe
-00016ec0: 6174 7572 6547 726f 7570 4454 4f22 0a20  atureGroupDTO". 
-00016ed0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00016ee0: 0a20 2020 2020 2020 2020 2020 205f 203d  .            _ =
-00016ef0: 206a 736f 6e5f 6465 6361 6d65 6c69 7a65   json_decamelize
-00016f00: 642e 706f 7028 2274 7970 6522 2c20 4e6f  d.pop("type", No
-00016f10: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
-00016f20: 6a73 6f6e 5f64 6563 616d 656c 697a 6564  json_decamelized
-00016f30: 2e70 6f70 2822 7661 6c69 6461 7469 6f6e  .pop("validation
-00016f40: 5f74 7970 6522 2c20 4e6f 6e65 290a 2020  _type", None).  
-00016f50: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00016f60: 2063 6c73 282a 2a6a 736f 6e5f 6465 6361   cls(**json_deca
-00016f70: 6d65 6c69 7a65 6429 0a20 2020 2020 2020  melized).       
-00016f80: 2066 6f72 2066 6720 696e 206a 736f 6e5f   for fg in json_
-00016f90: 6465 6361 6d65 6c69 7a65 643a 0a20 2020  decamelized:.   
-00016fa0: 2020 2020 2020 2020 2069 6620 2274 7970           if "typ
-00016fb0: 6522 2069 6e20 6667 3a0a 2020 2020 2020  e" in fg:.      
-00016fc0: 2020 2020 2020 2020 2020 6667 5b22 7374            fg["st
-00016fd0: 7265 616d 225d 203d 2066 675b 2274 7970  ream"] = fg["typ
-00016fe0: 6522 5d20 3d3d 2022 7374 7265 616d 4665  e"] == "streamFe
-00016ff0: 6174 7572 6547 726f 7570 4454 4f22 0a20  atureGroupDTO". 
-00017000: 2020 2020 2020 2020 2020 205f 203d 2066             _ = f
-00017010: 672e 706f 7028 2274 7970 6522 2c20 4e6f  g.pop("type", No
-00017020: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
-00017030: 6667 2e70 6f70 2822 7661 6c69 6461 7469  fg.pop("validati
-00017040: 6f6e 5f74 7970 6522 2c20 4e6f 6e65 290a  on_type", None).
-00017050: 2020 2020 2020 2020 7265 7475 726e 205b          return [
-00017060: 636c 7328 2a2a 6667 2920 666f 7220 6667  cls(**fg) for fg
-00017070: 2069 6e20 6a73 6f6e 5f64 6563 616d 656c   in json_decamel
-00017080: 697a 6564 5d0a 0a20 2020 2064 6566 2075  ized]..    def u
-00017090: 7064 6174 655f 6672 6f6d 5f72 6573 706f  pdate_from_respo
-000170a0: 6e73 655f 6a73 6f6e 2873 656c 662c 206a  nse_json(self, j
-000170b0: 736f 6e5f 6469 6374 293a 0a20 2020 2020  son_dict):.     
-000170c0: 2020 206a 736f 6e5f 6465 6361 6d65 6c69     json_decameli
-000170d0: 7a65 6420 3d20 6875 6d70 732e 6465 6361  zed = humps.deca
-000170e0: 6d65 6c69 7a65 286a 736f 6e5f 6469 6374  melize(json_dict
-000170f0: 290a 2020 2020 2020 2020 6a73 6f6e 5f64  ).        json_d
-00017100: 6563 616d 656c 697a 6564 5b22 7374 7265  ecamelized["stre
-00017110: 616d 225d 203d 206a 736f 6e5f 6465 6361  am"] = json_deca
-00017120: 6d65 6c69 7a65 645b 2274 7970 6522 5d20  melized["type"] 
-00017130: 3d3d 2022 7374 7265 616d 4665 6174 7572  == "streamFeatur
-00017140: 6547 726f 7570 4454 4f22 0a20 2020 2020  eGroupDTO".     
-00017150: 2020 205f 203d 206a 736f 6e5f 6465 6361     _ = json_deca
-00017160: 6d65 6c69 7a65 642e 706f 7028 2274 7970  melized.pop("typ
-00017170: 6522 290a 2020 2020 2020 2020 7365 6c66  e").        self
-00017180: 2e5f 5f69 6e69 745f 5f28 2a2a 6a73 6f6e  .__init__(**json
-00017190: 5f64 6563 616d 656c 697a 6564 290a 2020  _decamelized).  
-000171a0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000171b0: 660a 0a20 2020 2064 6566 206a 736f 6e28  f..    def json(
-000171c0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-000171d0: 2222 4765 7420 7370 6563 6966 6963 2046  ""Get specific F
-000171e0: 6561 7475 7265 2047 726f 7570 206d 6574  eature Group met
-000171f0: 6164 6174 6120 696e 206a 736f 6e20 666f  adata in json fo
-00017200: 726d 6174 2e0a 0a20 2020 2020 2020 2021  rmat...        !
-00017210: 2121 2065 7861 6d70 6c65 0a20 2020 2020  !! example.     
-00017220: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
-00017230: 0a20 2020 2020 2020 2020 2020 2066 672e  .            fg.
-00017240: 6a73 6f6e 2829 0a20 2020 2020 2020 2020  json().         
-00017250: 2020 2060 6060 0a20 2020 2020 2020 2022     ```.        "
-00017260: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-00017270: 6e20 6a73 6f6e 2e64 756d 7073 2873 656c  n json.dumps(sel
-00017280: 662c 2063 6c73 3d75 7469 6c2e 4665 6174  f, cls=util.Feat
-00017290: 7572 6553 746f 7265 456e 636f 6465 7229  ureStoreEncoder)
-000172a0: 0a0a 2020 2020 6465 6620 746f 5f64 6963  ..    def to_dic
-000172b0: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
-000172c0: 2022 2222 4765 7420 7374 7275 6374 7572   """Get structur
-000172d0: 6564 2069 6e66 6f20 6162 6f75 7420 7370  ed info about sp
-000172e0: 6563 6966 6963 2046 6561 7475 7265 2047  ecific Feature G
-000172f0: 726f 7570 2069 6e20 7079 7468 6f6e 2064  roup in python d
-00017300: 6963 7469 6f6e 6172 7920 666f 726d 6174  ictionary format
-00017310: 2e0a 0a20 2020 2020 2020 2021 2121 2065  ...        !!! e
-00017320: 7861 6d70 6c65 0a20 2020 2020 2020 2020  xample.         
-00017330: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
-00017340: 2020 2020 2020 2020 2023 2063 6f6e 6e65           # conne
-00017350: 6374 2074 6f20 7468 6520 4665 6174 7572  ct to the Featur
-00017360: 6520 5374 6f72 650a 2020 2020 2020 2020  e Store.        
-00017370: 2020 2020 6673 203d 202e 2e2e 0a0a 2020      fs = .....  
-00017380: 2020 2020 2020 2020 2020 2320 6765 7420            # get 
-00017390: 7468 6520 4665 6174 7572 6520 4772 6f75  the Feature Grou
-000173a0: 7020 696e 7374 616e 6365 0a20 2020 2020  p instance.     
-000173b0: 2020 2020 2020 2066 6720 3d20 6673 2e67         fg = fs.g
-000173c0: 6574 5f6f 725f 6372 6561 7465 5f66 6561  et_or_create_fea
-000173d0: 7475 7265 5f67 726f 7570 282e 2e2e 290a  ture_group(...).
-000173e0: 0a20 2020 2020 2020 2020 2020 2066 672e  .            fg.
-000173f0: 746f 5f64 6963 7428 290a 2020 2020 2020  to_dict().      
-00017400: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
-00017410: 2020 2222 220a 2020 2020 2020 2020 6667    """.        fg
-00017420: 5f6d 6574 615f 6469 6374 203d 207b 0a20  _meta_dict = {. 
-00017430: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
-00017440: 2073 656c 662e 5f69 642c 0a20 2020 2020   self._id,.     
-00017450: 2020 2020 2020 2022 6e61 6d65 223a 2073         "name": s
-00017460: 656c 662e 5f6e 616d 652c 0a20 2020 2020  elf._name,.     
-00017470: 2020 2020 2020 2022 7665 7273 696f 6e22         "version"
-00017480: 3a20 7365 6c66 2e5f 7665 7273 696f 6e2c  : self._version,
-00017490: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
-000174a0: 7363 7269 7074 696f 6e22 3a20 7365 6c66  scription": self
-000174b0: 2e5f 6465 7363 7269 7074 696f 6e2c 0a20  ._description,. 
-000174c0: 2020 2020 2020 2020 2020 2022 6f6e 6c69             "onli
-000174d0: 6e65 456e 6162 6c65 6422 3a20 7365 6c66  neEnabled": self
-000174e0: 2e5f 6f6e 6c69 6e65 5f65 6e61 626c 6564  ._online_enabled
-000174f0: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
-00017500: 696d 6554 7261 7665 6c46 6f72 6d61 7422  imeTravelFormat"
-00017510: 3a20 7365 6c66 2e5f 7469 6d65 5f74 7261  : self._time_tra
-00017520: 7665 6c5f 666f 726d 6174 2c0a 2020 2020  vel_format,.    
-00017530: 2020 2020 2020 2020 2266 6561 7475 7265          "feature
-00017540: 7322 3a20 7365 6c66 2e5f 6665 6174 7572  s": self._featur
-00017550: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00017560: 2266 6561 7475 7265 7374 6f72 6549 6422  "featurestoreId"
-00017570: 3a20 7365 6c66 2e5f 6665 6174 7572 655f  : self._feature_
-00017580: 7374 6f72 655f 6964 2c0a 2020 2020 2020  store_id,.      
-00017590: 2020 2020 2020 2274 7970 6522 3a20 2263        "type": "c
-000175a0: 6163 6865 6446 6561 7475 7265 6772 6f75  achedFeaturegrou
-000175b0: 7044 544f 220a 2020 2020 2020 2020 2020  pDTO".          
-000175c0: 2020 6966 206e 6f74 2073 656c 662e 5f73    if not self._s
-000175d0: 7472 6561 6d0a 2020 2020 2020 2020 2020  tream.          
-000175e0: 2020 656c 7365 2022 7374 7265 616d 4665    else "streamFe
-000175f0: 6174 7572 6547 726f 7570 4454 4f22 2c0a  atureGroupDTO",.
-00017600: 2020 2020 2020 2020 2020 2020 2273 7461              "sta
-00017610: 7469 7374 6963 7343 6f6e 6669 6722 3a20  tisticsConfig": 
-00017620: 7365 6c66 2e5f 7374 6174 6973 7469 6373  self._statistics
-00017630: 5f63 6f6e 6669 672c 0a20 2020 2020 2020  _config,.       
-00017640: 2020 2020 2022 6576 656e 7454 696d 6522       "eventTime"
-00017650: 3a20 7365 6c66 2e65 7665 6e74 5f74 696d  : self.event_tim
-00017660: 652c 0a20 2020 2020 2020 2020 2020 2022  e,.            "
-00017670: 6578 7065 6374 6174 696f 6e53 7569 7465  expectationSuite
-00017680: 223a 2073 656c 662e 5f65 7870 6563 7461  ": self._expecta
-00017690: 7469 6f6e 5f73 7569 7465 2c0a 2020 2020  tion_suite,.    
-000176a0: 2020 2020 2020 2020 2270 6172 656e 7473          "parents
-000176b0: 223a 2073 656c 662e 5f70 6172 656e 7473  ": self._parents
-000176c0: 2c0a 2020 2020 2020 2020 7d0a 2020 2020  ,.        }.    
-000176d0: 2020 2020 6966 2073 656c 662e 5f73 7472      if self._str
-000176e0: 6561 6d3a 0a20 2020 2020 2020 2020 2020  eam:.           
-000176f0: 2066 675f 6d65 7461 5f64 6963 745b 2264   fg_meta_dict["d
-00017700: 656c 7461 5374 7265 616d 6572 4a6f 6243  eltaStreamerJobC
-00017710: 6f6e 6622 5d20 3d20 7365 6c66 2e5f 6465  onf"] = self._de
-00017720: 6c74 6173 7472 6561 6d65 725f 6a6f 6263  ltastreamer_jobc
-00017730: 6f6e 660a 2020 2020 2020 2020 7265 7475  onf.        retu
-00017740: 726e 2066 675f 6d65 7461 5f64 6963 740a  rn fg_meta_dict.
-00017750: 0a20 2020 2064 6566 205f 6765 745f 7461  .    def _get_ta
-00017760: 626c 655f 6e61 6d65 2873 656c 6629 3a0a  ble_name(self):.
-00017770: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00017780: 656c 662e 6665 6174 7572 655f 7374 6f72  elf.feature_stor
-00017790: 655f 6e61 6d65 202b 2022 2e22 202b 2073  e_name + "." + s
-000177a0: 656c 662e 6e61 6d65 202b 2022 5f22 202b  elf.name + "_" +
-000177b0: 2073 7472 2873 656c 662e 7665 7273 696f   str(self.versio
-000177c0: 6e29 0a0a 2020 2020 6465 6620 5f67 6574  n)..    def _get
-000177d0: 5f6f 6e6c 696e 655f 7461 626c 655f 6e61  _online_table_na
-000177e0: 6d65 2873 656c 6629 3a0a 2020 2020 2020  me(self):.      
-000177f0: 2020 7265 7475 726e 2073 656c 662e 6e61    return self.na
-00017800: 6d65 202b 2022 5f22 202b 2073 7472 2873  me + "_" + str(s
-00017810: 656c 662e 7665 7273 696f 6e29 0a0a 2020  elf.version)..  
-00017820: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00017830: 6465 6620 6964 2873 656c 6629 3a0a 2020  def id(self):.  
-00017840: 2020 2020 2020 2222 2246 6561 7475 7265        """Feature
-00017850: 2067 726f 7570 2069 642e 2222 220a 2020   group id.""".  
-00017860: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00017870: 662e 5f69 640a 0a20 2020 2040 7072 6f70  f._id..    @prop
-00017880: 6572 7479 0a20 2020 2064 6566 206e 616d  erty.    def nam
-00017890: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-000178a0: 2022 2222 4e61 6d65 206f 6620 7468 6520   """Name of the 
-000178b0: 6665 6174 7572 6520 6772 6f75 702e 2222  feature group.""
-000178c0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-000178d0: 2073 656c 662e 5f6e 616d 650a 0a20 2020   self._name..   
-000178e0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-000178f0: 6566 2076 6572 7369 6f6e 2873 656c 6629  ef version(self)
-00017900: 3a0a 2020 2020 2020 2020 2222 2256 6572  :.        """Ver
-00017910: 7369 6f6e 206e 756d 6265 7220 6f66 2074  sion number of t
-00017920: 6865 2066 6561 7475 7265 2067 726f 7570  he feature group
-00017930: 2e22 2222 0a20 2020 2020 2020 2072 6574  .""".        ret
-00017940: 7572 6e20 7365 6c66 2e5f 7665 7273 696f  urn self._versio
-00017950: 6e0a 0a20 2020 2040 7072 6f70 6572 7479  n..    @property
-00017960: 0a20 2020 2064 6566 2064 6573 6372 6970  .    def descrip
-00017970: 7469 6f6e 2873 656c 6629 3a0a 2020 2020  tion(self):.    
-00017980: 2020 2020 2222 2244 6573 6372 6970 7469      """Descripti
-00017990: 6f6e 206f 6620 7468 6520 6665 6174 7572  on of the featur
-000179a0: 6520 6772 6f75 7020 636f 6e74 656e 7473  e group contents
-000179b0: 2e22 2222 0a20 2020 2020 2020 2072 6574  .""".        ret
-000179c0: 7572 6e20 7365 6c66 2e5f 6465 7363 7269  urn self._descri
-000179d0: 7074 696f 6e0a 0a20 2020 2040 7072 6f70  ption..    @prop
-000179e0: 6572 7479 0a20 2020 2064 6566 2066 6561  erty.    def fea
-000179f0: 7475 7265 7328 7365 6c66 293a 0a20 2020  tures(self):.   
-00017a00: 2020 2020 2022 2222 5363 6865 6d61 2069       """Schema i
-00017a10: 6e66 6f72 6d61 7469 6f6e 2e22 2222 0a20  nformation.""". 
-00017a20: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00017a30: 6c66 2e5f 6665 6174 7572 6573 0a0a 2020  lf._features..  
-00017a40: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00017a50: 6465 6620 7469 6d65 5f74 7261 7665 6c5f  def time_travel_
-00017a60: 666f 726d 6174 2873 656c 6629 3a0a 2020  format(self):.  
-00017a70: 2020 2020 2020 2222 2253 6574 7469 6e67        """Setting
-00017a80: 206f 6620 7468 6520 6665 6174 7572 6520   of the feature 
-00017a90: 6772 6f75 7020 7469 6d65 2074 7261 7665  group time trave
-00017aa0: 6c20 666f 726d 6174 2e22 2222 0a20 2020  l format.""".   
-00017ab0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00017ac0: 2e5f 7469 6d65 5f74 7261 7665 6c5f 666f  ._time_travel_fo
-00017ad0: 726d 6174 0a0a 2020 2020 4070 726f 7065  rmat..    @prope
-00017ae0: 7274 790a 2020 2020 6465 6620 7061 7274  rty.    def part
-00017af0: 6974 696f 6e5f 6b65 7928 7365 6c66 293a  ition_key(self):
-00017b00: 0a20 2020 2020 2020 2022 2222 4c69 7374  .        """List
-00017b10: 206f 6620 6665 6174 7572 6573 2062 7569   of features bui
-00017b20: 6c64 696e 6720 7468 6520 7061 7274 6974  lding the partit
-00017b30: 696f 6e20 6b65 792e 2222 220a 2020 2020  ion key.""".    
-00017b40: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00017b50: 5f70 6172 7469 7469 6f6e 5f6b 6579 0a0a  _partition_key..
-00017b60: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00017b70: 2020 6465 6620 6875 6469 5f70 7265 636f    def hudi_preco
-00017b80: 6d62 696e 655f 6b65 7928 7365 6c66 293a  mbine_key(self):
-00017b90: 0a20 2020 2020 2020 2022 2222 4665 6174  .        """Feat
-00017ba0: 7572 6520 6e61 6d65 2074 6861 7420 6973  ure name that is
-00017bb0: 2074 6865 2068 7564 6920 7072 6563 6f6d   the hudi precom
-00017bc0: 6269 6e65 206b 6579 2e22 2222 0a20 2020  bine key.""".   
-00017bd0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00017be0: 2e5f 6875 6469 5f70 7265 636f 6d62 696e  ._hudi_precombin
-00017bf0: 655f 6b65 790a 0a20 2020 2040 7072 6f70  e_key..    @prop
-00017c00: 6572 7479 0a20 2020 2064 6566 2066 6561  erty.    def fea
-00017c10: 7475 7265 5f73 746f 7265 5f69 6428 7365  ture_store_id(se
-00017c20: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
-00017c30: 7572 6e20 7365 6c66 2e5f 6665 6174 7572  urn self._featur
-00017c40: 655f 7374 6f72 655f 6964 0a0a 2020 2020  e_store_id..    
-00017c50: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00017c60: 6620 6665 6174 7572 655f 7374 6f72 655f  f feature_store_
-00017c70: 6e61 6d65 2873 656c 6629 3a0a 2020 2020  name(self):.    
-00017c80: 2020 2020 2222 224e 616d 6520 6f66 2074      """Name of t
-00017c90: 6865 2066 6561 7475 7265 2073 746f 7265  he feature store
-00017ca0: 2069 6e20 7768 6963 6820 7468 6520 6665   in which the fe
-00017cb0: 6174 7572 6520 6772 6f75 7020 6973 206c  ature group is l
-00017cc0: 6f63 6174 6564 2e22 2222 0a20 2020 2020  ocated.""".     
-00017cd0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00017ce0: 6665 6174 7572 655f 7374 6f72 655f 6e61  feature_store_na
-00017cf0: 6d65 0a0a 2020 2020 4070 726f 7065 7274  me..    @propert
-00017d00: 790a 2020 2020 6465 6620 6372 6561 746f  y.    def creato
-00017d10: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
-00017d20: 2022 2222 5573 6572 6e61 6d65 206f 6620   """Username of 
-00017d30: 7468 6520 6372 6561 746f 722e 2222 220a  the creator.""".
-00017d40: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00017d50: 656c 662e 5f63 7265 6174 6f72 0a0a 2020  elf._creator..  
-00017d60: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
-00017d70: 6465 6620 6372 6561 7465 6428 7365 6c66  def created(self
-00017d80: 293a 0a20 2020 2020 2020 2022 2222 5469  ):.        """Ti
-00017d90: 6d65 7374 616d 7020 7768 656e 2074 6865  mestamp when the
-00017da0: 2066 6561 7475 7265 2067 726f 7570 2077   feature group w
-00017db0: 6173 2063 7265 6174 6564 2e22 2222 0a20  as created.""". 
-00017dc0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00017dd0: 6c66 2e5f 6372 6561 7465 640a 0a20 2020  lf._created..   
-00017de0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00017df0: 6566 2073 7472 6561 6d28 7365 6c66 293a  ef stream(self):
-00017e00: 0a20 2020 2020 2020 2022 2222 5768 6574  .        """Whet
-00017e10: 6865 7220 746f 2065 6e61 626c 6520 7265  her to enable re
-00017e20: 616c 2074 696d 6520 7374 7265 616d 2077  al time stream w
-00017e30: 7269 7469 6e67 2063 6170 6162 696c 6974  riting capabilit
-00017e40: 6965 732e 2222 220a 2020 2020 2020 2020  ies.""".        
-00017e50: 7265 7475 726e 2073 656c 662e 5f73 7472  return self._str
-00017e60: 6561 6d0a 0a20 2020 2040 7072 6f70 6572  eam..    @proper
-00017e70: 7479 0a20 2020 2064 6566 2070 6172 656e  ty.    def paren
-00017e80: 7473 2873 656c 6629 3a0a 2020 2020 2020  ts(self):.      
-00017e90: 2020 2222 2250 6172 656e 7420 6665 6174    """Parent feat
-00017ea0: 7572 6520 6772 6f75 7073 2061 7320 6f72  ure groups as or
-00017eb0: 6967 696e 206f 6620 7468 6520 6461 7461  igin of the data
-00017ec0: 2069 6e20 7468 6520 6375 7272 656e 7420   in the current 
-00017ed0: 6665 6174 7572 6520 6772 6f75 702e 0a20  feature group.. 
-00017ee0: 2020 2020 2020 2054 6869 7320 6973 2070         This is p
-00017ef0: 6172 7420 6f66 2065 7870 6c69 6369 7420  art of explicit 
-00017f00: 7072 6f76 656e 616e 6365 2222 220a 2020  provenance""".  
-00017f10: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00017f20: 662e 5f70 6172 656e 7473 0a0a 2020 2020  f._parents..    
-00017f30: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00017f40: 6620 6261 636b 6669 6c6c 5f6a 6f62 2873  f backfill_job(s
-00017f50: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00017f60: 2247 6574 2074 6865 204a 6f62 206f 626a  "Get the Job obj
-00017f70: 6563 7420 7265 6665 7265 6e63 6520 666f  ect reference fo
-00017f80: 7220 7468 6520 6261 636b 6669 6c6c 206a  r the backfill j
-00017f90: 6f62 2066 6f72 2074 6869 730a 2020 2020  ob for this.    
-00017fa0: 2020 2020 4665 6174 7572 6520 4772 6f75      Feature Grou
-00017fb0: 702e 2222 220a 2020 2020 2020 2020 6966  p.""".        if
-00017fc0: 2073 656c 662e 5f62 6163 6b66 696c 6c5f   self._backfill_
-00017fd0: 6a6f 6220 6973 204e 6f6e 653a 0a20 2020  job is None:.   
-00017fe0: 2020 2020 2020 2020 206a 6f62 5f6e 616d           job_nam
-00017ff0: 6520 3d20 227b 6667 5f6e 616d 657d 5f7b  e = "{fg_name}_{
-00018000: 7665 7273 696f 6e7d 5f6f 6666 6c69 6e65  version}_offline
-00018010: 5f66 675f 6261 636b 6669 6c6c 222e 666f  _fg_backfill".fo
-00018020: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-00018030: 2020 2020 2020 6667 5f6e 616d 653d 7365        fg_name=se
-00018040: 6c66 2e5f 6e61 6d65 2c20 7665 7273 696f  lf._name, versio
-00018050: 6e3d 7365 6c66 2e5f 7665 7273 696f 6e0a  n=self._version.
-00018060: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00018070: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00018080: 6261 636b 6669 6c6c 5f6a 6f62 203d 206a  backfill_job = j
-00018090: 6f62 5f61 7069 2e4a 6f62 4170 6928 292e  ob_api.JobApi().
-000180a0: 6765 7428 6a6f 625f 6e61 6d65 290a 2020  get(job_name).  
-000180b0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000180c0: 662e 5f62 6163 6b66 696c 6c5f 6a6f 620a  f._backfill_job.
-000180d0: 0a20 2020 2040 7665 7273 696f 6e2e 7365  .    @version.se
-000180e0: 7474 6572 0a20 2020 2064 6566 2076 6572  tter.    def ver
-000180f0: 7369 6f6e 2873 656c 662c 2076 6572 7369  sion(self, versi
-00018100: 6f6e 293a 0a20 2020 2020 2020 2073 656c  on):.        sel
-00018110: 662e 5f76 6572 7369 6f6e 203d 2076 6572  f._version = ver
-00018120: 7369 6f6e 0a0a 2020 2020 4064 6573 6372  sion..    @descr
-00018130: 6970 7469 6f6e 2e73 6574 7465 720a 2020  iption.setter.  
-00018140: 2020 6465 6620 6465 7363 7269 7074 696f    def descriptio
-00018150: 6e28 7365 6c66 2c20 6e65 775f 6465 7363  n(self, new_desc
-00018160: 7269 7074 696f 6e29 3a0a 2020 2020 2020  ription):.      
-00018170: 2020 7365 6c66 2e5f 6465 7363 7269 7074    self._descript
-00018180: 696f 6e20 3d20 6e65 775f 6465 7363 7269  ion = new_descri
-00018190: 7074 696f 6e0a 0a20 2020 2040 6665 6174  ption..    @feat
-000181a0: 7572 6573 2e73 6574 7465 720a 2020 2020  ures.setter.    
-000181b0: 6465 6620 6665 6174 7572 6573 2873 656c  def features(sel
-000181c0: 662c 206e 6577 5f66 6561 7475 7265 7329  f, new_features)
-000181d0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-000181e0: 6665 6174 7572 6573 203d 206e 6577 5f66  features = new_f
-000181f0: 6561 7475 7265 730a 0a20 2020 2040 7469  eatures..    @ti
-00018200: 6d65 5f74 7261 7665 6c5f 666f 726d 6174  me_travel_format
-00018210: 2e73 6574 7465 720a 2020 2020 6465 6620  .setter.    def 
-00018220: 7469 6d65 5f74 7261 7665 6c5f 666f 726d  time_travel_form
-00018230: 6174 2873 656c 662c 206e 6577 5f74 696d  at(self, new_tim
-00018240: 655f 7472 6176 656c 5f66 6f72 6d61 7429  e_travel_format)
-00018250: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
-00018260: 7469 6d65 5f74 7261 7665 6c5f 666f 726d  time_travel_form
-00018270: 6174 203d 206e 6577 5f74 696d 655f 7472  at = new_time_tr
-00018280: 6176 656c 5f66 6f72 6d61 740a 0a20 2020  avel_format..   
-00018290: 2040 7061 7274 6974 696f 6e5f 6b65 792e   @partition_key.
-000182a0: 7365 7474 6572 0a20 2020 2064 6566 2070  setter.    def p
-000182b0: 6172 7469 7469 6f6e 5f6b 6579 2873 656c  artition_key(sel
-000182c0: 662c 206e 6577 5f70 6172 7469 7469 6f6e  f, new_partition
-000182d0: 5f6b 6579 293a 0a20 2020 2020 2020 2073  _key):.        s
-000182e0: 656c 662e 5f70 6172 7469 7469 6f6e 5f6b  elf._partition_k
-000182f0: 6579 203d 205b 706b 2e6c 6f77 6572 2829  ey = [pk.lower()
-00018300: 2066 6f72 2070 6b20 696e 206e 6577 5f70   for pk in new_p
-00018310: 6172 7469 7469 6f6e 5f6b 6579 5d0a 0a20  artition_key].. 
-00018320: 2020 2040 6875 6469 5f70 7265 636f 6d62     @hudi_precomb
-00018330: 696e 655f 6b65 792e 7365 7474 6572 0a20  ine_key.setter. 
-00018340: 2020 2064 6566 2068 7564 695f 7072 6563     def hudi_prec
-00018350: 6f6d 6269 6e65 5f6b 6579 2873 656c 662c  ombine_key(self,
-00018360: 2068 7564 695f 7072 6563 6f6d 6269 6e65   hudi_precombine
-00018370: 5f6b 6579 293a 0a20 2020 2020 2020 2073  _key):.        s
-00018380: 656c 662e 5f68 7564 695f 7072 6563 6f6d  elf._hudi_precom
-00018390: 6269 6e65 5f6b 6579 203d 2068 7564 695f  bine_key = hudi_
-000183a0: 7072 6563 6f6d 6269 6e65 5f6b 6579 2e6c  precombine_key.l
-000183b0: 6f77 6572 2829 0a0a 2020 2020 4073 7472  ower()..    @str
-000183c0: 6561 6d2e 7365 7474 6572 0a20 2020 2064  eam.setter.    d
-000183d0: 6566 2073 7472 6561 6d28 7365 6c66 2c20  ef stream(self, 
-000183e0: 7374 7265 616d 293a 0a20 2020 2020 2020  stream):.       
-000183f0: 2073 656c 662e 5f73 7472 6561 6d20 3d20   self._stream = 
-00018400: 7374 7265 616d 0a0a 2020 2020 4070 6172  stream..    @par
-00018410: 656e 7473 2e73 6574 7465 720a 2020 2020  ents.setter.    
-00018420: 6465 6620 7061 7265 6e74 7328 7365 6c66  def parents(self
-00018430: 2c20 6e65 775f 7061 7265 6e74 7329 3a0a  , new_parents):.
-00018440: 2020 2020 2020 2020 7365 6c66 2e5f 7061          self._pa
-00018450: 7265 6e74 7320 3d20 6e65 775f 7061 7265  rents = new_pare
-00018460: 6e74 730a 0a0a 636c 6173 7320 4578 7465  nts...class Exte
-00018470: 726e 616c 4665 6174 7572 6547 726f 7570  rnalFeatureGroup
-00018480: 2846 6561 7475 7265 4772 6f75 7042 6173  (FeatureGroupBas
-00018490: 6529 3a0a 2020 2020 4558 5445 524e 414c  e):.    EXTERNAL
-000184a0: 5f46 4541 5455 5245 5f47 524f 5550 203d  _FEATURE_GROUP =
-000184b0: 2022 4f4e 5f44 454d 414e 445f 4645 4154   "ON_DEMAND_FEAT
-000184c0: 5552 455f 4752 4f55 5022 0a20 2020 2045  URE_GROUP".    E
-000184d0: 4e54 4954 595f 5459 5045 203d 2022 6665  NTITY_TYPE = "fe
-000184e0: 6174 7572 6567 726f 7570 7322 0a0a 2020  aturegroups"..  
-000184f0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-00018500: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00018510: 2020 2020 2020 7374 6f72 6167 655f 636f        storage_co
-00018520: 6e6e 6563 746f 722c 0a20 2020 2020 2020  nnector,.       
-00018530: 2071 7565 7279 3d4e 6f6e 652c 0a20 2020   query=None,.   
-00018540: 2020 2020 2064 6174 615f 666f 726d 6174       data_format
-00018550: 3d4e 6f6e 652c 0a20 2020 2020 2020 2070  =None,.        p
-00018560: 6174 683d 4e6f 6e65 2c0a 2020 2020 2020  ath=None,.      
-00018570: 2020 6f70 7469 6f6e 733d 7b7d 2c0a 2020    options={},.  
-00018580: 2020 2020 2020 6e61 6d65 3d4e 6f6e 652c        name=None,
-00018590: 0a20 2020 2020 2020 2076 6572 7369 6f6e  .        version
-000185a0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2064  =None,.        d
-000185b0: 6573 6372 6970 7469 6f6e 3d4e 6f6e 652c  escription=None,
-000185c0: 0a20 2020 2020 2020 2070 7269 6d61 7279  .        primary
-000185d0: 5f6b 6579 3d4e 6f6e 652c 0a20 2020 2020  _key=None,.     
-000185e0: 2020 2066 6561 7475 7265 7374 6f72 655f     featurestore_
-000185f0: 6964 3d4e 6f6e 652c 0a20 2020 2020 2020  id=None,.       
-00018600: 2066 6561 7475 7265 7374 6f72 655f 6e61   featurestore_na
-00018610: 6d65 3d4e 6f6e 652c 0a20 2020 2020 2020  me=None,.       
-00018620: 2063 7265 6174 6564 3d4e 6f6e 652c 0a20   created=None,. 
-00018630: 2020 2020 2020 2063 7265 6174 6f72 3d4e         creator=N
-00018640: 6f6e 652c 0a20 2020 2020 2020 2069 643d  one,.        id=
-00018650: 4e6f 6e65 2c0a 2020 2020 2020 2020 6665  None,.        fe
-00018660: 6174 7572 6573 3d4e 6f6e 652c 0a20 2020  atures=None,.   
-00018670: 2020 2020 206c 6f63 6174 696f 6e3d 4e6f       location=No
-00018680: 6e65 2c0a 2020 2020 2020 2020 7374 6174  ne,.        stat
-00018690: 6973 7469 6373 5f63 6f6e 6669 673d 4e6f  istics_config=No
-000186a0: 6e65 2c0a 2020 2020 2020 2020 6576 656e  ne,.        even
-000186b0: 745f 7469 6d65 3d4e 6f6e 652c 0a20 2020  t_time=None,.   
-000186c0: 2020 2020 2065 7870 6563 7461 7469 6f6e       expectation
-000186d0: 5f73 7569 7465 3d4e 6f6e 652c 0a20 2020  _suite=None,.   
-000186e0: 2020 2020 206f 6e6c 696e 655f 656e 6162       online_enab
-000186f0: 6c65 643d 4661 6c73 652c 0a20 2020 2020  led=False,.     
-00018700: 2020 2068 7265 663d 4e6f 6e65 2c0a 2020     href=None,.  
-00018710: 2020 2020 2020 6f6e 6c69 6e65 5f74 6f70        online_top
-00018720: 6963 5f6e 616d 653d 4e6f 6e65 2c0a 2020  ic_name=None,.  
-00018730: 2020 293a 0a20 2020 2020 2020 2073 7570    ):.        sup
-00018740: 6572 2829 2e5f 5f69 6e69 745f 5f28 0a20  er().__init__(. 
-00018750: 2020 2020 2020 2020 2020 2066 6561 7475             featu
-00018760: 7265 7374 6f72 655f 6964 2c0a 2020 2020  restore_id,.    
-00018770: 2020 2020 2020 2020 6c6f 6361 7469 6f6e          location
-00018780: 2c0a 2020 2020 2020 2020 2020 2020 6576  ,.            ev
-00018790: 656e 745f 7469 6d65 3d65 7665 6e74 5f74  ent_time=event_t
-000187a0: 696d 652c 0a20 2020 2020 2020 2020 2020  ime,.           
-000187b0: 206f 6e6c 696e 655f 656e 6162 6c65 643d   online_enabled=
-000187c0: 6f6e 6c69 6e65 5f65 6e61 626c 6564 2c0a  online_enabled,.
-000187d0: 2020 2020 2020 2020 2020 2020 6964 3d69              id=i
-000187e0: 642c 0a20 2020 2020 2020 2020 2020 2065  d,.            e
-000187f0: 7870 6563 7461 7469 6f6e 5f73 7569 7465  xpectation_suite
-00018800: 3d65 7870 6563 7461 7469 6f6e 5f73 7569  =expectation_sui
-00018810: 7465 2c0a 2020 2020 2020 2020 2020 2020  te,.            
-00018820: 6f6e 6c69 6e65 5f74 6f70 6963 5f6e 616d  online_topic_nam
-00018830: 653d 6f6e 6c69 6e65 5f74 6f70 6963 5f6e  e=online_topic_n
-00018840: 616d 652c 0a20 2020 2020 2020 2029 0a0a  ame,.        )..
-00018850: 2020 2020 2020 2020 7365 6c66 2e5f 6665          self._fe
-00018860: 6174 7572 655f 7374 6f72 655f 6e61 6d65  ature_store_name
-00018870: 203d 2066 6561 7475 7265 7374 6f72 655f   = featurestore_
-00018880: 6e61 6d65 0a20 2020 2020 2020 2073 656c  name.        sel
-00018890: 662e 5f64 6573 6372 6970 7469 6f6e 203d  f._description =
-000188a0: 2064 6573 6372 6970 7469 6f6e 0a20 2020   description.   
-000188b0: 2020 2020 2073 656c 662e 5f63 7265 6174       self._creat
-000188c0: 6564 203d 2063 7265 6174 6564 0a20 2020  ed = created.   
-000188d0: 2020 2020 2073 656c 662e 5f63 7265 6174       self._creat
-000188e0: 6f72 203d 2075 7365 722e 5573 6572 2e66  or = user.User.f
-000188f0: 726f 6d5f 7265 7370 6f6e 7365 5f6a 736f  rom_response_jso
-00018900: 6e28 6372 6561 746f 7229 0a20 2020 2020  n(creator).     
-00018910: 2020 2073 656c 662e 5f76 6572 7369 6f6e     self._version
-00018920: 203d 2076 6572 7369 6f6e 0a20 2020 2020   = version.     
-00018930: 2020 2073 656c 662e 5f6e 616d 6520 3d20     self._name = 
-00018940: 6e61 6d65 0a20 2020 2020 2020 2073 656c  name.        sel
-00018950: 662e 5f71 7565 7279 203d 2071 7565 7279  f._query = query
-00018960: 0a20 2020 2020 2020 2073 656c 662e 5f64  .        self._d
-00018970: 6174 615f 666f 726d 6174 203d 2064 6174  ata_format = dat
-00018980: 615f 666f 726d 6174 2e75 7070 6572 2829  a_format.upper()
-00018990: 2069 6620 6461 7461 5f66 6f72 6d61 7420   if data_format 
-000189a0: 656c 7365 204e 6f6e 650a 2020 2020 2020  else None.      
-000189b0: 2020 7365 6c66 2e5f 7061 7468 203d 2070    self._path = p
-000189c0: 6174 680a 0a20 2020 2020 2020 2073 656c  ath..        sel
-000189d0: 662e 5f66 6561 7475 7265 7320 3d20 5b0a  f._features = [.
-000189e0: 2020 2020 2020 2020 2020 2020 6665 6174              feat
-000189f0: 7572 652e 4665 6174 7572 652e 6672 6f6d  ure.Feature.from
-00018a00: 5f72 6573 706f 6e73 655f 6a73 6f6e 2866  _response_json(f
-00018a10: 6561 7429 2069 6620 6973 696e 7374 616e  eat) if isinstan
-00018a20: 6365 2866 6561 742c 2064 6963 7429 2065  ce(feat, dict) e
-00018a30: 6c73 6520 6665 6174 0a20 2020 2020 2020  lse feat.       
-00018a40: 2020 2020 2066 6f72 2066 6561 7420 696e       for feat in
-00018a50: 2028 6665 6174 7572 6573 206f 7220 5b5d   (features or []
-00018a60: 290a 2020 2020 2020 2020 5d0a 0a20 2020  ).        ]..   
-00018a70: 2020 2020 2073 656c 662e 5f66 6561 7475       self._featu
-00018a80: 7265 5f67 726f 7570 5f65 6e67 696e 6520  re_group_engine 
-00018a90: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00018aa0: 6578 7465 726e 616c 5f66 6561 7475 7265  external_feature
-00018ab0: 5f67 726f 7570 5f65 6e67 696e 652e 4578  _group_engine.Ex
-00018ac0: 7465 726e 616c 4665 6174 7572 6547 726f  ternalFeatureGro
-00018ad0: 7570 456e 6769 6e65 2866 6561 7475 7265  upEngine(feature
-00018ae0: 7374 6f72 655f 6964 290a 2020 2020 2020  store_id).      
-00018af0: 2020 290a 0a20 2020 2020 2020 2069 6620    )..        if 
-00018b00: 7365 6c66 2e5f 6964 3a0a 2020 2020 2020  self._id:.      
-00018b10: 2020 2020 2020 2320 476f 7420 6672 6f6d        # Got from
-00018b20: 2048 6f70 7377 6f72 6b73 2c20 6465 7365   Hopsworks, dese
-00018b30: 7269 616c 697a 6520 6665 6174 7572 6573  rialize features
-00018b40: 2061 6e64 2073 746f 7261 6765 2063 6f6e   and storage con
-00018b50: 6e65 6374 6f72 0a20 2020 2020 2020 2020  nector.         
-00018b60: 2020 2073 656c 662e 5f66 6561 7475 7265     self._feature
-00018b70: 7320 3d20 280a 2020 2020 2020 2020 2020  s = (.          
-00018b80: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
-00018b90: 2020 2020 2020 2020 2020 2020 6665 6174              feat
-00018ba0: 7572 652e 4665 6174 7572 652e 6672 6f6d  ure.Feature.from
-00018bb0: 5f72 6573 706f 6e73 655f 6a73 6f6e 2866  _response_json(f
-00018bc0: 6561 7429 0a20 2020 2020 2020 2020 2020  eat).           
-00018bd0: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
-00018be0: 7374 616e 6365 2866 6561 742c 2064 6963  stance(feat, dic
-00018bf0: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
-00018c00: 2020 2020 2020 2065 6c73 6520 6665 6174         else feat
-00018c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018c20: 2020 2020 2066 6f72 2066 6561 7420 696e       for feat in
-00018c30: 2066 6561 7475 7265 730a 2020 2020 2020   features.      
-00018c40: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
-00018c50: 2020 2020 2020 2020 2020 2020 6966 2066              if f
-00018c60: 6561 7475 7265 730a 2020 2020 2020 2020  eatures.        
-00018c70: 2020 2020 2020 2020 656c 7365 204e 6f6e          else Non
-00018c80: 650a 2020 2020 2020 2020 2020 2020 290a  e.            ).
-00018c90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018ca0: 2e70 7269 6d61 7279 5f6b 6579 203d 2028  .primary_key = (
-00018cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018cc0: 205b 6665 6174 2e6e 616d 6520 666f 7220   [feat.name for 
-00018cd0: 6665 6174 2069 6e20 7365 6c66 2e5f 6665  feat in self._fe
-00018ce0: 6174 7572 6573 2069 6620 6665 6174 2e70  atures if feat.p
-00018cf0: 7269 6d61 7279 2069 7320 5472 7565 5d0a  rimary is True].
-00018d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d10: 6966 2073 656c 662e 5f66 6561 7475 7265  if self._feature
-00018d20: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00018d30: 2020 656c 7365 205b 5d0a 2020 2020 2020    else [].      
-00018d40: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00018d50: 2020 2020 7365 6c66 2e73 7461 7469 7374      self.statist
-00018d60: 6963 735f 636f 6e66 6967 203d 2073 7461  ics_config = sta
-00018d70: 7469 7374 6963 735f 636f 6e66 6967 0a0a  tistics_config..
-00018d80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018d90: 2e5f 6f70 7469 6f6e 7320 3d20 280a 2020  ._options = (.  
-00018da0: 2020 2020 2020 2020 2020 2020 2020 7b6f                {o
-00018db0: 7074 696f 6e5b 226e 616d 6522 5d3a 206f  ption["name"]: o
-00018dc0: 7074 696f 6e5b 2276 616c 7565 225d 2066  ption["value"] f
-00018dd0: 6f72 206f 7074 696f 6e20 696e 206f 7074  or option in opt
-00018de0: 696f 6e73 7d0a 2020 2020 2020 2020 2020  ions}.          
-00018df0: 2020 2020 2020 6966 206f 7074 696f 6e73        if options
-00018e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018e10: 2065 6c73 6520 4e6f 6e65 0a20 2020 2020   else None.     
-00018e20: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00018e30: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00018e40: 2020 2073 656c 662e 7072 696d 6172 795f     self.primary_
-00018e50: 6b65 7920 3d20 7072 696d 6172 795f 6b65  key = primary_ke
-00018e60: 790a 2020 2020 2020 2020 2020 2020 7365  y.            se
-00018e70: 6c66 2e73 7461 7469 7374 6963 735f 636f  lf.statistics_co
-00018e80: 6e66 6967 203d 2073 7461 7469 7374 6963  nfig = statistic
-00018e90: 735f 636f 6e66 6967 0a20 2020 2020 2020  s_config.       
-00018ea0: 2020 2020 2073 656c 662e 5f66 6561 7475       self._featu
-00018eb0: 7265 7320 3d20 6665 6174 7572 6573 0a20  res = features. 
-00018ec0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018ed0: 5f6f 7074 696f 6e73 203d 206f 7074 696f  _options = optio
-00018ee0: 6e73 0a0a 2020 2020 2020 2020 6966 2073  ns..        if s
-00018ef0: 746f 7261 6765 5f63 6f6e 6e65 6374 6f72  torage_connector
-00018f00: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-00018f10: 2069 7369 6e73 7461 6e63 6528 7374 6f72   isinstance(stor
-00018f20: 6167 655f 636f 6e6e 6563 746f 722c 2064  age_connector, d
-00018f30: 6963 7429 3a0a 2020 2020 2020 2020 2020  ict):.          
-00018f40: 2020 7365 6c66 2e5f 7374 6f72 6167 655f    self._storage_
-00018f50: 636f 6e6e 6563 746f 7220 3d20 7363 2e53  connector = sc.S
-00018f60: 746f 7261 6765 436f 6e6e 6563 746f 722e  torageConnector.
-00018f70: 6672 6f6d 5f72 6573 706f 6e73 655f 6a73  from_response_js
-00018f80: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-00018f90: 2020 2020 7374 6f72 6167 655f 636f 6e6e      storage_conn
-00018fa0: 6563 746f 720a 2020 2020 2020 2020 2020  ector.          
-00018fb0: 2020 290a 2020 2020 2020 2020 656c 7365    ).        else
-00018fc0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00018fd0: 6c66 2e5f 7374 6f72 6167 655f 636f 6e6e  lf._storage_conn
-00018fe0: 6563 746f 7220 3d20 7374 6f72 6167 655f  ector = storage_
-00018ff0: 636f 6e6e 6563 746f 720a 0a20 2020 2020  connector..     
-00019000: 2020 2073 656c 662e 5f68 7265 6620 3d20     self._href = 
-00019010: 6872 6566 0a0a 2020 2020 6465 6620 7361  href..    def sa
-00019020: 7665 2873 656c 6629 3a0a 2020 2020 2020  ve(self):.      
-00019030: 2020 2222 2250 6572 7369 7374 2074 6865    """Persist the
-00019040: 206d 6574 6164 6174 6120 666f 7220 7468   metadata for th
-00019050: 6973 2065 7874 6572 6e61 6c20 6665 6174  is external feat
-00019060: 7572 6520 6772 6f75 702e 0a0a 2020 2020  ure group...    
-00019070: 2020 2020 5769 7468 6f75 7420 6361 6c6c      Without call
-00019080: 696e 6720 7468 6973 206d 6574 686f 642c  ing this method,
-00019090: 2079 6f75 7220 6665 6174 7572 6520 6772   your feature gr
-000190a0: 6f75 7020 7769 6c6c 206f 6e6c 7920 6578  oup will only ex
-000190b0: 6973 740a 2020 2020 2020 2020 696e 2079  ist.        in y
-000190c0: 6f75 7220 5079 7468 6f6e 204b 6572 6e65  our Python Kerne
-000190d0: 6c2c 2062 7574 206e 6f74 2069 6e20 486f  l, but not in Ho
-000190e0: 7073 776f 726b 732e 0a0a 2020 2020 2020  psworks...      
-000190f0: 2020 6060 6070 7974 686f 6e0a 2020 2020    ```python.    
-00019100: 2020 2020 7175 6572 7920 3d20 2253 454c      query = "SEL
-00019110: 4543 5420 2a20 4652 4f4d 2073 616c 6573  ECT * FROM sales
-00019120: 220a 0a20 2020 2020 2020 2066 6720 3d20  "..        fg = 
-00019130: 6665 6174 7572 655f 7374 6f72 652e 6372  feature_store.cr
-00019140: 6561 7465 5f65 7874 6572 6e61 6c5f 6665  eate_external_fe
-00019150: 6174 7572 655f 6772 6f75 7028 6e61 6d65  ature_group(name
-00019160: 3d22 7361 6c65 7322 2c0a 2020 2020 2020  ="sales",.      
-00019170: 2020 2020 2020 7665 7273 696f 6e3d 312c        version=1,
-00019180: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-00019190: 6372 6970 7469 6f6e 3d22 5068 7973 6963  cription="Physic
-000191a0: 616c 2073 686f 7020 7361 6c65 7320 6665  al shop sales fe
-000191b0: 6174 7572 6573 222c 0a20 2020 2020 2020  atures",.       
-000191c0: 2020 2020 2071 7565 7279 3d71 7565 7279       query=query
-000191d0: 2c0a 2020 2020 2020 2020 2020 2020 7374  ,.            st
-000191e0: 6f72 6167 655f 636f 6e6e 6563 746f 723d  orage_connector=
-000191f0: 636f 6e6e 6563 746f 722c 0a20 2020 2020  connector,.     
-00019200: 2020 2020 2020 2070 7269 6d61 7279 5f6b         primary_k
-00019210: 6579 3d5b 2773 735f 7374 6f72 655f 736b  ey=['ss_store_sk
-00019220: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
-00019230: 6576 656e 745f 7469 6d65 3d27 7361 6c65  event_time='sale
-00019240: 5f64 6174 6527 0a20 2020 2020 2020 2029  _date'.        )
-00019250: 0a0a 2020 2020 2020 2020 6667 2e73 6176  ..        fg.sav
-00019260: 6528 290a 2020 2020 2020 2020 2222 220a  e().        """.
-00019270: 2020 2020 2020 2020 7365 6c66 2e5f 6665          self._fe
-00019280: 6174 7572 655f 6772 6f75 705f 656e 6769  ature_group_engi
-00019290: 6e65 2e73 6176 6528 7365 6c66 290a 2020  ne.save(self).  
-000192a0: 2020 2020 2020 7365 6c66 2e5f 636f 6465        self._code
-000192b0: 5f65 6e67 696e 652e 7361 7665 5f63 6f64  _engine.save_cod
-000192c0: 6528 7365 6c66 290a 0a20 2020 2020 2020  e(self)..       
-000192d0: 2069 6620 7365 6c66 2e73 7461 7469 7374   if self.statist
-000192e0: 6963 735f 636f 6e66 6967 2e65 6e61 626c  ics_config.enabl
-000192f0: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
-00019300: 7365 6c66 2e5f 7374 6174 6973 7469 6373  self._statistics
-00019310: 5f65 6e67 696e 652e 636f 6d70 7574 655f  _engine.compute_
-00019320: 7374 6174 6973 7469 6373 2873 656c 6629  statistics(self)
-00019330: 0a0a 2020 2020 6465 6620 696e 7365 7274  ..    def insert
-00019340: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00019350: 2020 2020 2020 2020 6665 6174 7572 6573          features
-00019360: 3a20 556e 696f 6e5b 0a20 2020 2020 2020  : Union[.       
-00019370: 2020 2020 2070 642e 4461 7461 4672 616d       pd.DataFram
-00019380: 652c 0a20 2020 2020 2020 2020 2020 2054  e,.            T
-00019390: 7970 6556 6172 2822 7079 7370 6172 6b2e  ypeVar("pyspark.
-000193a0: 7371 6c2e 4461 7461 4672 616d 6522 292c  sql.DataFrame"),
-000193b0: 2020 2320 6e6f 7161 3a20 4638 3231 0a20    # noqa: F821. 
-000193c0: 2020 2020 2020 2020 2020 2054 7970 6556             TypeV
-000193d0: 6172 2822 7079 7370 6172 6b2e 5244 4422  ar("pyspark.RDD"
-000193e0: 292c 2020 2320 6e6f 7161 3a20 4638 3231  ),  # noqa: F821
-000193f0: 0a20 2020 2020 2020 2020 2020 206e 702e  .            np.
-00019400: 6e64 6172 7261 792c 0a20 2020 2020 2020  ndarray,.       
-00019410: 2020 2020 204c 6973 745b 6c69 7374 5d2c       List[list],
-00019420: 0a20 2020 2020 2020 205d 2c0a 2020 2020  .        ],.    
-00019430: 2020 2020 7772 6974 655f 6f70 7469 6f6e      write_option
-00019440: 733a 204f 7074 696f 6e61 6c5b 4469 6374  s: Optional[Dict
-00019450: 5b73 7472 2c20 416e 795d 5d20 3d20 7b7d  [str, Any]] = {}
-00019460: 2c0a 2020 2020 2020 2020 7661 6c69 6461  ,.        valida
-00019470: 7469 6f6e 5f6f 7074 696f 6e73 3a20 4f70  tion_options: Op
-00019480: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
-00019490: 2041 6e79 5d5d 203d 207b 7d2c 0a20 2020   Any]] = {},.   
-000194a0: 2020 2020 2073 6176 655f 636f 6465 3a20       save_code: 
-000194b0: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
-000194c0: 2054 7275 652c 0a20 2020 2029 202d 3e20   True,.    ) -> 
-000194d0: 5475 706c 655b 4f70 7469 6f6e 616c 5b4a  Tuple[Optional[J
-000194e0: 6f62 5d2c 204f 7074 696f 6e61 6c5b 5661  ob], Optional[Va
-000194f0: 6c69 6461 7469 6f6e 5265 706f 7274 5d5d  lidationReport]]
-00019500: 3a0a 2020 2020 2020 2020 6665 6174 7572  :.        featur
-00019510: 655f 6461 7461 6672 616d 6520 3d20 656e  e_dataframe = en
-00019520: 6769 6e65 2e67 6574 5f69 6e73 7461 6e63  gine.get_instanc
-00019530: 6528 292e 636f 6e76 6572 745f 746f 5f64  e().convert_to_d
-00019540: 6566 6175 6c74 5f64 6174 6166 7261 6d65  efault_dataframe
-00019550: 2866 6561 7475 7265 7329 0a0a 2020 2020  (features)..    
-00019560: 2020 2020 6a6f 622c 2067 655f 7265 706f      job, ge_repo
-00019570: 7274 203d 2073 656c 662e 5f66 6561 7475  rt = self._featu
-00019580: 7265 5f67 726f 7570 5f65 6e67 696e 652e  re_group_engine.
-00019590: 696e 7365 7274 280a 2020 2020 2020 2020  insert(.        
-000195a0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-000195b0: 2020 2020 2020 6665 6174 7572 655f 6461        feature_da
-000195c0: 7461 6672 616d 653d 6665 6174 7572 655f  taframe=feature_
-000195d0: 6461 7461 6672 616d 652c 0a20 2020 2020  dataframe,.     
-000195e0: 2020 2020 2020 2077 7269 7465 5f6f 7074         write_opt
-000195f0: 696f 6e73 3d77 7269 7465 5f6f 7074 696f  ions=write_optio
-00019600: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
-00019610: 7661 6c69 6461 7469 6f6e 5f6f 7074 696f  validation_optio
-00019620: 6e73 3d7b 2273 6176 655f 7265 706f 7274  ns={"save_report
-00019630: 223a 2054 7275 652c 202a 2a76 616c 6964  ": True, **valid
-00019640: 6174 696f 6e5f 6f70 7469 6f6e 737d 2c0a  ation_options},.
-00019650: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00019660: 2020 2069 6620 7361 7665 5f63 6f64 6520     if save_code 
-00019670: 616e 6420 280a 2020 2020 2020 2020 2020  and (.          
-00019680: 2020 6765 5f72 6570 6f72 7420 6973 204e    ge_report is N
-00019690: 6f6e 6520 6f72 2067 655f 7265 706f 7274  one or ge_report
-000196a0: 2e69 6e67 6573 7469 6f6e 5f72 6573 756c  .ingestion_resul
-000196b0: 7420 3d3d 2022 494e 4745 5354 4544 220a  t == "INGESTED".
-000196c0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-000196d0: 2020 2020 2020 2073 656c 662e 5f63 6f64         self._cod
-000196e0: 655f 656e 6769 6e65 2e73 6176 655f 636f  e_engine.save_co
-000196f0: 6465 2873 656c 6629 0a0a 2020 2020 2020  de(self)..      
-00019700: 2020 6966 2073 656c 662e 7374 6174 6973    if self.statis
-00019710: 7469 6373 5f63 6f6e 6669 672e 656e 6162  tics_config.enab
-00019720: 6c65 643a 0a20 2020 2020 2020 2020 2020  led:.           
-00019730: 2077 6172 6e69 6e67 732e 7761 726e 280a   warnings.warn(.
-00019740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019750: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00019760: 2020 2020 2020 2253 7461 7469 7374 6963        "Statistic
-00019770: 7320 6172 6520 6e6f 7420 636f 6d70 7574  s are not comput
-00019780: 6564 2066 6f72 2069 6e73 6572 7469 6f6e  ed for insertion
-00019790: 2074 6f20 6f6e 6c69 6e65 2065 6e61 626c   to online enabl
-000197a0: 6564 2065 7874 6572 6e61 6c20 6665 6174  ed external feat
-000197b0: 7572 6520 6772 6f75 7020 607b 7d60 2c20  ure group `{}`, 
-000197c0: 7769 7468 2076 6572 7369 6f6e 220a 2020  with version".  
-000197d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000197e0: 2020 2220 607b 7d60 2e20 4361 6c6c 2060    " `{}`. Call `
-000197f0: 636f 6d70 7574 655f 7374 6174 6973 7469  compute_statisti
-00019800: 6373 6020 6578 706c 6963 6974 6c79 2074  cs` explicitly t
-00019810: 6f20 636f 6d70 7574 6520 7374 6174 6973  o compute statis
-00019820: 7469 6373 206f 7665 7220 7468 6520 6461  tics over the da
-00019830: 7461 2069 6e20 7468 6520 6578 7465 726e  ta in the extern
-00019840: 616c 2073 746f 7261 6765 2073 7973 7465  al storage syste
-00019850: 6d2e 220a 2020 2020 2020 2020 2020 2020  m.".            
-00019860: 2020 2020 292e 666f 726d 6174 2873 656c      ).format(sel
-00019870: 662e 5f6e 616d 652c 2073 656c 662e 5f76  f._name, self._v
-00019880: 6572 7369 6f6e 292c 0a20 2020 2020 2020  ersion),.       
-00019890: 2020 2020 2020 2020 2075 7469 6c2e 5374           util.St
-000198a0: 6f72 6167 6557 6172 6e69 6e67 2c0a 2020  orageWarning,.  
-000198b0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-000198c0: 2020 2020 2072 6574 7572 6e20 280a 2020       return (.  
-000198d0: 2020 2020 2020 2020 2020 6a6f 622c 0a20            job,. 
-000198e0: 2020 2020 2020 2020 2020 2067 655f 7265             ge_re
-000198f0: 706f 7274 2e74 6f5f 6765 5f74 7970 6528  port.to_ge_type(
-00019900: 2920 6966 2067 655f 7265 706f 7274 2069  ) if ge_report i
-00019910: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
-00019920: 4e6f 6e65 2c0a 2020 2020 2020 2020 290a  None,.        ).
-00019930: 0a20 2020 2064 6566 2072 6561 6428 0a20  .    def read(. 
-00019940: 2020 2020 2020 2073 656c 662c 2064 6174         self, dat
-00019950: 6166 7261 6d65 5f74 7970 653a 204f 7074  aframe_type: Opt
-00019960: 696f 6e61 6c5b 7374 725d 203d 2022 6465  ional[str] = "de
-00019970: 6661 756c 7422 2c20 6f6e 6c69 6e65 3a20  fault", online: 
-00019980: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
-00019990: 2046 616c 7365 0a20 2020 2029 3a0a 2020   False.    ):.  
-000199a0: 2020 2020 2020 2222 2247 6574 2074 6865        """Get the
-000199b0: 2066 6561 7475 7265 2067 726f 7570 2061   feature group a
-000199c0: 7320 6120 4461 7461 4672 616d 652e 0a0a  s a DataFrame...
-000199d0: 2020 2020 2020 2020 2121 2120 6578 616d          !!! exam
-000199e0: 706c 650a 2020 2020 2020 2020 2020 2020  ple.            
-000199f0: 6060 6070 7974 686f 6e0a 2020 2020 2020  ```python.      
-00019a00: 2020 2020 2020 2320 636f 6e6e 6563 7420        # connect 
-00019a10: 746f 2074 6865 2046 6561 7475 7265 2053  to the Feature S
-00019a20: 746f 7265 0a20 2020 2020 2020 2020 2020  tore.           
-00019a30: 2066 7320 3d20 2e2e 2e0a 0a20 2020 2020   fs = .....     
-00019a40: 2020 2020 2020 2023 2067 6574 2074 6865         # get the
-00019a50: 2046 6561 7475 7265 2047 726f 7570 2069   Feature Group i
-00019a60: 6e73 7461 6e63 650a 2020 2020 2020 2020  nstance.        
-00019a70: 2020 2020 6667 203d 2066 732e 6765 745f      fg = fs.get_
-00019a80: 6f72 5f63 7265 6174 655f 6665 6174 7572  or_create_featur
-00019a90: 655f 6772 6f75 7028 2e2e 2e29 0a0a 2020  e_group(...)..  
-00019aa0: 2020 2020 2020 2020 2020 6466 203d 2066            df = f
-00019ab0: 672e 7265 6164 2829 0a20 2020 2020 2020  g.read().       
-00019ac0: 2020 2020 2060 6060 0a0a 2020 2020 2020       ```..      
-00019ad0: 2020 2121 2120 7761 726e 696e 6720 2245    !!! warning "E
-00019ae0: 6e67 696e 6520 5375 7070 6f72 7422 0a20  ngine Support". 
-00019af0: 2020 2020 2020 2020 2020 202a 2a53 7061             **Spa
-00019b00: 726b 206f 6e6c 792a 2a0a 0a20 2020 2020  rk only**..     
-00019b10: 2020 2020 2020 2052 6561 6469 6e67 2061         Reading a
-00019b20: 6e20 4578 7465 726e 616c 2046 6561 7475  n External Featu
-00019b30: 7265 2047 726f 7570 2064 6972 6563 746c  re Group directl
-00019b40: 7920 696e 746f 2061 2050 616e 6461 7320  y into a Pandas 
-00019b50: 4461 7461 6672 616d 6520 7573 696e 670a  Dataframe using.
-00019b60: 2020 2020 2020 2020 2020 2020 5079 7468              Pyth
-00019b70: 6f6e 2f50 616e 6461 7320 6173 2045 6e67  on/Pandas as Eng
-00019b80: 696e 6520 6973 206e 6f74 2073 7570 706f  ine is not suppo
-00019b90: 7274 6564 2c20 686f 7765 7665 722c 2079  rted, however, y
-00019ba0: 6f75 2063 616e 2075 7365 2074 6865 0a20  ou can use the. 
-00019bb0: 2020 2020 2020 2020 2020 2051 7565 7279             Query
-00019bc0: 2041 5049 2074 6f20 6372 6561 7465 2046   API to create F
-00019bd0: 6561 7475 7265 2056 6965 7773 2f54 7261  eature Views/Tra
-00019be0: 696e 696e 6720 4461 7461 2063 6f6e 7461  ining Data conta
-00019bf0: 696e 696e 6720 4578 7465 726e 616c 0a20  ining External. 
-00019c00: 2020 2020 2020 2020 2020 2046 6561 7475             Featu
-00019c10: 7265 2047 726f 7570 732e 0a0a 2020 2020  re Groups...    
-00019c20: 2020 2020 2320 4172 6775 6d65 6e74 730a      # Arguments.
-00019c30: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00019c40: 6672 616d 655f 7479 7065 3a20 7374 722c  frame_type: str,
-00019c50: 206f 7074 696f 6e61 6c2e 2050 6f73 7369   optional. Possi
-00019c60: 626c 6520 7661 6c75 6573 2061 7265 2060  ble values are `
-00019c70: 2264 6566 6175 6c74 2260 2c20 6022 7370  "default"`, `"sp
-00019c80: 6172 6b22 602c 0a20 2020 2020 2020 2020  ark"`,.         
-00019c90: 2020 2020 2020 2060 2270 616e 6461 7322         `"pandas"
-00019ca0: 602c 2060 226e 756d 7079 2260 206f 7220  `, `"numpy"` or 
-00019cb0: 6022 7079 7468 6f6e 2260 2c20 6465 6661  `"python"`, defa
-00019cc0: 756c 7473 2074 6f20 6022 6465 6661 756c  ults to `"defaul
-00019cd0: 7422 602e 0a20 2020 2020 2020 2020 2020  t"`..           
-00019ce0: 206f 6e6c 696e 653a 2062 6f6f 6c2c 206f   online: bool, o
-00019cf0: 7074 696f 6e61 6c2e 2049 6620 6054 7275  ptional. If `Tru
-00019d00: 6560 2072 6561 6420 6672 6f6d 206f 6e6c  e` read from onl
-00019d10: 696e 6520 6665 6174 7572 6520 7374 6f72  ine feature stor
-00019d20: 652c 2064 6566 6175 6c74 730a 2020 2020  e, defaults.    
-00019d30: 2020 2020 2020 2020 2020 2020 746f 2060              to `
-00019d40: 4661 6c73 6560 2e0a 0a20 2020 2020 2020  False`...       
-00019d50: 2023 2052 6574 7572 6e73 0a20 2020 2020   # Returns.     
-00019d60: 2020 2020 2020 2060 4461 7461 4672 616d         `DataFram
-00019d70: 6560 3a20 5468 6520 7370 6172 6b20 6461  e`: The spark da
-00019d80: 7461 6672 616d 6520 636f 6e74 6169 6e69  taframe containi
-00019d90: 6e67 2074 6865 2066 6561 7475 7265 2064  ng the feature d
-00019da0: 6174 612e 0a20 2020 2020 2020 2020 2020  ata..           
-00019db0: 2060 7079 7370 6172 6b2e 4461 7461 4672   `pyspark.DataFr
-00019dc0: 616d 6560 2e20 4120 5370 6172 6b20 4461  ame`. A Spark Da
-00019dd0: 7461 4672 616d 652e 0a20 2020 2020 2020  taFrame..       
-00019de0: 2020 2020 2060 7061 6e64 6173 2e44 6174       `pandas.Dat
-00019df0: 6146 7261 6d65 602e 2041 2050 616e 6461  aFrame`. A Panda
-00019e00: 7320 4461 7461 4672 616d 652e 0a20 2020  s DataFrame..   
-00019e10: 2020 2020 2020 2020 2060 6e75 6d70 792e           `numpy.
-00019e20: 6e64 6172 7261 7960 2e20 4120 7477 6f2d  ndarray`. A two-
-00019e30: 6469 6d65 6e73 696f 6e61 6c20 4e75 6d70  dimensional Nump
-00019e40: 7920 6172 7261 792e 0a20 2020 2020 2020  y array..       
-00019e50: 2020 2020 2060 6c69 7374 602e 2041 2074       `list`. A t
-00019e60: 776f 2d64 696d 656e 7369 6f6e 616c 2050  wo-dimensional P
-00019e70: 7974 686f 6e20 6c69 7374 2e0a 0a20 2020  ython list...   
-00019e80: 2020 2020 2023 2052 6169 7365 730a 2020       # Raises.  
-00019e90: 2020 2020 2020 2020 2020 6068 7366 732e            `hsfs.
-00019ea0: 636c 6965 6e74 2e65 7863 6570 7469 6f6e  client.exception
-00019eb0: 732e 5265 7374 4150 4945 7272 6f72 602e  s.RestAPIError`.
-00019ec0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00019ed0: 2020 2020 2069 6620 656e 6769 6e65 2e67       if engine.g
-00019ee0: 6574 5f74 7970 6528 2920 3d3d 2022 7079  et_type() == "py
-00019ef0: 7468 6f6e 2220 616e 6420 6e6f 7420 6f6e  thon" and not on
-00019f00: 6c69 6e65 3a0a 2020 2020 2020 2020 2020  line:.          
-00019f10: 2020 7261 6973 6520 4665 6174 7572 6553    raise FeatureS
-00019f20: 746f 7265 4578 6365 7074 696f 6e28 0a20  toreException(. 
-00019f30: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00019f40: 5265 6164 696e 6720 616e 2045 7874 6572  Reading an Exter
-00019f50: 6e61 6c20 4665 6174 7572 6520 4772 6f75  nal Feature Grou
-00019f60: 7020 6469 7265 6374 6c79 2069 6e74 6f20  p directly into 
-00019f70: 6120 5061 6e64 6173 2044 6174 6166 7261  a Pandas Datafra
-00019f80: 6d65 2075 7369 6e67 2022 0a20 2020 2020  me using ".     
-00019f90: 2020 2020 2020 2020 2020 202b 2022 5079             + "Py
-00019fa0: 7468 6f6e 2f50 616e 6461 7320 6173 2045  thon/Pandas as E
-00019fb0: 6e67 696e 6520 6672 6f6d 2074 6865 2065  ngine from the e
-00019fc0: 7874 6572 6e61 6c20 7374 6f72 6167 6520  xternal storage 
-00019fd0: 7379 7374 656d 2022 0a20 2020 2020 2020  system ".       
-00019fe0: 2020 2020 2020 2020 202b 2022 6973 206e           + "is n
-00019ff0: 6f74 2073 7570 706f 7274 6564 2c20 686f  ot supported, ho
-0001a000: 7765 7665 722c 2069 6620 7468 6520 6665  wever, if the fe
-0001a010: 6174 7572 6520 6772 6f75 7020 6973 206f  ature group is o
-0001a020: 6e6c 696e 6520 656e 6162 6c65 642c 2079  nline enabled, y
-0001a030: 6f75 2063 616e 2072 6561 6420 220a 2020  ou can read ".  
-0001a040: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-0001a050: 2266 726f 6d20 6f6e 6c69 6e65 2073 746f  "from online sto
-0001a060: 7261 6765 206f 7220 796f 7520 6361 6e20  rage or you can 
-0001a070: 7573 6520 7468 6520 220a 2020 2020 2020  use the ".      
-0001a080: 2020 2020 2020 2020 2020 2b20 2251 7565            + "Que
-0001a090: 7279 2041 5049 2074 6f20 6372 6561 7465  ry API to create
-0001a0a0: 2046 6561 7475 7265 2056 6965 7773 2f54   Feature Views/T
-0001a0b0: 7261 696e 696e 6720 4461 7461 2063 6f6e  raining Data con
-0001a0c0: 7461 696e 696e 6720 4578 7465 726e 616c  taining External
-0001a0d0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-0001a0e0: 2020 202b 2022 4665 6174 7572 6520 4772     + "Feature Gr
-0001a0f0: 6f75 7073 2e22 0a20 2020 2020 2020 2020  oups.".         
-0001a100: 2020 2029 0a20 2020 2020 2020 2065 6e67     ).        eng
-0001a110: 696e 652e 6765 745f 696e 7374 616e 6365  ine.get_instance
-0001a120: 2829 2e73 6574 5f6a 6f62 5f67 726f 7570  ().set_job_group
-0001a130: 280a 2020 2020 2020 2020 2020 2020 2246  (.            "F
-0001a140: 6574 6368 696e 6720 4665 6174 7572 6520  etching Feature 
-0001a150: 6772 6f75 7022 2c0a 2020 2020 2020 2020  group",.        
-0001a160: 2020 2020 2247 6574 7469 6e67 2066 6561      "Getting fea
-0001a170: 7475 7265 2067 726f 7570 3a20 7b7d 2066  ture group: {} f
-0001a180: 726f 6d20 7468 6520 6665 6174 7572 6573  rom the features
-0001a190: 746f 7265 207b 7d22 2e66 6f72 6d61 7428  tore {}".format(
-0001a1a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a1b0: 2073 656c 662e 5f6e 616d 652c 2073 656c   self._name, sel
-0001a1c0: 662e 5f66 6561 7475 7265 5f73 746f 7265  f._feature_store
-0001a1d0: 5f6e 616d 650a 2020 2020 2020 2020 2020  _name.          
-0001a1e0: 2020 292c 0a20 2020 2020 2020 2029 0a20    ),.        ). 
-0001a1f0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0001a200: 6c66 2e73 656c 6563 745f 616c 6c28 292e  lf.select_all().
-0001a210: 7265 6164 2864 6174 6166 7261 6d65 5f74  read(dataframe_t
-0001a220: 7970 653d 6461 7461 6672 616d 655f 7479  ype=dataframe_ty
-0001a230: 7065 2c20 6f6e 6c69 6e65 3d6f 6e6c 696e  pe, online=onlin
-0001a240: 6529 0a0a 2020 2020 6465 6620 7368 6f77  e)..    def show
-0001a250: 2873 656c 662c 206e 293a 0a20 2020 2020  (self, n):.     
-0001a260: 2020 2022 2222 5368 6f77 2074 6865 2066     """Show the f
-0001a270: 6972 7374 206e 2072 6f77 7320 6f66 2074  irst n rows of t
-0001a280: 6865 2066 6561 7475 7265 2067 726f 7570  he feature group
-0001a290: 2e0a 0a20 2020 2020 2020 2021 2121 2065  ...        !!! e
-0001a2a0: 7861 6d70 6c65 0a20 2020 2020 2020 2020  xample.         
-0001a2b0: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
-0001a2c0: 2020 2020 2020 2020 2023 2063 6f6e 6e65           # conne
-0001a2d0: 6374 2074 6f20 7468 6520 4665 6174 7572  ct to the Featur
-0001a2e0: 6520 5374 6f72 650a 2020 2020 2020 2020  e Store.        
-0001a2f0: 2020 2020 6673 203d 202e 2e2e 0a0a 2020      fs = .....  
-0001a300: 2020 2020 2020 2020 2020 2320 6765 7420            # get 
-0001a310: 7468 6520 4665 6174 7572 6520 4772 6f75  the Feature Grou
-0001a320: 7020 696e 7374 616e 6365 0a20 2020 2020  p instance.     
-0001a330: 2020 2020 2020 2066 6720 3d20 6673 2e67         fg = fs.g
-0001a340: 6574 5f6f 725f 6372 6561 7465 5f66 6561  et_or_create_fea
-0001a350: 7475 7265 5f67 726f 7570 282e 2e2e 290a  ture_group(...).
-0001a360: 0a20 2020 2020 2020 2020 2020 2066 672e  .            fg.
-0001a370: 7368 6f77 2835 290a 2020 2020 2020 2020  show(5).        
-0001a380: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
-0001a390: 2222 220a 2020 2020 2020 2020 656e 6769  """.        engi
-0001a3a0: 6e65 2e67 6574 5f69 6e73 7461 6e63 6528  ne.get_instance(
-0001a3b0: 292e 7365 745f 6a6f 625f 6772 6f75 7028  ).set_job_group(
-0001a3c0: 0a20 2020 2020 2020 2020 2020 2022 4665  .            "Fe
-0001a3d0: 7463 6869 6e67 2046 6561 7475 7265 2067  tching Feature g
-0001a3e0: 726f 7570 222c 0a20 2020 2020 2020 2020  roup",.         
-0001a3f0: 2020 2022 4765 7474 696e 6720 6665 6174     "Getting feat
-0001a400: 7572 6520 6772 6f75 703a 207b 7d20 6672  ure group: {} fr
-0001a410: 6f6d 2074 6865 2066 6561 7475 7265 7374  om the featurest
-0001a420: 6f72 6520 7b7d 222e 666f 726d 6174 280a  ore {}".format(.
-0001a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a440: 7365 6c66 2e5f 6e61 6d65 2c20 7365 6c66  self._name, self
-0001a450: 2e5f 6665 6174 7572 655f 7374 6f72 655f  ._feature_store_
-0001a460: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
-0001a470: 2029 2c0a 2020 2020 2020 2020 290a 2020   ),.        ).  
-0001a480: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0001a490: 662e 7365 6c65 6374 5f61 6c6c 2829 2e73  f.select_all().s
-0001a4a0: 686f 7728 6e29 0a0a 2020 2020 4063 6c61  how(n)..    @cla
-0001a4b0: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
-0001a4c0: 2066 726f 6d5f 7265 7370 6f6e 7365 5f6a   from_response_j
-0001a4d0: 736f 6e28 636c 732c 206a 736f 6e5f 6469  son(cls, json_di
-0001a4e0: 6374 293a 0a20 2020 2020 2020 206a 736f  ct):.        jso
-0001a4f0: 6e5f 6465 6361 6d65 6c69 7a65 6420 3d20  n_decamelized = 
-0001a500: 6875 6d70 732e 6465 6361 6d65 6c69 7a65  humps.decamelize
-0001a510: 286a 736f 6e5f 6469 6374 290a 2020 2020  (json_dict).    
-0001a520: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-0001a530: 6528 6a73 6f6e 5f64 6563 616d 656c 697a  e(json_decameliz
-0001a540: 6564 2c20 6469 6374 293a 0a20 2020 2020  ed, dict):.     
-0001a550: 2020 2020 2020 205f 203d 206a 736f 6e5f         _ = json_
-0001a560: 6465 6361 6d65 6c69 7a65 642e 706f 7028  decamelized.pop(
-0001a570: 2274 7970 6522 2c20 4e6f 6e65 290a 2020  "type", None).  
-0001a580: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001a590: 2063 6c73 282a 2a6a 736f 6e5f 6465 6361   cls(**json_deca
-0001a5a0: 6d65 6c69 7a65 6429 0a20 2020 2020 2020  melized).       
-0001a5b0: 2066 6f72 2066 6720 696e 206a 736f 6e5f   for fg in json_
-0001a5c0: 6465 6361 6d65 6c69 7a65 643a 0a20 2020  decamelized:.   
-0001a5d0: 2020 2020 2020 2020 205f 203d 2066 672e           _ = fg.
-0001a5e0: 706f 7028 2274 7970 6522 2c20 4e6f 6e65  pop("type", None
-0001a5f0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0001a600: 205b 636c 7328 2a2a 6667 2920 666f 7220   [cls(**fg) for 
-0001a610: 6667 2069 6e20 6a73 6f6e 5f64 6563 616d  fg in json_decam
-0001a620: 656c 697a 6564 5d0a 0a20 2020 2064 6566  elized]..    def
-0001a630: 2075 7064 6174 655f 6672 6f6d 5f72 6573   update_from_res
-0001a640: 706f 6e73 655f 6a73 6f6e 2873 656c 662c  ponse_json(self,
-0001a650: 206a 736f 6e5f 6469 6374 293a 0a20 2020   json_dict):.   
-0001a660: 2020 2020 206a 736f 6e5f 6465 6361 6d65       json_decame
-0001a670: 6c69 7a65 6420 3d20 6875 6d70 732e 6465  lized = humps.de
-0001a680: 6361 6d65 6c69 7a65 286a 736f 6e5f 6469  camelize(json_di
-0001a690: 6374 290a 2020 2020 2020 2020 6966 2022  ct).        if "
-0001a6a0: 7479 7065 2220 696e 206a 736f 6e5f 6465  type" in json_de
-0001a6b0: 6361 6d65 6c69 7a65 643a 0a20 2020 2020  camelized:.     
-0001a6c0: 2020 2020 2020 205f 203d 206a 736f 6e5f         _ = json_
-0001a6d0: 6465 6361 6d65 6c69 7a65 642e 706f 7028  decamelized.pop(
-0001a6e0: 2274 7970 6522 290a 2020 2020 2020 2020  "type").        
-0001a6f0: 7365 6c66 2e5f 5f69 6e69 745f 5f28 2a2a  self.__init__(**
-0001a700: 6a73 6f6e 5f64 6563 616d 656c 697a 6564  json_decamelized
-0001a710: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0001a720: 2073 656c 660a 0a20 2020 2064 6566 206a   self..    def j
-0001a730: 736f 6e28 7365 6c66 293a 0a20 2020 2020  son(self):.     
-0001a740: 2020 2072 6574 7572 6e20 6a73 6f6e 2e64     return json.d
-0001a750: 756d 7073 2873 656c 662c 2063 6c73 3d75  umps(self, cls=u
-0001a760: 7469 6c2e 4665 6174 7572 6553 746f 7265  til.FeatureStore
-0001a770: 456e 636f 6465 7229 0a0a 2020 2020 6465  Encoder)..    de
-0001a780: 6620 746f 5f64 6963 7428 7365 6c66 293a  f to_dict(self):
-0001a790: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001a7a0: 7b0a 2020 2020 2020 2020 2020 2020 2269  {.            "i
-0001a7b0: 6422 3a20 7365 6c66 2e5f 6964 2c0a 2020  d": self._id,.  
-0001a7c0: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
-0001a7d0: 3a20 7365 6c66 2e5f 6e61 6d65 2c0a 2020  : self._name,.  
-0001a7e0: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-0001a7f0: 6970 7469 6f6e 223a 2073 656c 662e 5f64  iption": self._d
-0001a800: 6573 6372 6970 7469 6f6e 2c0a 2020 2020  escription,.    
-0001a810: 2020 2020 2020 2020 2276 6572 7369 6f6e          "version
-0001a820: 223a 2073 656c 662e 5f76 6572 7369 6f6e  ": self._version
-0001a830: 2c0a 2020 2020 2020 2020 2020 2020 2266  ,.            "f
-0001a840: 6561 7475 7265 7322 3a20 7365 6c66 2e5f  eatures": self._
-0001a850: 6665 6174 7572 6573 2c0a 2020 2020 2020  features,.      
-0001a860: 2020 2020 2020 2266 6561 7475 7265 7374        "featurest
-0001a870: 6f72 6549 6422 3a20 7365 6c66 2e5f 6665  oreId": self._fe
-0001a880: 6174 7572 655f 7374 6f72 655f 6964 2c0a  ature_store_id,.
-0001a890: 2020 2020 2020 2020 2020 2020 2271 7565              "que
-0001a8a0: 7279 223a 2073 656c 662e 5f71 7565 7279  ry": self._query
-0001a8b0: 2c0a 2020 2020 2020 2020 2020 2020 2264  ,.            "d
-0001a8c0: 6174 6146 6f72 6d61 7422 3a20 7365 6c66  ataFormat": self
-0001a8d0: 2e5f 6461 7461 5f66 6f72 6d61 742c 0a20  ._data_format,. 
-0001a8e0: 2020 2020 2020 2020 2020 2022 7061 7468             "path
-0001a8f0: 223a 2073 656c 662e 5f70 6174 682c 0a20  ": self._path,. 
-0001a900: 2020 2020 2020 2020 2020 2022 6f70 7469             "opti
-0001a910: 6f6e 7322 3a20 5b7b 226e 616d 6522 3a20  ons": [{"name": 
-0001a920: 6b2c 2022 7661 6c75 6522 3a20 767d 2066  k, "value": v} f
-0001a930: 6f72 206b 2c20 7620 696e 2073 656c 662e  or k, v in self.
-0001a940: 5f6f 7074 696f 6e73 2e69 7465 6d73 2829  _options.items()
-0001a950: 5d0a 2020 2020 2020 2020 2020 2020 6966  ].            if
-0001a960: 2073 656c 662e 5f6f 7074 696f 6e73 0a20   self._options. 
-0001a970: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
-0001a980: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-0001a990: 2020 2273 746f 7261 6765 436f 6e6e 6563    "storageConnec
-0001a9a0: 746f 7222 3a20 7365 6c66 2e5f 7374 6f72  tor": self._stor
-0001a9b0: 6167 655f 636f 6e6e 6563 746f 722e 746f  age_connector.to
-0001a9c0: 5f64 6963 7428 292c 0a20 2020 2020 2020  _dict(),.       
-0001a9d0: 2020 2020 2022 7479 7065 223a 2022 6f6e       "type": "on
-0001a9e0: 4465 6d61 6e64 4665 6174 7572 6567 726f  DemandFeaturegro
-0001a9f0: 7570 4454 4f22 2c0a 2020 2020 2020 2020  upDTO",.        
-0001aa00: 2020 2020 2273 7461 7469 7374 6963 7343      "statisticsC
-0001aa10: 6f6e 6669 6722 3a20 7365 6c66 2e5f 7374  onfig": self._st
-0001aa20: 6174 6973 7469 6373 5f63 6f6e 6669 672c  atistics_config,
-0001aa30: 0a20 2020 2020 2020 2020 2020 2022 6576  .            "ev
-0001aa40: 656e 7454 696d 6522 3a20 7365 6c66 2e5f  entTime": self._
-0001aa50: 6576 656e 745f 7469 6d65 2c0a 2020 2020  event_time,.    
-0001aa60: 2020 2020 2020 2020 2265 7870 6563 7461          "expecta
-0001aa70: 7469 6f6e 5375 6974 6522 3a20 7365 6c66  tionSuite": self
-0001aa80: 2e5f 6578 7065 6374 6174 696f 6e5f 7375  ._expectation_su
-0001aa90: 6974 652c 0a20 2020 2020 2020 2020 2020  ite,.           
-0001aaa0: 2022 6f6e 6c69 6e65 456e 6162 6c65 6422   "onlineEnabled"
-0001aab0: 3a20 7365 6c66 2e5f 6f6e 6c69 6e65 5f65  : self._online_e
-0001aac0: 6e61 626c 6564 2c0a 2020 2020 2020 2020  nabled,.        
-0001aad0: 7d0a 0a20 2020 2040 7072 6f70 6572 7479  }..    @property
-0001aae0: 0a20 2020 2064 6566 2069 6428 7365 6c66  .    def id(self
-0001aaf0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-0001ab00: 6e20 7365 6c66 2e5f 6964 0a0a 2020 2020  n self._id..    
-0001ab10: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0001ab20: 6620 6e61 6d65 2873 656c 6629 3a0a 2020  f name(self):.  
-0001ab30: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0001ab40: 662e 5f6e 616d 650a 0a20 2020 2040 7072  f._name..    @pr
-0001ab50: 6f70 6572 7479 0a20 2020 2064 6566 2076  operty.    def v
-0001ab60: 6572 7369 6f6e 2873 656c 6629 3a0a 2020  ersion(self):.  
-0001ab70: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0001ab80: 662e 5f76 6572 7369 6f6e 0a0a 2020 2020  f._version..    
-0001ab90: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0001aba0: 6620 6465 7363 7269 7074 696f 6e28 7365  f description(se
-0001abb0: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
-0001abc0: 7572 6e20 7365 6c66 2e5f 6465 7363 7269  urn self._descri
-0001abd0: 7074 696f 6e0a 0a20 2020 2040 7072 6f70  ption..    @prop
-0001abe0: 6572 7479 0a20 2020 2064 6566 2066 6561  erty.    def fea
-0001abf0: 7475 7265 7328 7365 6c66 293a 0a20 2020  tures(self):.   
-0001ac00: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0001ac10: 2e5f 6665 6174 7572 6573 0a0a 2020 2020  ._features..    
-0001ac20: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-0001ac30: 6620 7175 6572 7928 7365 6c66 293a 0a20  f query(self):. 
-0001ac40: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0001ac50: 6c66 2e5f 7175 6572 790a 0a20 2020 2040  lf._query..    @
-0001ac60: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-0001ac70: 2064 6174 615f 666f 726d 6174 2873 656c   data_format(sel
-0001ac80: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-0001ac90: 726e 2073 656c 662e 5f64 6174 615f 666f  rn self._data_fo
-0001aca0: 726d 6174 0a0a 2020 2020 4070 726f 7065  rmat..    @prope
-0001acb0: 7274 790a 2020 2020 6465 6620 7061 7468  rty.    def path
-0001acc0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0001acd0: 7265 7475 726e 2073 656c 662e 5f70 6174  return self._pat
-0001ace0: 680a 0a20 2020 2040 7072 6f70 6572 7479  h..    @property
-0001acf0: 0a20 2020 2064 6566 206f 7074 696f 6e73  .    def options
-0001ad00: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0001ad10: 7265 7475 726e 2073 656c 662e 5f6f 7074  return self._opt
-0001ad20: 696f 6e73 0a0a 2020 2020 4070 726f 7065  ions..    @prope
-0001ad30: 7274 790a 2020 2020 6465 6620 7374 6f72  rty.    def stor
-0001ad40: 6167 655f 636f 6e6e 6563 746f 7228 7365  age_connector(se
-0001ad50: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
-0001ad60: 7572 6e20 7365 6c66 2e5f 7374 6f72 6167  urn self._storag
-0001ad70: 655f 636f 6e6e 6563 746f 720a 0a20 2020  e_connector..   
-0001ad80: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-0001ad90: 6566 2063 7265 6174 6f72 2873 656c 6629  ef creator(self)
-0001ada0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-0001adb0: 2073 656c 662e 5f63 7265 6174 6f72 0a0a   self._creator..
-0001adc0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-0001add0: 2020 6465 6620 6372 6561 7465 6428 7365    def created(se
-0001ade0: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
-0001adf0: 7572 6e20 7365 6c66 2e5f 6372 6561 7465  urn self._create
-0001ae00: 640a 0a20 2020 2040 7665 7273 696f 6e2e  d..    @version.
-0001ae10: 7365 7474 6572 0a20 2020 2064 6566 2076  setter.    def v
-0001ae20: 6572 7369 6f6e 2873 656c 662c 2076 6572  ersion(self, ver
-0001ae30: 7369 6f6e 293a 0a20 2020 2020 2020 2073  sion):.        s
-0001ae40: 656c 662e 5f76 6572 7369 6f6e 203d 2076  elf._version = v
-0001ae50: 6572 7369 6f6e 0a0a 2020 2020 4064 6573  ersion..    @des
-0001ae60: 6372 6970 7469 6f6e 2e73 6574 7465 720a  cription.setter.
-0001ae70: 2020 2020 6465 6620 6465 7363 7269 7074      def descript
-0001ae80: 696f 6e28 7365 6c66 2c20 6e65 775f 6465  ion(self, new_de
-0001ae90: 7363 7269 7074 696f 6e29 3a0a 2020 2020  scription):.    
-0001aea0: 2020 2020 7365 6c66 2e5f 6465 7363 7269      self._descri
-0001aeb0: 7074 696f 6e20 3d20 6e65 775f 6465 7363  ption = new_desc
-0001aec0: 7269 7074 696f 6e0a 0a20 2020 2040 6665  ription..    @fe
-0001aed0: 6174 7572 6573 2e73 6574 7465 720a 2020  atures.setter.  
-0001aee0: 2020 6465 6620 6665 6174 7572 6573 2873    def features(s
-0001aef0: 656c 662c 206e 6577 5f66 6561 7475 7265  elf, new_feature
-0001af00: 7329 3a0a 2020 2020 2020 2020 7365 6c66  s):.        self
-0001af10: 2e5f 6665 6174 7572 6573 203d 206e 6577  ._features = new
-0001af20: 5f66 6561 7475 7265 730a 0a20 2020 2040  _features..    @
-0001af30: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
-0001af40: 2066 6561 7475 7265 5f73 746f 7265 5f6e   feature_store_n
-0001af50: 616d 6528 7365 6c66 293a 0a20 2020 2020  ame(self):.     
-0001af60: 2020 2022 2222 4e61 6d65 206f 6620 7468     """Name of th
-0001af70: 6520 6665 6174 7572 6520 7374 6f72 6520  e feature store 
-0001af80: 696e 2077 6869 6368 2074 6865 2066 6561  in which the fea
-0001af90: 7475 7265 2067 726f 7570 2069 7320 6c6f  ture group is lo
-0001afa0: 6361 7465 642e 2222 220a 2020 2020 2020  cated.""".      
-0001afb0: 2020 7265 7475 726e 2073 656c 662e 5f66    return self._f
-0001afc0: 6561 7475 7265 5f73 746f 7265 5f6e 616d  eature_store_nam
-0001afd0: 650a 0a20 2020 2040 7072 6f70 6572 7479  e..    @property
-0001afe0: 0a20 2020 2064 6566 2066 6561 7475 7265  .    def feature
-0001aff0: 5f73 746f 7265 5f69 6428 7365 6c66 293a  _store_id(self):
-0001b000: 0a20 2020 2020 2020 2022 2222 4964 206f  .        """Id o
-0001b010: 6620 7468 6520 6665 6174 7572 6520 7374  f the feature st
-0001b020: 6f72 6520 696e 2077 6869 6368 2074 6865  ore in which the
-0001b030: 2066 6561 7475 7265 2067 726f 7570 2069   feature group i
-0001b040: 7320 6c6f 6361 7465 642e 2222 220a 2020  s located.""".  
-0001b050: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0001b060: 662e 5f66 6561 7475 7265 5f73 746f 7265  f._feature_store
-0001b070: 5f69 640a                                _id.
+00012240: 7269 7465 722e 696e 7365 7274 2873 6d61  riter.insert(sma
+00012250: 6c6c 5f62 6174 6368 5f64 6629 0a20 2020  ll_batch_df).   
+00012260: 2020 2020 2020 2020 2060 6060 0a20 2020           ```.   
+00012270: 2020 2020 2020 2020 2054 6865 2077 7269           The wri
+00012280: 7465 7220 6261 7463 6865 7320 7468 6520  ter batches the 
+00012290: 736d 616c 6c20 4461 7461 6672 616d 6573  small Dataframes
+000122a0: 2061 6e64 2074 7261 6e73 6d69 7473 2074   and transmits t
+000122b0: 6865 6d20 746f 2048 6f70 7377 6f72 6b73  hem to Hopsworks
+000122c0: 0a20 2020 2020 2020 2020 2020 2065 6666  .            eff
+000122d0: 6963 6965 6e74 6c79 2e0a 2020 2020 2020  iciently..      
+000122e0: 2020 2020 2020 5768 656e 2065 7869 7469        When exiti
+000122f0: 6e67 2074 6865 2063 6f6e 7465 7874 2c20  ng the context, 
+00012300: 7468 6520 6665 6174 7572 6520 6772 6f75  the feature grou
+00012310: 7020 7772 6974 6572 2069 7320 7375 7265  p writer is sure
+00012320: 2074 6f20 6578 6974 0a20 2020 2020 2020   to exit.       
+00012330: 2020 2020 206f 6e6c 7920 6f6e 6365 2061       only once a
+00012340: 6c6c 2074 6865 2072 6f77 7320 6861 7665  ll the rows have
+00012350: 2062 6565 6e20 7472 616e 736d 6974 7465   been transmitte
+00012360: 642e 0a0a 2020 2020 2020 2020 2121 2120  d...        !!! 
+00012370: 6578 616d 706c 6520 224d 756c 7469 2070  example "Multi p
+00012380: 6172 7420 696e 7365 7274 2077 6974 6820  art insert with 
+00012390: 6d61 6e75 616c 2063 6f6e 7465 7874 206d  manual context m
+000123a0: 616e 6167 656d 656e 7422 0a20 2020 2020  anagement".     
+000123b0: 2020 2020 2020 2049 6e73 7465 6164 206f         Instead o
+000123c0: 6620 6c65 7474 696e 6720 5079 7468 6f6e  f letting Python
+000123d0: 2068 616e 646c 6520 7468 6520 656e 7465   handle the ente
+000123e0: 7269 6e67 2061 6e64 2065 7869 7469 6e67  ring and exiting
+000123f0: 206f 6620 7468 650a 2020 2020 2020 2020   of the.        
+00012400: 2020 2020 6d75 6c74 6920 7061 7274 2069      multi part i
+00012410: 6e73 6572 7420 636f 6e74 6578 742c 2079  nsert context, y
+00012420: 6f75 2063 616e 2073 7461 7274 2061 6e64  ou can start and
+00012430: 2066 696e 616c 697a 6520 7468 6520 636f   finalize the co
+00012440: 6e74 6578 740a 2020 2020 2020 2020 2020  ntext.          
+00012450: 2020 6d61 6e75 616c 6c79 2e0a 2020 2020    manually..    
+00012460: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
+00012470: 6e0a 2020 2020 2020 2020 2020 2020 6665  n.            fe
+00012480: 6174 7572 655f 6772 6f75 7020 3d20 6673  ature_group = fs
+00012490: 2e67 6574 5f6f 725f 6372 6561 7465 5f66  .get_or_create_f
+000124a0: 6561 7475 7265 5f67 726f 7570 2822 6667  eature_group("fg
+000124b0: 5f6e 616d 6522 2c20 7665 7273 696f 6e3d  _name", version=
+000124c0: 3129 0a0a 2020 2020 2020 2020 2020 2020  1)..            
+000124d0: 7768 696c 6520 6c6f 6f70 3a0a 2020 2020  while loop:.    
+000124e0: 2020 2020 2020 2020 2020 2020 736d 616c              smal
+000124f0: 6c5f 6261 7463 685f 6466 203d 202e 2e2e  l_batch_df = ...
+00012500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012510: 2066 6561 7475 7265 5f67 726f 7570 2e6d   feature_group.m
+00012520: 756c 7469 5f70 6172 745f 696e 7365 7274  ulti_part_insert
+00012530: 2873 6d61 6c6c 5f62 6174 6368 5f64 6629  (small_batch_df)
+00012540: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00012550: 494d 504f 5254 414e 543a 2066 696e 616c  IMPORTANT: final
+00012560: 697a 6520 7468 6520 6d75 6c74 6920 7061  ize the multi pa
+00012570: 7274 2069 6e73 6572 7420 746f 206d 616b  rt insert to mak
+00012580: 6520 7375 7265 2061 6c6c 2072 6f77 730a  e sure all rows.
+00012590: 2020 2020 2020 2020 2020 2020 2320 6861              # ha
+000125a0: 7665 2062 6565 6e20 7472 616e 736d 6974  ve been transmit
+000125b0: 7465 640a 2020 2020 2020 2020 2020 2020  ted.            
+000125c0: 6665 6174 7572 655f 6772 6f75 702e 6669  feature_group.fi
+000125d0: 6e61 6c69 7a65 5f6d 756c 7469 5f70 6172  nalize_multi_par
+000125e0: 745f 696e 7365 7274 2829 0a20 2020 2020  t_insert().     
+000125f0: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
+00012600: 2020 2020 2020 204e 6f74 6520 7468 6174         Note that
+00012610: 2074 6865 2066 6972 7374 2063 616c 6c20   the first call 
+00012620: 746f 2060 6d75 6c74 695f 7061 7274 5f69  to `multi_part_i
+00012630: 6e73 6572 7460 2069 6e69 7469 6174 6573  nsert` initiates
+00012640: 2074 6865 2063 6f6e 7465 7874 0a20 2020   the context.   
+00012650: 2020 2020 2020 2020 2061 6e64 2062 6520           and be 
+00012660: 7375 7265 2074 6f20 6669 6e61 6c69 7a65  sure to finalize
+00012670: 2069 742e 2054 6865 2060 6669 6e61 6c69   it. The `finali
+00012680: 7a65 5f6d 756c 7469 5f70 6172 745f 696e  ze_multi_part_in
+00012690: 7365 7274 6020 6973 2061 0a20 2020 2020  sert` is a.     
+000126a0: 2020 2020 2020 2062 6c6f 636b 696e 6720         blocking 
+000126b0: 6361 6c6c 2074 6861 7420 7265 7475 726e  call that return
+000126c0: 7320 6f6e 6365 2061 6c6c 2072 6f77 7320  s once all rows 
+000126d0: 6861 7665 2062 6565 6e20 7472 616e 736d  have been transm
+000126e0: 6974 7465 642e 0a0a 2020 2020 2020 2020  itted...        
+000126f0: 2020 2020 4f6e 6365 2079 6f75 2061 7265      Once you are
+00012700: 2064 6f6e 6520 7769 7468 2074 6865 206d   done with the m
+00012710: 756c 7469 2070 6172 7420 696e 7365 7274  ulti part insert
+00012720: 2c20 6974 2069 7320 676f 6f64 2070 7261  , it is good pra
+00012730: 6374 6963 6520 746f 0a20 2020 2020 2020  ctice to.       
+00012740: 2020 2020 2073 7461 7274 2074 6865 2062       start the b
+00012750: 6163 6b66 696c 6c20 6a6f 6220 696e 206f  ackfill job in o
+00012760: 7264 6572 2074 6f20 7772 6974 6520 7468  rder to write th
+00012770: 6520 6461 7461 2074 6f20 7468 6520 6f66  e data to the of
+00012780: 666c 696e 650a 2020 2020 2020 2020 2020  fline.          
+00012790: 2020 7374 6f72 6167 653a 0a20 2020 2020    storage:.     
+000127a0: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
+000127b0: 0a20 2020 2020 2020 2020 2020 2066 6561  .            fea
+000127c0: 7475 7265 5f67 726f 7570 2e62 6163 6b66  ture_group.backf
+000127d0: 696c 6c5f 6a6f 622e 7275 6e28 6177 6169  ill_job.run(awai
+000127e0: 745f 7465 726d 696e 6174 696f 6e3d 5472  t_termination=Tr
+000127f0: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+00012800: 6060 600a 0a20 2020 2020 2020 2023 2041  ```..        # A
+00012810: 7267 756d 656e 7473 0a20 2020 2020 2020  rguments.       
+00012820: 2020 2020 2066 6561 7475 7265 733a 2044       features: D
+00012830: 6174 6146 7261 6d65 2c20 5244 442c 204e  ataFrame, RDD, N
+00012840: 6461 7272 6179 2c20 6c69 7374 2e20 4665  darray, list. Fe
+00012850: 6174 7572 6573 2074 6f20 6265 2073 6176  atures to be sav
+00012860: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+00012870: 6f76 6572 7772 6974 653a 2044 726f 7020  overwrite: Drop 
+00012880: 616c 6c20 6461 7461 2069 6e20 7468 6520  all data in the 
+00012890: 6665 6174 7572 6520 6772 6f75 7020 6265  feature group be
+000128a0: 666f 7265 0a20 2020 2020 2020 2020 2020  fore.           
+000128b0: 2020 2020 2069 6e73 6572 7469 6e67 206e       inserting n
+000128c0: 6577 2064 6174 612e 2054 6869 7320 646f  ew data. This do
+000128d0: 6573 206e 6f74 2061 6666 6563 7420 6d65  es not affect me
+000128e0: 7461 6461 7461 2c20 6465 6661 756c 7473  tadata, defaults
+000128f0: 2074 6f20 4661 6c73 652e 0a20 2020 2020   to False..     
+00012900: 2020 2020 2020 206f 7065 7261 7469 6f6e         operation
+00012910: 3a20 4170 6163 6865 2048 7564 6920 6f70  : Apache Hudi op
+00012920: 6572 6174 696f 6e20 7479 7065 2060 2269  eration type `"i
+00012930: 6e73 6572 7422 6020 6f72 2060 2275 7073  nsert"` or `"ups
+00012940: 6572 7422 602e 0a20 2020 2020 2020 2020  ert"`..         
+00012950: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
+00012960: 746f 2060 2275 7073 6572 7422 602e 0a20  to `"upsert"`.. 
+00012970: 2020 2020 2020 2020 2020 2073 746f 7261             stora
+00012980: 6765 3a20 4f76 6572 7772 6974 6520 6465  ge: Overwrite de
+00012990: 6661 756c 7420 6265 6861 7669 6f75 722c  fault behaviour,
+000129a0: 2077 7269 7465 2074 6f20 6f66 666c 696e   write to offlin
+000129b0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+000129c0: 2020 7374 6f72 6167 6520 6f6e 6c79 2077    storage only w
+000129d0: 6974 6820 6022 6f66 666c 696e 6522 6020  ith `"offline"` 
+000129e0: 6f72 206f 6e6c 696e 6520 6f6e 6c79 2077  or online only w
+000129f0: 6974 6820 6022 6f6e 6c69 6e65 2260 2c20  ith `"online"`, 
+00012a00: 6465 6661 756c 7473 0a20 2020 2020 2020  defaults.       
+00012a10: 2020 2020 2020 2020 2074 6f20 604e 6f6e           to `Non
+00012a20: 6560 2e0a 2020 2020 2020 2020 2020 2020  e`..            
+00012a30: 7772 6974 655f 6f70 7469 6f6e 733a 2041  write_options: A
+00012a40: 6464 6974 696f 6e61 6c20 7772 6974 6520  dditional write 
+00012a50: 6f70 7469 6f6e 7320 6173 206b 6579 2d76  options as key-v
+00012a60: 616c 7565 2070 6169 7273 2c20 6465 6661  alue pairs, defa
+00012a70: 756c 7473 2074 6f20 607b 7d60 2e0a 2020  ults to `{}`..  
+00012a80: 2020 2020 2020 2020 2020 2020 2020 5768                Wh
+00012a90: 656e 2075 7369 6e67 2074 6865 2060 7079  en using the `py
+00012aa0: 7468 6f6e 6020 656e 6769 6e65 2c20 7772  thon` engine, wr
+00012ab0: 6974 655f 6f70 7469 6f6e 7320 6361 6e20  ite_options can 
+00012ac0: 636f 6e74 6169 6e20 7468 650a 2020 2020  contain the.    
+00012ad0: 2020 2020 2020 2020 2020 2020 666f 6c6c              foll
+00012ae0: 6f77 696e 6720 656e 7472 6965 733a 0a20  owing entries:. 
+00012af0: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+00012b00: 206b 6579 2060 7370 6172 6b60 2061 6e64   key `spark` and
+00012b10: 2076 616c 7565 2061 6e20 6f62 6a65 6374   value an object
+00012b20: 206f 6620 7479 7065 0a20 2020 2020 2020   of type.       
+00012b30: 2020 2020 2020 2020 205b 6873 6673 2e63           [hsfs.c
+00012b40: 6f72 652e 6a6f 625f 636f 6e66 6967 7572  ore.job_configur
+00012b50: 6174 696f 6e2e 4a6f 6243 6f6e 6669 6775  ation.JobConfigu
+00012b60: 7261 7469 6f6e 5d28 2e2e 2f6a 6f62 5f63  ration](../job_c
+00012b70: 6f6e 6669 6775 7261 7469 6f6e 290a 2020  onfiguration).  
+00012b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b90: 746f 2063 6f6e 6669 6775 7265 2074 6865  to configure the
+00012ba0: 2048 6f70 7377 6f72 6b73 204a 6f62 2075   Hopsworks Job u
+00012bb0: 7365 6420 746f 2077 7269 7465 2064 6174  sed to write dat
+00012bc0: 6120 696e 746f 2074 6865 0a20 2020 2020  a into the.     
+00012bd0: 2020 2020 2020 2020 2020 2020 2066 6561               fea
+00012be0: 7475 7265 2067 726f 7570 2e0a 2020 2020  ture group..    
+00012bf0: 2020 2020 2020 2020 2020 2020 2a20 6b65              * ke
+00012c00: 7920 6077 6169 745f 666f 725f 6a6f 6260  y `wait_for_job`
+00012c10: 2061 6e64 2076 616c 7565 2060 5472 7565   and value `True
+00012c20: 6020 6f72 2060 4661 6c73 6560 2074 6f20  ` or `False` to 
+00012c30: 636f 6e66 6967 7572 650a 2020 2020 2020  configure.      
+00012c40: 2020 2020 2020 2020 2020 2020 7768 6574              whet
+00012c50: 6865 7220 6f72 206e 6f74 2074 6f20 7468  her or not to th
+00012c60: 6520 696e 7365 7274 2063 616c 6c20 7368  e insert call sh
+00012c70: 6f75 6c64 2072 6574 7572 6e20 6f6e 6c79  ould return only
+00012c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012c90: 2020 2061 6674 6572 2074 6865 2048 6f70     after the Hop
+00012ca0: 7377 6f72 6b73 204a 6f62 2068 6173 2066  sworks Job has f
+00012cb0: 696e 6973 6865 642e 2042 7920 6465 6661  inished. By defa
+00012cc0: 756c 7420 6974 2077 6169 7473 2e0a 2020  ult it waits..  
+00012cd0: 2020 2020 2020 2020 2020 2020 2020 2a20                * 
+00012ce0: 6b65 7920 6073 7461 7274 5f6f 6666 6c69  key `start_offli
+00012cf0: 6e65 5f62 6163 6b66 696c 6c60 2061 6e64  ne_backfill` and
+00012d00: 2076 616c 7565 2060 5472 7565 6020 6f72   value `True` or
+00012d10: 2060 4661 6c73 6560 2074 6f20 636f 6e66   `False` to conf
+00012d20: 6967 7572 650a 2020 2020 2020 2020 2020  igure.          
+00012d30: 2020 2020 2020 2020 7768 6574 6865 7220          whether 
+00012d40: 6f72 206e 6f74 2074 6f20 7374 6172 7420  or not to start 
+00012d50: 7468 6520 6261 636b 6669 6c6c 206a 6f62  the backfill job
+00012d60: 2074 6f20 7772 6974 6520 6461 7461 2074   to write data t
+00012d70: 6f20 7468 6520 6f66 666c 696e 650a 2020  o the offline.  
+00012d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d90: 7374 6f72 6167 652e 2042 7920 6465 6661  storage. By defa
+00012da0: 756c 7420 7468 6520 6261 636b 6669 6c6c  ult the backfill
+00012db0: 206a 6f62 2064 6f65 7320 6e6f 7420 6765   job does not ge
+00012dc0: 7420 7374 6172 7465 6420 6175 746f 6d61  t started automa
+00012dd0: 7469 6361 6c6c 790a 2020 2020 2020 2020  tically.        
+00012de0: 2020 2020 2020 2020 2020 666f 7220 6d75            for mu
+00012df0: 6c74 6920 7061 7274 2069 6e73 6572 7473  lti part inserts
+00012e00: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012e10: 2020 2a20 6b65 7920 6069 6e74 6572 6e61    * key `interna
+00012e20: 6c5f 6b61 666b 6160 2061 6e64 2076 616c  l_kafka` and val
+00012e30: 7565 2060 5472 7565 6020 6f72 2060 4661  ue `True` or `Fa
+00012e40: 6c73 6560 2069 6e20 6361 7365 2079 6f75  lse` in case you
+00012e50: 2065 7374 6162 6c69 7368 6564 0a20 2020   established.   
+00012e60: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00012e70: 6f6e 6e65 6374 6976 6974 7920 6672 6f6d  onnectivity from
+00012e80: 2079 6f75 2050 7974 686f 6e20 656e 7669   you Python envi
+00012e90: 726f 6e6d 656e 7420 746f 2074 6865 2069  ronment to the i
+00012ea0: 6e74 6572 6e61 6c20 6164 7665 7274 6973  nternal advertis
+00012eb0: 6564 0a20 2020 2020 2020 2020 2020 2020  ed.             
+00012ec0: 2020 2020 206c 6973 7465 6e65 7273 206f       listeners o
+00012ed0: 6620 7468 6520 486f 7073 776f 726b 7320  f the Hopsworks 
+00012ee0: 4b61 666b 6120 436c 7573 7465 722e 2044  Kafka Cluster. D
+00012ef0: 6566 6175 6c74 7320 746f 2060 4661 6c73  efaults to `Fals
+00012f00: 6560 2061 6e64 0a20 2020 2020 2020 2020  e` and.         
+00012f10: 2020 2020 2020 2020 2077 696c 6c20 7573           will us
+00012f20: 6520 6578 7465 726e 616c 206c 6973 7465  e external liste
+00012f30: 6e65 7273 2077 6865 6e20 636f 6e6e 6563  ners when connec
+00012f40: 7469 6e67 2066 726f 6d20 6f75 7473 6964  ting from outsid
+00012f50: 6520 6f66 2048 6f70 7377 6f72 6b73 2e0a  e of Hopsworks..
+00012f60: 2020 2020 2020 2020 2020 2020 7661 6c69              vali
+00012f70: 6461 7469 6f6e 5f6f 7074 696f 6e73 3a20  dation_options: 
+00012f80: 4164 6469 7469 6f6e 616c 2076 616c 6964  Additional valid
+00012f90: 6174 696f 6e20 6f70 7469 6f6e 7320 6173  ation options as
+00012fa0: 206b 6579 2d76 616c 7565 2070 6169 7273   key-value pairs
+00012fb0: 2c20 6465 6661 756c 7473 2074 6f20 607b  , defaults to `{
+00012fc0: 7d60 2e0a 2020 2020 2020 2020 2020 2020  }`..            
+00012fd0: 2020 2020 2a20 6b65 7920 6072 756e 5f76      * key `run_v
+00012fe0: 616c 6964 6174 696f 6e60 2062 6f6f 6c65  alidation` boole
+00012ff0: 616e 2076 616c 7565 2c20 7365 7420 746f  an value, set to
+00013000: 2060 4661 6c73 6560 2074 6f20 736b 6970   `False` to skip
+00013010: 2076 616c 6964 6174 696f 6e20 7465 6d70   validation temp
+00013020: 6f72 6172 696c 7920 6f6e 2069 6e67 6573  orarily on inges
+00013030: 7469 6f6e 2e0a 2020 2020 2020 2020 2020  tion..          
+00013040: 2020 2020 2020 2a20 6b65 7920 6073 6176        * key `sav
+00013050: 655f 7265 706f 7274 6020 626f 6f6c 6561  e_report` boolea
+00013060: 6e20 7661 6c75 652c 2073 6574 2074 6f20  n value, set to 
+00013070: 6046 616c 7365 6020 746f 2073 6b69 7020  `False` to skip 
+00013080: 7570 6c6f 6164 206f 6620 7468 6520 7661  upload of the va
+00013090: 6c69 6461 7469 6f6e 2072 6570 6f72 7420  lidation report 
+000130a0: 746f 2048 6f70 7377 6f72 6b73 2e0a 2020  to Hopsworks..  
+000130b0: 2020 2020 2020 2020 2020 2020 2020 2a20                * 
+000130c0: 6b65 7920 6067 655f 7661 6c69 6461 7465  key `ge_validate
+000130d0: 5f6b 7761 7267 7360 2061 2064 6963 7469  _kwargs` a dicti
+000130e0: 6f6e 6172 7920 636f 6e74 6169 6e69 6e67  onary containing
+000130f0: 206b 7761 7267 7320 666f 7220 7468 6520   kwargs for the 
+00013100: 7661 6c69 6461 7465 206d 6574 686f 6420  validate method 
+00013110: 6f66 2047 7265 6174 2045 7870 6563 7461  of Great Expecta
+00013120: 7469 6f6e 732e 0a20 2020 2020 2020 2020  tions..         
+00013130: 2020 2020 2020 202a 206b 6579 2060 6665         * key `fe
+00013140: 7463 685f 6578 7065 6374 6174 696f 6e5f  tch_expectation_
+00013150: 7375 6974 6560 2061 2062 6f6f 6c65 616e  suite` a boolean
+00013160: 2076 616c 7565 2c20 6279 2064 6566 6175   value, by defau
+00013170: 6c74 2060 4661 6c73 6560 2066 6f72 206d  lt `False` for m
+00013180: 756c 7469 2070 6172 7420 696e 7365 7274  ulti part insert
+00013190: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+000131a0: 2020 2020 2020 746f 2063 6f6e 7472 6f6c        to control
+000131b0: 2077 6865 7468 6572 2074 6865 2065 7870   whether the exp
+000131c0: 6563 7461 7469 6f6e 2073 7569 7465 206f  ectation suite o
+000131d0: 6620 7468 6520 6665 6174 7572 6520 6772  f the feature gr
+000131e0: 6f75 7020 7368 6f75 6c64 2062 6520 6665  oup should be fe
+000131f0: 7463 6865 6420 6265 666f 7265 2065 7665  tched before eve
+00013200: 7279 2069 6e73 6572 742e 0a0a 2020 2020  ry insert...    
+00013210: 2020 2020 2320 5265 7475 726e 730a 2020      # Returns.  
+00013220: 2020 2020 2020 2020 2020 2860 4a6f 6260            (`Job`
+00013230: 2c20 6056 616c 6964 6174 696f 6e52 6570  , `ValidationRep
+00013240: 6f72 7460 2920 4120 7475 706c 6520 7769  ort`) A tuple wi
+00013250: 7468 206a 6f62 2069 6e66 6f72 6d61 7469  th job informati
+00013260: 6f6e 2069 6620 7079 7468 6f6e 2065 6e67  on if python eng
+00013270: 696e 6520 6973 2075 7365 6420 616e 6420  ine is used and 
+00013280: 7468 6520 7661 6c69 6461 7469 6f6e 2072  the validation r
+00013290: 6570 6f72 7420 6966 2076 616c 6964 6174  eport if validat
+000132a0: 696f 6e20 6973 2065 6e61 626c 6564 2e0a  ion is enabled..
+000132b0: 2020 2020 2020 2020 2020 2020 6046 6561              `Fea
+000132c0: 7475 7265 4772 6f75 7057 7269 7465 7260  tureGroupWriter`
+000132d0: 2057 6865 6e20 7573 6564 2061 7320 6120   When used as a 
+000132e0: 636f 6e74 6578 7420 6d61 6e61 6765 7220  context manager 
+000132f0: 7769 7468 2050 7974 686f 6e20 6077 6974  with Python `wit
+00013300: 6860 2073 7461 7465 6d65 6e74 2e0a 2020  h` statement..  
+00013310: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00013320: 2020 7365 6c66 2e5f 6d75 6c74 695f 7061    self._multi_pa
+00013330: 7274 5f69 6e73 6572 7420 3d20 5472 7565  rt_insert = True
+00013340: 0a20 2020 2020 2020 206d 756c 7469 5f70  .        multi_p
+00013350: 6172 745f 7772 6974 6572 203d 2066 6561  art_writer = fea
+00013360: 7475 7265 5f67 726f 7570 5f77 7269 7465  ture_group_write
+00013370: 722e 4665 6174 7572 6547 726f 7570 5772  r.FeatureGroupWr
+00013380: 6974 6572 2873 656c 6629 0a20 2020 2020  iter(self).     
+00013390: 2020 2069 6620 6665 6174 7572 6573 2069     if features i
+000133a0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+000133b0: 2020 2020 7265 7475 726e 206d 756c 7469      return multi
+000133c0: 5f70 6172 745f 7772 6974 6572 0a20 2020  _part_writer.   
+000133d0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000133e0: 2020 2020 2020 2023 2067 6f20 7468 726f         # go thro
+000133f0: 7567 6820 7772 6974 6572 2074 6f20 6176  ugh writer to av
+00013400: 6f69 6420 7365 7474 696e 6720 6d75 6c74  oid setting mult
+00013410: 6920 696e 7365 7274 2064 6566 6175 6c74  i insert default
+00013420: 7320 6167 6169 6e0a 2020 2020 2020 2020  s again.        
+00013430: 2020 2020 7265 7475 726e 206d 756c 7469      return multi
+00013440: 5f70 6172 745f 7772 6974 6572 2e69 6e73  _part_writer.ins
+00013450: 6572 7428 0a20 2020 2020 2020 2020 2020  ert(.           
+00013460: 2020 2020 2066 6561 7475 7265 732c 0a20       features,. 
+00013470: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00013480: 7665 7277 7269 7465 2c0a 2020 2020 2020  verwrite,.      
+00013490: 2020 2020 2020 2020 2020 6f70 6572 6174            operat
+000134a0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
+000134b0: 2020 2020 2073 746f 7261 6765 2c0a 2020       storage,.  
+000134c0: 2020 2020 2020 2020 2020 2020 2020 7772                wr
+000134d0: 6974 655f 6f70 7469 6f6e 732c 0a20 2020  ite_options,.   
+000134e0: 2020 2020 2020 2020 2020 2020 2076 616c               val
+000134f0: 6964 6174 696f 6e5f 6f70 7469 6f6e 732c  idation_options,
+00013500: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00013510: 2020 2020 6465 6620 6669 6e61 6c69 7a65      def finalize
+00013520: 5f6d 756c 7469 5f70 6172 745f 696e 7365  _multi_part_inse
+00013530: 7274 2873 656c 6629 3a0a 2020 2020 2020  rt(self):.      
+00013540: 2020 2222 2246 696e 616c 697a 6573 2061    """Finalizes a
+00013550: 6e64 2065 7869 7473 2074 6865 206d 756c  nd exits the mul
+00013560: 7469 2070 6172 7420 696e 7365 7274 2063  ti part insert c
+00013570: 6f6e 7465 7874 206f 7065 6e65 6420 6279  ontext opened by
+00013580: 2060 6d75 6c74 695f 7061 7274 5f69 6e73   `multi_part_ins
+00013590: 6572 7460 0a20 2020 2020 2020 2069 6e20  ert`.        in 
+000135a0: 6120 626c 6f63 6b69 6e67 2066 6173 6869  a blocking fashi
+000135b0: 6f6e 206f 6e63 6520 616c 6c20 726f 7773  on once all rows
+000135c0: 2068 6176 6520 6265 656e 2074 7261 6e73   have been trans
+000135d0: 6d69 7474 6564 2e0a 0a20 2020 2020 2020  mitted...       
+000135e0: 2021 2121 2065 7861 6d70 6c65 2022 4d75   !!! example "Mu
+000135f0: 6c74 6920 7061 7274 2069 6e73 6572 7420  lti part insert 
+00013600: 7769 7468 206d 616e 7561 6c20 636f 6e74  with manual cont
+00013610: 6578 7420 6d61 6e61 6765 6d65 6e74 220a  ext management".
+00013620: 2020 2020 2020 2020 2020 2020 496e 7374              Inst
+00013630: 6561 6420 6f66 206c 6574 7469 6e67 2050  ead of letting P
+00013640: 7974 686f 6e20 6861 6e64 6c65 2074 6865  ython handle the
+00013650: 2065 6e74 6572 696e 6720 616e 6420 6578   entering and ex
+00013660: 6974 696e 6720 6f66 2074 6865 0a20 2020  iting of the.   
+00013670: 2020 2020 2020 2020 206d 756c 7469 2070           multi p
+00013680: 6172 7420 696e 7365 7274 2063 6f6e 7465  art insert conte
+00013690: 7874 2c20 796f 7520 6361 6e20 7374 6172  xt, you can star
+000136a0: 7420 616e 6420 6669 6e61 6c69 7a65 2074  t and finalize t
+000136b0: 6865 2063 6f6e 7465 7874 0a20 2020 2020  he context.     
+000136c0: 2020 2020 2020 206d 616e 7561 6c6c 792e         manually.
+000136d0: 0a20 2020 2020 2020 2020 2020 2060 6060  .            ```
+000136e0: 7079 7468 6f6e 0a20 2020 2020 2020 2020  python.         
+000136f0: 2020 2066 6561 7475 7265 5f67 726f 7570     feature_group
+00013700: 203d 2066 732e 6765 745f 6f72 5f63 7265   = fs.get_or_cre
+00013710: 6174 655f 6665 6174 7572 655f 6772 6f75  ate_feature_grou
+00013720: 7028 2266 675f 6e61 6d65 222c 2076 6572  p("fg_name", ver
+00013730: 7369 6f6e 3d31 290a 0a20 2020 2020 2020  sion=1)..       
+00013740: 2020 2020 2077 6869 6c65 206c 6f6f 703a       while loop:
+00013750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013760: 2073 6d61 6c6c 5f62 6174 6368 5f64 6620   small_batch_df 
+00013770: 3d20 2e2e 2e0a 2020 2020 2020 2020 2020  = ....          
+00013780: 2020 2020 2020 6665 6174 7572 655f 6772        feature_gr
+00013790: 6f75 702e 6d75 6c74 695f 7061 7274 5f69  oup.multi_part_i
+000137a0: 6e73 6572 7428 736d 616c 6c5f 6261 7463  nsert(small_batc
+000137b0: 685f 6466 290a 0a20 2020 2020 2020 2020  h_df)..         
+000137c0: 2020 2023 2049 4d50 4f52 5441 4e54 3a20     # IMPORTANT: 
+000137d0: 6669 6e61 6c69 7a65 2074 6865 206d 756c  finalize the mul
+000137e0: 7469 2070 6172 7420 696e 7365 7274 2074  ti part insert t
+000137f0: 6f20 6d61 6b65 2073 7572 6520 616c 6c20  o make sure all 
+00013800: 726f 7773 0a20 2020 2020 2020 2020 2020  rows.           
+00013810: 2023 2068 6176 6520 6265 656e 2074 7261   # have been tra
+00013820: 6e73 6d69 7474 6564 0a20 2020 2020 2020  nsmitted.       
+00013830: 2020 2020 2066 6561 7475 7265 5f67 726f       feature_gro
+00013840: 7570 2e66 696e 616c 697a 655f 6d75 6c74  up.finalize_mult
+00013850: 695f 7061 7274 5f69 6e73 6572 7428 290a  i_part_insert().
+00013860: 2020 2020 2020 2020 2020 2020 6060 600a              ```.
+00013870: 2020 2020 2020 2020 2020 2020 4e6f 7465              Note
+00013880: 2074 6861 7420 7468 6520 6669 7273 7420   that the first 
+00013890: 6361 6c6c 2074 6f20 606d 756c 7469 5f70  call to `multi_p
+000138a0: 6172 745f 696e 7365 7274 6020 696e 6974  art_insert` init
+000138b0: 6961 7465 7320 7468 6520 636f 6e74 6578  iates the contex
+000138c0: 740a 2020 2020 2020 2020 2020 2020 616e  t.            an
+000138d0: 6420 6265 2073 7572 6520 746f 2066 696e  d be sure to fin
+000138e0: 616c 697a 6520 6974 2e20 5468 6520 6066  alize it. The `f
+000138f0: 696e 616c 697a 655f 6d75 6c74 695f 7061  inalize_multi_pa
+00013900: 7274 5f69 6e73 6572 7460 2069 7320 610a  rt_insert` is a.
+00013910: 2020 2020 2020 2020 2020 2020 626c 6f63              bloc
+00013920: 6b69 6e67 2063 616c 6c20 7468 6174 2072  king call that r
+00013930: 6574 7572 6e73 206f 6e63 6520 616c 6c20  eturns once all 
+00013940: 726f 7773 2068 6176 6520 6265 656e 2074  rows have been t
+00013950: 7261 6e73 6d69 7474 6564 2e0a 2020 2020  ransmitted..    
+00013960: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00013970: 6966 2073 656c 662e 5f6b 6166 6b61 5f70  if self._kafka_p
+00013980: 726f 6475 6365 7220 6973 206e 6f74 204e  roducer is not N
+00013990: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000139a0: 2073 656c 662e 5f6b 6166 6b61 5f70 726f   self._kafka_pro
+000139b0: 6475 6365 722e 666c 7573 6828 290a 2020  ducer.flush().  
+000139c0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000139d0: 6b61 666b 615f 7072 6f64 7563 6572 203d  kafka_producer =
+000139e0: 204e 6f6e 650a 2020 2020 2020 2020 7365   None.        se
+000139f0: 6c66 2e5f 6665 6174 7572 655f 7772 6974  lf._feature_writ
+00013a00: 6572 7320 3d20 4e6f 6e65 0a20 2020 2020  ers = None.     
+00013a10: 2020 2073 656c 662e 5f77 7269 7465 7220     self._writer 
+00013a20: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
+00013a30: 656c 662e 5f6d 756c 7469 5f70 6172 745f  elf._multi_part_
+00013a40: 696e 7365 7274 203d 2046 616c 7365 0a0a  insert = False..
+00013a50: 2020 2020 6465 6620 696e 7365 7274 5f73      def insert_s
+00013a60: 7472 6561 6d28 0a20 2020 2020 2020 2073  tream(.        s
+00013a70: 656c 662c 0a20 2020 2020 2020 2066 6561  elf,.        fea
+00013a80: 7475 7265 733a 2054 7970 6556 6172 2822  tures: TypeVar("
+00013a90: 7079 7370 6172 6b2e 7371 6c2e 4461 7461  pyspark.sql.Data
+00013aa0: 4672 616d 6522 292c 2020 2320 6e6f 7161  Frame"),  # noqa
+00013ab0: 3a20 4638 3231 0a20 2020 2020 2020 2071  : F821.        q
+00013ac0: 7565 7279 5f6e 616d 653a 204f 7074 696f  uery_name: Optio
+00013ad0: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+00013ae0: 0a20 2020 2020 2020 206f 7574 7075 745f  .        output_
+00013af0: 6d6f 6465 3a20 4f70 7469 6f6e 616c 5b73  mode: Optional[s
+00013b00: 7472 5d20 3d20 2261 7070 656e 6422 2c0a  tr] = "append",.
+00013b10: 2020 2020 2020 2020 6177 6169 745f 7465          await_te
+00013b20: 726d 696e 6174 696f 6e3a 204f 7074 696f  rmination: Optio
+00013b30: 6e61 6c5b 626f 6f6c 5d20 3d20 4661 6c73  nal[bool] = Fals
+00013b40: 652c 0a20 2020 2020 2020 2074 696d 656f  e,.        timeo
+00013b50: 7574 3a20 4f70 7469 6f6e 616c 5b69 6e74  ut: Optional[int
+00013b60: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00013b70: 2020 6368 6563 6b70 6f69 6e74 5f64 6972    checkpoint_dir
+00013b80: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00013b90: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00013ba0: 7772 6974 655f 6f70 7469 6f6e 733a 204f  write_options: O
+00013bb0: 7074 696f 6e61 6c5b 4469 6374 5b41 6e79  ptional[Dict[Any
+00013bc0: 2c20 416e 795d 5d20 3d20 7b7d 2c0a 2020  , Any]] = {},.  
+00013bd0: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
+00013be0: 496e 6765 7374 2061 2053 7061 726b 2053  Ingest a Spark S
+00013bf0: 7472 7563 7475 7265 6420 5374 7265 616d  tructured Stream
+00013c00: 696e 6720 4461 7461 6672 616d 6520 746f  ing Dataframe to
+00013c10: 2074 6865 206f 6e6c 696e 6520 6665 6174   the online feat
+00013c20: 7572 6520 7374 6f72 652e 0a0a 2020 2020  ure store...    
+00013c30: 2020 2020 5468 6973 206d 6574 686f 6420      This method 
+00013c40: 6372 6561 7465 7320 6120 6c6f 6e67 2072  creates a long r
+00013c50: 756e 6e69 6e67 2053 7061 726b 2053 7472  unning Spark Str
+00013c60: 6561 6d69 6e67 2051 7565 7279 2c20 796f  eaming Query, yo
+00013c70: 7520 6361 6e20 636f 6e74 726f 6c20 7468  u can control th
+00013c80: 650a 2020 2020 2020 2020 7465 726d 696e  e.        termin
+00013c90: 6174 696f 6e20 6f66 2074 6865 2071 7565  ation of the que
+00013ca0: 7279 2074 6872 6f75 6768 2074 6865 2061  ry through the a
+00013cb0: 7267 756d 656e 7473 2e0a 0a20 2020 2020  rguments...     
+00013cc0: 2020 2049 7420 6973 2070 6f73 7369 626c     It is possibl
+00013cd0: 6520 746f 2073 746f 7020 7468 6520 7265  e to stop the re
+00013ce0: 7475 726e 6564 2071 7565 7279 2077 6974  turned query wit
+00013cf0: 6820 7468 6520 602e 7374 6f70 2829 6020  h the `.stop()` 
+00013d00: 616e 6420 6368 6563 6b20 6974 730a 2020  and check its.  
+00013d10: 2020 2020 2020 7374 6174 7573 2077 6974        status wit
+00013d20: 6820 602e 6973 4163 7469 7665 602e 0a0a  h `.isActive`...
+00013d30: 2020 2020 2020 2020 546f 2067 6574 2061          To get a
+00013d40: 206c 6973 7420 6f66 2061 6c6c 2061 6374   list of all act
+00013d50: 6976 6520 7175 6572 6965 732c 2075 7365  ive queries, use
+00013d60: 3a0a 0a20 2020 2020 2020 2060 6060 7079  :..        ```py
+00013d70: 7468 6f6e 0a20 2020 2020 2020 2073 716d  thon.        sqm
+00013d80: 203d 2073 7061 726b 2e73 7472 6561 6d73   = spark.streams
+00013d90: 0a0a 2020 2020 2020 2020 2320 6765 7420  ..        # get 
+00013da0: 7468 6520 6c69 7374 206f 6620 6163 7469  the list of acti
+00013db0: 7665 2073 7472 6561 6d69 6e67 2071 7565  ve streaming que
+00013dc0: 7269 6573 0a20 2020 2020 2020 205b 712e  ries.        [q.
+00013dd0: 6e61 6d65 2066 6f72 2071 2069 6e20 7371  name for q in sq
+00013de0: 6d2e 6163 7469 7665 5d0a 2020 2020 2020  m.active].      
+00013df0: 2020 6060 600a 0a20 2020 2020 2020 2021    ```..        !
+00013e00: 2121 2077 6172 6e69 6e67 2022 456e 6769  !! warning "Engi
+00013e10: 6e65 2053 7570 706f 7274 220a 2020 2020  ne Support".    
+00013e20: 2020 2020 2020 2020 2a2a 5370 6172 6b20          **Spark 
+00013e30: 6f6e 6c79 2a2a 0a0a 2020 2020 2020 2020  only**..        
+00013e40: 2020 2020 5374 7265 616d 2069 6e67 6573      Stream inges
+00013e50: 7469 6f6e 2075 7369 6e67 2050 616e 6461  tion using Panda
+00013e60: 732f 5079 7468 6f6e 2061 7320 656e 6769  s/Python as engi
+00013e70: 6e65 2069 7320 6375 7272 656e 746c 7920  ne is currently 
+00013e80: 6e6f 7420 7375 7070 6f72 7465 642e 0a20  not supported.. 
+00013e90: 2020 2020 2020 2020 2020 2050 7974 686f             Pytho
+00013ea0: 6e2f 5061 6e64 6173 2068 6173 206e 6f20  n/Pandas has no 
+00013eb0: 6e6f 7469 6f6e 206f 6620 7374 7265 616d  notion of stream
+00013ec0: 696e 672e 0a0a 2020 2020 2020 2020 2121  ing...        !!
+00013ed0: 2120 7761 726e 696e 6720 2244 6174 6120  ! warning "Data 
+00013ee0: 5661 6c69 6461 7469 6f6e 2053 7570 706f  Validation Suppo
+00013ef0: 7274 220a 2020 2020 2020 2020 2020 2020  rt".            
+00013f00: 6069 6e73 6572 745f 7374 7265 616d 6020  `insert_stream` 
+00013f10: 646f 6573 206e 6f74 2070 6572 666f 726d  does not perform
+00013f20: 2061 6e79 2064 6174 6120 7661 6c69 6461   any data valida
+00013f30: 7469 6f6e 2075 7369 6e67 2047 7265 6174  tion using Great
+00013f40: 2045 7870 6563 7461 7469 6f6e 730a 2020   Expectations.  
+00013f50: 2020 2020 2020 2020 2020 6576 656e 2077            even w
+00013f60: 6865 6e20 6120 6578 7065 6374 6174 696f  hen a expectatio
+00013f70: 6e20 7375 6974 6520 6973 2061 7474 6163  n suite is attac
+00013f80: 6865 642e 0a0a 2020 2020 2020 2020 2320  hed...        # 
+00013f90: 4172 6775 6d65 6e74 730a 2020 2020 2020  Arguments.      
+00013fa0: 2020 2020 2020 6665 6174 7572 6573 3a20        features: 
+00013fb0: 4665 6174 7572 6573 2069 6e20 5374 7265  Features in Stre
+00013fc0: 616d 696e 6720 4461 7461 6672 616d 6520  aming Dataframe 
+00013fd0: 746f 2062 6520 7361 7665 642e 0a20 2020  to be saved..   
+00013fe0: 2020 2020 2020 2020 2071 7565 7279 5f6e           query_n
+00013ff0: 616d 653a 2049 7420 6973 2070 6f73 7369  ame: It is possi
+00014000: 626c 6520 746f 206f 7074 696f 6e61 6c6c  ble to optionall
+00014010: 7920 7370 6563 6966 7920 6120 6e61 6d65  y specify a name
+00014020: 2066 6f72 2074 6865 2071 7565 7279 2074   for the query t
+00014030: 6f0a 2020 2020 2020 2020 2020 2020 2020  o.              
+00014040: 2020 6d61 6b65 2069 7420 6561 7369 6572    make it easier
+00014050: 2074 6f20 7265 636f 676e 6973 6520 696e   to recognise in
+00014060: 2074 6865 2053 7061 726b 2055 492e 2044   the Spark UI. D
+00014070: 6566 6175 6c74 7320 746f 2060 4e6f 6e65  efaults to `None
+00014080: 602e 0a20 2020 2020 2020 2020 2020 206f  `..            o
+00014090: 7574 7075 745f 6d6f 6465 3a20 5370 6563  utput_mode: Spec
+000140a0: 6966 6965 7320 686f 7720 6461 7461 206f  ifies how data o
+000140b0: 6620 6120 7374 7265 616d 696e 6720 4461  f a streaming Da
+000140c0: 7461 4672 616d 652f 4461 7461 7365 7420  taFrame/Dataset 
+000140d0: 6973 0a20 2020 2020 2020 2020 2020 2020  is.             
+000140e0: 2020 2077 7269 7474 656e 2074 6f20 6120     written to a 
+000140f0: 7374 7265 616d 696e 6720 7369 6e6b 2e20  streaming sink. 
+00014100: 2831 2920 6022 6170 7065 6e64 2260 3a20  (1) `"append"`: 
+00014110: 4f6e 6c79 2074 6865 206e 6577 2072 6f77  Only the new row
+00014120: 7320 696e 2074 6865 0a20 2020 2020 2020  s in the.       
+00014130: 2020 2020 2020 2020 2073 7472 6561 6d69           streami
+00014140: 6e67 2044 6174 6146 7261 6d65 2f44 6174  ng DataFrame/Dat
+00014150: 6173 6574 2077 696c 6c20 6265 2077 7269  aset will be wri
+00014160: 7474 656e 2074 6f20 7468 6520 7369 6e6b  tten to the sink
+00014170: 2e20 2832 290a 2020 2020 2020 2020 2020  . (2).          
+00014180: 2020 2020 2020 6022 636f 6d70 6c65 7465        `"complete
+00014190: 2260 3a20 416c 6c20 7468 6520 726f 7773  "`: All the rows
+000141a0: 2069 6e20 7468 6520 7374 7265 616d 696e   in the streamin
+000141b0: 6720 4461 7461 4672 616d 652f 4461 7461  g DataFrame/Data
+000141c0: 7365 7420 7769 6c6c 2062 650a 2020 2020  set will be.    
+000141d0: 2020 2020 2020 2020 2020 2020 7772 6974              writ
+000141e0: 7465 6e20 746f 2074 6865 2073 696e 6b20  ten to the sink 
+000141f0: 6576 6572 7920 7469 6d65 2074 6865 7265  every time there
+00014200: 2069 7320 736f 6d65 2075 7064 6174 652e   is some update.
+00014210: 2028 3329 2060 2275 7064 6174 6522 603a   (3) `"update"`:
+00014220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014230: 206f 6e6c 7920 7468 6520 726f 7773 2074   only the rows t
+00014240: 6861 7420 7765 7265 2075 7064 6174 6564  hat were updated
+00014250: 2069 6e20 7468 6520 7374 7265 616d 696e   in the streamin
+00014260: 6720 4461 7461 4672 616d 652f 4461 7461  g DataFrame/Data
+00014270: 7365 7420 7769 6c6c 0a20 2020 2020 2020  set will.       
+00014280: 2020 2020 2020 2020 2062 6520 7772 6974           be writ
+00014290: 7465 6e20 746f 2074 6865 2073 696e 6b20  ten to the sink 
+000142a0: 6576 6572 7920 7469 6d65 2074 6865 7265  every time there
+000142b0: 2061 7265 2073 6f6d 6520 7570 6461 7465   are some update
+000142c0: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
+000142d0: 2020 2049 6620 7468 6520 7175 6572 7920     If the query 
+000142e0: 646f 6573 6ee2 8099 7420 636f 6e74 6169  doesn...t contai
+000142f0: 6e20 6167 6772 6567 6174 696f 6e73 2c20  n aggregations, 
+00014300: 6974 2077 696c 6c20 6265 2065 7175 6976  it will be equiv
+00014310: 616c 656e 7420 746f 0a20 2020 2020 2020  alent to.       
+00014320: 2020 2020 2020 2020 2061 7070 656e 6420           append 
+00014330: 6d6f 6465 2e20 4465 6661 756c 7473 2074  mode. Defaults t
+00014340: 6f20 6022 6170 7065 6e64 2260 2e0a 2020  o `"append"`..  
+00014350: 2020 2020 2020 2020 2020 6177 6169 745f            await_
+00014360: 7465 726d 696e 6174 696f 6e3a 2057 6169  termination: Wai
+00014370: 7473 2066 6f72 2074 6865 2074 6572 6d69  ts for the termi
+00014380: 6e61 7469 6f6e 206f 6620 7468 6973 2071  nation of this q
+00014390: 7565 7279 2c20 6569 7468 6572 2062 790a  uery, either by.
+000143a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000143b0: 7175 6572 792e 7374 6f70 2829 206f 7220  query.stop() or 
+000143c0: 6279 2061 6e20 6578 6365 7074 696f 6e2e  by an exception.
+000143d0: 2049 6620 7468 6520 7175 6572 7920 6861   If the query ha
+000143e0: 7320 7465 726d 696e 6174 6564 2077 6974  s terminated wit
+000143f0: 6820 616e 0a20 2020 2020 2020 2020 2020  h an.           
+00014400: 2020 2020 2065 7863 6570 7469 6f6e 2c20       exception, 
+00014410: 7468 656e 2074 6865 2065 7863 6570 7469  then the excepti
+00014420: 6f6e 2077 696c 6c20 6265 2074 6872 6f77  on will be throw
+00014430: 6e2e 2049 6620 7469 6d65 6f75 7420 6973  n. If timeout is
+00014440: 2073 6574 2c20 6974 0a20 2020 2020 2020   set, it.       
+00014450: 2020 2020 2020 2020 2072 6574 7572 6e73           returns
+00014460: 2077 6865 7468 6572 2074 6865 2071 7565   whether the que
+00014470: 7279 2068 6173 2074 6572 6d69 6e61 7465  ry has terminate
+00014480: 6420 6f72 206e 6f74 2077 6974 6869 6e20  d or not within 
+00014490: 7468 6520 7469 6d65 6f75 740a 2020 2020  the timeout.    
+000144a0: 2020 2020 2020 2020 2020 2020 7365 636f              seco
+000144b0: 6e64 732e 2044 6566 6175 6c74 7320 746f  nds. Defaults to
+000144c0: 2060 4661 6c73 6560 2e0a 2020 2020 2020   `False`..      
+000144d0: 2020 2020 2020 7469 6d65 6f75 743a 204f        timeout: O
+000144e0: 6e6c 7920 7265 6c65 7661 6e74 2069 6e20  nly relevant in 
+000144f0: 636f 6d62 696e 6174 696f 6e20 7769 7468  combination with
+00014500: 2060 6177 6169 745f 7465 726d 696e 6174   `await_terminat
+00014510: 696f 6e3d 5472 7565 602e 0a20 2020 2020  ion=True`..     
+00014520: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
+00014530: 6c74 7320 746f 2060 4e6f 6e65 602e 0a20  lts to `None`.. 
+00014540: 2020 2020 2020 2020 2020 2063 6865 636b             check
+00014550: 706f 696e 745f 6469 723a 2043 6865 636b  point_dir: Check
+00014560: 706f 696e 7420 6469 7265 6374 6f72 7920  point directory 
+00014570: 6c6f 6361 7469 6f6e 2e20 5468 6973 2077  location. This w
+00014580: 696c 6c20 6265 2075 7365 6420 746f 2061  ill be used to a
+00014590: 7320 6120 7265 6665 7265 6e63 6520 746f  s a reference to
+000145a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000145b0: 2066 726f 6d20 7768 6572 6520 746f 2072   from where to r
+000145c0: 6573 756d 6520 7468 6520 7374 7265 616d  esume the stream
+000145d0: 696e 6720 6a6f 622e 2049 6620 604e 6f6e  ing job. If `Non
+000145e0: 6560 2074 6865 6e20 6873 6673 2077 696c  e` then hsfs wil
+000145f0: 6c20 636f 6e73 7472 7563 7420 6173 0a20  l construct as. 
+00014600: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00014610: 696e 7365 7274 5f73 7472 6561 6d5f 2220  insert_stream_" 
+00014620: 2b20 6f6e 6c69 6e65 5f74 6f70 6963 5f6e  + online_topic_n
+00014630: 616d 652e 2044 6566 6175 6c74 7320 746f  ame. Defaults to
+00014640: 2060 4e6f 6e65 602e 0a20 2020 2020 2020   `None`..       
+00014650: 2020 2020 2020 2020 2077 7269 7465 5f6f           write_o
+00014660: 7074 696f 6e73 3a20 4164 6469 7469 6f6e  ptions: Addition
+00014670: 616c 2077 7269 7465 206f 7074 696f 6e73  al write options
+00014680: 2066 6f72 2053 7061 726b 2061 7320 6b65   for Spark as ke
+00014690: 792d 7661 6c75 6520 7061 6972 732e 0a20  y-value pairs.. 
+000146a0: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+000146b0: 6566 6175 6c74 7320 746f 2060 7b7d 602e  efaults to `{}`.
+000146c0: 0a0a 2020 2020 2020 2020 2320 5265 7475  ..        # Retu
+000146d0: 726e 730a 2020 2020 2020 2020 2020 2020  rns.            
+000146e0: 6053 7472 6561 6d69 6e67 5175 6572 7960  `StreamingQuery`
+000146f0: 3a20 5370 6172 6b20 5374 7275 6374 7572  : Spark Structur
+00014700: 6564 2053 7472 6561 6d69 6e67 2051 7565  ed Streaming Que
+00014710: 7279 206f 626a 6563 742e 0a20 2020 2020  ry object..     
+00014720: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00014730: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+00014740: 6e6f 7420 656e 6769 6e65 2e67 6574 5f69  not engine.get_i
+00014750: 6e73 7461 6e63 6528 292e 6973 5f73 7061  nstance().is_spa
+00014760: 726b 5f64 6174 6166 7261 6d65 2866 6561  rk_dataframe(fea
+00014770: 7475 7265 7329 0a20 2020 2020 2020 2020  tures).         
+00014780: 2020 206f 7220 6e6f 7420 6665 6174 7572     or not featur
+00014790: 6573 2e69 7353 7472 6561 6d69 6e67 0a20  es.isStreaming. 
+000147a0: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+000147b0: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
+000147c0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+000147d0: 2020 2020 2020 2022 4665 6174 7572 6573         "Features
+000147e0: 2068 6176 6520 746f 2062 6520 6120 7374   have to be a st
+000147f0: 7265 616d 696e 6720 7479 7065 2073 7061  reaming type spa
+00014800: 726b 2064 6174 6166 7261 6d65 2e20 5573  rk dataframe. Us
+00014810: 6520 6069 6e73 6572 7428 2960 206d 6574  e `insert()` met
+00014820: 686f 6420 696e 7374 6561 642e 220a 2020  hod instead.".  
+00014830: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00014840: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00014850: 2020 2020 2020 2320 6c6f 7765 7220 6361        # lower ca
+00014860: 7369 6e67 2066 6561 7475 7265 206e 616d  sing feature nam
+00014870: 6573 0a20 2020 2020 2020 2020 2020 2066  es.            f
+00014880: 6561 7475 7265 5f64 6174 6166 7261 6d65  eature_dataframe
+00014890: 203d 2065 6e67 696e 652e 6765 745f 696e   = engine.get_in
+000148a0: 7374 616e 6365 2829 2e63 6f6e 7665 7274  stance().convert
+000148b0: 5f74 6f5f 6465 6661 756c 745f 6461 7461  _to_default_data
+000148c0: 6672 616d 6528 0a20 2020 2020 2020 2020  frame(.         
+000148d0: 2020 2020 2020 2066 6561 7475 7265 730a         features.
+000148e0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000148f0: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
+00014900: 6773 2e77 6172 6e28 0a20 2020 2020 2020  gs.warn(.       
+00014910: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
+00014920: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00014930: 5374 7265 616d 2069 6e67 6573 7469 6f6e  Stream ingestion
+00014940: 2066 6f72 2066 6561 7475 7265 2067 726f   for feature gro
+00014950: 7570 2060 7b7d 602c 2077 6974 6820 7665  up `{}`, with ve
+00014960: 7273 696f 6e22 0a20 2020 2020 2020 2020  rsion".         
+00014970: 2020 2020 2020 2020 2020 2022 2060 7b7d             " `{}
+00014980: 6020 7769 6c6c 206e 6f74 2063 6f6d 7075  ` will not compu
+00014990: 7465 2073 7461 7469 7374 6963 732e 220a  te statistics.".
+000149a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000149b0: 292e 666f 726d 6174 2873 656c 662e 5f6e  ).format(self._n
+000149c0: 616d 652c 2073 656c 662e 5f76 6572 7369  ame, self._versi
+000149d0: 6f6e 292c 0a20 2020 2020 2020 2020 2020  on),.           
+000149e0: 2020 2020 2075 7469 6c2e 5374 6174 6973       util.Statis
+000149f0: 7469 6373 5761 726e 696e 672c 0a20 2020  ticsWarning,.   
+00014a00: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00014a10: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00014a20: 656c 662e 5f66 6561 7475 7265 5f67 726f  elf._feature_gro
+00014a30: 7570 5f65 6e67 696e 652e 696e 7365 7274  up_engine.insert
+00014a40: 5f73 7472 6561 6d28 0a20 2020 2020 2020  _stream(.       
+00014a50: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
+00014a60: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00014a70: 6561 7475 7265 5f64 6174 6166 7261 6d65  eature_dataframe
+00014a80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00014a90: 2020 7175 6572 795f 6e61 6d65 2c0a 2020    query_name,.  
+00014aa0: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
+00014ab0: 7470 7574 5f6d 6f64 652c 0a20 2020 2020  tput_mode,.     
+00014ac0: 2020 2020 2020 2020 2020 2061 7761 6974             await
+00014ad0: 5f74 6572 6d69 6e61 7469 6f6e 2c0a 2020  _termination,.  
+00014ae0: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+00014af0: 6d65 6f75 742c 0a20 2020 2020 2020 2020  meout,.         
+00014b00: 2020 2020 2020 2063 6865 636b 706f 696e         checkpoin
+00014b10: 745f 6469 722c 0a20 2020 2020 2020 2020  t_dir,.         
+00014b20: 2020 2020 2020 2077 7269 7465 5f6f 7074         write_opt
+00014b30: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
+00014b40: 2020 290a 0a20 2020 2064 6566 2063 6f6d    )..    def com
+00014b50: 6d69 745f 6465 7461 696c 7328 0a20 2020  mit_details(.   
+00014b60: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00014b70: 2020 2077 616c 6c63 6c6f 636b 5f74 696d     wallclock_tim
+00014b80: 653a 204f 7074 696f 6e61 6c5b 556e 696f  e: Optional[Unio
+00014b90: 6e5b 7374 722c 2069 6e74 2c20 6461 7465  n[str, int, date
+00014ba0: 7469 6d65 2c20 6461 7465 5d5d 203d 204e  time, date]] = N
+00014bb0: 6f6e 652c 0a20 2020 2020 2020 206c 696d  one,.        lim
+00014bc0: 6974 3a20 4f70 7469 6f6e 616c 5b69 6e74  it: Optional[int
+00014bd0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 293a  ] = None,.    ):
+00014be0: 0a20 2020 2020 2020 2022 2222 5265 7472  .        """Retr
+00014bf0: 6965 7665 7320 636f 6d6d 6974 2074 696d  ieves commit tim
+00014c00: 656c 696e 6520 666f 7220 7468 6973 2066  eline for this f
+00014c10: 6561 7475 7265 2067 726f 7570 2e20 5468  eature group. Th
+00014c20: 6973 206d 6574 686f 6420 6361 6e20 6f6e  is method can on
+00014c30: 6c79 2062 6520 7573 6564 0a20 2020 2020  ly be used.     
+00014c40: 2020 206f 6e20 7469 6d65 2074 7261 7665     on time trave
+00014c50: 6c20 656e 6162 6c65 6420 6665 6174 7572  l enabled featur
+00014c60: 6520 6772 6f75 7073 0a0a 2020 2020 2020  e groups..      
+00014c70: 2020 2121 2120 6578 616d 706c 650a 2020    !!! example.  
+00014c80: 2020 2020 2020 2020 2020 6060 6070 7974            ```pyt
+00014c90: 686f 6e0a 2020 2020 2020 2020 2020 2020  hon.            
+00014ca0: 2320 636f 6e6e 6563 7420 746f 2074 6865  # connect to the
+00014cb0: 2046 6561 7475 7265 2053 746f 7265 0a20   Feature Store. 
+00014cc0: 2020 2020 2020 2020 2020 2066 7320 3d20             fs = 
+00014cd0: 2e2e 2e0a 0a20 2020 2020 2020 2020 2020  .....           
+00014ce0: 2023 2067 6574 2074 6865 2046 6561 7475   # get the Featu
+00014cf0: 7265 2047 726f 7570 2069 6e73 7461 6e63  re Group instanc
+00014d00: 650a 2020 2020 2020 2020 2020 2020 6667  e.            fg
+00014d10: 203d 2066 732e 6765 745f 6f72 5f63 7265   = fs.get_or_cre
+00014d20: 6174 655f 6665 6174 7572 655f 6772 6f75  ate_feature_grou
+00014d30: 7028 2e2e 2e29 0a0a 2020 2020 2020 2020  p(...)..        
+00014d40: 2020 2020 636f 6d6d 6974 5f64 6574 6169      commit_detai
+00014d50: 6c73 203d 2066 672e 636f 6d6d 6974 5f64  ls = fg.commit_d
+00014d60: 6574 6169 6c73 2829 0a20 2020 2020 2020  etails().       
+00014d70: 2020 2020 2060 6060 0a0a 2020 2020 2020       ```..      
+00014d80: 2020 2320 4172 6775 6d65 6e74 730a 2020    # Arguments.  
+00014d90: 2020 2020 2020 2020 2020 7761 6c6c 636c            wallcl
+00014da0: 6f63 6b5f 7469 6d65 3a20 436f 6d6d 6974  ock_time: Commit
+00014db0: 2064 6574 6169 6c73 2061 7320 6f66 2073   details as of s
+00014dc0: 7065 6369 6669 6320 706f 696e 7420 696e  pecific point in
+00014dd0: 2074 696d 652e 2044 6566 6175 6c74 7320   time. Defaults 
+00014de0: 746f 2060 4e6f 6e65 602e 0a20 2020 2020  to `None`..     
+00014df0: 2020 2020 2020 2020 2020 2020 5374 7269              Stri
+00014e00: 6e67 7320 7368 6f75 6c64 2062 6520 666f  ngs should be fo
+00014e10: 726d 6174 7465 6420 696e 206f 6e65 206f  rmatted in one o
+00014e20: 6620 7468 6520 666f 6c6c 6f77 696e 6720  f the following 
+00014e30: 666f 726d 6174 7320 6025 592d 256d 2d25  formats `%Y-%m-%
+00014e40: 6460 2c20 6025 592d 256d 2d25 6420 2548  d`, `%Y-%m-%d %H
+00014e50: 602c 2060 2559 2d25 6d2d 2564 2025 483a  `, `%Y-%m-%d %H:
+00014e60: 254d 602c 0a20 2020 2020 2020 2020 2020  %M`,.           
+00014e70: 2020 2020 2060 2559 2d25 6d2d 2564 2025       `%Y-%m-%d %
+00014e80: 483a 254d 3a25 5360 2c20 6f72 2060 2559  H:%M:%S`, or `%Y
+00014e90: 2d25 6d2d 2564 2025 483a 254d 3a25 532e  -%m-%d %H:%M:%S.
+00014ea0: 2566 602e 0a20 2020 2020 2020 2020 2020  %f`..           
+00014eb0: 206c 696d 6974 3a20 4e75 6d62 6572 206f   limit: Number o
+00014ec0: 6620 636f 6d6d 6974 7320 746f 2072 6574  f commits to ret
+00014ed0: 7269 6576 652e 2044 6566 6175 6c74 7320  rieve. Defaults 
+00014ee0: 746f 2060 4e6f 6e65 602e 0a0a 2020 2020  to `None`...    
+00014ef0: 2020 2020 2320 5265 7475 726e 730a 2020      # Returns.  
+00014f00: 2020 2020 2020 2020 2020 6044 6963 745b            `Dict[
+00014f10: 7374 722c 2044 6963 745b 7374 722c 2073  str, Dict[str, s
+00014f20: 7472 5d5d 602e 2044 6963 7469 6f6e 6172  tr]]`. Dictionar
+00014f30: 7920 6f62 6a65 6374 206f 6620 636f 6d6d  y object of comm
+00014f40: 6974 206d 6574 6164 6174 6120 7469 6d65  it metadata time
+00014f50: 6c69 6e65 2c20 7768 6572 6520 4b65 7920  line, where Key 
+00014f60: 6973 2063 6f6d 6d69 7420 6964 2061 6e64  is commit id and
+00014f70: 2076 616c 7565 0a20 2020 2020 2020 2020   value.         
+00014f80: 2020 2069 7320 6044 6963 745b 7374 722c     is `Dict[str,
+00014f90: 2073 7472 5d60 2077 6974 6820 6b65 7920   str]` with key 
+00014fa0: 7661 6c75 6520 7061 6972 7320 6f66 2064  value pairs of d
+00014fb0: 6174 6520 636f 6d6d 6974 7465 6420 6f6e  ate committed on
+00014fc0: 2c20 6e75 6d62 6572 206f 6620 726f 7773  , number of rows
+00014fd0: 2075 7064 6174 6564 2c20 696e 7365 7274   updated, insert
+00014fe0: 6564 2061 6e64 2064 656c 6574 6564 2e0a  ed and deleted..
+00014ff0: 0a20 2020 2020 2020 2023 2052 6169 7365  .        # Raise
+00015000: 730a 2020 2020 2020 2020 2020 2020 6068  s.            `h
+00015010: 7366 732e 636c 6965 6e74 2e65 7863 6570  sfs.client.excep
+00015020: 7469 6f6e 732e 5265 7374 4150 4945 7272  tions.RestAPIErr
+00015030: 6f72 602e 0a20 2020 2020 2020 2020 2020  or`..           
+00015040: 2060 6873 6673 2e63 6c69 656e 742e 6578   `hsfs.client.ex
+00015050: 6365 7074 696f 6e73 2e46 6561 7475 7265  ceptions.Feature
+00015060: 5374 6f72 6545 7863 6570 7469 6f6e 602e  StoreException`.
+00015070: 2049 6620 7468 6520 6665 6174 7572 6520   If the feature 
+00015080: 6772 6f75 7020 646f 6573 206e 6f74 2068  group does not h
+00015090: 6176 6520 6048 5544 4960 2074 696d 6520  ave `HUDI` time 
+000150a0: 7472 6176 656c 2066 6f72 6d61 740a 2020  travel format.  
+000150b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000150c0: 2020 7265 7475 726e 2073 656c 662e 5f66    return self._f
+000150d0: 6561 7475 7265 5f67 726f 7570 5f65 6e67  eature_group_eng
+000150e0: 696e 652e 636f 6d6d 6974 5f64 6574 6169  ine.commit_detai
+000150f0: 6c73 2873 656c 662c 2077 616c 6c63 6c6f  ls(self, wallclo
+00015100: 636b 5f74 696d 652c 206c 696d 6974 290a  ck_time, limit).
+00015110: 0a20 2020 2064 6566 2063 6f6d 6d69 745f  .    def commit_
+00015120: 6465 6c65 7465 5f72 6563 6f72 6428 0a20  delete_record(. 
+00015130: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00015140: 2020 2020 2064 656c 6574 655f 6466 3a20       delete_df: 
+00015150: 5479 7065 5661 7228 2270 7973 7061 726b  TypeVar("pyspark
+00015160: 2e73 716c 2e44 6174 6146 7261 6d65 2229  .sql.DataFrame")
+00015170: 2c20 2023 206e 6f71 613a 2046 3832 310a  ,  # noqa: F821.
+00015180: 2020 2020 2020 2020 7772 6974 655f 6f70          write_op
+00015190: 7469 6f6e 733a 204f 7074 696f 6e61 6c5b  tions: Optional[
+000151a0: 4469 6374 5b41 6e79 2c20 416e 795d 5d20  Dict[Any, Any]] 
+000151b0: 3d20 7b7d 2c0a 2020 2020 293a 0a20 2020  = {},.    ):.   
+000151c0: 2020 2020 2022 2222 4472 6f70 7320 7265       """Drops re
+000151d0: 636f 7264 7320 7072 6573 656e 7420 696e  cords present in
+000151e0: 2074 6865 2070 726f 7669 6465 6420 4461   the provided Da
+000151f0: 7461 4672 616d 6520 616e 6420 636f 6d6d  taFrame and comm
+00015200: 6974 7320 6974 2061 7320 7570 6461 7465  its it as update
+00015210: 2074 6f20 7468 6973 0a20 2020 2020 2020   to this.       
+00015220: 2046 6561 7475 7265 2067 726f 7570 2e20   Feature group. 
+00015230: 5468 6973 206d 6574 686f 6420 6361 6e20  This method can 
+00015240: 6f6e 6c79 2062 6520 7573 6564 206f 6e20  only be used on 
+00015250: 7469 6d65 2074 7261 7665 6c20 656e 6162  time travel enab
+00015260: 6c65 6420 6665 6174 7572 6520 6772 6f75  led feature grou
+00015270: 7073 2e0a 0a20 2020 2020 2020 2023 2041  ps...        # A
+00015280: 7267 756d 656e 7473 0a20 2020 2020 2020  rguments.       
+00015290: 2020 2020 2064 656c 6574 655f 6466 3a20       delete_df: 
+000152a0: 6461 7461 4672 616d 6520 636f 6e74 6169  dataFrame contai
+000152b0: 6e69 6e67 2072 6563 6f72 6473 2074 6f20  ning records to 
+000152c0: 6265 2064 656c 6574 6564 2e0a 2020 2020  be deleted..    
+000152d0: 2020 2020 2020 2020 7772 6974 655f 6f70          write_op
+000152e0: 7469 6f6e 733a 2055 7365 7220 7072 6f76  tions: User prov
+000152f0: 6964 6564 2077 7269 7465 206f 7074 696f  ided write optio
+00015300: 6e73 2e20 4465 6661 756c 7473 2074 6f20  ns. Defaults to 
+00015310: 607b 7d60 2e0a 0a20 2020 2020 2020 2023  `{}`...        #
+00015320: 2052 6169 7365 730a 2020 2020 2020 2020   Raises.        
+00015330: 2020 2020 6068 7366 732e 636c 6965 6e74      `hsfs.client
+00015340: 2e65 7863 6570 7469 6f6e 732e 5265 7374  .exceptions.Rest
+00015350: 4150 4945 7272 6f72 602e 0a20 2020 2020  APIError`..     
+00015360: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
+00015370: 656c 662e 5f66 6561 7475 7265 5f67 726f  elf._feature_gro
+00015380: 7570 5f65 6e67 696e 652e 636f 6d6d 6974  up_engine.commit
+00015390: 5f64 656c 6574 6528 7365 6c66 2c20 6465  _delete(self, de
+000153a0: 6c65 7465 5f64 662c 2077 7269 7465 5f6f  lete_df, write_o
+000153b0: 7074 696f 6e73 290a 0a20 2020 2064 6566  ptions)..    def
+000153c0: 2061 735f 6f66 280a 2020 2020 2020 2020   as_of(.        
+000153d0: 7365 6c66 2c0a 2020 2020 2020 2020 7761  self,.        wa
+000153e0: 6c6c 636c 6f63 6b5f 7469 6d65 3a20 4f70  llclock_time: Op
+000153f0: 7469 6f6e 616c 5b55 6e69 6f6e 5b73 7472  tional[Union[str
+00015400: 2c20 696e 742c 2064 6174 6574 696d 652c  , int, datetime,
+00015410: 2064 6174 655d 5d20 3d20 4e6f 6e65 2c0a   date]] = None,.
+00015420: 2020 2020 2020 2020 6578 636c 7564 655f          exclude_
+00015430: 756e 7469 6c3a 204f 7074 696f 6e61 6c5b  until: Optional[
+00015440: 556e 696f 6e5b 7374 722c 2069 6e74 2c20  Union[str, int, 
+00015450: 6461 7465 7469 6d65 2c20 6461 7465 5d5d  datetime, date]]
+00015460: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+00015470: 2020 2020 2020 2020 2222 2247 6574 2051          """Get Q
+00015480: 7565 7279 206f 626a 6563 7420 746f 2072  uery object to r
+00015490: 6574 7269 6576 6520 616c 6c20 6665 6174  etrieve all feat
+000154a0: 7572 6573 206f 6620 7468 6520 6772 6f75  ures of the grou
+000154b0: 7020 6174 2061 2070 6f69 6e74 2069 6e20  p at a point in 
+000154c0: 7468 6520 7061 7374 2e0a 0a20 2020 2020  the past...     
+000154d0: 2020 2054 6869 7320 6d65 7468 6f64 2073     This method s
+000154e0: 656c 6563 7473 2061 6c6c 2066 6561 7475  elects all featu
+000154f0: 7265 7320 696e 2074 6865 2066 6561 7475  res in the featu
+00015500: 7265 2067 726f 7570 2061 6e64 2072 6574  re group and ret
+00015510: 7572 6e73 2061 2051 7565 7279 206f 626a  urns a Query obj
+00015520: 6563 740a 2020 2020 2020 2020 6174 2074  ect.        at t
+00015530: 6865 2073 7065 6369 6669 6564 2070 6f69  he specified poi
+00015540: 6e74 2069 6e20 7469 6d65 2e20 4f70 7469  nt in time. Opti
+00015550: 6f6e 616c 6c79 2c20 636f 6d6d 6974 7320  onally, commits 
+00015560: 6265 666f 7265 2061 2073 7065 6369 6669  before a specifi
+00015570: 6564 2070 6f69 6e74 2069 6e20 7469 6d65  ed point in time
+00015580: 2063 616e 2062 650a 2020 2020 2020 2020   can be.        
+00015590: 6578 636c 7564 6564 2066 726f 6d20 7468  excluded from th
+000155a0: 6520 7175 6572 792e 2054 6865 2051 7565  e query. The Que
+000155b0: 7279 2063 616e 2074 6865 6e20 6569 7468  ry can then eith
+000155c0: 6572 2062 6520 7265 6164 2069 6e74 6f20  er be read into 
+000155d0: 6120 4461 7461 6672 616d 650a 2020 2020  a Dataframe.    
+000155e0: 2020 2020 6f72 2075 7365 6420 6675 7274      or used furt
+000155f0: 6865 7220 746f 2070 6572 666f 726d 206a  her to perform j
+00015600: 6f69 6e73 206f 7220 636f 6e73 7472 7563  oins or construc
+00015610: 7420 6120 7472 6169 6e69 6e67 2064 6174  t a training dat
+00015620: 6173 6574 2e0a 0a20 2020 2020 2020 2021  aset...        !
+00015630: 2121 2065 7861 6d70 6c65 2022 5265 6164  !! example "Read
+00015640: 696e 6720 6665 6174 7572 6573 2061 7420  ing features at 
+00015650: 6120 7370 6563 6966 6963 2070 6f69 6e74  a specific point
+00015660: 2069 6e20 7469 6d65 3a22 0a20 2020 2020   in time:".     
+00015670: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
+00015680: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+00015690: 6f6e 6e65 6374 2074 6f20 7468 6520 4665  onnect to the Fe
+000156a0: 6174 7572 6520 5374 6f72 650a 2020 2020  ature Store.    
+000156b0: 2020 2020 2020 2020 6673 203d 202e 2e2e          fs = ...
+000156c0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+000156d0: 6765 7420 7468 6520 4665 6174 7572 6520  get the Feature 
+000156e0: 4772 6f75 7020 696e 7374 616e 6365 0a20  Group instance. 
+000156f0: 2020 2020 2020 2020 2020 2066 6720 3d20             fg = 
+00015700: 6673 2e67 6574 5f6f 725f 6372 6561 7465  fs.get_or_create
+00015710: 5f66 6561 7475 7265 5f67 726f 7570 282e  _feature_group(.
+00015720: 2e2e 290a 0a20 2020 2020 2020 2020 2020  ..)..           
+00015730: 2023 2067 6574 2064 6174 6120 6174 2061   # get data at a
+00015740: 2073 7065 6369 6669 6320 706f 696e 7420   specific point 
+00015750: 696e 2074 696d 6520 616e 6420 7368 6f77  in time and show
+00015760: 2069 740a 2020 2020 2020 2020 2020 2020   it.            
+00015770: 6667 2e61 735f 6f66 2822 3230 3230 2d31  fg.as_of("2020-1
+00015780: 302d 3230 2030 373a 3334 3a31 3122 292e  0-20 07:34:11").
+00015790: 7265 6164 2829 2e73 686f 7728 290a 2020  read().show().  
+000157a0: 2020 2020 2020 2020 2020 6060 600a 0a20            ```.. 
+000157b0: 2020 2020 2020 2021 2121 2065 7861 6d70         !!! examp
+000157c0: 6c65 2022 5265 6164 696e 6720 636f 6d6d  le "Reading comm
+000157d0: 6974 7320 696e 6372 656d 656e 7461 6c6c  its incrementall
+000157e0: 7920 6265 7477 6565 6e20 7370 6563 6966  y between specif
+000157f0: 6965 6420 706f 696e 7473 2069 6e20 7469  ied points in ti
+00015800: 6d65 3a22 0a20 2020 2020 2020 2020 2020  me:".           
+00015810: 2060 6060 7079 7468 6f6e 0a20 2020 2020   ```python.     
+00015820: 2020 2020 2020 2066 672e 6173 5f6f 6628         fg.as_of(
+00015830: 2232 3032 302d 3130 2d32 3020 3037 3a33  "2020-10-20 07:3
+00015840: 343a 3131 222c 2065 7863 6c75 6465 5f75  4:11", exclude_u
+00015850: 6e74 696c 3d22 3230 3230 2d31 302d 3139  ntil="2020-10-19
+00015860: 2030 373a 3334 3a31 3122 292e 7265 6164   07:34:11").read
+00015870: 2829 2e73 686f 7728 290a 2020 2020 2020  ().show().      
+00015880: 2020 2020 2020 6060 600a 0a20 2020 2020        ```..     
+00015890: 2020 2054 6865 2066 6972 7374 2070 6172     The first par
+000158a0: 616d 6574 6572 2069 7320 696e 636c 7573  ameter is inclus
+000158b0: 6976 6520 7768 696c 6520 7468 6520 6c61  ive while the la
+000158c0: 7474 6572 2069 7320 6578 636c 7573 6976  tter is exclusiv
+000158d0: 652e 0a20 2020 2020 2020 2054 6861 7420  e..        That 
+000158e0: 6d65 616e 732c 2069 6e20 6f72 6465 7220  means, in order 
+000158f0: 746f 2071 7565 7279 2061 2073 696e 676c  to query a singl
+00015900: 6520 636f 6d6d 6974 2c20 796f 7520 6e65  e commit, you ne
+00015910: 6564 2074 6f20 7175 6572 7920 7468 6174  ed to query that
+00015920: 2063 6f6d 6d69 7420 7469 6d65 0a20 2020   commit time.   
+00015930: 2020 2020 2061 6e64 2065 7863 6c75 6465       and exclude
+00015940: 2065 7665 7279 7468 696e 6720 6a75 7374   everything just
+00015950: 2062 6566 6f72 6520 7468 6520 636f 6d6d   before the comm
+00015960: 6974 2e0a 0a20 2020 2020 2020 2021 2121  it...        !!!
+00015970: 2065 7861 6d70 6c65 2022 5265 6164 696e   example "Readin
+00015980: 6720 6f6e 6c79 2074 6865 2063 6861 6e67  g only the chang
+00015990: 6573 2066 726f 6d20 6120 7369 6e67 6c65  es from a single
+000159a0: 2063 6f6d 6d69 7422 0a20 2020 2020 2020   commit".       
+000159b0: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
+000159c0: 2020 2020 2020 2020 2020 2066 672e 6173             fg.as
+000159d0: 5f6f 6628 2232 3032 302d 3130 2d32 3020  _of("2020-10-20 
+000159e0: 3037 3a33 313a 3338 222c 2065 7863 6c75  07:31:38", exclu
+000159f0: 6465 5f75 6e74 696c 3d22 3230 3230 2d31  de_until="2020-1
+00015a00: 302d 3230 2030 373a 3331 3a33 3722 292e  0-20 07:31:37").
+00015a10: 7265 6164 2829 2e73 686f 7728 290a 2020  read().show().  
+00015a20: 2020 2020 2020 2020 2020 6060 600a 0a20            ```.. 
+00015a30: 2020 2020 2020 2057 6865 6e20 6e6f 2077         When no w
+00015a40: 616c 6c63 6c6f 636b 5f74 696d 6520 6973  allclock_time is
+00015a50: 2067 6976 656e 2c20 7468 6520 6c61 7465   given, the late
+00015a60: 7374 2073 7461 7465 206f 6620 6665 6174  st state of feat
+00015a70: 7572 6573 2069 7320 7265 7475 726e 6564  ures is returned
+00015a80: 2e20 4f70 7469 6f6e 616c 6c79 2c20 636f  . Optionally, co
+00015a90: 6d6d 6974 7320 6265 666f 7265 0a20 2020  mmits before.   
+00015aa0: 2020 2020 2061 2073 7065 6369 6669 6564       a specified
+00015ab0: 2070 6f69 6e74 2069 6e20 7469 6d65 2063   point in time c
+00015ac0: 616e 2073 7469 6c6c 2062 6520 6578 636c  an still be excl
+00015ad0: 7564 6564 2e0a 0a20 2020 2020 2020 2021  uded...        !
+00015ae0: 2121 2065 7861 6d70 6c65 2022 5265 6164  !! example "Read
+00015af0: 696e 6720 7468 6520 6c61 7465 7374 2073  ing the latest s
+00015b00: 7461 7465 206f 6620 6665 6174 7572 6573  tate of features
+00015b10: 2c20 6578 636c 7564 696e 6720 636f 6d6d  , excluding comm
+00015b20: 6974 7320 6265 666f 7265 2061 2073 7065  its before a spe
+00015b30: 6369 6669 6564 2070 6f69 6e74 2069 6e20  cified point in 
+00015b40: 7469 6d65 3a22 0a20 2020 2020 2020 2020  time:".         
+00015b50: 2020 2060 6060 7079 7468 6f6e 0a20 2020     ```python.   
+00015b60: 2020 2020 2020 2020 2066 672e 6173 5f6f           fg.as_o
+00015b70: 6628 4e6f 6e65 2c20 6578 636c 7564 655f  f(None, exclude_
+00015b80: 756e 7469 6c3d 2232 3032 302d 3130 2d32  until="2020-10-2
+00015b90: 3020 3037 3a33 313a 3338 2229 2e72 6561  0 07:31:38").rea
+00015ba0: 6428 292e 7368 6f77 2829 0a20 2020 2020  d().show().     
+00015bb0: 2020 2020 2020 2060 6060 0a0a 2020 2020         ```..    
+00015bc0: 2020 2020 4e6f 7465 2074 6861 7420 7468      Note that th
+00015bd0: 6520 696e 7465 7276 616c 2077 696c 6c20  e interval will 
+00015be0: 6265 2061 7070 6c69 6564 2074 6f20 616c  be applied to al
+00015bf0: 6c20 6a6f 696e 7320 696e 2074 6865 2071  l joins in the q
+00015c00: 7565 7279 2e0a 2020 2020 2020 2020 4966  uery..        If
+00015c10: 2079 6f75 2077 616e 7420 746f 2071 7565   you want to que
+00015c20: 7279 2064 6966 6665 7265 6e74 2069 6e74  ry different int
+00015c30: 6572 7661 6c73 2066 6f72 2064 6966 6665  ervals for diffe
+00015c40: 7265 6e74 2066 6561 7475 7265 2067 726f  rent feature gro
+00015c50: 7570 7320 696e 0a20 2020 2020 2020 2074  ups in.        t
+00015c60: 6865 2071 7565 7279 2c20 796f 7520 6861  he query, you ha
+00015c70: 7665 2074 6f20 6170 706c 7920 7468 656d  ve to apply them
+00015c80: 2069 6e20 6120 6e65 7374 6564 2066 6173   in a nested fas
+00015c90: 6869 6f6e 3a0a 2020 2020 2020 2020 2121  hion:.        !!
+00015ca0: 2120 6578 616d 706c 650a 2020 2020 2020  ! example.      
+00015cb0: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
+00015cc0: 2020 2020 2020 2020 2020 2020 2320 636f              # co
+00015cd0: 6e6e 6563 7420 746f 2074 6865 2046 6561  nnect to the Fea
+00015ce0: 7475 7265 2053 746f 7265 0a20 2020 2020  ture Store.     
+00015cf0: 2020 2020 2020 2066 7320 3d20 2e2e 2e0a         fs = ....
+00015d00: 0a20 2020 2020 2020 2020 2020 2023 2067  .            # g
+00015d10: 6574 2074 6865 2046 6561 7475 7265 2047  et the Feature G
+00015d20: 726f 7570 2069 6e73 7461 6e63 650a 2020  roup instance.  
+00015d30: 2020 2020 2020 2020 2020 6667 3120 3d20            fg1 = 
+00015d40: 6673 2e67 6574 5f6f 725f 6372 6561 7465  fs.get_or_create
+00015d50: 5f66 6561 7475 7265 5f67 726f 7570 282e  _feature_group(.
+00015d60: 2e2e 290a 2020 2020 2020 2020 2020 2020  ..).            
+00015d70: 6667 3220 3d20 6673 2e67 6574 5f6f 725f  fg2 = fs.get_or_
+00015d80: 6372 6561 7465 5f66 6561 7475 7265 5f67  create_feature_g
+00015d90: 726f 7570 282e 2e2e 290a 0a20 2020 2020  roup(...)..     
+00015da0: 2020 2020 2020 2066 6731 2e73 656c 6563         fg1.selec
+00015db0: 745f 616c 6c28 292e 6173 5f6f 6628 2232  t_all().as_of("2
+00015dc0: 3032 302d 3130 2d32 3022 2c20 6578 636c  020-10-20", excl
+00015dd0: 7564 655f 756e 7469 6c3d 2232 3032 302d  ude_until="2020-
+00015de0: 3130 2d31 3922 290a 2020 2020 2020 2020  10-19").        
+00015df0: 2020 2020 2020 2020 2e6a 6f69 6e28 6667          .join(fg
+00015e00: 322e 7365 6c65 6374 5f61 6c6c 2829 2e61  2.select_all().a
+00015e10: 735f 6f66 2822 3230 3230 2d31 302d 3230  s_of("2020-10-20
+00015e20: 222c 2065 7863 6c75 6465 5f75 6e74 696c  ", exclude_until
+00015e30: 3d22 3230 3230 2d31 302d 3139 2229 290a  ="2020-10-19")).
+00015e40: 2020 2020 2020 2020 2020 2020 6060 600a              ```.
+00015e50: 0a20 2020 2020 2020 2049 6620 696e 7374  .        If inst
+00015e60: 6561 6420 796f 7520 6170 706c 7920 616e  ead you apply an
+00015e70: 6f74 6865 7220 6061 735f 6f66 6020 7365  other `as_of` se
+00015e80: 6c65 6374 696f 6e20 6166 7465 7220 7468  lection after th
+00015e90: 6520 6a6f 696e 2c20 616c 6c0a 2020 2020  e join, all.    
+00015ea0: 2020 2020 6a6f 696e 6564 2066 6561 7475      joined featu
+00015eb0: 7265 2067 726f 7570 7320 7769 6c6c 2062  re groups will b
+00015ec0: 6520 7175 6572 6965 6420 7769 7468 2074  e queried with t
+00015ed0: 6869 7320 696e 7465 7276 616c 3a0a 2020  his interval:.  
+00015ee0: 2020 2020 2020 2121 2120 6578 616d 706c        !!! exampl
+00015ef0: 650a 2020 2020 2020 2020 2020 2020 6060  e.            ``
+00015f00: 6070 7974 686f 6e0a 2020 2020 2020 2020  `python.        
+00015f10: 2020 2020 6667 312e 7365 6c65 6374 5f61      fg1.select_a
+00015f20: 6c6c 2829 2e61 735f 6f66 2822 3230 3230  ll().as_of("2020
+00015f30: 2d31 302d 3230 222c 2065 7863 6c75 6465  -10-20", exclude
+00015f40: 5f75 6e74 696c 3d22 3230 3230 2d31 302d  _until="2020-10-
+00015f50: 3139 2229 2020 2320 6173 5f6f 6620 6973  19")  # as_of is
+00015f60: 206e 6f74 2061 7070 6c69 6564 0a20 2020   not applied.   
+00015f70: 2020 2020 2020 2020 2020 2020 202e 6a6f               .jo
+00015f80: 696e 2866 6732 2e73 656c 6563 745f 616c  in(fg2.select_al
+00015f90: 6c28 292e 6173 5f6f 6628 2232 3032 302d  l().as_of("2020-
+00015fa0: 3130 2d32 3022 2c20 6578 636c 7564 655f  10-20", exclude_
+00015fb0: 756e 7469 6c3d 2232 3032 302d 3130 2d31  until="2020-10-1
+00015fc0: 3522 2929 2020 2320 6173 5f6f 6620 6973  5"))  # as_of is
+00015fd0: 206e 6f74 2061 7070 6c69 6564 0a20 2020   not applied.   
+00015fe0: 2020 2020 2020 2020 2020 2020 202e 6173               .as
+00015ff0: 5f6f 6628 2232 3032 302d 3130 2d32 3022  _of("2020-10-20"
+00016000: 2c20 6578 636c 7564 655f 756e 7469 6c3d  , exclude_until=
+00016010: 2232 3032 302d 3130 2d31 3922 290a 2020  "2020-10-19").  
+00016020: 2020 2020 2020 2020 2020 6060 600a 0a20            ```.. 
+00016030: 2020 2020 2020 2021 2121 2077 6172 6e69         !!! warni
+00016040: 6e67 0a20 2020 2020 2020 2020 2020 2054  ng.            T
+00016050: 6869 7320 6675 6e63 7469 6f6e 206f 6e6c  his function onl
+00016060: 7920 776f 726b 7320 666f 7220 6665 6174  y works for feat
+00016070: 7572 6520 6772 6f75 7073 2077 6974 6820  ure groups with 
+00016080: 7469 6d65 5f74 7261 7665 6c5f 666f 726d  time_travel_form
+00016090: 6174 3d27 4855 4449 272e 0a0a 2020 2020  at='HUDI'...    
+000160a0: 2020 2020 2121 2120 7761 726e 696e 670a      !!! warning.
+000160b0: 2020 2020 2020 2020 2020 2020 4578 636c              Excl
+000160c0: 7564 696e 6720 636f 6d6d 6974 7320 7669  uding commits vi
+000160d0: 6120 6578 636c 7564 655f 756e 7469 6c20  a exclude_until 
+000160e0: 6973 206f 6e6c 7920 706f 7373 6962 6c65  is only possible
+000160f0: 2077 6974 6869 6e20 7468 6520 7261 6e67   within the rang
+00016100: 6520 6f66 2074 6865 2048 7564 6920 6163  e of the Hudi ac
+00016110: 7469 7665 2074 696d 656c 696e 652e 0a20  tive timeline.. 
+00016120: 2020 2020 2020 2020 2020 2042 7920 6465             By de
+00016130: 6661 756c 742c 2048 7564 6920 6b65 6570  fault, Hudi keep
+00016140: 7320 7468 6520 6c61 7374 2032 3020 746f  s the last 20 to
+00016150: 2033 3020 636f 6d6d 6974 7320 696e 2074   30 commits in t
+00016160: 6865 2061 6374 6976 6520 7469 6d65 6c69  he active timeli
+00016170: 6e65 2e0a 2020 2020 2020 2020 2020 2020  ne..            
+00016180: 4966 2079 6f75 206e 6565 6420 746f 206b  If you need to k
+00016190: 6565 7020 6120 6c6f 6e67 6572 2061 6374  eep a longer act
+000161a0: 6976 6520 7469 6d65 6c69 6e65 2c20 796f  ive timeline, yo
+000161b0: 7520 6361 6e20 6f76 6572 7772 6974 6520  u can overwrite 
+000161c0: 7468 6520 6f70 7469 6f6e 733a 0a20 2020  the options:.   
+000161d0: 2020 2020 2020 2020 2060 686f 6f64 6965           `hoodie
+000161e0: 2e6b 6565 702e 6d69 6e2e 636f 6d6d 6974  .keep.min.commit
+000161f0: 7360 2061 6e64 2060 686f 6f64 6965 2e6b  s` and `hoodie.k
+00016200: 6565 702e 6d61 782e 636f 6d6d 6974 7360  eep.max.commits`
+00016210: 0a20 2020 2020 2020 2020 2020 2077 6865  .            whe
+00016220: 6e20 6361 6c6c 696e 6720 7468 6520 6069  n calling the `i
+00016230: 6e73 6572 7428 2960 206d 6574 686f 642e  nsert()` method.
+00016240: 0a0a 2020 2020 2020 2020 2320 4172 6775  ..        # Argu
+00016250: 6d65 6e74 730a 2020 2020 2020 2020 2020  ments.          
+00016260: 2020 7761 6c6c 636c 6f63 6b5f 7469 6d65    wallclock_time
+00016270: 3a20 5265 6164 2064 6174 6120 6173 206f  : Read data as o
+00016280: 6620 7468 6973 2070 6f69 6e74 2069 6e20  f this point in 
+00016290: 7469 6d65 2e20 5374 7269 6e67 7320 7368  time. Strings sh
+000162a0: 6f75 6c64 2062 6520 666f 726d 6174 7465  ould be formatte
+000162b0: 6420 696e 206f 6e65 206f 6620 7468 650a  d in one of the.
+000162c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000162d0: 666f 6c6c 6f77 696e 6720 666f 726d 6174  following format
+000162e0: 7320 6025 592d 256d 2d25 6460 2c20 6025  s `%Y-%m-%d`, `%
+000162f0: 592d 256d 2d25 6420 2548 602c 2060 2559  Y-%m-%d %H`, `%Y
+00016300: 2d25 6d2d 2564 2025 483a 254d 602c 206f  -%m-%d %H:%M`, o
+00016310: 7220 6025 592d 256d 2d25 6420 2548 3a25  r `%Y-%m-%d %H:%
+00016320: 4d3a 2553 602e 0a20 2020 2020 2020 2020  M:%S`..         
+00016330: 2020 2065 7863 6c75 6465 5f75 6e74 696c     exclude_until
+00016340: 3a20 4578 636c 7564 6520 636f 6d6d 6974  : Exclude commit
+00016350: 7320 756e 7469 6c20 7468 6973 2070 6f69  s until this poi
+00016360: 6e74 2069 6e20 7469 6d65 2e20 5374 7269  nt in time. Stri
+00016370: 6e67 2073 686f 756c 6420 6265 2066 6f72  ng should be for
+00016380: 6d61 7474 6564 2069 6e20 6f6e 6520 6f66  matted in one of
+00016390: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
+000163a0: 2020 2020 2066 6f6c 6c6f 7769 6e67 2066       following f
+000163b0: 6f72 6d61 7473 2060 2559 2d25 6d2d 2564  ormats `%Y-%m-%d
+000163c0: 602c 2060 2559 2d25 6d2d 2564 2025 4860  `, `%Y-%m-%d %H`
+000163d0: 2c20 6025 592d 256d 2d25 6420 2548 3a25  , `%Y-%m-%d %H:%
+000163e0: 4d60 2c20 6f72 2060 2559 2d25 6d2d 2564  M`, or `%Y-%m-%d
+000163f0: 2025 483a 254d 3a25 5360 2e0a 0a20 2020   %H:%M:%S`...   
+00016400: 2020 2020 2023 2052 6574 7572 6e73 0a20       # Returns. 
+00016410: 2020 2020 2020 2020 2020 2060 5175 6572             `Quer
+00016420: 7960 2e20 5468 6520 7175 6572 7920 6f62  y`. The query ob
+00016430: 6a65 6374 2077 6974 6820 7468 6520 6170  ject with the ap
+00016440: 706c 6965 6420 7469 6d65 2074 7261 7665  plied time trave
+00016450: 6c20 636f 6e64 6974 696f 6e2e 0a20 2020  l condition..   
+00016460: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00016470: 2072 6574 7572 6e20 7365 6c66 2e73 656c   return self.sel
+00016480: 6563 745f 616c 6c28 292e 6173 5f6f 6628  ect_all().as_of(
+00016490: 7761 6c6c 636c 6f63 6b5f 7469 6d65 2c20  wallclock_time, 
+000164a0: 6578 636c 7564 655f 756e 7469 6c29 0a0a  exclude_until)..
+000164b0: 2020 2020 6465 6620 636f 6d70 7574 655f      def compute_
+000164c0: 7374 6174 6973 7469 6373 280a 2020 2020  statistics(.    
+000164d0: 2020 2020 7365 6c66 2c20 7761 6c6c 636c      self, wallcl
+000164e0: 6f63 6b5f 7469 6d65 3a20 4f70 7469 6f6e  ock_time: Option
+000164f0: 616c 5b55 6e69 6f6e 5b73 7472 2c20 696e  al[Union[str, in
+00016500: 742c 2064 6174 6574 696d 652c 2064 6174  t, datetime, dat
+00016510: 655d 5d20 3d20 4e6f 6e65 0a20 2020 2029  e]] = None.    )
+00016520: 3a0a 2020 2020 2020 2020 2222 2252 6563  :.        """Rec
+00016530: 6f6d 7075 7465 2074 6865 2073 7461 7469  ompute the stati
+00016540: 7374 6963 7320 666f 7220 7468 6520 6665  stics for the fe
+00016550: 6174 7572 6520 6772 6f75 7020 616e 6420  ature group and 
+00016560: 7361 7665 2074 6865 6d20 746f 2074 6865  save them to the
+00016570: 0a20 2020 2020 2020 2066 6561 7475 7265  .        feature
+00016580: 2073 746f 7265 2e0a 0a20 2020 2020 2020   store...       
+00016590: 2053 7461 7469 7374 6963 7320 6172 6520   Statistics are 
+000165a0: 6f6e 6c79 2063 6f6d 7075 7465 6420 666f  only computed fo
+000165b0: 7220 6461 7461 2069 6e20 7468 6520 6f66  r data in the of
+000165c0: 666c 696e 6520 7374 6f72 6167 6520 6f66  fline storage of
+000165d0: 2074 6865 2066 6561 7475 7265 0a20 2020   the feature.   
+000165e0: 2020 2020 2067 726f 7570 2e0a 0a20 2020       group...   
+000165f0: 2020 2020 2023 2041 7267 756d 656e 7473       # Arguments
+00016600: 0a20 2020 2020 2020 2020 2020 2077 616c  .            wal
+00016610: 6c63 6c6f 636b 5f74 696d 653a 2049 6620  lclock_time: If 
+00016620: 7370 6563 6966 6965 6420 7769 6c6c 2072  specified will r
+00016630: 6563 6f6d 7075 7465 2073 7461 7469 7374  ecompute statist
+00016640: 6963 7320 6f6e 0a20 2020 2020 2020 2020  ics on.         
+00016650: 2020 2020 2020 2066 6561 7475 7265 2067         feature g
+00016660: 726f 7570 2061 7320 6f66 2073 7065 6369  roup as of speci
+00016670: 6669 6320 706f 696e 7420 696e 2074 696d  fic point in tim
+00016680: 652e 2049 6620 6e6f 7420 7370 6563 6966  e. If not specif
+00016690: 6965 6420 7468 656e 2077 696c 6c20 636f  ied then will co
+000166a0: 6d70 7574 6520 7374 6174 6973 7469 6373  mpute statistics
+000166b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000166c0: 2061 7320 6f66 206d 6f73 7420 7265 6365   as of most rece
+000166d0: 6e74 2074 696d 6520 6f66 2074 6869 7320  nt time of this 
+000166e0: 6665 6174 7572 6520 6772 6f75 702e 2044  feature group. D
+000166f0: 6566 6175 6c74 7320 746f 2060 4e6f 6e65  efaults to `None
+00016700: 602e 2053 7472 696e 6773 2073 686f 756c  `. Strings shoul
+00016710: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+00016720: 2020 6265 2066 6f72 6d61 7474 6564 2069    be formatted i
+00016730: 6e20 6f6e 6520 6f66 2074 6865 2066 6f6c  n one of the fol
+00016740: 6c6f 7769 6e67 2066 6f72 6d61 7473 2060  lowing formats `
+00016750: 2559 2d25 6d2d 2564 602c 2060 2559 2d25  %Y-%m-%d`, `%Y-%
+00016760: 6d2d 2564 2025 4860 2c20 6025 592d 256d  m-%d %H`, `%Y-%m
+00016770: 2d25 6420 2548 3a25 4d60 2c20 6025 592d  -%d %H:%M`, `%Y-
+00016780: 256d 2d25 6420 2548 3a25 4d3a 2553 602c  %m-%d %H:%M:%S`,
+00016790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000167a0: 206f 7220 6025 592d 256d 2d25 6420 2548   or `%Y-%m-%d %H
+000167b0: 3a25 4d3a 2553 2e25 6660 2e0a 0a20 2020  :%M:%S.%f`...   
+000167c0: 2020 2020 2023 2052 6574 7572 6e73 0a20       # Returns. 
+000167d0: 2020 2020 2020 2020 2020 2060 5374 6174             `Stat
+000167e0: 6973 7469 6373 602e 2054 6865 2073 7461  istics`. The sta
+000167f0: 7469 7374 6963 7320 6d65 7461 6461 7461  tistics metadata
+00016800: 206f 626a 6563 742e 0a0a 2020 2020 2020   object...      
+00016810: 2020 2320 5261 6973 6573 0a20 2020 2020    # Raises.     
+00016820: 2020 2020 2020 2060 6873 6673 2e63 6c69         `hsfs.cli
+00016830: 656e 742e 6578 6365 7074 696f 6e73 2e52  ent.exceptions.R
+00016840: 6573 7441 5049 4572 726f 7260 2e20 556e  estAPIError`. Un
+00016850: 6162 6c65 2074 6f20 7065 7273 6973 7420  able to persist 
+00016860: 7468 6520 7374 6174 6973 7469 6373 2e0a  the statistics..
+00016870: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00016880: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
+00016890: 6973 7469 6373 5f63 6f6e 6669 672e 656e  istics_config.en
+000168a0: 6162 6c65 643a 0a20 2020 2020 2020 2020  abled:.         
+000168b0: 2020 2023 2044 6f6e 2774 2072 6561 6420     # Don't read 
+000168c0: 7468 6520 6461 7461 6672 616d 6520 6865  the dataframe he
+000168d0: 7265 2c20 746f 2061 766f 6964 2074 7269  re, to avoid tri
+000168e0: 6767 6572 696e 6720 6120 7265 6164 206f  ggering a read o
+000168f0: 7065 7261 7469 6f6e 0a20 2020 2020 2020  peration.       
+00016900: 2020 2020 2023 2066 6f72 2074 6865 2050       # for the P
+00016910: 7974 686f 6e20 656e 6769 6e65 2e20 5468  ython engine. Th
+00016920: 6520 5079 7468 6f6e 2065 6e67 696e 6520  e Python engine 
+00016930: 6973 2067 6f69 6e67 2074 6f20 7365 7475  is going to setu
+00016940: 7020 6120 5370 6172 6b20 4a6f 620a 2020  p a Spark Job.  
+00016950: 2020 2020 2020 2020 2020 2320 746f 2075            # to u
+00016960: 7064 6174 6520 7468 6520 7374 6174 6973  pdate the statis
+00016970: 7469 6373 2e0a 0a20 2020 2020 2020 2020  tics...         
+00016980: 2020 2066 675f 636f 6d6d 6974 5f69 6420     fg_commit_id 
+00016990: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+000169a0: 2020 2069 6620 7761 6c6c 636c 6f63 6b5f     if wallclock_
+000169b0: 7469 6d65 2069 7320 6e6f 7420 4e6f 6e65  time is not None
+000169c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000169d0: 2020 2320 5265 7472 6965 7665 2066 6720    # Retrieve fg 
+000169e0: 636f 6d6d 6974 2069 6420 7265 6c61 7465  commit id relate
+000169f0: 6420 746f 2074 6869 7320 7761 6c6c 2063  d to this wall c
+00016a00: 6c6f 636b 2074 696d 6520 616e 6420 7265  lock time and re
+00016a10: 636f 6d70 7574 6520 7374 6174 6973 7469  compute statisti
+00016a20: 6373 2e20 4974 2077 696c 6c20 7468 726f  cs. It will thro
+00016a30: 770a 2020 2020 2020 2020 2020 2020 2020  w.              
+00016a40: 2020 2320 6578 6365 7074 696f 6e20 6966    # exception if
+00016a50: 2069 7473 206e 6f74 2074 696d 6520 7472   its not time tr
+00016a60: 6176 656c 2065 6e61 626c 6564 2066 6561  avel enabled fea
+00016a70: 7475 7265 2067 726f 7570 2e0a 2020 2020  ture group..    
+00016a80: 2020 2020 2020 2020 2020 2020 6667 5f63              fg_c
+00016a90: 6f6d 6d69 745f 6964 203d 205b 0a20 2020  ommit_id = [.   
+00016aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ab0: 2063 6f6d 6d69 745f 6964 0a20 2020 2020   commit_id.     
+00016ac0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00016ad0: 6f72 2063 6f6d 6d69 745f 6964 2069 6e20  or commit_id in 
+00016ae0: 7365 6c66 2e5f 6665 6174 7572 655f 6772  self._feature_gr
+00016af0: 6f75 705f 656e 6769 6e65 2e63 6f6d 6d69  oup_engine.commi
+00016b00: 745f 6465 7461 696c 7328 0a20 2020 2020  t_details(.     
+00016b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b20: 2020 2073 656c 662c 2077 616c 6c63 6c6f     self, wallclo
+00016b30: 636b 5f74 696d 652c 2031 0a20 2020 2020  ck_time, 1.     
+00016b40: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00016b50: 2e6b 6579 7328 290a 2020 2020 2020 2020  .keys().        
+00016b60: 2020 2020 2020 2020 5d5b 305d 0a0a 2020          ][0]..  
+00016b70: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00016b80: 2073 656c 662e 5f73 7461 7469 7374 6963   self._statistic
+00016b90: 735f 656e 6769 6e65 2e63 6f6d 7075 7465  s_engine.compute
+00016ba0: 5f73 7461 7469 7374 6963 7328 0a20 2020  _statistics(.   
+00016bb0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016bc0: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
+00016bd0: 2020 2066 6561 7475 7265 5f67 726f 7570     feature_group
+00016be0: 5f63 6f6d 6d69 745f 6964 3d66 675f 636f  _commit_id=fg_co
+00016bf0: 6d6d 6974 5f69 640a 2020 2020 2020 2020  mmit_id.        
+00016c00: 2020 2020 2020 2020 6966 2066 675f 636f          if fg_co
+00016c10: 6d6d 6974 5f69 6420 6973 206e 6f74 204e  mmit_id is not N
+00016c20: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+00016c30: 2020 2020 656c 7365 204e 6f6e 652c 0a20      else None,. 
+00016c40: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00016c50: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00016c60: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
+00016c70: 7761 726e 280a 2020 2020 2020 2020 2020  warn(.          
+00016c80: 2020 2020 2020 280a 2020 2020 2020 2020        (.        
+00016c90: 2020 2020 2020 2020 2020 2020 2254 6865              "The
+00016ca0: 2073 7461 7469 7374 6963 7320 6172 6520   statistics are 
+00016cb0: 6e6f 7420 656e 6162 6c65 6420 6f66 2066  not enabled of f
+00016cc0: 6561 7475 7265 2067 726f 7570 2060 7b7d  eature group `{}
+00016cd0: 602c 2077 6974 6820 7665 7273 696f 6e22  `, with version"
+00016ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016cf0: 2020 2020 2022 2060 7b7d 602e 204e 6f20       " `{}`. No 
+00016d00: 7374 6174 6973 7469 6373 2063 6f6d 7075  statistics compu
+00016d10: 7465 642e 220a 2020 2020 2020 2020 2020  ted.".          
+00016d20: 2020 2020 2020 292e 666f 726d 6174 2873        ).format(s
+00016d30: 656c 662e 5f6e 616d 652c 2073 656c 662e  elf._name, self.
+00016d40: 5f76 6572 7369 6f6e 292c 0a20 2020 2020  _version),.     
+00016d50: 2020 2020 2020 2020 2020 2075 7469 6c2e             util.
+00016d60: 5374 6f72 6167 6557 6172 6e69 6e67 2c0a  StorageWarning,.
+00016d70: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00016d80: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+00016d90: 2020 2020 6465 6620 6672 6f6d 5f72 6573      def from_res
+00016da0: 706f 6e73 655f 6a73 6f6e 2863 6c73 2c20  ponse_json(cls, 
+00016db0: 6a73 6f6e 5f64 6963 7429 3a0a 2020 2020  json_dict):.    
+00016dc0: 2020 2020 6a73 6f6e 5f64 6563 616d 656c      json_decamel
+00016dd0: 697a 6564 203d 2068 756d 7073 2e64 6563  ized = humps.dec
+00016de0: 616d 656c 697a 6528 6a73 6f6e 5f64 6963  amelize(json_dic
+00016df0: 7429 0a20 2020 2020 2020 2069 6620 6973  t).        if is
+00016e00: 696e 7374 616e 6365 286a 736f 6e5f 6465  instance(json_de
+00016e10: 6361 6d65 6c69 7a65 642c 2064 6963 7429  camelized, dict)
+00016e20: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00016e30: 2022 7479 7065 2220 696e 206a 736f 6e5f   "type" in json_
+00016e40: 6465 6361 6d65 6c69 7a65 643a 0a20 2020  decamelized:.   
+00016e50: 2020 2020 2020 2020 2020 2020 206a 736f               jso
+00016e60: 6e5f 6465 6361 6d65 6c69 7a65 645b 2273  n_decamelized["s
+00016e70: 7472 6561 6d22 5d20 3d20 280a 2020 2020  tream"] = (.    
+00016e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e90: 6a73 6f6e 5f64 6563 616d 656c 697a 6564  json_decamelized
+00016ea0: 5b22 7479 7065 225d 203d 3d20 2273 7472  ["type"] == "str
+00016eb0: 6561 6d46 6561 7475 7265 4772 6f75 7044  eamFeatureGroupD
+00016ec0: 544f 220a 2020 2020 2020 2020 2020 2020  TO".            
+00016ed0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00016ee0: 2020 5f20 3d20 6a73 6f6e 5f64 6563 616d    _ = json_decam
+00016ef0: 656c 697a 6564 2e70 6f70 2822 7479 7065  elized.pop("type
+00016f00: 222c 204e 6f6e 6529 0a20 2020 2020 2020  ", None).       
+00016f10: 2020 2020 206a 736f 6e5f 6465 6361 6d65       json_decame
+00016f20: 6c69 7a65 642e 706f 7028 2276 616c 6964  lized.pop("valid
+00016f30: 6174 696f 6e5f 7479 7065 222c 204e 6f6e  ation_type", Non
+00016f40: 6529 0a20 2020 2020 2020 2020 2020 2072  e).            r
+00016f50: 6574 7572 6e20 636c 7328 2a2a 6a73 6f6e  eturn cls(**json
+00016f60: 5f64 6563 616d 656c 697a 6564 290a 2020  _decamelized).  
+00016f70: 2020 2020 2020 666f 7220 6667 2069 6e20        for fg in 
+00016f80: 6a73 6f6e 5f64 6563 616d 656c 697a 6564  json_decamelized
+00016f90: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00016fa0: 2022 7479 7065 2220 696e 2066 673a 0a20   "type" in fg:. 
+00016fb0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00016fc0: 675b 2273 7472 6561 6d22 5d20 3d20 6667  g["stream"] = fg
+00016fd0: 5b22 7479 7065 225d 203d 3d20 2273 7472  ["type"] == "str
+00016fe0: 6561 6d46 6561 7475 7265 4772 6f75 7044  eamFeatureGroupD
+00016ff0: 544f 220a 2020 2020 2020 2020 2020 2020  TO".            
+00017000: 5f20 3d20 6667 2e70 6f70 2822 7479 7065  _ = fg.pop("type
+00017010: 222c 204e 6f6e 6529 0a20 2020 2020 2020  ", None).       
+00017020: 2020 2020 2066 672e 706f 7028 2276 616c       fg.pop("val
+00017030: 6964 6174 696f 6e5f 7479 7065 222c 204e  idation_type", N
+00017040: 6f6e 6529 0a20 2020 2020 2020 2072 6574  one).        ret
+00017050: 7572 6e20 5b63 6c73 282a 2a66 6729 2066  urn [cls(**fg) f
+00017060: 6f72 2066 6720 696e 206a 736f 6e5f 6465  or fg in json_de
+00017070: 6361 6d65 6c69 7a65 645d 0a0a 2020 2020  camelized]..    
+00017080: 6465 6620 7570 6461 7465 5f66 726f 6d5f  def update_from_
+00017090: 7265 7370 6f6e 7365 5f6a 736f 6e28 7365  response_json(se
+000170a0: 6c66 2c20 6a73 6f6e 5f64 6963 7429 3a0a  lf, json_dict):.
+000170b0: 2020 2020 2020 2020 6a73 6f6e 5f64 6563          json_dec
+000170c0: 616d 656c 697a 6564 203d 2068 756d 7073  amelized = humps
+000170d0: 2e64 6563 616d 656c 697a 6528 6a73 6f6e  .decamelize(json
+000170e0: 5f64 6963 7429 0a20 2020 2020 2020 206a  _dict).        j
+000170f0: 736f 6e5f 6465 6361 6d65 6c69 7a65 645b  son_decamelized[
+00017100: 2273 7472 6561 6d22 5d20 3d20 6a73 6f6e  "stream"] = json
+00017110: 5f64 6563 616d 656c 697a 6564 5b22 7479  _decamelized["ty
+00017120: 7065 225d 203d 3d20 2273 7472 6561 6d46  pe"] == "streamF
+00017130: 6561 7475 7265 4772 6f75 7044 544f 220a  eatureGroupDTO".
+00017140: 2020 2020 2020 2020 5f20 3d20 6a73 6f6e          _ = json
+00017150: 5f64 6563 616d 656c 697a 6564 2e70 6f70  _decamelized.pop
+00017160: 2822 7479 7065 2229 0a20 2020 2020 2020  ("type").       
+00017170: 2073 656c 662e 5f5f 696e 6974 5f5f 282a   self.__init__(*
+00017180: 2a6a 736f 6e5f 6465 6361 6d65 6c69 7a65  *json_decamelize
+00017190: 6429 0a20 2020 2020 2020 2072 6574 7572  d).        retur
+000171a0: 6e20 7365 6c66 0a0a 2020 2020 6465 6620  n self..    def 
+000171b0: 6a73 6f6e 2873 656c 6629 3a0a 2020 2020  json(self):.    
+000171c0: 2020 2020 2222 2247 6574 2073 7065 6369      """Get speci
+000171d0: 6669 6320 4665 6174 7572 6520 4772 6f75  fic Feature Grou
+000171e0: 7020 6d65 7461 6461 7461 2069 6e20 6a73  p metadata in js
+000171f0: 6f6e 2066 6f72 6d61 742e 0a0a 2020 2020  on format...    
+00017200: 2020 2020 2121 2120 6578 616d 706c 650a      !!! example.
+00017210: 2020 2020 2020 2020 2020 2020 6060 6070              ```p
+00017220: 7974 686f 6e0a 2020 2020 2020 2020 2020  ython.          
+00017230: 2020 6667 2e6a 736f 6e28 290a 2020 2020    fg.json().    
+00017240: 2020 2020 2020 2020 6060 600a 2020 2020          ```.    
+00017250: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00017260: 7265 7475 726e 206a 736f 6e2e 6475 6d70  return json.dump
+00017270: 7328 7365 6c66 2c20 636c 733d 7574 696c  s(self, cls=util
+00017280: 2e46 6561 7475 7265 5374 6f72 6545 6e63  .FeatureStoreEnc
+00017290: 6f64 6572 290a 0a20 2020 2064 6566 2074  oder)..    def t
+000172a0: 6f5f 6469 6374 2873 656c 6629 3a0a 2020  o_dict(self):.  
+000172b0: 2020 2020 2020 2222 2247 6574 2073 7472        """Get str
+000172c0: 7563 7475 7265 6420 696e 666f 2061 626f  uctured info abo
+000172d0: 7574 2073 7065 6369 6669 6320 4665 6174  ut specific Feat
+000172e0: 7572 6520 4772 6f75 7020 696e 2070 7974  ure Group in pyt
+000172f0: 686f 6e20 6469 6374 696f 6e61 7279 2066  hon dictionary f
+00017300: 6f72 6d61 742e 0a0a 2020 2020 2020 2020  ormat...        
+00017310: 2121 2120 6578 616d 706c 650a 2020 2020  !!! example.    
+00017320: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
+00017330: 6e0a 2020 2020 2020 2020 2020 2020 2320  n.            # 
+00017340: 636f 6e6e 6563 7420 746f 2074 6865 2046  connect to the F
+00017350: 6561 7475 7265 2053 746f 7265 0a20 2020  eature Store.   
+00017360: 2020 2020 2020 2020 2066 7320 3d20 2e2e           fs = ..
+00017370: 2e0a 0a20 2020 2020 2020 2020 2020 2023  ...            #
+00017380: 2067 6574 2074 6865 2046 6561 7475 7265   get the Feature
+00017390: 2047 726f 7570 2069 6e73 7461 6e63 650a   Group instance.
+000173a0: 2020 2020 2020 2020 2020 2020 6667 203d              fg =
+000173b0: 2066 732e 6765 745f 6f72 5f63 7265 6174   fs.get_or_creat
+000173c0: 655f 6665 6174 7572 655f 6772 6f75 7028  e_feature_group(
+000173d0: 2e2e 2e29 0a0a 2020 2020 2020 2020 2020  ...)..          
+000173e0: 2020 6667 2e74 6f5f 6469 6374 2829 0a20    fg.to_dict(). 
+000173f0: 2020 2020 2020 2020 2020 2060 6060 0a20             ```. 
+00017400: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00017410: 2020 2066 675f 6d65 7461 5f64 6963 7420     fg_meta_dict 
+00017420: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+00017430: 2269 6422 3a20 7365 6c66 2e5f 6964 2c0a  "id": self._id,.
+00017440: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
+00017450: 6522 3a20 7365 6c66 2e5f 6e61 6d65 2c0a  e": self._name,.
+00017460: 2020 2020 2020 2020 2020 2020 2276 6572              "ver
+00017470: 7369 6f6e 223a 2073 656c 662e 5f76 6572  sion": self._ver
+00017480: 7369 6f6e 2c0a 2020 2020 2020 2020 2020  sion,.          
+00017490: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+000174a0: 2073 656c 662e 5f64 6573 6372 6970 7469   self._descripti
+000174b0: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+000174c0: 226f 6e6c 696e 6545 6e61 626c 6564 223a  "onlineEnabled":
+000174d0: 2073 656c 662e 5f6f 6e6c 696e 655f 656e   self._online_en
+000174e0: 6162 6c65 642c 0a20 2020 2020 2020 2020  abled,.         
+000174f0: 2020 2022 7469 6d65 5472 6176 656c 466f     "timeTravelFo
+00017500: 726d 6174 223a 2073 656c 662e 5f74 696d  rmat": self._tim
+00017510: 655f 7472 6176 656c 5f66 6f72 6d61 742c  e_travel_format,
+00017520: 0a20 2020 2020 2020 2020 2020 2022 6665  .            "fe
+00017530: 6174 7572 6573 223a 2073 656c 662e 5f66  atures": self._f
+00017540: 6561 7475 7265 732c 0a20 2020 2020 2020  eatures,.       
+00017550: 2020 2020 2022 6665 6174 7572 6573 746f       "featuresto
+00017560: 7265 4964 223a 2073 656c 662e 5f66 6561  reId": self._fea
+00017570: 7475 7265 5f73 746f 7265 5f69 642c 0a20  ture_store_id,. 
+00017580: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+00017590: 223a 2022 6361 6368 6564 4665 6174 7572  ": "cachedFeatur
+000175a0: 6567 726f 7570 4454 4f22 0a20 2020 2020  egroupDTO".     
+000175b0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+000175c0: 6c66 2e5f 7374 7265 616d 0a20 2020 2020  lf._stream.     
+000175d0: 2020 2020 2020 2065 6c73 6520 2273 7472         else "str
+000175e0: 6561 6d46 6561 7475 7265 4772 6f75 7044  eamFeatureGroupD
+000175f0: 544f 222c 0a20 2020 2020 2020 2020 2020  TO",.           
+00017600: 2022 7374 6174 6973 7469 6373 436f 6e66   "statisticsConf
+00017610: 6967 223a 2073 656c 662e 5f73 7461 7469  ig": self._stati
+00017620: 7374 6963 735f 636f 6e66 6967 2c0a 2020  stics_config,.  
+00017630: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
+00017640: 5469 6d65 223a 2073 656c 662e 6576 656e  Time": self.even
+00017650: 745f 7469 6d65 2c0a 2020 2020 2020 2020  t_time,.        
+00017660: 2020 2020 2265 7870 6563 7461 7469 6f6e      "expectation
+00017670: 5375 6974 6522 3a20 7365 6c66 2e5f 6578  Suite": self._ex
+00017680: 7065 6374 6174 696f 6e5f 7375 6974 652c  pectation_suite,
+00017690: 0a20 2020 2020 2020 2020 2020 2022 7061  .            "pa
+000176a0: 7265 6e74 7322 3a20 7365 6c66 2e5f 7061  rents": self._pa
+000176b0: 7265 6e74 732c 0a20 2020 2020 2020 207d  rents,.        }
+000176c0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000176d0: 2e5f 7374 7265 616d 3a0a 2020 2020 2020  ._stream:.      
+000176e0: 2020 2020 2020 6667 5f6d 6574 615f 6469        fg_meta_di
+000176f0: 6374 5b22 6465 6c74 6153 7472 6561 6d65  ct["deltaStreame
+00017700: 724a 6f62 436f 6e66 225d 203d 2073 656c  rJobConf"] = sel
+00017710: 662e 5f64 656c 7461 7374 7265 616d 6572  f._deltastreamer
+00017720: 5f6a 6f62 636f 6e66 0a20 2020 2020 2020  _jobconf.       
+00017730: 2072 6574 7572 6e20 6667 5f6d 6574 615f   return fg_meta_
+00017740: 6469 6374 0a0a 2020 2020 6465 6620 5f67  dict..    def _g
+00017750: 6574 5f74 6162 6c65 5f6e 616d 6528 7365  et_table_name(se
+00017760: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
+00017770: 7572 6e20 7365 6c66 2e66 6561 7475 7265  urn self.feature
+00017780: 5f73 746f 7265 5f6e 616d 6520 2b20 222e  _store_name + ".
+00017790: 2220 2b20 7365 6c66 2e6e 616d 6520 2b20  " + self.name + 
+000177a0: 225f 2220 2b20 7374 7228 7365 6c66 2e76  "_" + str(self.v
+000177b0: 6572 7369 6f6e 290a 0a20 2020 2064 6566  ersion)..    def
+000177c0: 205f 6765 745f 6f6e 6c69 6e65 5f74 6162   _get_online_tab
+000177d0: 6c65 5f6e 616d 6528 7365 6c66 293a 0a20  le_name(self):. 
+000177e0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000177f0: 6c66 2e6e 616d 6520 2b20 225f 2220 2b20  lf.name + "_" + 
+00017800: 7374 7228 7365 6c66 2e76 6572 7369 6f6e  str(self.version
+00017810: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
+00017820: 0a20 2020 2064 6566 2069 6428 7365 6c66  .    def id(self
+00017830: 293a 0a20 2020 2020 2020 2022 2222 4665  ):.        """Fe
+00017840: 6174 7572 6520 6772 6f75 7020 6964 2e22  ature group id."
+00017850: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+00017860: 6e20 7365 6c66 2e5f 6964 0a0a 2020 2020  n self._id..    
+00017870: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00017880: 6620 6e61 6d65 2873 656c 6629 3a0a 2020  f name(self):.  
+00017890: 2020 2020 2020 2222 224e 616d 6520 6f66        """Name of
+000178a0: 2074 6865 2066 6561 7475 7265 2067 726f   the feature gro
+000178b0: 7570 2e22 2222 0a20 2020 2020 2020 2072  up.""".        r
+000178c0: 6574 7572 6e20 7365 6c66 2e5f 6e61 6d65  eturn self._name
+000178d0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+000178e0: 2020 2020 6465 6620 7665 7273 696f 6e28      def version(
+000178f0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00017900: 2222 5665 7273 696f 6e20 6e75 6d62 6572  ""Version number
+00017910: 206f 6620 7468 6520 6665 6174 7572 6520   of the feature 
+00017920: 6772 6f75 702e 2222 220a 2020 2020 2020  group.""".      
+00017930: 2020 7265 7475 726e 2073 656c 662e 5f76    return self._v
+00017940: 6572 7369 6f6e 0a0a 2020 2020 4070 726f  ersion..    @pro
+00017950: 7065 7274 790a 2020 2020 6465 6620 6465  perty.    def de
+00017960: 7363 7269 7074 696f 6e28 7365 6c66 293a  scription(self):
+00017970: 0a20 2020 2020 2020 2022 2222 4465 7363  .        """Desc
+00017980: 7269 7074 696f 6e20 6f66 2074 6865 2066  ription of the f
+00017990: 6561 7475 7265 2067 726f 7570 2063 6f6e  eature group con
+000179a0: 7465 6e74 732e 2222 220a 2020 2020 2020  tents.""".      
+000179b0: 2020 7265 7475 726e 2073 656c 662e 5f64    return self._d
+000179c0: 6573 6372 6970 7469 6f6e 0a0a 2020 2020  escription..    
+000179d0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+000179e0: 6620 6665 6174 7572 6573 2873 656c 6629  f features(self)
+000179f0: 3a0a 2020 2020 2020 2020 2222 2253 6368  :.        """Sch
+00017a00: 656d 6120 696e 666f 726d 6174 696f 6e2e  ema information.
+00017a10: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00017a20: 726e 2073 656c 662e 5f66 6561 7475 7265  rn self._feature
+00017a30: 730a 0a20 2020 2040 7072 6f70 6572 7479  s..    @property
+00017a40: 0a20 2020 2064 6566 2074 696d 655f 7472  .    def time_tr
+00017a50: 6176 656c 5f66 6f72 6d61 7428 7365 6c66  avel_format(self
+00017a60: 293a 0a20 2020 2020 2020 2022 2222 5365  ):.        """Se
+00017a70: 7474 696e 6720 6f66 2074 6865 2066 6561  tting of the fea
+00017a80: 7475 7265 2067 726f 7570 2074 696d 6520  ture group time 
+00017a90: 7472 6176 656c 2066 6f72 6d61 742e 2222  travel format.""
+00017aa0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+00017ab0: 2073 656c 662e 5f74 696d 655f 7472 6176   self._time_trav
+00017ac0: 656c 5f66 6f72 6d61 740a 0a20 2020 2040  el_format..    @
+00017ad0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00017ae0: 2070 6172 7469 7469 6f6e 5f6b 6579 2873   partition_key(s
+00017af0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00017b00: 224c 6973 7420 6f66 2066 6561 7475 7265  "List of feature
+00017b10: 7320 6275 696c 6469 6e67 2074 6865 2070  s building the p
+00017b20: 6172 7469 7469 6f6e 206b 6579 2e22 2222  artition key."""
+00017b30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00017b40: 7365 6c66 2e5f 7061 7274 6974 696f 6e5f  self._partition_
+00017b50: 6b65 790a 0a20 2020 2040 7072 6f70 6572  key..    @proper
+00017b60: 7479 0a20 2020 2064 6566 2068 7564 695f  ty.    def hudi_
+00017b70: 7072 6563 6f6d 6269 6e65 5f6b 6579 2873  precombine_key(s
+00017b80: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00017b90: 2246 6561 7475 7265 206e 616d 6520 7468  "Feature name th
+00017ba0: 6174 2069 7320 7468 6520 6875 6469 2070  at is the hudi p
+00017bb0: 7265 636f 6d62 696e 6520 6b65 792e 2222  recombine key.""
+00017bc0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+00017bd0: 2073 656c 662e 5f68 7564 695f 7072 6563   self._hudi_prec
+00017be0: 6f6d 6269 6e65 5f6b 6579 0a0a 2020 2020  ombine_key..    
+00017bf0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00017c00: 6620 6665 6174 7572 655f 7374 6f72 655f  f feature_store_
+00017c10: 6964 2873 656c 6629 3a0a 2020 2020 2020  id(self):.      
+00017c20: 2020 7265 7475 726e 2073 656c 662e 5f66    return self._f
+00017c30: 6561 7475 7265 5f73 746f 7265 5f69 640a  eature_store_id.
+00017c40: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00017c50: 2020 2064 6566 2066 6561 7475 7265 5f73     def feature_s
+00017c60: 746f 7265 5f6e 616d 6528 7365 6c66 293a  tore_name(self):
+00017c70: 0a20 2020 2020 2020 2022 2222 4e61 6d65  .        """Name
+00017c80: 206f 6620 7468 6520 6665 6174 7572 6520   of the feature 
+00017c90: 7374 6f72 6520 696e 2077 6869 6368 2074  store in which t
+00017ca0: 6865 2066 6561 7475 7265 2067 726f 7570  he feature group
+00017cb0: 2069 7320 6c6f 6361 7465 642e 2222 220a   is located.""".
+00017cc0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00017cd0: 656c 662e 5f66 6561 7475 7265 5f73 746f  elf._feature_sto
+00017ce0: 7265 5f6e 616d 650a 0a20 2020 2040 7072  re_name..    @pr
+00017cf0: 6f70 6572 7479 0a20 2020 2064 6566 2063  operty.    def c
+00017d00: 7265 6174 6f72 2873 656c 6629 3a0a 2020  reator(self):.  
+00017d10: 2020 2020 2020 2222 2255 7365 726e 616d        """Usernam
+00017d20: 6520 6f66 2074 6865 2063 7265 6174 6f72  e of the creator
+00017d30: 2e22 2222 0a20 2020 2020 2020 2072 6574  .""".        ret
+00017d40: 7572 6e20 7365 6c66 2e5f 6372 6561 746f  urn self._creato
+00017d50: 720a 0a20 2020 2040 7072 6f70 6572 7479  r..    @property
+00017d60: 0a20 2020 2064 6566 2063 7265 6174 6564  .    def created
+00017d70: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00017d80: 2222 2254 696d 6573 7461 6d70 2077 6865  """Timestamp whe
+00017d90: 6e20 7468 6520 6665 6174 7572 6520 6772  n the feature gr
+00017da0: 6f75 7020 7761 7320 6372 6561 7465 642e  oup was created.
+00017db0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00017dc0: 726e 2073 656c 662e 5f63 7265 6174 6564  rn self._created
+00017dd0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+00017de0: 2020 2020 6465 6620 7374 7265 616d 2873      def stream(s
+00017df0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00017e00: 2257 6865 7468 6572 2074 6f20 656e 6162  "Whether to enab
+00017e10: 6c65 2072 6561 6c20 7469 6d65 2073 7472  le real time str
+00017e20: 6561 6d20 7772 6974 696e 6720 6361 7061  eam writing capa
+00017e30: 6269 6c69 7469 6573 2e22 2222 0a20 2020  bilities.""".   
+00017e40: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00017e50: 2e5f 7374 7265 616d 0a0a 2020 2020 4070  ._stream..    @p
+00017e60: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00017e70: 7061 7265 6e74 7328 7365 6c66 293a 0a20  parents(self):. 
+00017e80: 2020 2020 2020 2022 2222 5061 7265 6e74         """Parent
+00017e90: 2066 6561 7475 7265 2067 726f 7570 7320   feature groups 
+00017ea0: 6173 206f 7269 6769 6e20 6f66 2074 6865  as origin of the
+00017eb0: 2064 6174 6120 696e 2074 6865 2063 7572   data in the cur
+00017ec0: 7265 6e74 2066 6561 7475 7265 2067 726f  rent feature gro
+00017ed0: 7570 2e0a 2020 2020 2020 2020 5468 6973  up..        This
+00017ee0: 2069 7320 7061 7274 206f 6620 6578 706c   is part of expl
+00017ef0: 6963 6974 2070 726f 7665 6e61 6e63 6522  icit provenance"
+00017f00: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+00017f10: 6e20 7365 6c66 2e5f 7061 7265 6e74 730a  n self._parents.
+00017f20: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00017f30: 2020 2064 6566 2062 6163 6b66 696c 6c5f     def backfill_
+00017f40: 6a6f 6228 7365 6c66 293a 0a20 2020 2020  job(self):.     
+00017f50: 2020 2022 2222 4765 7420 7468 6520 4a6f     """Get the Jo
+00017f60: 6220 6f62 6a65 6374 2072 6566 6572 656e  b object referen
+00017f70: 6365 2066 6f72 2074 6865 2062 6163 6b66  ce for the backf
+00017f80: 696c 6c20 6a6f 6220 666f 7220 7468 6973  ill job for this
+00017f90: 0a20 2020 2020 2020 2046 6561 7475 7265  .        Feature
+00017fa0: 2047 726f 7570 2e22 2222 0a20 2020 2020   Group.""".     
+00017fb0: 2020 2069 6620 7365 6c66 2e5f 6261 636b     if self._back
+00017fc0: 6669 6c6c 5f6a 6f62 2069 7320 4e6f 6e65  fill_job is None
+00017fd0: 3a0a 2020 2020 2020 2020 2020 2020 6a6f  :.            jo
+00017fe0: 625f 6e61 6d65 203d 2022 7b66 675f 6e61  b_name = "{fg_na
+00017ff0: 6d65 7d5f 7b76 6572 7369 6f6e 7d5f 6f66  me}_{version}_of
+00018000: 666c 696e 655f 6667 5f62 6163 6b66 696c  fline_fg_backfil
+00018010: 6c22 2e66 6f72 6d61 7428 0a20 2020 2020  l".format(.     
+00018020: 2020 2020 2020 2020 2020 2066 675f 6e61             fg_na
+00018030: 6d65 3d73 656c 662e 5f6e 616d 652c 2076  me=self._name, v
+00018040: 6572 7369 6f6e 3d73 656c 662e 5f76 6572  ersion=self._ver
+00018050: 7369 6f6e 0a20 2020 2020 2020 2020 2020  sion.           
+00018060: 2029 0a20 2020 2020 2020 2020 2020 2073   ).            s
+00018070: 656c 662e 5f62 6163 6b66 696c 6c5f 6a6f  elf._backfill_jo
+00018080: 6220 3d20 6a6f 625f 6170 692e 4a6f 6241  b = job_api.JobA
+00018090: 7069 2829 2e67 6574 286a 6f62 5f6e 616d  pi().get(job_nam
+000180a0: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
+000180b0: 6e20 7365 6c66 2e5f 6261 636b 6669 6c6c  n self._backfill
+000180c0: 5f6a 6f62 0a0a 2020 2020 4076 6572 7369  _job..    @versi
+000180d0: 6f6e 2e73 6574 7465 720a 2020 2020 6465  on.setter.    de
+000180e0: 6620 7665 7273 696f 6e28 7365 6c66 2c20  f version(self, 
+000180f0: 7665 7273 696f 6e29 3a0a 2020 2020 2020  version):.      
+00018100: 2020 7365 6c66 2e5f 7665 7273 696f 6e20    self._version 
+00018110: 3d20 7665 7273 696f 6e0a 0a20 2020 2040  = version..    @
+00018120: 6465 7363 7269 7074 696f 6e2e 7365 7474  description.sett
+00018130: 6572 0a20 2020 2064 6566 2064 6573 6372  er.    def descr
+00018140: 6970 7469 6f6e 2873 656c 662c 206e 6577  iption(self, new
+00018150: 5f64 6573 6372 6970 7469 6f6e 293a 0a20  _description):. 
+00018160: 2020 2020 2020 2073 656c 662e 5f64 6573         self._des
+00018170: 6372 6970 7469 6f6e 203d 206e 6577 5f64  cription = new_d
+00018180: 6573 6372 6970 7469 6f6e 0a0a 2020 2020  escription..    
+00018190: 4066 6561 7475 7265 732e 7365 7474 6572  @features.setter
+000181a0: 0a20 2020 2064 6566 2066 6561 7475 7265  .    def feature
+000181b0: 7328 7365 6c66 2c20 6e65 775f 6665 6174  s(self, new_feat
+000181c0: 7572 6573 293a 0a20 2020 2020 2020 2073  ures):.        s
+000181d0: 656c 662e 5f66 6561 7475 7265 7320 3d20  elf._features = 
+000181e0: 6e65 775f 6665 6174 7572 6573 0a0a 2020  new_features..  
+000181f0: 2020 4074 696d 655f 7472 6176 656c 5f66    @time_travel_f
+00018200: 6f72 6d61 742e 7365 7474 6572 0a20 2020  ormat.setter.   
+00018210: 2064 6566 2074 696d 655f 7472 6176 656c   def time_travel
+00018220: 5f66 6f72 6d61 7428 7365 6c66 2c20 6e65  _format(self, ne
+00018230: 775f 7469 6d65 5f74 7261 7665 6c5f 666f  w_time_travel_fo
+00018240: 726d 6174 293a 0a20 2020 2020 2020 2073  rmat):.        s
+00018250: 656c 662e 5f74 696d 655f 7472 6176 656c  elf._time_travel
+00018260: 5f66 6f72 6d61 7420 3d20 6e65 775f 7469  _format = new_ti
+00018270: 6d65 5f74 7261 7665 6c5f 666f 726d 6174  me_travel_format
+00018280: 0a0a 2020 2020 4070 6172 7469 7469 6f6e  ..    @partition
+00018290: 5f6b 6579 2e73 6574 7465 720a 2020 2020  _key.setter.    
+000182a0: 6465 6620 7061 7274 6974 696f 6e5f 6b65  def partition_ke
+000182b0: 7928 7365 6c66 2c20 6e65 775f 7061 7274  y(self, new_part
+000182c0: 6974 696f 6e5f 6b65 7929 3a0a 2020 2020  ition_key):.    
+000182d0: 2020 2020 7365 6c66 2e5f 7061 7274 6974      self._partit
+000182e0: 696f 6e5f 6b65 7920 3d20 5b70 6b2e 6c6f  ion_key = [pk.lo
+000182f0: 7765 7228 2920 666f 7220 706b 2069 6e20  wer() for pk in 
+00018300: 6e65 775f 7061 7274 6974 696f 6e5f 6b65  new_partition_ke
+00018310: 795d 0a0a 2020 2020 4068 7564 695f 7072  y]..    @hudi_pr
+00018320: 6563 6f6d 6269 6e65 5f6b 6579 2e73 6574  ecombine_key.set
+00018330: 7465 720a 2020 2020 6465 6620 6875 6469  ter.    def hudi
+00018340: 5f70 7265 636f 6d62 696e 655f 6b65 7928  _precombine_key(
+00018350: 7365 6c66 2c20 6875 6469 5f70 7265 636f  self, hudi_preco
+00018360: 6d62 696e 655f 6b65 7929 3a0a 2020 2020  mbine_key):.    
+00018370: 2020 2020 7365 6c66 2e5f 6875 6469 5f70      self._hudi_p
+00018380: 7265 636f 6d62 696e 655f 6b65 7920 3d20  recombine_key = 
+00018390: 6875 6469 5f70 7265 636f 6d62 696e 655f  hudi_precombine_
+000183a0: 6b65 792e 6c6f 7765 7228 290a 0a20 2020  key.lower()..   
+000183b0: 2040 7374 7265 616d 2e73 6574 7465 720a   @stream.setter.
+000183c0: 2020 2020 6465 6620 7374 7265 616d 2873      def stream(s
+000183d0: 656c 662c 2073 7472 6561 6d29 3a0a 2020  elf, stream):.  
+000183e0: 2020 2020 2020 7365 6c66 2e5f 7374 7265        self._stre
+000183f0: 616d 203d 2073 7472 6561 6d0a 0a20 2020  am = stream..   
+00018400: 2040 7061 7265 6e74 732e 7365 7474 6572   @parents.setter
+00018410: 0a20 2020 2064 6566 2070 6172 656e 7473  .    def parents
+00018420: 2873 656c 662c 206e 6577 5f70 6172 656e  (self, new_paren
+00018430: 7473 293a 0a20 2020 2020 2020 2073 656c  ts):.        sel
+00018440: 662e 5f70 6172 656e 7473 203d 206e 6577  f._parents = new
+00018450: 5f70 6172 656e 7473 0a0a 0a63 6c61 7373  _parents...class
+00018460: 2045 7874 6572 6e61 6c46 6561 7475 7265   ExternalFeature
+00018470: 4772 6f75 7028 4665 6174 7572 6547 726f  Group(FeatureGro
+00018480: 7570 4261 7365 293a 0a20 2020 2045 5854  upBase):.    EXT
+00018490: 4552 4e41 4c5f 4645 4154 5552 455f 4752  ERNAL_FEATURE_GR
+000184a0: 4f55 5020 3d20 224f 4e5f 4445 4d41 4e44  OUP = "ON_DEMAND
+000184b0: 5f46 4541 5455 5245 5f47 524f 5550 220a  _FEATURE_GROUP".
+000184c0: 2020 2020 454e 5449 5459 5f54 5950 4520      ENTITY_TYPE 
+000184d0: 3d20 2266 6561 7475 7265 6772 6f75 7073  = "featuregroups
+000184e0: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
+000184f0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+00018500: 662c 0a20 2020 2020 2020 2073 746f 7261  f,.        stora
+00018510: 6765 5f63 6f6e 6e65 6374 6f72 2c0a 2020  ge_connector,.  
+00018520: 2020 2020 2020 7175 6572 793d 4e6f 6e65        query=None
+00018530: 2c0a 2020 2020 2020 2020 6461 7461 5f66  ,.        data_f
+00018540: 6f72 6d61 743d 4e6f 6e65 2c0a 2020 2020  ormat=None,.    
+00018550: 2020 2020 7061 7468 3d4e 6f6e 652c 0a20      path=None,. 
+00018560: 2020 2020 2020 206f 7074 696f 6e73 3d7b         options={
+00018570: 7d2c 0a20 2020 2020 2020 206e 616d 653d  },.        name=
+00018580: 4e6f 6e65 2c0a 2020 2020 2020 2020 7665  None,.        ve
+00018590: 7273 696f 6e3d 4e6f 6e65 2c0a 2020 2020  rsion=None,.    
+000185a0: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
+000185b0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7072  None,.        pr
+000185c0: 696d 6172 795f 6b65 793d 4e6f 6e65 2c0a  imary_key=None,.
+000185d0: 2020 2020 2020 2020 6665 6174 7572 6573          features
+000185e0: 746f 7265 5f69 643d 4e6f 6e65 2c0a 2020  tore_id=None,.  
+000185f0: 2020 2020 2020 6665 6174 7572 6573 746f        featuresto
+00018600: 7265 5f6e 616d 653d 4e6f 6e65 2c0a 2020  re_name=None,.  
+00018610: 2020 2020 2020 6372 6561 7465 643d 4e6f        created=No
+00018620: 6e65 2c0a 2020 2020 2020 2020 6372 6561  ne,.        crea
+00018630: 746f 723d 4e6f 6e65 2c0a 2020 2020 2020  tor=None,.      
+00018640: 2020 6964 3d4e 6f6e 652c 0a20 2020 2020    id=None,.     
+00018650: 2020 2066 6561 7475 7265 733d 4e6f 6e65     features=None
+00018660: 2c0a 2020 2020 2020 2020 6c6f 6361 7469  ,.        locati
+00018670: 6f6e 3d4e 6f6e 652c 0a20 2020 2020 2020  on=None,.       
+00018680: 2073 7461 7469 7374 6963 735f 636f 6e66   statistics_conf
+00018690: 6967 3d4e 6f6e 652c 0a20 2020 2020 2020  ig=None,.       
+000186a0: 2065 7665 6e74 5f74 696d 653d 4e6f 6e65   event_time=None
+000186b0: 2c0a 2020 2020 2020 2020 6578 7065 6374  ,.        expect
+000186c0: 6174 696f 6e5f 7375 6974 653d 4e6f 6e65  ation_suite=None
+000186d0: 2c0a 2020 2020 2020 2020 6f6e 6c69 6e65  ,.        online
+000186e0: 5f65 6e61 626c 6564 3d46 616c 7365 2c0a  _enabled=False,.
+000186f0: 2020 2020 2020 2020 6872 6566 3d4e 6f6e          href=Non
+00018700: 652c 0a20 2020 2020 2020 206f 6e6c 696e  e,.        onlin
+00018710: 655f 746f 7069 635f 6e61 6d65 3d4e 6f6e  e_topic_name=Non
+00018720: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+00018730: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
+00018740: 5f5f 280a 2020 2020 2020 2020 2020 2020  __(.            
+00018750: 6665 6174 7572 6573 746f 7265 5f69 642c  featurestore_id,
+00018760: 0a20 2020 2020 2020 2020 2020 206c 6f63  .            loc
+00018770: 6174 696f 6e2c 0a20 2020 2020 2020 2020  ation,.         
+00018780: 2020 2065 7665 6e74 5f74 696d 653d 6576     event_time=ev
+00018790: 656e 745f 7469 6d65 2c0a 2020 2020 2020  ent_time,.      
+000187a0: 2020 2020 2020 6f6e 6c69 6e65 5f65 6e61        online_ena
+000187b0: 626c 6564 3d6f 6e6c 696e 655f 656e 6162  bled=online_enab
+000187c0: 6c65 642c 0a20 2020 2020 2020 2020 2020  led,.           
+000187d0: 2069 643d 6964 2c0a 2020 2020 2020 2020   id=id,.        
+000187e0: 2020 2020 6578 7065 6374 6174 696f 6e5f      expectation_
+000187f0: 7375 6974 653d 6578 7065 6374 6174 696f  suite=expectatio
+00018800: 6e5f 7375 6974 652c 0a20 2020 2020 2020  n_suite,.       
+00018810: 2020 2020 206f 6e6c 696e 655f 746f 7069       online_topi
+00018820: 635f 6e61 6d65 3d6f 6e6c 696e 655f 746f  c_name=online_to
+00018830: 7069 635f 6e61 6d65 2c0a 2020 2020 2020  pic_name,.      
+00018840: 2020 290a 0a20 2020 2020 2020 2073 656c    )..        sel
+00018850: 662e 5f66 6561 7475 7265 5f73 746f 7265  f._feature_store
+00018860: 5f6e 616d 6520 3d20 6665 6174 7572 6573  _name = features
+00018870: 746f 7265 5f6e 616d 650a 2020 2020 2020  tore_name.      
+00018880: 2020 7365 6c66 2e5f 6465 7363 7269 7074    self._descript
+00018890: 696f 6e20 3d20 6465 7363 7269 7074 696f  ion = descriptio
+000188a0: 6e0a 2020 2020 2020 2020 7365 6c66 2e5f  n.        self._
+000188b0: 6372 6561 7465 6420 3d20 6372 6561 7465  created = create
+000188c0: 640a 2020 2020 2020 2020 7365 6c66 2e5f  d.        self._
+000188d0: 6372 6561 746f 7220 3d20 7573 6572 2e55  creator = user.U
+000188e0: 7365 722e 6672 6f6d 5f72 6573 706f 6e73  ser.from_respons
+000188f0: 655f 6a73 6f6e 2863 7265 6174 6f72 290a  e_json(creator).
+00018900: 2020 2020 2020 2020 7365 6c66 2e5f 7665          self._ve
+00018910: 7273 696f 6e20 3d20 7665 7273 696f 6e0a  rsion = version.
+00018920: 2020 2020 2020 2020 7365 6c66 2e5f 6e61          self._na
+00018930: 6d65 203d 206e 616d 650a 2020 2020 2020  me = name.      
+00018940: 2020 7365 6c66 2e5f 7175 6572 7920 3d20    self._query = 
+00018950: 7175 6572 790a 2020 2020 2020 2020 7365  query.        se
+00018960: 6c66 2e5f 6461 7461 5f66 6f72 6d61 7420  lf._data_format 
+00018970: 3d20 6461 7461 5f66 6f72 6d61 742e 7570  = data_format.up
+00018980: 7065 7228 2920 6966 2064 6174 615f 666f  per() if data_fo
+00018990: 726d 6174 2065 6c73 6520 4e6f 6e65 0a20  rmat else None. 
+000189a0: 2020 2020 2020 2073 656c 662e 5f70 6174         self._pat
+000189b0: 6820 3d20 7061 7468 0a0a 2020 2020 2020  h = path..      
+000189c0: 2020 7365 6c66 2e5f 6665 6174 7572 6573    self._features
+000189d0: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+000189e0: 2066 6561 7475 7265 2e46 6561 7475 7265   feature.Feature
+000189f0: 2e66 726f 6d5f 7265 7370 6f6e 7365 5f6a  .from_response_j
+00018a00: 736f 6e28 6665 6174 2920 6966 2069 7369  son(feat) if isi
+00018a10: 6e73 7461 6e63 6528 6665 6174 2c20 6469  nstance(feat, di
+00018a20: 6374 2920 656c 7365 2066 6561 740a 2020  ct) else feat.  
+00018a30: 2020 2020 2020 2020 2020 666f 7220 6665            for fe
+00018a40: 6174 2069 6e20 2866 6561 7475 7265 7320  at in (features 
+00018a50: 6f72 205b 5d29 0a20 2020 2020 2020 205d  or []).        ]
+00018a60: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00018a70: 6665 6174 7572 655f 6772 6f75 705f 656e  feature_group_en
+00018a80: 6769 6e65 203d 2028 0a20 2020 2020 2020  gine = (.       
+00018a90: 2020 2020 2065 7874 6572 6e61 6c5f 6665       external_fe
+00018aa0: 6174 7572 655f 6772 6f75 705f 656e 6769  ature_group_engi
+00018ab0: 6e65 2e45 7874 6572 6e61 6c46 6561 7475  ne.ExternalFeatu
+00018ac0: 7265 4772 6f75 7045 6e67 696e 6528 6665  reGroupEngine(fe
+00018ad0: 6174 7572 6573 746f 7265 5f69 6429 0a20  aturestore_id). 
+00018ae0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00018af0: 2020 6966 2073 656c 662e 5f69 643a 0a20    if self._id:. 
+00018b00: 2020 2020 2020 2020 2020 2023 2047 6f74             # Got
+00018b10: 2066 726f 6d20 486f 7073 776f 726b 732c   from Hopsworks,
+00018b20: 2064 6573 6572 6961 6c69 7a65 2066 6561   deserialize fea
+00018b30: 7475 7265 7320 616e 6420 7374 6f72 6167  tures and storag
+00018b40: 6520 636f 6e6e 6563 746f 720a 2020 2020  e connector.    
+00018b50: 2020 2020 2020 2020 7365 6c66 2e5f 6665          self._fe
+00018b60: 6174 7572 6573 203d 2028 0a20 2020 2020  atures = (.     
+00018b70: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
+00018b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b90: 2066 6561 7475 7265 2e46 6561 7475 7265   feature.Feature
+00018ba0: 2e66 726f 6d5f 7265 7370 6f6e 7365 5f6a  .from_response_j
+00018bb0: 736f 6e28 6665 6174 290a 2020 2020 2020  son(feat).      
+00018bc0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00018bd0: 2069 7369 6e73 7461 6e63 6528 6665 6174   isinstance(feat
+00018be0: 2c20 6469 6374 290a 2020 2020 2020 2020  , dict).        
+00018bf0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00018c00: 2066 6561 740a 2020 2020 2020 2020 2020   feat.          
+00018c10: 2020 2020 2020 2020 2020 666f 7220 6665            for fe
+00018c20: 6174 2069 6e20 6665 6174 7572 6573 0a20  at in features. 
+00018c30: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00018c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018c50: 2069 6620 6665 6174 7572 6573 0a20 2020   if features.   
+00018c60: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00018c70: 6520 4e6f 6e65 0a20 2020 2020 2020 2020  e None.         
+00018c80: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00018c90: 2073 656c 662e 7072 696d 6172 795f 6b65   self.primary_ke
+00018ca0: 7920 3d20 280a 2020 2020 2020 2020 2020  y = (.          
+00018cb0: 2020 2020 2020 5b66 6561 742e 6e61 6d65        [feat.name
+00018cc0: 2066 6f72 2066 6561 7420 696e 2073 656c   for feat in sel
+00018cd0: 662e 5f66 6561 7475 7265 7320 6966 2066  f._features if f
+00018ce0: 6561 742e 7072 696d 6172 7920 6973 2054  eat.primary is T
+00018cf0: 7275 655d 0a20 2020 2020 2020 2020 2020  rue].           
+00018d00: 2020 2020 2069 6620 7365 6c66 2e5f 6665       if self._fe
+00018d10: 6174 7572 6573 0a20 2020 2020 2020 2020  atures.         
+00018d20: 2020 2020 2020 2065 6c73 6520 5b5d 0a20         else []. 
+00018d30: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00018d40: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+00018d50: 6174 6973 7469 6373 5f63 6f6e 6669 6720  atistics_config 
+00018d60: 3d20 7374 6174 6973 7469 6373 5f63 6f6e  = statistics_con
+00018d70: 6669 670a 0a20 2020 2020 2020 2020 2020  fig..           
+00018d80: 2073 656c 662e 5f6f 7074 696f 6e73 203d   self._options =
+00018d90: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00018da0: 2020 207b 6f70 7469 6f6e 5b22 6e61 6d65     {option["name
+00018db0: 225d 3a20 6f70 7469 6f6e 5b22 7661 6c75  "]: option["valu
+00018dc0: 6522 5d20 666f 7220 6f70 7469 6f6e 2069  e"] for option i
+00018dd0: 6e20 6f70 7469 6f6e 737d 0a20 2020 2020  n options}.     
+00018de0: 2020 2020 2020 2020 2020 2069 6620 6f70             if op
+00018df0: 7469 6f6e 730a 2020 2020 2020 2020 2020  tions.          
+00018e00: 2020 2020 2020 656c 7365 204e 6f6e 650a        else None.
+00018e10: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00018e20: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00018e30: 2020 2020 2020 2020 7365 6c66 2e70 7269          self.pri
+00018e40: 6d61 7279 5f6b 6579 203d 2070 7269 6d61  mary_key = prima
+00018e50: 7279 5f6b 6579 0a20 2020 2020 2020 2020  ry_key.         
+00018e60: 2020 2073 656c 662e 7374 6174 6973 7469     self.statisti
+00018e70: 6373 5f63 6f6e 6669 6720 3d20 7374 6174  cs_config = stat
+00018e80: 6973 7469 6373 5f63 6f6e 6669 670a 2020  istics_config.  
+00018e90: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00018ea0: 6665 6174 7572 6573 203d 2066 6561 7475  features = featu
+00018eb0: 7265 730a 2020 2020 2020 2020 2020 2020  res.            
+00018ec0: 7365 6c66 2e5f 6f70 7469 6f6e 7320 3d20  self._options = 
+00018ed0: 6f70 7469 6f6e 730a 0a20 2020 2020 2020  options..       
+00018ee0: 2069 6620 7374 6f72 6167 655f 636f 6e6e   if storage_conn
+00018ef0: 6563 746f 7220 6973 206e 6f74 204e 6f6e  ector is not Non
+00018f00: 6520 616e 6420 6973 696e 7374 616e 6365  e and isinstance
+00018f10: 2873 746f 7261 6765 5f63 6f6e 6e65 6374  (storage_connect
+00018f20: 6f72 2c20 6469 6374 293a 0a20 2020 2020  or, dict):.     
+00018f30: 2020 2020 2020 2073 656c 662e 5f73 746f         self._sto
+00018f40: 7261 6765 5f63 6f6e 6e65 6374 6f72 203d  rage_connector =
+00018f50: 2073 632e 5374 6f72 6167 6543 6f6e 6e65   sc.StorageConne
+00018f60: 6374 6f72 2e66 726f 6d5f 7265 7370 6f6e  ctor.from_respon
+00018f70: 7365 5f6a 736f 6e28 0a20 2020 2020 2020  se_json(.       
+00018f80: 2020 2020 2020 2020 2073 746f 7261 6765           storage
+00018f90: 5f63 6f6e 6e65 6374 6f72 0a20 2020 2020  _connector.     
+00018fa0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00018fb0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00018fc0: 2020 2073 656c 662e 5f73 746f 7261 6765     self._storage
+00018fd0: 5f63 6f6e 6e65 6374 6f72 203d 2073 746f  _connector = sto
+00018fe0: 7261 6765 5f63 6f6e 6e65 6374 6f72 0a0a  rage_connector..
+00018ff0: 2020 2020 2020 2020 7365 6c66 2e5f 6872          self._hr
+00019000: 6566 203d 2068 7265 660a 0a20 2020 2064  ef = href..    d
+00019010: 6566 2073 6176 6528 7365 6c66 293a 0a20  ef save(self):. 
+00019020: 2020 2020 2020 2022 2222 5065 7273 6973         """Persis
+00019030: 7420 7468 6520 6d65 7461 6461 7461 2066  t the metadata f
+00019040: 6f72 2074 6869 7320 6578 7465 726e 616c  or this external
+00019050: 2066 6561 7475 7265 2067 726f 7570 2e0a   feature group..
+00019060: 0a20 2020 2020 2020 2057 6974 686f 7574  .        Without
+00019070: 2063 616c 6c69 6e67 2074 6869 7320 6d65   calling this me
+00019080: 7468 6f64 2c20 796f 7572 2066 6561 7475  thod, your featu
+00019090: 7265 2067 726f 7570 2077 696c 6c20 6f6e  re group will on
+000190a0: 6c79 2065 7869 7374 0a20 2020 2020 2020  ly exist.       
+000190b0: 2069 6e20 796f 7572 2050 7974 686f 6e20   in your Python 
+000190c0: 4b65 726e 656c 2c20 6275 7420 6e6f 7420  Kernel, but not 
+000190d0: 696e 2048 6f70 7377 6f72 6b73 2e0a 0a20  in Hopsworks... 
+000190e0: 2020 2020 2020 2060 6060 7079 7468 6f6e         ```python
+000190f0: 0a20 2020 2020 2020 2071 7565 7279 203d  .        query =
+00019100: 2022 5345 4c45 4354 202a 2046 524f 4d20   "SELECT * FROM 
+00019110: 7361 6c65 7322 0a0a 2020 2020 2020 2020  sales"..        
+00019120: 6667 203d 2066 6561 7475 7265 5f73 746f  fg = feature_sto
+00019130: 7265 2e63 7265 6174 655f 6578 7465 726e  re.create_extern
+00019140: 616c 5f66 6561 7475 7265 5f67 726f 7570  al_feature_group
+00019150: 286e 616d 653d 2273 616c 6573 222c 0a20  (name="sales",. 
+00019160: 2020 2020 2020 2020 2020 2076 6572 7369             versi
+00019170: 6f6e 3d31 2c0a 2020 2020 2020 2020 2020  on=1,.          
+00019180: 2020 6465 7363 7269 7074 696f 6e3d 2250    description="P
+00019190: 6879 7369 6361 6c20 7368 6f70 2073 616c  hysical shop sal
+000191a0: 6573 2066 6561 7475 7265 7322 2c0a 2020  es features",.  
+000191b0: 2020 2020 2020 2020 2020 7175 6572 793d            query=
+000191c0: 7175 6572 792c 0a20 2020 2020 2020 2020  query,.         
+000191d0: 2020 2073 746f 7261 6765 5f63 6f6e 6e65     storage_conne
+000191e0: 6374 6f72 3d63 6f6e 6e65 6374 6f72 2c0a  ctor=connector,.
+000191f0: 2020 2020 2020 2020 2020 2020 7072 696d              prim
+00019200: 6172 795f 6b65 793d 5b27 7373 5f73 746f  ary_key=['ss_sto
+00019210: 7265 5f73 6b27 5d2c 0a20 2020 2020 2020  re_sk'],.       
+00019220: 2020 2020 2065 7665 6e74 5f74 696d 653d       event_time=
+00019230: 2773 616c 655f 6461 7465 270a 2020 2020  'sale_date'.    
+00019240: 2020 2020 290a 0a20 2020 2020 2020 2066      )..        f
+00019250: 672e 7361 7665 2829 0a20 2020 2020 2020  g.save().       
+00019260: 2022 2222 0a20 2020 2020 2020 2073 656c   """.        sel
+00019270: 662e 5f66 6561 7475 7265 5f67 726f 7570  f._feature_group
+00019280: 5f65 6e67 696e 652e 7361 7665 2873 656c  _engine.save(sel
+00019290: 6629 0a20 2020 2020 2020 2073 656c 662e  f).        self.
+000192a0: 5f63 6f64 655f 656e 6769 6e65 2e73 6176  _code_engine.sav
+000192b0: 655f 636f 6465 2873 656c 6629 0a0a 2020  e_code(self)..  
+000192c0: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
+000192d0: 6174 6973 7469 6373 5f63 6f6e 6669 672e  atistics_config.
+000192e0: 656e 6162 6c65 643a 0a20 2020 2020 2020  enabled:.       
+000192f0: 2020 2020 2073 656c 662e 5f73 7461 7469       self._stati
+00019300: 7374 6963 735f 656e 6769 6e65 2e63 6f6d  stics_engine.com
+00019310: 7075 7465 5f73 7461 7469 7374 6963 7328  pute_statistics(
+00019320: 7365 6c66 290a 0a20 2020 2064 6566 2069  self)..    def i
+00019330: 6e73 6572 7428 0a20 2020 2020 2020 2073  nsert(.        s
+00019340: 656c 662c 0a20 2020 2020 2020 2066 6561  elf,.        fea
+00019350: 7475 7265 733a 2055 6e69 6f6e 5b0a 2020  tures: Union[.  
+00019360: 2020 2020 2020 2020 2020 7064 2e44 6174            pd.Dat
+00019370: 6146 7261 6d65 2c0a 2020 2020 2020 2020  aFrame,.        
+00019380: 2020 2020 5479 7065 5661 7228 2270 7973      TypeVar("pys
+00019390: 7061 726b 2e73 716c 2e44 6174 6146 7261  park.sql.DataFra
+000193a0: 6d65 2229 2c20 2023 206e 6f71 613a 2046  me"),  # noqa: F
+000193b0: 3832 310a 2020 2020 2020 2020 2020 2020  821.            
+000193c0: 5479 7065 5661 7228 2270 7973 7061 726b  TypeVar("pyspark
+000193d0: 2e52 4444 2229 2c20 2023 206e 6f71 613a  .RDD"),  # noqa:
+000193e0: 2046 3832 310a 2020 2020 2020 2020 2020   F821.          
+000193f0: 2020 6e70 2e6e 6461 7272 6179 2c0a 2020    np.ndarray,.  
+00019400: 2020 2020 2020 2020 2020 4c69 7374 5b6c            List[l
+00019410: 6973 745d 2c0a 2020 2020 2020 2020 5d2c  ist],.        ],
+00019420: 0a20 2020 2020 2020 2077 7269 7465 5f6f  .        write_o
+00019430: 7074 696f 6e73 3a20 4f70 7469 6f6e 616c  ptions: Optional
+00019440: 5b44 6963 745b 7374 722c 2041 6e79 5d5d  [Dict[str, Any]]
+00019450: 203d 207b 7d2c 0a20 2020 2020 2020 2076   = {},.        v
+00019460: 616c 6964 6174 696f 6e5f 6f70 7469 6f6e  alidation_option
+00019470: 733a 204f 7074 696f 6e61 6c5b 4469 6374  s: Optional[Dict
+00019480: 5b73 7472 2c20 416e 795d 5d20 3d20 7b7d  [str, Any]] = {}
+00019490: 2c0a 2020 2020 2020 2020 7361 7665 5f63  ,.        save_c
+000194a0: 6f64 653a 204f 7074 696f 6e61 6c5b 626f  ode: Optional[bo
+000194b0: 6f6c 5d20 3d20 5472 7565 2c0a 2020 2020  ol] = True,.    
+000194c0: 2920 2d3e 2054 7570 6c65 5b4f 7074 696f  ) -> Tuple[Optio
+000194d0: 6e61 6c5b 4a6f 625d 2c20 4f70 7469 6f6e  nal[Job], Option
+000194e0: 616c 5b56 616c 6964 6174 696f 6e52 6570  al[ValidationRep
+000194f0: 6f72 745d 5d3a 0a20 2020 2020 2020 2066  ort]]:.        f
+00019500: 6561 7475 7265 5f64 6174 6166 7261 6d65  eature_dataframe
+00019510: 203d 2065 6e67 696e 652e 6765 745f 696e   = engine.get_in
+00019520: 7374 616e 6365 2829 2e63 6f6e 7665 7274  stance().convert
+00019530: 5f74 6f5f 6465 6661 756c 745f 6461 7461  _to_default_data
+00019540: 6672 616d 6528 6665 6174 7572 6573 290a  frame(features).
+00019550: 0a20 2020 2020 2020 206a 6f62 2c20 6765  .        job, ge
+00019560: 5f72 6570 6f72 7420 3d20 7365 6c66 2e5f  _report = self._
+00019570: 6665 6174 7572 655f 6772 6f75 705f 656e  feature_group_en
+00019580: 6769 6e65 2e69 6e73 6572 7428 0a20 2020  gine.insert(.   
+00019590: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
+000195a0: 2020 2020 2020 2020 2020 2066 6561 7475             featu
+000195b0: 7265 5f64 6174 6166 7261 6d65 3d66 6561  re_dataframe=fea
+000195c0: 7475 7265 5f64 6174 6166 7261 6d65 2c0a  ture_dataframe,.
+000195d0: 2020 2020 2020 2020 2020 2020 7772 6974              writ
+000195e0: 655f 6f70 7469 6f6e 733d 7772 6974 655f  e_options=write_
+000195f0: 6f70 7469 6f6e 732c 0a20 2020 2020 2020  options,.       
+00019600: 2020 2020 2076 616c 6964 6174 696f 6e5f       validation_
+00019610: 6f70 7469 6f6e 733d 7b22 7361 7665 5f72  options={"save_r
+00019620: 6570 6f72 7422 3a20 5472 7565 2c20 2a2a  eport": True, **
+00019630: 7661 6c69 6461 7469 6f6e 5f6f 7074 696f  validation_optio
+00019640: 6e73 7d2c 0a20 2020 2020 2020 2029 0a0a  ns},.        )..
+00019650: 2020 2020 2020 2020 6966 2073 6176 655f          if save_
+00019660: 636f 6465 2061 6e64 2028 0a20 2020 2020  code and (.     
+00019670: 2020 2020 2020 2067 655f 7265 706f 7274         ge_report
+00019680: 2069 7320 4e6f 6e65 206f 7220 6765 5f72   is None or ge_r
+00019690: 6570 6f72 742e 696e 6765 7374 696f 6e5f  eport.ingestion_
+000196a0: 7265 7375 6c74 203d 3d20 2249 4e47 4553  result == "INGES
+000196b0: 5445 4422 0a20 2020 2020 2020 2029 3a0a  TED".        ):.
+000196c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000196d0: 2e5f 636f 6465 5f65 6e67 696e 652e 7361  ._code_engine.sa
+000196e0: 7665 5f63 6f64 6528 7365 6c66 290a 0a20  ve_code(self).. 
+000196f0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+00019700: 7461 7469 7374 6963 735f 636f 6e66 6967  tatistics_config
+00019710: 2e65 6e61 626c 6564 3a0a 2020 2020 2020  .enabled:.      
+00019720: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
+00019730: 6172 6e28 0a20 2020 2020 2020 2020 2020  arn(.           
+00019740: 2020 2020 2028 0a20 2020 2020 2020 2020       (.         
+00019750: 2020 2020 2020 2020 2020 2022 5374 6174             "Stat
+00019760: 6973 7469 6373 2061 7265 206e 6f74 2063  istics are not c
+00019770: 6f6d 7075 7465 6420 666f 7220 696e 7365  omputed for inse
+00019780: 7274 696f 6e20 746f 206f 6e6c 696e 6520  rtion to online 
+00019790: 656e 6162 6c65 6420 6578 7465 726e 616c  enabled external
+000197a0: 2066 6561 7475 7265 2067 726f 7570 2060   feature group `
+000197b0: 7b7d 602c 2077 6974 6820 7665 7273 696f  {}`, with versio
+000197c0: 6e22 0a20 2020 2020 2020 2020 2020 2020  n".             
+000197d0: 2020 2020 2020 2022 2060 7b7d 602e 2043         " `{}`. C
+000197e0: 616c 6c20 6063 6f6d 7075 7465 5f73 7461  all `compute_sta
+000197f0: 7469 7374 6963 7360 2065 7870 6c69 6369  tistics` explici
+00019800: 746c 7920 746f 2063 6f6d 7075 7465 2073  tly to compute s
+00019810: 7461 7469 7374 6963 7320 6f76 6572 2074  tatistics over t
+00019820: 6865 2064 6174 6120 696e 2074 6865 2065  he data in the e
+00019830: 7874 6572 6e61 6c20 7374 6f72 6167 6520  xternal storage 
+00019840: 7379 7374 656d 2e22 0a20 2020 2020 2020  system.".       
+00019850: 2020 2020 2020 2020 2029 2e66 6f72 6d61           ).forma
+00019860: 7428 7365 6c66 2e5f 6e61 6d65 2c20 7365  t(self._name, se
+00019870: 6c66 2e5f 7665 7273 696f 6e29 2c0a 2020  lf._version),.  
+00019880: 2020 2020 2020 2020 2020 2020 2020 7574                ut
+00019890: 696c 2e53 746f 7261 6765 5761 726e 696e  il.StorageWarnin
+000198a0: 672c 0a20 2020 2020 2020 2020 2020 2029  g,.            )
+000198b0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000198c0: 2028 0a20 2020 2020 2020 2020 2020 206a   (.            j
+000198d0: 6f62 2c0a 2020 2020 2020 2020 2020 2020  ob,.            
+000198e0: 6765 5f72 6570 6f72 742e 746f 5f67 655f  ge_report.to_ge_
+000198f0: 7479 7065 2829 2069 6620 6765 5f72 6570  type() if ge_rep
+00019900: 6f72 7420 6973 206e 6f74 204e 6f6e 6520  ort is not None 
+00019910: 656c 7365 204e 6f6e 652c 0a20 2020 2020  else None,.     
+00019920: 2020 2029 0a0a 2020 2020 6465 6620 7265     )..    def re
+00019930: 6164 280a 2020 2020 2020 2020 7365 6c66  ad(.        self
+00019940: 2c20 6461 7461 6672 616d 655f 7479 7065  , dataframe_type
+00019950: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00019960: 3d20 2264 6566 6175 6c74 222c 206f 6e6c  = "default", onl
+00019970: 696e 653a 204f 7074 696f 6e61 6c5b 626f  ine: Optional[bo
+00019980: 6f6c 5d20 3d20 4661 6c73 650a 2020 2020  ol] = False.    
+00019990: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
+000199a0: 7420 7468 6520 6665 6174 7572 6520 6772  t the feature gr
+000199b0: 6f75 7020 6173 2061 2044 6174 6146 7261  oup as a DataFra
+000199c0: 6d65 2e0a 0a20 2020 2020 2020 2021 2121  me...        !!!
+000199d0: 2065 7861 6d70 6c65 0a20 2020 2020 2020   example.       
+000199e0: 2020 2020 2060 6060 7079 7468 6f6e 0a20       ```python. 
+000199f0: 2020 2020 2020 2020 2020 2023 2063 6f6e             # con
+00019a00: 6e65 6374 2074 6f20 7468 6520 4665 6174  nect to the Feat
+00019a10: 7572 6520 5374 6f72 650a 2020 2020 2020  ure Store.      
+00019a20: 2020 2020 2020 6673 203d 202e 2e2e 0a0a        fs = .....
+00019a30: 2020 2020 2020 2020 2020 2020 2320 6765              # ge
+00019a40: 7420 7468 6520 4665 6174 7572 6520 4772  t the Feature Gr
+00019a50: 6f75 7020 696e 7374 616e 6365 0a20 2020  oup instance.   
+00019a60: 2020 2020 2020 2020 2066 6720 3d20 6673           fg = fs
+00019a70: 2e67 6574 5f6f 725f 6372 6561 7465 5f66  .get_or_create_f
+00019a80: 6561 7475 7265 5f67 726f 7570 282e 2e2e  eature_group(...
+00019a90: 290a 0a20 2020 2020 2020 2020 2020 2064  )..            d
+00019aa0: 6620 3d20 6667 2e72 6561 6428 290a 2020  f = fg.read().  
+00019ab0: 2020 2020 2020 2020 2020 6060 600a 0a20            ```.. 
+00019ac0: 2020 2020 2020 2021 2121 2077 6172 6e69         !!! warni
+00019ad0: 6e67 2022 456e 6769 6e65 2053 7570 706f  ng "Engine Suppo
+00019ae0: 7274 220a 2020 2020 2020 2020 2020 2020  rt".            
+00019af0: 2a2a 5370 6172 6b20 6f6e 6c79 2a2a 0a0a  **Spark only**..
+00019b00: 2020 2020 2020 2020 2020 2020 5265 6164              Read
+00019b10: 696e 6720 616e 2045 7874 6572 6e61 6c20  ing an External 
+00019b20: 4665 6174 7572 6520 4772 6f75 7020 6469  Feature Group di
+00019b30: 7265 6374 6c79 2069 6e74 6f20 6120 5061  rectly into a Pa
+00019b40: 6e64 6173 2044 6174 6166 7261 6d65 2075  ndas Dataframe u
+00019b50: 7369 6e67 0a20 2020 2020 2020 2020 2020  sing.           
+00019b60: 2050 7974 686f 6e2f 5061 6e64 6173 2061   Python/Pandas a
+00019b70: 7320 456e 6769 6e65 2069 7320 6e6f 7420  s Engine is not 
+00019b80: 7375 7070 6f72 7465 642c 2068 6f77 6576  supported, howev
+00019b90: 6572 2c20 796f 7520 6361 6e20 7573 6520  er, you can use 
+00019ba0: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+00019bb0: 5175 6572 7920 4150 4920 746f 2063 7265  Query API to cre
+00019bc0: 6174 6520 4665 6174 7572 6520 5669 6577  ate Feature View
+00019bd0: 732f 5472 6169 6e69 6e67 2044 6174 6120  s/Training Data 
+00019be0: 636f 6e74 6169 6e69 6e67 2045 7874 6572  containing Exter
+00019bf0: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
+00019c00: 4665 6174 7572 6520 4772 6f75 7073 2e0a  Feature Groups..
+00019c10: 0a20 2020 2020 2020 2023 2041 7267 756d  .        # Argum
+00019c20: 656e 7473 0a20 2020 2020 2020 2020 2020  ents.           
+00019c30: 2064 6174 6166 7261 6d65 5f74 7970 653a   dataframe_type:
+00019c40: 2073 7472 2c20 6f70 7469 6f6e 616c 2e20   str, optional. 
+00019c50: 506f 7373 6962 6c65 2076 616c 7565 7320  Possible values 
+00019c60: 6172 6520 6022 6465 6661 756c 7422 602c  are `"default"`,
+00019c70: 2060 2273 7061 726b 2260 2c0a 2020 2020   `"spark"`,.    
+00019c80: 2020 2020 2020 2020 2020 2020 6022 7061              `"pa
+00019c90: 6e64 6173 2260 2c20 6022 6e75 6d70 7922  ndas"`, `"numpy"
+00019ca0: 6020 6f72 2060 2270 7974 686f 6e22 602c  ` or `"python"`,
+00019cb0: 2064 6566 6175 6c74 7320 746f 2060 2264   defaults to `"d
+00019cc0: 6566 6175 6c74 2260 2e0a 2020 2020 2020  efault"`..      
+00019cd0: 2020 2020 2020 6f6e 6c69 6e65 3a20 626f        online: bo
+00019ce0: 6f6c 2c20 6f70 7469 6f6e 616c 2e20 4966  ol, optional. If
+00019cf0: 2060 5472 7565 6020 7265 6164 2066 726f   `True` read fro
+00019d00: 6d20 6f6e 6c69 6e65 2066 6561 7475 7265  m online feature
+00019d10: 2073 746f 7265 2c20 6465 6661 756c 7473   store, defaults
+00019d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019d30: 2074 6f20 6046 616c 7365 602e 0a0a 2020   to `False`...  
+00019d40: 2020 2020 2020 2320 5265 7475 726e 730a        # Returns.
+00019d50: 2020 2020 2020 2020 2020 2020 6044 6174              `Dat
+00019d60: 6146 7261 6d65 603a 2054 6865 2073 7061  aFrame`: The spa
+00019d70: 726b 2064 6174 6166 7261 6d65 2063 6f6e  rk dataframe con
+00019d80: 7461 696e 696e 6720 7468 6520 6665 6174  taining the feat
+00019d90: 7572 6520 6461 7461 2e0a 2020 2020 2020  ure data..      
+00019da0: 2020 2020 2020 6070 7973 7061 726b 2e44        `pyspark.D
+00019db0: 6174 6146 7261 6d65 602e 2041 2053 7061  ataFrame`. A Spa
+00019dc0: 726b 2044 6174 6146 7261 6d65 2e0a 2020  rk DataFrame..  
+00019dd0: 2020 2020 2020 2020 2020 6070 616e 6461            `panda
+00019de0: 732e 4461 7461 4672 616d 6560 2e20 4120  s.DataFrame`. A 
+00019df0: 5061 6e64 6173 2044 6174 6146 7261 6d65  Pandas DataFrame
+00019e00: 2e0a 2020 2020 2020 2020 2020 2020 606e  ..            `n
+00019e10: 756d 7079 2e6e 6461 7272 6179 602e 2041  umpy.ndarray`. A
+00019e20: 2074 776f 2d64 696d 656e 7369 6f6e 616c   two-dimensional
+00019e30: 204e 756d 7079 2061 7272 6179 2e0a 2020   Numpy array..  
+00019e40: 2020 2020 2020 2020 2020 606c 6973 7460            `list`
+00019e50: 2e20 4120 7477 6f2d 6469 6d65 6e73 696f  . A two-dimensio
+00019e60: 6e61 6c20 5079 7468 6f6e 206c 6973 742e  nal Python list.
+00019e70: 0a0a 2020 2020 2020 2020 2320 5261 6973  ..        # Rais
+00019e80: 6573 0a20 2020 2020 2020 2020 2020 2060  es.            `
+00019e90: 6873 6673 2e63 6c69 656e 742e 6578 6365  hsfs.client.exce
+00019ea0: 7074 696f 6e73 2e52 6573 7441 5049 4572  ptions.RestAPIEr
+00019eb0: 726f 7260 2e0a 2020 2020 2020 2020 2222  ror`..        ""
+00019ec0: 220a 2020 2020 2020 2020 6966 2065 6e67  ".        if eng
+00019ed0: 696e 652e 6765 745f 7479 7065 2829 203d  ine.get_type() =
+00019ee0: 3d20 2270 7974 686f 6e22 2061 6e64 206e  = "python" and n
+00019ef0: 6f74 206f 6e6c 696e 653a 0a20 2020 2020  ot online:.     
+00019f00: 2020 2020 2020 2072 6169 7365 2046 6561         raise Fea
+00019f10: 7475 7265 5374 6f72 6545 7863 6570 7469  tureStoreExcepti
+00019f20: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+00019f30: 2020 2020 2252 6561 6469 6e67 2061 6e20      "Reading an 
+00019f40: 4578 7465 726e 616c 2046 6561 7475 7265  External Feature
+00019f50: 2047 726f 7570 2064 6972 6563 746c 7920   Group directly 
+00019f60: 696e 746f 2061 2050 616e 6461 7320 4461  into a Pandas Da
+00019f70: 7461 6672 616d 6520 7573 696e 6720 220a  taframe using ".
+00019f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019f90: 2b20 2250 7974 686f 6e2f 5061 6e64 6173  + "Python/Pandas
+00019fa0: 2061 7320 456e 6769 6e65 2066 726f 6d20   as Engine from 
+00019fb0: 7468 6520 6578 7465 726e 616c 2073 746f  the external sto
+00019fc0: 7261 6765 2073 7973 7465 6d20 220a 2020  rage system ".  
+00019fd0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+00019fe0: 2269 7320 6e6f 7420 7375 7070 6f72 7465  "is not supporte
+00019ff0: 642c 2068 6f77 6576 6572 2c20 6966 2074  d, however, if t
+0001a000: 6865 2066 6561 7475 7265 2067 726f 7570  he feature group
+0001a010: 2069 7320 6f6e 6c69 6e65 2065 6e61 626c   is online enabl
+0001a020: 6564 2c20 796f 7520 6361 6e20 7265 6164  ed, you can read
+0001a030: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+0001a040: 2020 202b 2022 6672 6f6d 206f 6e6c 696e     + "from onlin
+0001a050: 6520 7374 6f72 6167 6520 6f72 2079 6f75  e storage or you
+0001a060: 2063 616e 2075 7365 2074 6865 2022 0a20   can use the ". 
+0001a070: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+0001a080: 2022 5175 6572 7920 4150 4920 746f 2063   "Query API to c
+0001a090: 7265 6174 6520 4665 6174 7572 6520 5669  reate Feature Vi
+0001a0a0: 6577 732f 5472 6169 6e69 6e67 2044 6174  ews/Training Dat
+0001a0b0: 6120 636f 6e74 6169 6e69 6e67 2045 7874  a containing Ext
+0001a0c0: 6572 6e61 6c20 220a 2020 2020 2020 2020  ernal ".        
+0001a0d0: 2020 2020 2020 2020 2b20 2246 6561 7475          + "Featu
+0001a0e0: 7265 2047 726f 7570 732e 220a 2020 2020  re Groups.".    
+0001a0f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0001a100: 2020 656e 6769 6e65 2e67 6574 5f69 6e73    engine.get_ins
+0001a110: 7461 6e63 6528 292e 7365 745f 6a6f 625f  tance().set_job_
+0001a120: 6772 6f75 7028 0a20 2020 2020 2020 2020  group(.         
+0001a130: 2020 2022 4665 7463 6869 6e67 2046 6561     "Fetching Fea
+0001a140: 7475 7265 2067 726f 7570 222c 0a20 2020  ture group",.   
+0001a150: 2020 2020 2020 2020 2022 4765 7474 696e           "Gettin
+0001a160: 6720 6665 6174 7572 6520 6772 6f75 703a  g feature group:
+0001a170: 207b 7d20 6672 6f6d 2074 6865 2066 6561   {} from the fea
+0001a180: 7475 7265 7374 6f72 6520 7b7d 222e 666f  turestore {}".fo
+0001a190: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
+0001a1a0: 2020 2020 2020 7365 6c66 2e5f 6e61 6d65        self._name
+0001a1b0: 2c20 7365 6c66 2e5f 6665 6174 7572 655f  , self._feature_
+0001a1c0: 7374 6f72 655f 6e61 6d65 0a20 2020 2020  store_name.     
+0001a1d0: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+0001a1e0: 2020 290a 2020 2020 2020 2020 7265 7475    ).        retu
+0001a1f0: 726e 2073 656c 662e 7365 6c65 6374 5f61  rn self.select_a
+0001a200: 6c6c 2829 2e72 6561 6428 6461 7461 6672  ll().read(datafr
+0001a210: 616d 655f 7479 7065 3d64 6174 6166 7261  ame_type=datafra
+0001a220: 6d65 5f74 7970 652c 206f 6e6c 696e 653d  me_type, online=
+0001a230: 6f6e 6c69 6e65 290a 0a20 2020 2064 6566  online)..    def
+0001a240: 2073 686f 7728 7365 6c66 2c20 6e29 3a0a   show(self, n):.
+0001a250: 2020 2020 2020 2020 2222 2253 686f 7720          """Show 
+0001a260: 7468 6520 6669 7273 7420 6e20 726f 7773  the first n rows
+0001a270: 206f 6620 7468 6520 6665 6174 7572 6520   of the feature 
+0001a280: 6772 6f75 702e 0a0a 2020 2020 2020 2020  group...        
+0001a290: 2121 2120 6578 616d 706c 650a 2020 2020  !!! example.    
+0001a2a0: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
+0001a2b0: 6e0a 2020 2020 2020 2020 2020 2020 2320  n.            # 
+0001a2c0: 636f 6e6e 6563 7420 746f 2074 6865 2046  connect to the F
+0001a2d0: 6561 7475 7265 2053 746f 7265 0a20 2020  eature Store.   
+0001a2e0: 2020 2020 2020 2020 2066 7320 3d20 2e2e           fs = ..
+0001a2f0: 2e0a 0a20 2020 2020 2020 2020 2020 2023  ...            #
+0001a300: 2067 6574 2074 6865 2046 6561 7475 7265   get the Feature
+0001a310: 2047 726f 7570 2069 6e73 7461 6e63 650a   Group instance.
+0001a320: 2020 2020 2020 2020 2020 2020 6667 203d              fg =
+0001a330: 2066 732e 6765 745f 6f72 5f63 7265 6174   fs.get_or_creat
+0001a340: 655f 6665 6174 7572 655f 6772 6f75 7028  e_feature_group(
+0001a350: 2e2e 2e29 0a0a 2020 2020 2020 2020 2020  ...)..          
+0001a360: 2020 6667 2e73 686f 7728 3529 0a20 2020    fg.show(5).   
+0001a370: 2020 2020 2020 2020 2060 6060 0a20 2020           ```.   
+0001a380: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0001a390: 2065 6e67 696e 652e 6765 745f 696e 7374   engine.get_inst
+0001a3a0: 616e 6365 2829 2e73 6574 5f6a 6f62 5f67  ance().set_job_g
+0001a3b0: 726f 7570 280a 2020 2020 2020 2020 2020  roup(.          
+0001a3c0: 2020 2246 6574 6368 696e 6720 4665 6174    "Fetching Feat
+0001a3d0: 7572 6520 6772 6f75 7022 2c0a 2020 2020  ure group",.    
+0001a3e0: 2020 2020 2020 2020 2247 6574 7469 6e67          "Getting
+0001a3f0: 2066 6561 7475 7265 2067 726f 7570 3a20   feature group: 
+0001a400: 7b7d 2066 726f 6d20 7468 6520 6665 6174  {} from the feat
+0001a410: 7572 6573 746f 7265 207b 7d22 2e66 6f72  urestore {}".for
+0001a420: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
+0001a430: 2020 2020 2073 656c 662e 5f6e 616d 652c       self._name,
+0001a440: 2073 656c 662e 5f66 6561 7475 7265 5f73   self._feature_s
+0001a450: 746f 7265 5f6e 616d 650a 2020 2020 2020  tore_name.      
+0001a460: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+0001a470: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
+0001a480: 6e20 7365 6c66 2e73 656c 6563 745f 616c  n self.select_al
+0001a490: 6c28 292e 7368 6f77 286e 290a 0a20 2020  l().show(n)..   
+0001a4a0: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+0001a4b0: 2020 6465 6620 6672 6f6d 5f72 6573 706f    def from_respo
+0001a4c0: 6e73 655f 6a73 6f6e 2863 6c73 2c20 6a73  nse_json(cls, js
+0001a4d0: 6f6e 5f64 6963 7429 3a0a 2020 2020 2020  on_dict):.      
+0001a4e0: 2020 6a73 6f6e 5f64 6563 616d 656c 697a    json_decameliz
+0001a4f0: 6564 203d 2068 756d 7073 2e64 6563 616d  ed = humps.decam
+0001a500: 656c 697a 6528 6a73 6f6e 5f64 6963 7429  elize(json_dict)
+0001a510: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+0001a520: 7374 616e 6365 286a 736f 6e5f 6465 6361  stance(json_deca
+0001a530: 6d65 6c69 7a65 642c 2064 6963 7429 3a0a  melized, dict):.
+0001a540: 2020 2020 2020 2020 2020 2020 5f20 3d20              _ = 
+0001a550: 6a73 6f6e 5f64 6563 616d 656c 697a 6564  json_decamelized
+0001a560: 2e70 6f70 2822 7479 7065 222c 204e 6f6e  .pop("type", Non
+0001a570: 6529 0a20 2020 2020 2020 2020 2020 2072  e).            r
+0001a580: 6574 7572 6e20 636c 7328 2a2a 6a73 6f6e  eturn cls(**json
+0001a590: 5f64 6563 616d 656c 697a 6564 290a 2020  _decamelized).  
+0001a5a0: 2020 2020 2020 666f 7220 6667 2069 6e20        for fg in 
+0001a5b0: 6a73 6f6e 5f64 6563 616d 656c 697a 6564  json_decamelized
+0001a5c0: 3a0a 2020 2020 2020 2020 2020 2020 5f20  :.            _ 
+0001a5d0: 3d20 6667 2e70 6f70 2822 7479 7065 222c  = fg.pop("type",
+0001a5e0: 204e 6f6e 6529 0a20 2020 2020 2020 2072   None).        r
+0001a5f0: 6574 7572 6e20 5b63 6c73 282a 2a66 6729  eturn [cls(**fg)
+0001a600: 2066 6f72 2066 6720 696e 206a 736f 6e5f   for fg in json_
+0001a610: 6465 6361 6d65 6c69 7a65 645d 0a0a 2020  decamelized]..  
+0001a620: 2020 6465 6620 7570 6461 7465 5f66 726f    def update_fro
+0001a630: 6d5f 7265 7370 6f6e 7365 5f6a 736f 6e28  m_response_json(
+0001a640: 7365 6c66 2c20 6a73 6f6e 5f64 6963 7429  self, json_dict)
+0001a650: 3a0a 2020 2020 2020 2020 6a73 6f6e 5f64  :.        json_d
+0001a660: 6563 616d 656c 697a 6564 203d 2068 756d  ecamelized = hum
+0001a670: 7073 2e64 6563 616d 656c 697a 6528 6a73  ps.decamelize(js
+0001a680: 6f6e 5f64 6963 7429 0a20 2020 2020 2020  on_dict).       
+0001a690: 2069 6620 2274 7970 6522 2069 6e20 6a73   if "type" in js
+0001a6a0: 6f6e 5f64 6563 616d 656c 697a 6564 3a0a  on_decamelized:.
+0001a6b0: 2020 2020 2020 2020 2020 2020 5f20 3d20              _ = 
+0001a6c0: 6a73 6f6e 5f64 6563 616d 656c 697a 6564  json_decamelized
+0001a6d0: 2e70 6f70 2822 7479 7065 2229 0a20 2020  .pop("type").   
+0001a6e0: 2020 2020 2073 656c 662e 5f5f 696e 6974       self.__init
+0001a6f0: 5f5f 282a 2a6a 736f 6e5f 6465 6361 6d65  __(**json_decame
+0001a700: 6c69 7a65 6429 0a20 2020 2020 2020 2072  lized).        r
+0001a710: 6574 7572 6e20 7365 6c66 0a0a 2020 2020  eturn self..    
+0001a720: 6465 6620 6a73 6f6e 2873 656c 6629 3a0a  def json(self):.
+0001a730: 2020 2020 2020 2020 7265 7475 726e 206a          return j
+0001a740: 736f 6e2e 6475 6d70 7328 7365 6c66 2c20  son.dumps(self, 
+0001a750: 636c 733d 7574 696c 2e46 6561 7475 7265  cls=util.Feature
+0001a760: 5374 6f72 6545 6e63 6f64 6572 290a 0a20  StoreEncoder).. 
+0001a770: 2020 2064 6566 2074 6f5f 6469 6374 2873     def to_dict(s
+0001a780: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
+0001a790: 7475 726e 207b 0a20 2020 2020 2020 2020  turn {.         
+0001a7a0: 2020 2022 6964 223a 2073 656c 662e 5f69     "id": self._i
+0001a7b0: 642c 0a20 2020 2020 2020 2020 2020 2022  d,.            "
+0001a7c0: 6e61 6d65 223a 2073 656c 662e 5f6e 616d  name": self._nam
+0001a7d0: 652c 0a20 2020 2020 2020 2020 2020 2022  e,.            "
+0001a7e0: 6465 7363 7269 7074 696f 6e22 3a20 7365  description": se
+0001a7f0: 6c66 2e5f 6465 7363 7269 7074 696f 6e2c  lf._description,
+0001a800: 0a20 2020 2020 2020 2020 2020 2022 7665  .            "ve
+0001a810: 7273 696f 6e22 3a20 7365 6c66 2e5f 7665  rsion": self._ve
+0001a820: 7273 696f 6e2c 0a20 2020 2020 2020 2020  rsion,.         
+0001a830: 2020 2022 6665 6174 7572 6573 223a 2073     "features": s
+0001a840: 656c 662e 5f66 6561 7475 7265 732c 0a20  elf._features,. 
+0001a850: 2020 2020 2020 2020 2020 2022 6665 6174             "feat
+0001a860: 7572 6573 746f 7265 4964 223a 2073 656c  urestoreId": sel
+0001a870: 662e 5f66 6561 7475 7265 5f73 746f 7265  f._feature_store
+0001a880: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+0001a890: 2022 7175 6572 7922 3a20 7365 6c66 2e5f   "query": self._
+0001a8a0: 7175 6572 792c 0a20 2020 2020 2020 2020  query,.         
+0001a8b0: 2020 2022 6461 7461 466f 726d 6174 223a     "dataFormat":
+0001a8c0: 2073 656c 662e 5f64 6174 615f 666f 726d   self._data_form
+0001a8d0: 6174 2c0a 2020 2020 2020 2020 2020 2020  at,.            
+0001a8e0: 2270 6174 6822 3a20 7365 6c66 2e5f 7061  "path": self._pa
+0001a8f0: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+0001a900: 226f 7074 696f 6e73 223a 205b 7b22 6e61  "options": [{"na
+0001a910: 6d65 223a 206b 2c20 2276 616c 7565 223a  me": k, "value":
+0001a920: 2076 7d20 666f 7220 6b2c 2076 2069 6e20   v} for k, v in 
+0001a930: 7365 6c66 2e5f 6f70 7469 6f6e 732e 6974  self._options.it
+0001a940: 656d 7328 295d 0a20 2020 2020 2020 2020  ems()].         
+0001a950: 2020 2069 6620 7365 6c66 2e5f 6f70 7469     if self._opti
+0001a960: 6f6e 730a 2020 2020 2020 2020 2020 2020  ons.            
+0001a970: 656c 7365 204e 6f6e 652c 0a20 2020 2020  else None,.     
+0001a980: 2020 2020 2020 2022 7374 6f72 6167 6543         "storageC
+0001a990: 6f6e 6e65 6374 6f72 223a 2073 656c 662e  onnector": self.
+0001a9a0: 5f73 746f 7261 6765 5f63 6f6e 6e65 6374  _storage_connect
+0001a9b0: 6f72 2e74 6f5f 6469 6374 2829 2c0a 2020  or.to_dict(),.  
+0001a9c0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
+0001a9d0: 3a20 226f 6e44 656d 616e 6446 6561 7475  : "onDemandFeatu
+0001a9e0: 7265 6772 6f75 7044 544f 222c 0a20 2020  regroupDTO",.   
+0001a9f0: 2020 2020 2020 2020 2022 7374 6174 6973           "statis
+0001aa00: 7469 6373 436f 6e66 6967 223a 2073 656c  ticsConfig": sel
+0001aa10: 662e 5f73 7461 7469 7374 6963 735f 636f  f._statistics_co
+0001aa20: 6e66 6967 2c0a 2020 2020 2020 2020 2020  nfig,.          
+0001aa30: 2020 2265 7665 6e74 5469 6d65 223a 2073    "eventTime": s
+0001aa40: 656c 662e 5f65 7665 6e74 5f74 696d 652c  elf._event_time,
+0001aa50: 0a20 2020 2020 2020 2020 2020 2022 6578  .            "ex
+0001aa60: 7065 6374 6174 696f 6e53 7569 7465 223a  pectationSuite":
+0001aa70: 2073 656c 662e 5f65 7870 6563 7461 7469   self._expectati
+0001aa80: 6f6e 5f73 7569 7465 2c0a 2020 2020 2020  on_suite,.      
+0001aa90: 2020 2020 2020 226f 6e6c 696e 6545 6e61        "onlineEna
+0001aaa0: 626c 6564 223a 2073 656c 662e 5f6f 6e6c  bled": self._onl
+0001aab0: 696e 655f 656e 6162 6c65 642c 0a20 2020  ine_enabled,.   
+0001aac0: 2020 2020 207d 0a0a 2020 2020 4070 726f       }..    @pro
+0001aad0: 7065 7274 790a 2020 2020 6465 6620 6964  perty.    def id
+0001aae0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0001aaf0: 7265 7475 726e 2073 656c 662e 5f69 640a  return self._id.
+0001ab00: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+0001ab10: 2020 2064 6566 206e 616d 6528 7365 6c66     def name(self
+0001ab20: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+0001ab30: 6e20 7365 6c66 2e5f 6e61 6d65 0a0a 2020  n self._name..  
+0001ab40: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+0001ab50: 6465 6620 7665 7273 696f 6e28 7365 6c66  def version(self
+0001ab60: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+0001ab70: 6e20 7365 6c66 2e5f 7665 7273 696f 6e0a  n self._version.
+0001ab80: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+0001ab90: 2020 2064 6566 2064 6573 6372 6970 7469     def descripti
+0001aba0: 6f6e 2873 656c 6629 3a0a 2020 2020 2020  on(self):.      
+0001abb0: 2020 7265 7475 726e 2073 656c 662e 5f64    return self._d
+0001abc0: 6573 6372 6970 7469 6f6e 0a0a 2020 2020  escription..    
+0001abd0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0001abe0: 6620 6665 6174 7572 6573 2873 656c 6629  f features(self)
+0001abf0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0001ac00: 2073 656c 662e 5f66 6561 7475 7265 730a   self._features.
+0001ac10: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+0001ac20: 2020 2064 6566 2071 7565 7279 2873 656c     def query(sel
+0001ac30: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+0001ac40: 726e 2073 656c 662e 5f71 7565 7279 0a0a  rn self._query..
+0001ac50: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0001ac60: 2020 6465 6620 6461 7461 5f66 6f72 6d61    def data_forma
+0001ac70: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+0001ac80: 2072 6574 7572 6e20 7365 6c66 2e5f 6461   return self._da
+0001ac90: 7461 5f66 6f72 6d61 740a 0a20 2020 2040  ta_format..    @
+0001aca0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+0001acb0: 2070 6174 6828 7365 6c66 293a 0a20 2020   path(self):.   
+0001acc0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0001acd0: 2e5f 7061 7468 0a0a 2020 2020 4070 726f  ._path..    @pro
+0001ace0: 7065 7274 790a 2020 2020 6465 6620 6f70  perty.    def op
+0001acf0: 7469 6f6e 7328 7365 6c66 293a 0a20 2020  tions(self):.   
+0001ad00: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0001ad10: 2e5f 6f70 7469 6f6e 730a 0a20 2020 2040  ._options..    @
+0001ad20: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+0001ad30: 2073 746f 7261 6765 5f63 6f6e 6e65 6374   storage_connect
+0001ad40: 6f72 2873 656c 6629 3a0a 2020 2020 2020  or(self):.      
+0001ad50: 2020 7265 7475 726e 2073 656c 662e 5f73    return self._s
+0001ad60: 746f 7261 6765 5f63 6f6e 6e65 6374 6f72  torage_connector
+0001ad70: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
+0001ad80: 2020 2020 6465 6620 6372 6561 746f 7228      def creator(
+0001ad90: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
+0001ada0: 6574 7572 6e20 7365 6c66 2e5f 6372 6561  eturn self._crea
+0001adb0: 746f 720a 0a20 2020 2040 7072 6f70 6572  tor..    @proper
+0001adc0: 7479 0a20 2020 2064 6566 2063 7265 6174  ty.    def creat
+0001add0: 6564 2873 656c 6629 3a0a 2020 2020 2020  ed(self):.      
+0001ade0: 2020 7265 7475 726e 2073 656c 662e 5f63    return self._c
+0001adf0: 7265 6174 6564 0a0a 2020 2020 4076 6572  reated..    @ver
+0001ae00: 7369 6f6e 2e73 6574 7465 720a 2020 2020  sion.setter.    
+0001ae10: 6465 6620 7665 7273 696f 6e28 7365 6c66  def version(self
+0001ae20: 2c20 7665 7273 696f 6e29 3a0a 2020 2020  , version):.    
+0001ae30: 2020 2020 7365 6c66 2e5f 7665 7273 696f      self._versio
+0001ae40: 6e20 3d20 7665 7273 696f 6e0a 0a20 2020  n = version..   
+0001ae50: 2040 6465 7363 7269 7074 696f 6e2e 7365   @description.se
+0001ae60: 7474 6572 0a20 2020 2064 6566 2064 6573  tter.    def des
+0001ae70: 6372 6970 7469 6f6e 2873 656c 662c 206e  cription(self, n
+0001ae80: 6577 5f64 6573 6372 6970 7469 6f6e 293a  ew_description):
+0001ae90: 0a20 2020 2020 2020 2073 656c 662e 5f64  .        self._d
+0001aea0: 6573 6372 6970 7469 6f6e 203d 206e 6577  escription = new
+0001aeb0: 5f64 6573 6372 6970 7469 6f6e 0a0a 2020  _description..  
+0001aec0: 2020 4066 6561 7475 7265 732e 7365 7474    @features.sett
+0001aed0: 6572 0a20 2020 2064 6566 2066 6561 7475  er.    def featu
+0001aee0: 7265 7328 7365 6c66 2c20 6e65 775f 6665  res(self, new_fe
+0001aef0: 6174 7572 6573 293a 0a20 2020 2020 2020  atures):.       
+0001af00: 2073 656c 662e 5f66 6561 7475 7265 7320   self._features 
+0001af10: 3d20 6e65 775f 6665 6174 7572 6573 0a0a  = new_features..
+0001af20: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0001af30: 2020 6465 6620 6665 6174 7572 655f 7374    def feature_st
+0001af40: 6f72 655f 6e61 6d65 2873 656c 6629 3a0a  ore_name(self):.
+0001af50: 2020 2020 2020 2020 2222 224e 616d 6520          """Name 
+0001af60: 6f66 2074 6865 2066 6561 7475 7265 2073  of the feature s
+0001af70: 746f 7265 2069 6e20 7768 6963 6820 7468  tore in which th
+0001af80: 6520 6665 6174 7572 6520 6772 6f75 7020  e feature group 
+0001af90: 6973 206c 6f63 6174 6564 2e22 2222 0a20  is located.""". 
+0001afa0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0001afb0: 6c66 2e5f 6665 6174 7572 655f 7374 6f72  lf._feature_stor
+0001afc0: 655f 6e61 6d65 0a0a 2020 2020 4070 726f  e_name..    @pro
+0001afd0: 7065 7274 790a 2020 2020 6465 6620 6665  perty.    def fe
+0001afe0: 6174 7572 655f 7374 6f72 655f 6964 2873  ature_store_id(s
+0001aff0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+0001b000: 2249 6420 6f66 2074 6865 2066 6561 7475  "Id of the featu
+0001b010: 7265 2073 746f 7265 2069 6e20 7768 6963  re store in whic
+0001b020: 6820 7468 6520 6665 6174 7572 6520 6772  h the feature gr
+0001b030: 6f75 7020 6973 206c 6f63 6174 6564 2e22  oup is located."
+0001b040: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+0001b050: 6e20 7365 6c66 2e5f 6665 6174 7572 655f  n self._feature_
+0001b060: 7374 6f72 655f 6964 0a                   store_id.
```

### Comparing `hsfs-3.2.0rc1/hsfs/feature_group_commit.py` & `hsfs-3.2.0rc2/hsfs/feature_group_commit.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/feature_group_writer.py` & `hsfs-3.2.0rc2/hsfs/feature_group_writer.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/feature_store.py` & `hsfs-3.2.0rc2/hsfs/feature_store.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/feature_view.py` & `hsfs-3.2.0rc2/hsfs/feature_view.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/ge_expectation.py` & `hsfs-3.2.0rc2/hsfs/ge_expectation.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/ge_validation_result.py` & `hsfs-3.2.0rc2/hsfs/ge_validation_result.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/split_statistics.py` & `hsfs-3.2.0rc2/hsfs/split_statistics.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/statistics.py` & `hsfs-3.2.0rc2/hsfs/statistics.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/statistics_config.py` & `hsfs-3.2.0rc2/hsfs/statistics_config.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/storage_connector.py` & `hsfs-3.2.0rc2/hsfs/storage_connector.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/tag.py` & `hsfs-3.2.0rc2/hsfs/tag.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/training_dataset.py` & `hsfs-3.2.0rc2/hsfs/training_dataset.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/training_dataset_feature.py` & `hsfs-3.2.0rc2/hsfs/training_dataset_feature.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/training_dataset_split.py` & `hsfs-3.2.0rc2/hsfs/training_dataset_split.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/transformation_function.py` & `hsfs-3.2.0rc2/hsfs/transformation_function.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/transformation_function_attached.py` & `hsfs-3.2.0rc2/hsfs/transformation_function_attached.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/user.py` & `hsfs-3.2.0rc2/hsfs/user.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/util.py` & `hsfs-3.2.0rc2/hsfs/util.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/validation_report.py` & `hsfs-3.2.0rc2/hsfs/validation_report.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs/version.py` & `hsfs-3.2.0rc2/hsfs/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-__version__ = "3.2.0rc1"
+__version__ = "3.2.0rc2"
```

### Comparing `hsfs-3.2.0rc1/hsfs.egg-info/PKG-INFO` & `hsfs-3.2.0rc2/hsfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsfs
-Version: 3.2.0rc1
+Version: 3.2.0rc2
 Summary: HSFS: An environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api
 Author: Hopsworks AB
 Author-email: moritz@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc1
+Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc2
 Description: # Hopsworks Feature Store
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: hsfs Version: 3.2.0rc1 Summary: HSFS: An
+Metadata-Version: 2.1 Name: hsfs Version: 3.2.0rc2 Summary: HSFS: An
 environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api Author: Hopsworks
 AB Author-email: moritz@logicalclocks.com License: Apache License 2.0 Download-
-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc1
+URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.2.0rc2
 Description: # Hopsworks Feature Store
   [Hopsworks_Community] [Hopsworks_Feature_Store_Documentation] [PyPiStatus]
            [Scala/Java_Artifacts] [Downloads] [CodeStyle] [License]
 HSFS is the library to interact with the Hopsworks Feature Store. The library
 makes creating new features, feature groups and training datasets easy. The
 library is environment independent and can be used in two modes: - Spark mode:
 For data engineering jobs that create and write features into the feature store
```

### Comparing `hsfs-3.2.0rc1/hsfs.egg-info/SOURCES.txt` & `hsfs-3.2.0rc2/hsfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/hsfs.egg-info/requires.txt` & `hsfs-3.2.0rc2/hsfs.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hsfs-3.2.0rc1/setup.py` & `hsfs-3.2.0rc2/setup.py`

 * *Files identical despite different names*

