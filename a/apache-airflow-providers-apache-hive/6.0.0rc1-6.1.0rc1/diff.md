# Comparing `tmp/apache-airflow-providers-apache-hive-6.0.0rc1.tar.gz` & `tmp/apache-airflow-providers-apache-hive-6.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-hive-6.0.0rc1.tar", last modified: Sun Apr  2 05:47:04 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-apache-hive-6.1.0rc1.tar", last modified: Tue May 16 15:53:04 2023, max compression
```

## Comparing `apache-airflow-providers-apache-hive-6.0.0rc1.tar` & `apache-airflow-providers-apache-hive-6.1.0rc1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:04.000000 apache-airflow-providers-apache-hive-6.0.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-hive-6.0.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-04-02 05:47:02.000000 apache-airflow-providers-apache-hive-6.0.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-hive-6.0.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    17796 2023-04-02 05:47:04.000000 apache-airflow-providers-apache-hive-6.0.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16081 2023-04-02 05:47:02.000000 apache-airflow-providers-apache-hive-6.0.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:04.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:04.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:04.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:04.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5552 2023-04-02 05:47:02.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:04.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42219 2023-03-27 08:32:48.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/hooks/hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:04.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/macros/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/macros/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4581 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/macros/hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:04.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7280 2023-03-27 08:32:48.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/operators/hive.py
--rw-r--r--   0 root         (0) root         (0)     7454 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/operators/hive_stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:04.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/plugins/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/plugins/hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:04.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3039 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/sensors/hive_partition.py
--rw-r--r--   0 root         (0) root         (0)     3389 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/sensors/metastore_partition.py
--rw-r--r--   0 root         (0) root         (0)     4159 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/sensors/named_hive_partition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:04.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5279 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/transfers/hive_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     2973 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/transfers/hive_to_samba.py
--rw-r--r--   0 root         (0) root         (0)     5671 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/transfers/mssql_to_hive.py
--rw-r--r--   0 root         (0) root         (0)     6587 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/transfers/mysql_to_hive.py
--rw-r--r--   0 root         (0) root         (0)    11681 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/transfers/s3_to_hive.py
--rw-r--r--   0 root         (0) root         (0)     5548 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/transfers/vertica_to_hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:04.000000 apache-airflow-providers-apache-hive-6.0.0rc1/apache_airflow_providers_apache_hive.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17796 2023-04-02 05:47:04.000000 apache-airflow-providers-apache-hive-6.0.0rc1/apache_airflow_providers_apache_hive.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1643 2023-04-02 05:47:04.000000 apache-airflow-providers-apache-hive-6.0.0rc1/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:47:04.000000 apache-airflow-providers-apache-hive-6.0.0rc1/apache_airflow_providers_apache_hive.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      188 2023-04-02 05:47:04.000000 apache-airflow-providers-apache-hive-6.0.0rc1/apache_airflow_providers_apache_hive.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:47:04.000000 apache-airflow-providers-apache-hive-6.0.0rc1/apache_airflow_providers_apache_hive.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      499 2023-04-02 05:47:04.000000 apache-airflow-providers-apache-hive-6.0.0rc1/apache_airflow_providers_apache_hive.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-02 05:47:04.000000 apache-airflow-providers-apache-hive-6.0.0rc1/apache_airflow_providers_apache_hive.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5393 2023-04-01 16:40:04.000000 apache-airflow-providers-apache-hive-6.0.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2092 2023-04-02 05:47:04.000000 apache-airflow-providers-apache-hive-6.0.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1952 2023-04-02 05:47:02.000000 apache-airflow-providers-apache-hive-6.0.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-hive-6.1.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:53:03.000000 apache-airflow-providers-apache-hive-6.1.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-hive-6.1.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    18741 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17026 2023-05-16 15:53:03.000000 apache-airflow-providers-apache-hive-6.1.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/
+-rw-r--r--   0 root         (0) root         (0)     1394 2023-05-16 15:39:21.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5601 2023-05-16 15:53:03.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42315 2023-05-03 19:47:07.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/hooks/hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/macros/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/macros/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4581 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/macros/hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7383 2023-04-13 08:25:21.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/operators/hive.py
+-rw-r--r--   0 root         (0) root         (0)     7454 2023-04-30 16:55:11.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/operators/hive_stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/plugins/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/plugins/hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3039 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/sensors/hive_partition.py
+-rw-r--r--   0 root         (0) root         (0)     3389 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/sensors/metastore_partition.py
+-rw-r--r--   0 root         (0) root         (0)     4159 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/sensors/named_hive_partition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5279 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/hive_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     2973 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/hive_to_samba.py
+-rw-r--r--   0 root         (0) root         (0)     5671 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/mssql_to_hive.py
+-rw-r--r--   0 root         (0) root         (0)     6587 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/mysql_to_hive.py
+-rw-r--r--   0 root         (0) root         (0)    11742 2023-05-04 19:17:30.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/s3_to_hive.py
+-rw-r--r--   0 root         (0) root         (0)     5548 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/vertica_to_hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/apache_airflow_providers_apache_hive.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    18741 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/apache_airflow_providers_apache_hive.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/apache_airflow_providers_apache_hive.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      188 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/apache_airflow_providers_apache_hive.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/apache_airflow_providers_apache_hive.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      499 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/apache_airflow_providers_apache_hive.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/apache_airflow_providers_apache_hive.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-apache-hive-6.1.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-05-16 15:53:04.000000 apache-airflow-providers-apache-hive-6.1.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-05-16 15:53:02.000000 apache-airflow-providers-apache-hive-6.1.0rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/LICENSE` & `apache-airflow-providers-apache-hive-6.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/MANIFEST.in` & `apache-airflow-providers-apache-hive-6.1.0rc1/MANIFEST.in`

 * *Files 6% similar despite different names*

```diff
@@ -23,10 +23,9 @@
 # `MANIFEST_TEMPLATE.py.jinja2` IN the `provider_packages` DIRECTORY
 
 
 
 
 include NOTICE
 include LICENSE
