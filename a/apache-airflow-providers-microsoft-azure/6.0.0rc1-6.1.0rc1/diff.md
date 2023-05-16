# Comparing `tmp/apache-airflow-providers-microsoft-azure-6.0.0rc1.tar.gz` & `tmp/apache-airflow-providers-microsoft-azure-6.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-microsoft-azure-6.0.0rc1.tar", last modified: Fri Apr 21 19:49:40 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-microsoft-azure-6.1.0rc1.tar", last modified: Tue May 16 15:54:31 2023, max compression
```

## Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1.tar` & `apache-airflow-providers-microsoft-azure-6.1.0rc1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-04-21 19:49:34.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    25473 2023-04-21 19:49:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    23852 2023-04-21 19:49:34.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:39.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:39.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:39.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:39.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16641 2023-04-21 19:49:34.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8720 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/adx.py
--rw-r--r--   0 root         (0) root         (0)    10986 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/asb.py
--rw-r--r--   0 root         (0) root         (0)     4778 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/base_azure.py
--rw-r--r--   0 root         (0) root         (0)    15288 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/batch.py
--rw-r--r--   0 root         (0) root         (0)     6056 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/container_instance.py
--rw-r--r--   0 root         (0) root         (0)     2458 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/container_registry.py
--rw-r--r--   0 root         (0) root         (0)     4058 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/container_volume.py
--rw-r--r--   0 root         (0) root         (0)    14222 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/cosmos.py
--rw-r--r--   0 root         (0) root         (0)    42973 2023-03-30 19:12:06.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/data_factory.py
--rw-r--r--   0 root         (0) root         (0)    21695 2023-03-10 19:32:05.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/data_lake.py
--rw-r--r--   0 root         (0) root         (0)    12985 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/fileshare.py
--rw-r--r--   0 root         (0) root         (0)     7318 2023-03-16 20:46:35.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/synapse.py
--rw-r--r--   0 root         (0) root         (0)    27566 2023-04-01 16:40:04.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/wasb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10038 2023-03-10 19:31:58.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/log/wasb_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3788 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/adls.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/adx.py
--rw-r--r--   0 root         (0) root         (0)    29576 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/asb.py
--rw-r--r--   0 root         (0) root         (0)    16252 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/batch.py
--rw-r--r--   0 root         (0) root         (0)    15967 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/container_instances.py
--rw-r--r--   0 root         (0) root         (0)     2766 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/cosmos.py
--rw-r--r--   0 root         (0) root         (0)    11484 2023-04-13 08:25:21.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/data_factory.py
--rw-r--r--   0 root         (0) root         (0)     4422 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/synapse.py
--rw-r--r--   0 root         (0) root         (0)     2687 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7822 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/secrets/key_vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2643 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/sensors/cosmos.py
--rw-r--r--   0 root         (0) root         (0)     5611 2023-03-30 19:12:06.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/sensors/data_factory.py
--rw-r--r--   0 root         (0) root         (0)     6287 2023-04-19 10:00:26.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/sensors/wasb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4771 2023-04-21 10:05:41.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py
--rw-r--r--   0 root         (0) root         (0)     4765 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/local_to_adls.py
--rw-r--r--   0 root         (0) root         (0)     2936 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py
--rw-r--r--   0 root         (0) root         (0)     4575 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py
--rw-r--r--   0 root         (0) root         (0)     8215 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-03-14 06:24:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8863 2023-03-27 08:32:49.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/triggers/data_factory.py
--rw-r--r--   0 root         (0) root         (0)     3889 2023-04-01 16:40:04.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/triggers/wasb.py
--rw-r--r--   0 root         (0) root         (0)     2804 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/apache_airflow_providers_microsoft_azure.egg-info/
--rw-r--r--   0 root         (0) root         (0)    25473 2023-04-21 19:49:39.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2944 2023-04-21 19:49:39.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:49:39.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/apache_airflow_providers_microsoft_azure.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-04-21 19:49:39.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/apache_airflow_providers_microsoft_azure.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:49:39.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/apache_airflow_providers_microsoft_azure.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      609 2023-04-21 19:49:39.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/apache_airflow_providers_microsoft_azure.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:49:39.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/apache_airflow_providers_microsoft_azure.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2359 2023-04-21 19:49:40.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1874 2023-04-21 19:49:34.000000 apache-airflow-providers-microsoft-azure-6.0.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:31.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:54:29.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    26585 2023-05-16 15:54:31.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24964 2023-05-16 15:54:29.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:31.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:31.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:31.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:31.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-05-16 15:39:21.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-05-16 15:54:29.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:31.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8720 2023-04-30 16:55:11.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/adx.py
+-rw-r--r--   0 root         (0) root         (0)    10986 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/asb.py
+-rw-r--r--   0 root         (0) root         (0)     4778 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/base_azure.py
+-rw-r--r--   0 root         (0) root         (0)    15288 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/batch.py
+-rw-r--r--   0 root         (0) root         (0)     6176 2023-05-03 19:47:07.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/container_instance.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/container_registry.py
+-rw-r--r--   0 root         (0) root         (0)     4058 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/container_volume.py
+-rw-r--r--   0 root         (0) root         (0)    14222 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/cosmos.py
+-rw-r--r--   0 root         (0) root         (0)    42973 2023-03-30 19:12:06.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)    21695 2023-03-10 19:32:05.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/data_lake.py
+-rw-r--r--   0 root         (0) root         (0)    12985 2023-04-30 16:55:11.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/fileshare.py
+-rw-r--r--   0 root         (0) root         (0)     7318 2023-03-16 20:46:35.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/synapse.py
+-rw-r--r--   0 root         (0) root         (0)    27566 2023-04-01 16:40:04.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/wasb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:31.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10038 2023-03-10 19:31:58.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/log/wasb_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:31.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3788 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/operators/adls.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/operators/adx.py
+-rw-r--r--   0 root         (0) root         (0)    29576 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/operators/asb.py
+-rw-r--r--   0 root         (0) root         (0)    16252 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/operators/batch.py
+-rw-r--r--   0 root         (0) root         (0)    15967 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/operators/container_instances.py
+-rw-r--r--   0 root         (0) root         (0)     2766 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/operators/cosmos.py
+-rw-r--r--   0 root         (0) root         (0)    12432 2023-05-12 08:38:07.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/operators/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)     4422 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/operators/synapse.py
+-rw-r--r--   0 root         (0) root         (0)     2687 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:31.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7902 2023-05-03 19:47:07.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/secrets/key_vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:31.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2643 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/sensors/cosmos.py
+-rw-r--r--   0 root         (0) root         (0)     5763 2023-05-03 19:47:07.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/sensors/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)     7660 2023-05-03 19:47:07.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/sensors/wasb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:31.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4771 2023-04-21 10:05:41.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py
+-rw-r--r--   0 root         (0) root         (0)     4815 2023-05-03 19:47:07.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/transfers/local_to_adls.py
+-rw-r--r--   0 root         (0) root         (0)     2936 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py
+-rw-r--r--   0 root         (0) root         (0)     4575 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py
+-rw-r--r--   0 root         (0) root         (0)     8215 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:31.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-03-14 06:24:40.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8859 2023-04-24 21:04:25.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/triggers/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)     7381 2023-04-24 21:04:25.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/triggers/wasb.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-04-30 16:55:11.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:31.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/apache_airflow_providers_microsoft_azure.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    26585 2023-05-16 15:54:30.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2944 2023-05-16 15:54:31.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:30.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/apache_airflow_providers_microsoft_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-05-16 15:54:30.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/apache_airflow_providers_microsoft_azure.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:30.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/apache_airflow_providers_microsoft_azure.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      609 2023-05-16 15:54:30.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/apache_airflow_providers_microsoft_azure.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:54:30.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/apache_airflow_providers_microsoft_azure.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2359 2023-05-16 15:54:31.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-05-16 15:54:29.000000 apache-airflow-providers-microsoft-azure-6.1.0rc1/setup.py
```

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/LICENSE` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/MANIFEST.in` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/PKG-INFO` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-azure
-Version: 6.0.0rc1
+Version: 6.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-azure package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.0.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.1.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -51,28 +51,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-azure``
 
-Release: ``6.0.0rc1``
+Release: ``6.1.0rc1``
 
 
 `Microsoft Azure <https://azure.microsoft.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.azure`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.azure`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -82,15 +82,15 @@
 
 Requirements
 ------------
 
 ================================  ==================
 PIP package                       Version required
 ================================  ==================