-include CHANGELOG.txt
-include README.md
+include CHANGELOG.rst
 global-exclude __pycache__  *.pyc
```

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/PKG-INFO` & `apache-airflow-providers-apache-hive-6.1.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-hive
-Version: 6.0.0rc1
+Version: 6.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-hive package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.0.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -55,28 +55,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-hive``
 
-Release: ``6.0.0rc1``
+Release: ``6.1.0rc1``
 
 
 `Apache Hive <https://hive.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.hive`` provider. All classes for this provider package
 are in ``airflow.providers.apache.hive`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -86,15 +86,15 @@
 
 Requirements
 ------------
 
 =======================================  ==================================
 PIP package                              Version required
 =======================================  ==================================
-``apache-airflow``                       ``>=2.3.0``
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``hmsclient``                            ``>=0.1.0``
 ``pandas``                               ``>=0.17.1``
 ``pyhive[hive]``                         ``>=0.6.0``
 ``sasl``                                 ``>=0.3.1; python_version>="3.9"``
 ``thrift``                               ``>=0.9.2``
 =======================================  ==================================
@@ -146,14 +146,34 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+6.1.0
+.....
+
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+Misc
+~~~~
+
+* ``Bump minimum Airflow version in providers (#30917)``
+* ``Update return types of 'get_key' methods on 'S3Hook' (#30923)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Decouple "job runner" from BaseJob ORM model (#30255)``
+
 6.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 The auth option is moved from the extra field to the auth parameter in the Hook. If you have extra
@@ -234,16 +254,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 4.1.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 
 Bug Fixes
@@ -305,16 +326,17 @@
 
 3.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``chore: Refactoring and Cleaning Apache Providers (#24219)``
 * ``AIP-47 - Migrate hive DAGs to new design #22439 (#24204)``
```

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/README.rst` & `apache-airflow-providers-apache-hive-6.1.0rc1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-hive``
 
-Release: ``6.0.0rc1``
+Release: ``6.1.0rc1``
 
 
 `Apache Hive <https://hive.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.hive`` provider. All classes for this provider package
 are in ``airflow.providers.apache.hive`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -46,15 +46,15 @@
 
 Requirements
 ------------
 
 =======================================  ==================================
 PIP package                              Version required
 =======================================  ==================================
-``apache-airflow``                       ``>=2.3.0``
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``hmsclient``                            ``>=0.1.0``
 ``pandas``                               ``>=0.17.1``
 ``pyhive[hive]``                         ``>=0.6.0``
 ``sasl``                                 ``>=0.3.1; python_version>="3.9"``
 ``thrift``                               ``>=0.9.2``
 =======================================  ==================================