-``apache-airflow``                ``>=2.3.0``
+``apache-airflow``                ``>=2.4.0``
 ``azure-batch``                   ``>=8.0.0``
 ``azure-cosmos``                  ``>=4.0.0``
 ``azure-datalake-store``          ``>=0.0.45``
 ``azure-identity``                ``>=1.3.1``
 ``azure-keyvault-secrets``        ``>=4.1.0``
 ``azure-mgmt-datalake-store``     ``>=0.5.0``
 ``azure-mgmt-resource``           ``>=2.2.0``
@@ -149,14 +149,39 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+6.1.0
+.....
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+Features
+~~~~~~~~
+
+* ``Add deferrable mode to 'WasbPrefixSensor' (#30252)``
+
+Misc
+~~~~
+
+* ``Bump minimum Airflow version in providers (#30917)``
+* ``Optimize deferrable execution mode 'AzureDataFactoryPipelineRunStatusSensor' (#30983)``
+* ``Optimize deferred execution for AzureDataFactoryRunPipelineOperator (#31214)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Move TaskInstanceKey to a separate file (#31033)``
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Upgrade ruff to 0.0.262 (#30809)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+
 6.0.0
 ......
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 .. warning::
@@ -278,16 +303,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
 
 
 5.0.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 * In AzureFileShareHook, if both ``extra__azure_fileshare__foo`` and ``foo`` existed in connection extra
   dict, the prefixed version would be used; now, the non-prefixed version will be preferred.
 * ``Remove deprecated classes (#27417)``
@@ -381,16 +407,17 @@
 
 4.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Features
 ~~~~~~~~
 
 * ``Pass connection extra parameters to wasb BlobServiceClient (#24154)``
```

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/README.rst` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-azure``
 
-Release: ``6.0.0rc1``
+Release: ``6.1.0rc1``
 
 
 `Microsoft Azure <https://azure.microsoft.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.azure`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.azure`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -46,15 +46,15 @@
 
 Requirements
 ------------
 
 ================================  ==================
 PIP package                       Version required
 ================================  ==================
-``apache-airflow``                ``>=2.3.0``
+``apache-airflow``                ``>=2.4.0``
 ``azure-batch``                   ``>=8.0.0``
 ``azure-cosmos``                  ``>=4.0.0``
 ``azure-datalake-store``          ``>=0.0.45``
 ``azure-identity``                ``>=1.3.1``
 ``azure-keyvault-secrets``        ``>=4.1.0``
 ``azure-mgmt-datalake-store``     ``>=0.5.0``
 ``azure-mgmt-resource``           ``>=2.2.0``
@@ -113,14 +113,39 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+6.1.0
+.....
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+Features
+~~~~~~~~
+
+* ``Add deferrable mode to 'WasbPrefixSensor' (#30252)``
+
+Misc
+~~~~
+
+* ``Bump minimum Airflow version in providers (#30917)``
+* ``Optimize deferrable execution mode 'AzureDataFactoryPipelineRunStatusSensor' (#30983)``
+* ``Optimize deferred execution for AzureDataFactoryRunPipelineOperator (#31214)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Move TaskInstanceKey to a separate file (#31033)``
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Upgrade ruff to 0.0.262 (#30809)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+
 6.0.0
 ......
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 .. warning::
@@ -242,16 +267,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
 
 
 5.0.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 * In AzureFileShareHook, if both ``extra__azure_fileshare__foo`` and ``foo`` existed in connection extra
   dict, the prefixed version would be used; now, the non-prefixed version will be preferred.
 * ``Remove deprecated classes (#27417)``
@@ -345,16 +371,17 @@
 
 4.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Features
 ~~~~~~~~
 
 * ``Pass connection extra parameters to wasb BlobServiceClient (#24154)``
```

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/__init__.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/get_provider_info.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-microsoft-azure",
         "name": "Microsoft Azure",
         "description": "`Microsoft Azure <https://azure.microsoft.com/>`__\n",
         "suspended": False,
         "versions": [
+            "6.1.0",
             "6.0.0",
             "5.3.1",
             "5.3.0",
             "5.2.1",
             "5.2.0",
             "5.1.0",
             "5.0.2",
@@ -58,15 +59,15 @@
             "2.0.0",
             "1.3.0",
             "1.2.0",
             "1.1.0",
             "1.0.0",
         ],
         "dependencies": [
-            "apache-airflow>=2.3.0",
+            "apache-airflow>=2.4.0",
             "azure-batch>=8.0.0",
             "azure-cosmos>=4.0.0",
             "azure-datalake-store>=0.0.45",
             "azure-identity>=1.3.1",
             "azure-keyvault-secrets>=4.1.0",
             "azure-mgmt-datalake-store>=0.5.0",
             "azure-mgmt-resource>=2.2.0",
```

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/__init__.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/adx.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/adx.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/asb.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/asb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/base_azure.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/base_azure.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/batch.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/container_instance.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/container_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from __future__ import annotations
 
 import warnings
 
 from azure.mgmt.containerinstance import ContainerInstanceManagementClient
 from azure.mgmt.containerinstance.models import ContainerGroup
 
+from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.microsoft.azure.hooks.base_azure import AzureBaseHook
 
 
 class AzureContainerInstanceHook(AzureBaseHook):
     """
     A hook to communicate with Azure Container Instances.
 
@@ -65,15 +66,15 @@
         :param resource_group: the name of the resource group
         :param name: the name of the container group
         :return: A tuple with the state, exitcode, and details.
             If the exitcode is unknown 0 is returned.
         """
         warnings.warn(
             "get_state_exitcode_details() is deprecated. Related method is get_state()",
-            DeprecationWarning,
+            AirflowProviderDeprecationWarning,
             stacklevel=2,
         )
         cg_state = self.get_state(resource_group, name)
         c_state = cg_state.containers[0].instance_view.current_state
         return (c_state.state, c_state.exit_code, c_state.detail_status)
 
     def get_messages(self, resource_group: str, name: str) -> list:
@@ -81,15 +82,17 @@
         Get the messages of a container group
 
         :param resource_group: the name of the resource group
         :param name: the name of the container group
         :return: A list of the event messages
         """
         warnings.warn(
-            "get_messages() is deprecated. Related method is get_state()", DeprecationWarning, stacklevel=2
+            "get_messages() is deprecated. Related method is get_state()",
+            AirflowProviderDeprecationWarning,
+            stacklevel=2,
         )
         cg_state = self.get_state(resource_group, name)
         instance_view = cg_state.containers[0].instance_view
         return [event.message for event in instance_view.events]
 
     def get_state(self, resource_group: str, name: str) -> ContainerGroup:
         """
```

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/container_registry.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/container_registry.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/container_volume.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/container_volume.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/cosmos.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/data_lake.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/data_lake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/fileshare.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/fileshare.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/synapse.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/synapse.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/hooks/wasb.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/hooks/wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/log/__init__.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/log/wasb_task_handler.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/log/wasb_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/__init__.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/adls.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/operators/adls.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/adx.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/operators/adx.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/asb.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/operators/asb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/batch.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/operators/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/container_instances.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/operators/container_instances.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/cosmos.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/operators/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/operators/data_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,21 +23,22 @@
 from airflow.exceptions import AirflowException
 from airflow.hooks.base import BaseHook
 from airflow.models import BaseOperator, BaseOperatorLink, XCom
 from airflow.providers.microsoft.azure.hooks.data_factory import (
     AzureDataFactoryHook,
     AzureDataFactoryPipelineRunException,
     AzureDataFactoryPipelineRunStatus,
+    PipelineRunInfo,
     get_field,
 )
 from airflow.providers.microsoft.azure.triggers.data_factory import AzureDataFactoryTrigger
 from airflow.utils.log.logging_mixin import LoggingMixin
 
 if TYPE_CHECKING:
-    from airflow.models.taskinstance import TaskInstanceKey
+    from airflow.models.taskinstancekey import TaskInstanceKey
     from airflow.utils.context import Context
 
 
 class AzureDataFactoryPipelineRunLink(LoggingMixin, BaseOperatorLink):
     """Constructs a link to monitor a pipeline run in Azure Data Factory."""
 
     name = "Monitor Pipeline Run"
@@ -191,27 +192,40 @@
                     self.log.info("Pipeline run %s has completed successfully.", self.run_id)
                 else:
                     raise AzureDataFactoryPipelineRunException(
                         f"Pipeline run {self.run_id} has failed or has been cancelled."
                     )
             else:
                 end_time = time.time() + self.timeout
-                self.defer(
-                    timeout=self.execution_timeout,
-                    trigger=AzureDataFactoryTrigger(
-                        azure_data_factory_conn_id=self.azure_data_factory_conn_id,
-                        run_id=self.run_id,
-                        wait_for_termination=self.wait_for_termination,
-                        resource_group_name=self.resource_group_name,
-                        factory_name=self.factory_name,
-                        check_interval=self.check_interval,
-                        end_time=end_time,
-                    ),
-                    method_name="execute_complete",
+                pipeline_run_info = PipelineRunInfo(
+                    run_id=self.run_id,
+                    factory_name=self.factory_name,
+                    resource_group_name=self.resource_group_name,
                 )
+                pipeline_run_status = self.hook.get_pipeline_run_status(**pipeline_run_info)
+                if pipeline_run_status not in AzureDataFactoryPipelineRunStatus.TERMINAL_STATUSES:
+                    self.defer(
+                        timeout=self.execution_timeout,
+                        trigger=AzureDataFactoryTrigger(
+                            azure_data_factory_conn_id=self.azure_data_factory_conn_id,
+                            run_id=self.run_id,
+                            wait_for_termination=self.wait_for_termination,
+                            resource_group_name=self.resource_group_name,
+                            factory_name=self.factory_name,
+                            check_interval=self.check_interval,
+                            end_time=end_time,
+                        ),
+                        method_name="execute_complete",
+                    )
+                elif pipeline_run_status == AzureDataFactoryPipelineRunStatus.SUCCEEDED:
+                    self.log.info("Pipeline run %s has completed successfully.", self.run_id)
+                elif pipeline_run_status in AzureDataFactoryPipelineRunStatus.FAILURE_STATES:
+                    raise AzureDataFactoryPipelineRunException(
+                        f"Pipeline run {self.run_id} has failed or has been cancelled."
+                    )
         else:
             if self.deferrable is True:
                 warnings.warn(
                     "Argument `wait_for_termination` is False and `deferrable` is True , hence "
                     "`deferrable` parameter doesn't have any effect",
                 )
```

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/synapse.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/operators/synapse.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/secrets/__init__.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/secrets/key_vault.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/secrets/key_vault.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import warnings
 
 from azure.core.exceptions import ResourceNotFoundError
 from azure.identity import DefaultAzureCredential
 from azure.keyvault.secrets import SecretClient
 
 from airflow.compat.functools import cached_property
+from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.secrets import BaseSecretsBackend
 from airflow.utils.log.logging_mixin import LoggingMixin
 from airflow.version import version as airflow_version
 
 
 def _parse_version(val):
     val = re.sub(r"(\d+\.\d+\.\d+).*", lambda x: x.group(1), val)
@@ -124,15 +125,15 @@
         :param conn_id: the connection id
         :return: deserialized Connection
         """
         if _parse_version(airflow_version) >= (2, 3):
             warnings.warn(
                 f"Method `{self.__class__.__name__}.get_conn_uri` is deprecated and will be removed "
                 "in a future release.  Please use method `get_conn_value` instead.",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
         return self.get_conn_value(conn_id)
 
     def get_variable(self, key: str) -> str | None:
         """
         Get an Airflow Variable from an Azure Key Vault secret.
```

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/sensors/__init__.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/transfers/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
```

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/sensors/cosmos.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/sensors/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/sensors/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/sensors/data_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # under the License.
 from __future__ import annotations
 
 import warnings
 from datetime import timedelta
 from typing import TYPE_CHECKING, Any, Sequence
 
-from airflow import AirflowException
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.providers.microsoft.azure.hooks.data_factory import (
     AzureDataFactoryHook,
     AzureDataFactoryPipelineRunException,
     AzureDataFactoryPipelineRunStatus,
 )
 from airflow.providers.microsoft.azure.triggers.data_factory import ADFPipelineRunStatusSensorTrigger
 from airflow.sensors.base import BaseSensorOperator
@@ -90,25 +90,26 @@
     def execute(self, context: Context) -> None:
         """Defers trigger class to poll for state of the job run until
         it reaches a failure state or success state
         """
         if not self.deferrable:
             super().execute(context=context)
         else:
-            self.defer(
-                timeout=timedelta(seconds=self.timeout),
-                trigger=ADFPipelineRunStatusSensorTrigger(
-                    run_id=self.run_id,
-                    azure_data_factory_conn_id=self.azure_data_factory_conn_id,
-                    resource_group_name=self.resource_group_name,
-                    factory_name=self.factory_name,
-                    poke_interval=self.poke_interval,
-                ),
-                method_name="execute_complete",
-            )
+            if not self.poke(context=context):
+                self.defer(
+                    timeout=timedelta(seconds=self.timeout),
+                    trigger=ADFPipelineRunStatusSensorTrigger(
+                        run_id=self.run_id,
+                        azure_data_factory_conn_id=self.azure_data_factory_conn_id,
+                        resource_group_name=self.resource_group_name,
+                        factory_name=self.factory_name,
+                        poke_interval=self.poke_interval,
+                    ),
+                    method_name="execute_complete",
+                )
 
     def execute_complete(self, context: Context, event: dict[str, str]) -> None:
         """
         Callback for when the trigger fires - returns immediately.
         Relies on trigger to throw an exception, otherwise it assumes execution was
         successful.
         """
@@ -133,11 +134,11 @@
 
     def __init__(self, **kwargs: Any) -> None:
         warnings.warn(
             "Class `AzureDataFactoryPipelineRunStatusAsyncSensor` is deprecated and "
             "will be removed in a future release. "
             "Please use `AzureDataFactoryPipelineRunStatusSensor` and "
             "set `deferrable` attribute to `True` instead",
-            DeprecationWarning,
+            AirflowProviderDeprecationWarning,
             stacklevel=2,
         )
         super().__init__(**kwargs, deferrable=True)
```

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/sensors/wasb.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/sensors/wasb.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 # under the License.
 from __future__ import annotations
 
 import warnings
 from datetime import timedelta
 from typing import TYPE_CHECKING, Any, Sequence
 
-from airflow.exceptions import AirflowException
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.providers.microsoft.azure.hooks.wasb import WasbHook
-from airflow.providers.microsoft.azure.triggers.wasb import WasbBlobSensorTrigger
+from airflow.providers.microsoft.azure.triggers.wasb import WasbBlobSensorTrigger, WasbPrefixSensorTrigger
 from airflow.sensors.base import BaseSensorOperator
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class WasbBlobSensor(BaseSensorOperator):
@@ -118,15 +118,15 @@
 
     def __init__(self, **kwargs: Any) -> None:
         warnings.warn(
             "Class `WasbBlobAsyncSensor` is deprecated and "
             "will be removed in a future release. "
             "Please use `WasbBlobSensor` and "
             "set `deferrable` attribute to `True` instead",
-            DeprecationWarning,
+            AirflowProviderDeprecationWarning,
             stacklevel=2,
         )
         super().__init__(**kwargs, deferrable=True)
 
 
 class WasbPrefixSensor(BaseSensorOperator):
     """
@@ -144,21 +144,54 @@
     def __init__(
         self,
         *,
         container_name: str,
         prefix: str,
         wasb_conn_id: str = "wasb_default",
         check_options: dict | None = None,
+        deferrable: bool = False,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         if check_options is None:
             check_options = {}
         self.wasb_conn_id = wasb_conn_id
         self.container_name = container_name
         self.prefix = prefix
         self.check_options = check_options
+        self.deferrable = deferrable
 
     def poke(self, context: Context) -> bool:
         self.log.info("Poking for prefix: %s in wasb://%s", self.prefix, self.container_name)
         hook = WasbHook(wasb_conn_id=self.wasb_conn_id)
         return hook.check_for_prefix(self.container_name, self.prefix, **self.check_options)
+
+    def execute(self, context: Context) -> None:
+        """Defers trigger class to poll for state of the job run until it
+        reaches a failure state or success state
+        """
+        if not self.deferrable:
+            super().execute(context=context)
+        else:
+            self.defer(
+                timeout=timedelta(seconds=self.timeout),
+                trigger=WasbPrefixSensorTrigger(
+                    container_name=self.container_name,
+                    prefix=self.prefix,
+                    wasb_conn_id=self.wasb_conn_id,
+                    poke_interval=self.poke_interval,
+                ),
+                method_name="execute_complete",
+            )
+
+    def execute_complete(self, context: Context, event: dict[str, str]) -> None:
+        """
+        Callback for when the trigger fires - returns immediately.
+        Relies on trigger to throw an exception, otherwise it assumes execution was
+        successful.
+        """
+        if event:
+            if event["status"] == "error":
+                raise AirflowException(event["message"])
+            self.log.info(event["message"])
+        else:
+            raise AirflowException("Did not receive valid event from the triggerer")
```

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/__init__.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/local_to_adls.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/transfers/local_to_adls.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import warnings
 from typing import TYPE_CHECKING, Any, Sequence
 
-from airflow.exceptions import AirflowException
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.microsoft.azure.hooks.data_lake import AzureDataLakeHook
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
@@ -106,11 +106,11 @@
     """
 
     def __init__(self, *args, **kwargs):
         warnings.warn(
             """This class is deprecated.
             Please use
             `airflow.providers.microsoft.azure.transfers.local_to_adls.LocalFilesystemToADLSOperator`.""",
-            DeprecationWarning,
+            AirflowProviderDeprecationWarning,
             stacklevel=3,
         )
         super().__init__(*args, **kwargs)
```

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/triggers/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/triggers/data_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
                 "azure_data_factory_conn_id": self.azure_data_factory_conn_id,
                 "resource_group_name": self.resource_group_name,
                 "factory_name": self.factory_name,
                 "poke_interval": self.poke_interval,
             },
         )
 
-    async def run(self) -> AsyncIterator["TriggerEvent"]:
+    async def run(self) -> AsyncIterator[TriggerEvent]:
         """Make async connection to Azure Data Factory, polls for the pipeline run status"""
         hook = AzureDataFactoryAsyncHook(azure_data_factory_conn_id=self.azure_data_factory_conn_id)
         try:
             while True:
                 pipeline_status = await hook.get_adf_pipeline_run_status(
                     run_id=self.run_id,
                     resource_group_name=self.resource_group_name,
@@ -136,15 +136,15 @@
                 "wait_for_termination": self.wait_for_termination,
                 "resource_group_name": self.resource_group_name,
                 "factory_name": self.factory_name,
                 "end_time": self.end_time,
             },
         )
 
-    async def run(self) -> AsyncIterator["TriggerEvent"]:
+    async def run(self) -> AsyncIterator[TriggerEvent]:
         """Make async connection to Azure Data Factory, polls for the pipeline run status"""
         hook = AzureDataFactoryAsyncHook(azure_data_factory_conn_id=self.azure_data_factory_conn_id)
         try:
             pipeline_status = await hook.get_adf_pipeline_run_status(
                 run_id=self.run_id,
                 resource_group_name=self.resource_group_name,
                 factory_name=self.factory_name,
```

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/airflow/providers/microsoft/azure/utils.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/airflow/providers/microsoft/azure/utils.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-azure
-Version: 6.0.0rc1
+Version: 6.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-azure package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.0.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.1.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -51,28 +51,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-azure``
 
-Release: ``6.0.0rc1``
+Release: ``6.1.0rc1``
 
 
 `Microsoft Azure <https://azure.microsoft.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.azure`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.azure`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -82,15 +82,15 @@
 
 Requirements
 ------------
 
 ================================  ==================
 PIP package                       Version required
 ================================  ==================
-``apache-airflow``                ``>=2.3.0``
+``apache-airflow``                ``>=2.4.0``
 ``azure-batch``                   ``>=8.0.0``
 ``azure-cosmos``                  ``>=4.0.0``
 ``azure-datalake-store``          ``>=0.0.45``
 ``azure-identity``                ``>=1.3.1``
 ``azure-keyvault-secrets``        ``>=4.1.0``
 ``azure-mgmt-datalake-store``     ``>=0.5.0``
 ``azure-mgmt-resource``           ``>=2.2.0``
@@ -149,14 +149,39 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+6.1.0
+.....
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+Features
+~~~~~~~~
+
+* ``Add deferrable mode to 'WasbPrefixSensor' (#30252)``
+
+Misc
+~~~~
+
+* ``Bump minimum Airflow version in providers (#30917)``
+* ``Optimize deferrable execution mode 'AzureDataFactoryPipelineRunStatusSensor' (#30983)``
+* ``Optimize deferred execution for AzureDataFactoryRunPipelineOperator (#31214)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Move TaskInstanceKey to a separate file (#31033)``
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Upgrade ruff to 0.0.262 (#30809)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+
 6.0.0
 ......
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 .. warning::
@@ -278,16 +303,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
 
 
 5.0.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 * In AzureFileShareHook, if both ``extra__azure_fileshare__foo`` and ``foo`` existed in connection extra
   dict, the prefixed version would be used; now, the non-prefixed version will be preferred.
 * ``Remove deprecated classes (#27417)``
@@ -381,16 +407,17 @@
 
 4.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Features
 ~~~~~~~~
 
 * ``Pass connection extra parameters to wasb BlobServiceClient (#24154)``
```

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/apache_airflow_providers_microsoft_azure.egg-info/requires.txt` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/apache_airflow_providers_microsoft_azure.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 adal>=1.2.7
-apache-airflow>=2.3.0.dev0
+apache-airflow>=2.4.0.dev0
 azure-batch>=8.0.0
 azure-cosmos>=4.0.0
 azure-datalake-store>=0.0.45
 azure-identity>=1.3.1
 azure-keyvault-secrets>=4.1.0
 azure-kusto-data<0.1,>=0.0.43
 azure-mgmt-containerinstance<2.0,>=1.5.0
```

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/pyproject.toml` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 target-version = "py37"
 
 extend-select = [
     "I", # Missing required import (auto-fixable)
     "UP", # Pyupgrade
     "RUF100", # Unused noqa (auto-fixable)
 
+    # implicit single-line string concatenation
+    "ISC001",
     # We ignore more pydocstyle than we enable, so be more selective at what we enable
     "D101",
     "D106",
     "D2",
     "D3",
     # "D401", # Not enabled by ruff, but we don't want it
     "D402",
```

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/setup.cfg` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.0.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.1.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -43,15 +43,15 @@
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	adal>=1.2.7
-	apache-airflow>=2.3.0.dev0
+	apache-airflow>=2.4.0.dev0
 	azure-batch>=8.0.0
 	azure-cosmos>=4.0.0
 	azure-datalake-store>=0.0.45
 	azure-identity>=1.3.1
 	azure-keyvault-secrets>=4.1.0
 	azure-kusto-data>=0.0.43,<0.1
 	azure-mgmt-containerinstance>=1.5.0,<2.0
```

### Comparing `apache-airflow-providers-microsoft-azure-6.0.0rc1/setup.py` & `apache-airflow-providers-microsoft-azure-6.1.0rc1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-microsoft-azure package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "6.0.0"
+version = "6.1.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-microsoft-azure setup."""
     setup(
         version=version,
         extras_require={
```