@@ -106,14 +106,34 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+6.1.0
+.....
+
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+Misc
+~~~~
+
+* ``Bump minimum Airflow version in providers (#30917)``
+* ``Update return types of 'get_key' methods on 'S3Hook' (#30923)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Decouple "job runner" from BaseJob ORM model (#30255)``
+
 6.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 The auth option is moved from the extra field to the auth parameter in the Hook. If you have extra
@@ -194,16 +214,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 4.1.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 
 Bug Fixes
@@ -265,16 +286,17 @@
 
 3.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``chore: Refactoring and Cleaning Apache Providers (#24219)``
 * ``AIP-47 - Migrate hive DAGs to new design #22439 (#24204)``
```

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/__init__.py` & `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/get_provider_info.py` & `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-hive",
         "name": "Apache Hive",
         "description": "`Apache Hive <https://hive.apache.org/>`__\n",
+        "suspended": False,
         "versions": [
+            "6.1.0",
             "6.0.0",
             "5.1.3",
             "5.1.2",
             "5.1.1",
             "5.1.0",
             "5.0.0",
             "4.1.1",
@@ -52,15 +54,15 @@
             "2.0.0",
             "1.0.3",
             "1.0.2",
             "1.0.1",
             "1.0.0",
         ],
         "dependencies": [
-            "apache-airflow>=2.3.0",
+            "apache-airflow>=2.4.0",
             "apache-airflow-providers-common-sql>=1.3.1",
             "hmsclient>=0.1.0",
             "pandas>=0.17.1",
             "pyhive[hive]>=0.6.0",
             'sasl>=0.3.1; python_version>="3.9"',
             "thrift>=0.9.2",
         ],
```

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/hooks/__init__.py` & `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/hooks/hive.py` & `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/hooks/hive.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 import subprocess
 import time
 import warnings
 from collections import OrderedDict
 from tempfile import NamedTemporaryFile, TemporaryDirectory
 from typing import Any, Iterable, Mapping
 
+from airflow.exceptions import AirflowProviderDeprecationWarning
+
 try:
     import pandas
 except ImportError as e:
     from airflow.exceptions import AirflowOptionalProviderFeatureException
 
     raise AirflowOptionalProviderFeatureException(e)
 
@@ -525,15 +527,15 @@
 
         if not host:
             raise AirflowException("Failed to locate the valid server.")
 
         if "authMechanism" in conn.extra_dejson:
             warnings.warn(
                 "The 'authMechanism' option is deprecated. Please use 'auth_mechanism'.",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
             conn.extra_dejson["auth_mechanism"] = conn.extra_dejson["authMechanism"]
             del conn.extra_dejson["authMechanism"]
 
         auth_mechanism = conn.extra_dejson.get("auth_mechanism", "NOSASL")
 
@@ -840,15 +842,15 @@
         password: str | None = None
 
         db = self.get_connection(self.hiveserver2_conn_id)  # type: ignore
 
         if "authMechanism" in db.extra_dejson:
             warnings.warn(
                 "The 'authMechanism' option is deprecated. Please use 'auth_mechanism'.",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
             db.extra_dejson["auth_mechanism"] = db.extra_dejson["authMechanism"]
             del db.extra_dejson["authMechanism"]
 
         auth_mechanism = db.extra_dejson.get("auth_mechanism", "NONE")
         if auth_mechanism == "NONE" and db.login is None:
```

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/macros/__init__.py` & `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/macros/hive.py` & `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/macros/hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/operators/__init__.py` & `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/operators/hive.py` & `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/operators/hive.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,16 @@
     def execute(self, context: Context) -> None:
         self.log.info("Executing: %s", self.hql)
         self.hook = self.get_hook()
 
         # set the mapred_job_name if it's not set with dag, task, execution time info
         if not self.mapred_job_name:
             ti = context["ti"]
+            if ti.execution_date is None:
+                raise RuntimeError("execution_date is None")
             self.hook.mapred_job_name = self.mapred_job_name_template.format(
                 dag_id=ti.dag_id,
                 task_id=ti.task_id,
                 execution_date=ti.execution_date.isoformat(),
                 hostname=ti.hostname.split(".")[0],
             )
```

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/operators/hive_stats.py` & `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/operators/hive_stats.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/plugins/__init__.py` & `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/plugins/hive.py` & `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/plugins/hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/sensors/__init__.py` & `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/__init__.py`

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

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/sensors/hive_partition.py` & `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/sensors/hive_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/sensors/metastore_partition.py` & `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/sensors/metastore_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/sensors/named_hive_partition.py` & `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/sensors/named_hive_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/transfers/hive_to_mysql.py` & `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/hive_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/transfers/hive_to_samba.py` & `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/hive_to_samba.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/transfers/mssql_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/mssql_to_hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/transfers/mysql_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/mysql_to_hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/transfers/s3_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/s3_to_hive.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,14 +145,18 @@
                 raise AirflowException(f"No key matches {self.s3_key}")
             s3_key_object = s3_hook.get_wildcard_key(self.s3_key)
         elif s3_hook.check_for_key(self.s3_key):
             s3_key_object = s3_hook.get_key(self.s3_key)
 
         else:
             raise AirflowException(f"The key {self.s3_key} does not exists")
+
+        if TYPE_CHECKING:
+            assert s3_key_object
+
         _, file_ext = os.path.splitext(s3_key_object.key)
         if self.select_expression and self.input_compressed and file_ext.lower() != ".gz":
             raise AirflowException("GZIP is the only compression format Amazon S3 Select supports")
 
         with TemporaryDirectory(prefix="tmps32hive_") as tmp_dir, NamedTemporaryFile(
             mode="wb", dir=tmp_dir, suffix=file_ext
         ) as f:
```

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/airflow/providers/apache/hive/transfers/vertica_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.0rc1/airflow/providers/apache/hive/transfers/vertica_to_hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/apache_airflow_providers_apache_hive.egg-info/PKG-INFO` & `apache-airflow-providers-apache-hive-6.1.0rc1/apache_airflow_providers_apache_hive.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-hive
-Version: 6.0.0rc1
+Version: 6.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-hive package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.0.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -55,28 +55,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-hive``
 
-Release: ``6.0.0rc1``
+Release: ``6.1.0rc1``
 
 
 `Apache Hive <https://hive.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.hive`` provider. All classes for this provider package
 are in ``airflow.providers.apache.hive`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -86,15 +86,15 @@
 
 Requirements
 ------------
 
 =======================================  ==================================
 PIP package                              Version required
 =======================================  ==================================
-``apache-airflow``                       ``>=2.3.0``
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``hmsclient``                            ``>=0.1.0``
 ``pandas``                               ``>=0.17.1``
 ``pyhive[hive]``                         ``>=0.6.0``
 ``sasl``                                 ``>=0.3.1; python_version>="3.9"``
 ``thrift``                               ``>=0.9.2``
 =======================================  ==================================
@@ -146,14 +146,34 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+6.1.0
+.....
+
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+Misc
+~~~~
+
+* ``Bump minimum Airflow version in providers (#30917)``
+* ``Update return types of 'get_key' methods on 'S3Hook' (#30923)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Decouple "job runner" from BaseJob ORM model (#30255)``
+
 6.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 The auth option is moved from the extra field to the auth parameter in the Hook. If you have extra
@@ -234,16 +254,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 4.1.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 
 Bug Fixes
@@ -305,16 +326,17 @@
 
 3.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``chore: Refactoring and Cleaning Apache Providers (#24219)``
 * ``AIP-47 - Migrate hive DAGs to new design #22439 (#24204)``
```

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-hive-6.1.0rc1/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/pyproject.toml` & `apache-airflow-providers-apache-hive-6.1.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

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
@@ -135,18 +137,15 @@
 
 # The test_python.py is needed because adding __future__.annotations breaks runtime checks that are
 # needed for the test to work
 "tests/decorators/test_python.py" = ["I002"]
 
 # The Pydantic representations of SqlAlchemy Models are not parsed well with Pydantic
 # when __future__.annotations is used so we need to skip them from upgrading
-"airflow/models/pydantic/taskinstance.py" = ["I002"]
-"airflow/models/pydantic/dag_run.py" = ["I002"]
-"airflow/models/pydantic/dataset.py" = ["I002"]
-"airflow/jobs/pydantic/base_job.py" = ["I002"]
+"airflow/serialization/pydantic/*.py" = ["I002"]
 
 # Ignore pydoc style from these
 "*.pyi" = ["D"]
 "tests/*" = ["D"]
 "scripts/*" = ["D"]
 "dev/*" = ["D"]
 "docs/*" = ["D"]
```

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/setup.cfg` & `apache-airflow-providers-apache-hive-6.1.0rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.0.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.0/
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
 	apache-airflow-providers-common-sql>=1.3.1.dev0
-	apache-airflow>=2.3.0.dev0
+	apache-airflow>=2.4.0.dev0
 	hmsclient>=0.1.0
 	pandas>=0.17.1
 	pyhive[hive]>=0.6.0
 	sasl>=0.3.1; python_version>="3.9"
 	thrift>=0.9.2
 
 [options.entry_points]
```

### Comparing `apache-airflow-providers-apache-hive-6.0.0rc1/setup.py` & `apache-airflow-providers-apache-hive-6.1.0rc1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-hive package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "6.0.0"
+version = "6.1.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-hive setup."""
     setup(
         version=version,
         extras_require={
@@ -39,14 +39,19 @@
             "microsoft.mssql": ["apache-airflow-providers-microsoft-mssql"],
             "mysql": ["apache-airflow-providers-mysql"],
             "presto": ["apache-airflow-providers-presto"],
             "samba": ["apache-airflow-providers-samba"],
             "vertica": ["apache-airflow-providers-vertica"],
         },
         packages=find_namespace_packages(
-            include=["airflow.providers.apache.hive", "airflow.providers.apache.hive.*"]
+            include=[
+                "airflow.providers.apache.hive",
+                "airflow.providers.apache.hive.*",
+                "airflow.providers.apache.hive_vendor",
+                "airflow.providers.apache.hive_vendor.*",
+            ],
         ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

