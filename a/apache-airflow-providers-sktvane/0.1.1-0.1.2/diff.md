# Comparing `tmp/apache-airflow-providers-sktvane-0.1.1.tar.gz` & `tmp/apache-airflow-providers-sktvane-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-sktvane-0.1.1.tar", last modified: Tue May 16 01:18:04 2023, max compression
+gzip compressed data, was "apache-airflow-providers-sktvane-0.1.2.tar", last modified: Tue May 16 01:39:22 2023, max compression
```

## Comparing `apache-airflow-providers-sktvane-0.1.1.tar` & `apache-airflow-providers-sktvane-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:04.431607 apache-airflow-providers-sktvane-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-16 01:18:04.431607 apache-airflow-providers-sktvane-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:04.423607 apache-airflow-providers-sktvane-0.1.1/airflow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:04.423607 apache-airflow-providers-sktvane-0.1.1/airflow/providers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:04.423607 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:04.427607 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/macros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/macros/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/macros/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/macros/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/macros/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:04.427607 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/operators/nes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:04.427607 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/sensors/gcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:04.427607 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:04.431607 apache-airflow-providers-sktvane-0.1.1/apache_airflow_providers_sktvane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-16 01:18:04.000000 apache-airflow-providers-sktvane-0.1.1/apache_airflow_providers_sktvane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-16 01:18:04.000000 apache-airflow-providers-sktvane-0.1.1/apache_airflow_providers_sktvane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 01:18:04.000000 apache-airflow-providers-sktvane-0.1.1/apache_airflow_providers_sktvane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 01:18:04.000000 apache-airflow-providers-sktvane-0.1.1/apache_airflow_providers_sktvane.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 01:18:04.000000 apache-airflow-providers-sktvane-0.1.1/apache_airflow_providers_sktvane.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 01:18:04.431607 apache-airflow-providers-sktvane-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:22.929234 apache-airflow-providers-sktvane-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-16 01:39:22.929234 apache-airflow-providers-sktvane-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:22.925234 apache-airflow-providers-sktvane-0.1.2/airflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:22.925234 apache-airflow-providers-sktvane-0.1.2/airflow/providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:22.925234 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:22.925234 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/macros/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/macros/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/macros/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/macros/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:22.925234 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/operators/nes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:22.925234 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/sensors/gcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:22.925234 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:22.929234 apache-airflow-providers-sktvane-0.1.2/apache_airflow_providers_sktvane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-16 01:39:22.000000 apache-airflow-providers-sktvane-0.1.2/apache_airflow_providers_sktvane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-16 01:39:22.000000 apache-airflow-providers-sktvane-0.1.2/apache_airflow_providers_sktvane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 01:39:22.000000 apache-airflow-providers-sktvane-0.1.2/apache_airflow_providers_sktvane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 01:39:22.000000 apache-airflow-providers-sktvane-0.1.2/apache_airflow_providers_sktvane.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 01:39:22.000000 apache-airflow-providers-sktvane-0.1.2/apache_airflow_providers_sktvane.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 01:39:22.929234 apache-airflow-providers-sktvane-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/setup.py
```

### Comparing `apache-airflow-providers-sktvane-0.1.1/PKG-INFO` & `apache-airflow-providers-sktvane-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sktvane
-Version: 0.1.1
+Version: 0.1.2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt
 Home-page: https://github.com/sktaiflow/sktvane-airflow-providers
 Author: aidp
 Author-email: aidp@sktai.io
 License: MIT
 Download-URL: https://github.com/sktaiflow/sktvane-airflow-providers
 Keywords: airflow,sktvane
@@ -13,15 +13,18 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # apache-airflow-providers-sktvane
 
-- AIDP 가 제공하는 자원(`NES`, `BigQuery`, `Vault`) 에 접근하는 용도
+- AIDP 가 제공하는 자원들에 접근하는 용도
+  - `NES`
+  - `BigQuery`
+  - `Vault`
 - 기타 공용 목적의 코드
 
 ## PyPI
 
 - https://pypi.org/project/apache-airflow-providers-sktvane
 
 ## Deployment
@@ -36,16 +39,16 @@
     $ rm -rf build dist apache_airflow_providers_sktvane.egg-info 
     ```
 
 ## Components
 
 ###### Operators
 
-- `airflow.providers.sktvane.operators.nes`
-    - `NesOperator` : AIDP 의 `NES(Notebook Executor Service)` 연동 
+- `airflow.providers.sktvane.operators.nes` : AIDP 의 `NES` 연동
+    - `NesOperator` 
         ```python
         # import
         from airflow.providers.sktvane.operators.nes import NesOperator
         
         ...
         
         # usage
@@ -55,16 +58,16 @@
         	parameters={"current_date": "{{ ds }}", "channel": "#aim-statistics"},
         )
         ```
         
 
 ###### Sensors
 
-- `airflow.providers.sktvane.sensors.gcp`
-    - `BigqueryPartitionSensor` : AIDP 의 `BigQuery` 연동
+- `airflow.providers.sktvane.sensors.gcp` : AIDP 의 `GCP` 연동
+    - `BigqueryPartitionSensor`
         ```python
         # import
         from airflow.providers.sktvane.sensors.gcp import BigqueryPartitionSensor
         
         ...
         
         # usage
@@ -75,16 +78,16 @@
         	partition="dt = '{{ds}}'",
         )
         ```
         
 
 ###### Macros
 
-- `airflow.providers.sktvane.macros.slack`
-    - `send_fail_message` : AIDP 표준 포맷으로 에러 메시지를 `Slack` 으로 발송
+- `airflow.providers.sktvane.macros.slack` : AIDP 정의 규격으로 `Slack` 연동
+    - `send_fail_message`
         ```python
         # import
         from airflow.providers.sktvane.macros.slack import send_fail_message
         
         ...
         
         # usage
@@ -92,16 +95,16 @@
           send_fail_message(
             slack_channel="#aidp-airflow-monitoring",
             slack_username=f"Airflow-AlarmBot-{env}",
             slack_email=slack_email,
           )
         ```
         
-- `airflow.providers.sktvane.macros.gcp`
-    - `bigquery_client` : AIDP 관리 대상 `BigQuery` 연동
+- `airflow.providers.sktvane.macros.gcp` : AIDP 의 `GCP` 연동
+    - `bigquery_client`
         ```python
         # import
         from airflow.providers.sktvane.macros.gcp import bigquery_client
         
         ...
         
         # usage
@@ -113,16 +116,16 @@
             write_disposition="WRITE_TRUNCATE",
             destination=f"{bq_client.project}.prcpln_smp.{dest_table_name}",
           )
           job = bq_client.query(query, job_config=job_config)
           job.result()
         ```
         
-- `airflow.providers.sktvane.macros.vault`
-    - `get_secrets` : AIDP 의 `Vault` 를 사용, Secrets 관리
+- `airflow.providers.sktvane.macros.vault` : AIDP 의 `Vault` 연동
+    - `get_secrets`
         ```python
         # import
         from airflow.providers.sktvane.macros.vault import get_secrets
         
         ...
         
         # usage
@@ -133,16 +136,16 @@
           host = hiveserver2["ip"]
           port = hiveserver2["port"]
           user = hiveserver2["user"]
           conn = hive.connect(host, port=port, username=user)
           return conn
         ```
         
-- `airflow.providers.sktvane.macros.date`
-    - `ds_nodash_plus_days` : datetime 관련, 유틸리티성 용도
+- `airflow.providers.sktvane.macros.date` : AIDP 에서 제공하는 date 유틸리티
+    - `ds_nodash_plus_days`
         ```python
         # import
         from airflow.providers.sktvane.macros.date import ds_nodash_plus_days
         
         ...
         
         # usage
@@ -151,7 +154,8 @@
         ```
     - `ds_nodash_minus_days`
     - `ym_nodash_add_month`
     - `first_day_of_this_month`
     - `last_day_of_this_month`
     - `get_latest_loaded_dt`
 
+
```

### Comparing `apache-airflow-providers-sktvane-0.1.1/README.md` & `apache-airflow-providers-sktvane-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # apache-airflow-providers-sktvane
 
-- AIDP 가 제공하는 자원(`NES`, `BigQuery`, `Vault`) 에 접근하는 용도
+- AIDP 가 제공하는 자원들에 접근하는 용도
+  - `NES`
+  - `BigQuery`
+  - `Vault`
 - 기타 공용 목적의 코드
 
 ## PyPI
 
 - https://pypi.org/project/apache-airflow-providers-sktvane
 
 ## Deployment
@@ -19,16 +22,16 @@
     $ rm -rf build dist apache_airflow_providers_sktvane.egg-info 
     ```
 
 ## Components
 
 ###### Operators
 
-- `airflow.providers.sktvane.operators.nes`
-    - `NesOperator` : AIDP 의 `NES(Notebook Executor Service)` 연동 
+- `airflow.providers.sktvane.operators.nes` : AIDP 의 `NES` 연동
+    - `NesOperator` 
         ```python
         # import
         from airflow.providers.sktvane.operators.nes import NesOperator
         
         ...
         
         # usage
@@ -38,16 +41,16 @@
         	parameters={"current_date": "{{ ds }}", "channel": "#aim-statistics"},
         )
         ```
         
 
 ###### Sensors
 
-- `airflow.providers.sktvane.sensors.gcp`
-    - `BigqueryPartitionSensor` : AIDP 의 `BigQuery` 연동
+- `airflow.providers.sktvane.sensors.gcp` : AIDP 의 `GCP` 연동
+    - `BigqueryPartitionSensor`
         ```python
         # import
         from airflow.providers.sktvane.sensors.gcp import BigqueryPartitionSensor
         
         ...
         
         # usage
@@ -58,16 +61,16 @@
         	partition="dt = '{{ds}}'",
         )
         ```
         
 
 ###### Macros
 
-- `airflow.providers.sktvane.macros.slack`
-    - `send_fail_message` : AIDP 표준 포맷으로 에러 메시지를 `Slack` 으로 발송
+- `airflow.providers.sktvane.macros.slack` : AIDP 정의 규격으로 `Slack` 연동
+    - `send_fail_message`
         ```python
         # import
         from airflow.providers.sktvane.macros.slack import send_fail_message
         
         ...
         
         # usage
@@ -75,16 +78,16 @@
           send_fail_message(
             slack_channel="#aidp-airflow-monitoring",
             slack_username=f"Airflow-AlarmBot-{env}",
             slack_email=slack_email,
           )
         ```
         
-- `airflow.providers.sktvane.macros.gcp`
-    - `bigquery_client` : AIDP 관리 대상 `BigQuery` 연동
+- `airflow.providers.sktvane.macros.gcp` : AIDP 의 `GCP` 연동
+    - `bigquery_client`
         ```python
         # import
         from airflow.providers.sktvane.macros.gcp import bigquery_client
         
         ...
         
         # usage
@@ -96,16 +99,16 @@
             write_disposition="WRITE_TRUNCATE",
             destination=f"{bq_client.project}.prcpln_smp.{dest_table_name}",
           )
           job = bq_client.query(query, job_config=job_config)
           job.result()
         ```
         
-- `airflow.providers.sktvane.macros.vault`
-    - `get_secrets` : AIDP 의 `Vault` 를 사용, Secrets 관리
+- `airflow.providers.sktvane.macros.vault` : AIDP 의 `Vault` 연동
+    - `get_secrets`
         ```python
         # import
         from airflow.providers.sktvane.macros.vault import get_secrets
         
         ...
         
         # usage
@@ -116,24 +119,24 @@
           host = hiveserver2["ip"]
           port = hiveserver2["port"]
           user = hiveserver2["user"]
           conn = hive.connect(host, port=port, username=user)
           return conn
         ```
         
-- `airflow.providers.sktvane.macros.date`
-    - `ds_nodash_plus_days` : datetime 관련, 유틸리티성 용도
+- `airflow.providers.sktvane.macros.date` : AIDP 에서 제공하는 date 유틸리티
+    - `ds_nodash_plus_days`
         ```python
         # import
         from airflow.providers.sktvane.macros.date import ds_nodash_plus_days
         
         ...
         
         # usage
         def ds_nodash_tomorrow(ds):
             ds_nodash_plus_days(ds, 1)
         ```
     - `ds_nodash_minus_days`
     - `ym_nodash_add_month`
     - `first_day_of_this_month`
     - `last_day_of_this_month`
-    - `get_latest_loaded_dt`
+    - `get_latest_loaded_dt`
```

### Comparing `apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/macros/date.py` & `apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/macros/date.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/macros/gcp.py` & `apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/macros/gcp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/macros/slack.py` & `apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/macros/slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/operators/nes.py` & `apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/operators/nes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/sensors/gcp.py` & `apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/sensors/gcp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.1/apache_airflow_providers_sktvane.egg-info/PKG-INFO` & `apache-airflow-providers-sktvane-0.1.2/apache_airflow_providers_sktvane.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sktvane
-Version: 0.1.1
+Version: 0.1.2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt
 Home-page: https://github.com/sktaiflow/sktvane-airflow-providers
 Author: aidp
 Author-email: aidp@sktai.io
 License: MIT
 Download-URL: https://github.com/sktaiflow/sktvane-airflow-providers
 Keywords: airflow,sktvane
@@ -13,15 +13,18 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # apache-airflow-providers-sktvane
 
-- AIDP 가 제공하는 자원(`NES`, `BigQuery`, `Vault`) 에 접근하는 용도
+- AIDP 가 제공하는 자원들에 접근하는 용도
+  - `NES`
+  - `BigQuery`
+  - `Vault`
 - 기타 공용 목적의 코드
 
 ## PyPI
 
 - https://pypi.org/project/apache-airflow-providers-sktvane
 
 ## Deployment
@@ -36,16 +39,16 @@
     $ rm -rf build dist apache_airflow_providers_sktvane.egg-info 
     ```
 
 ## Components
 
 ###### Operators
 
-- `airflow.providers.sktvane.operators.nes`
-    - `NesOperator` : AIDP 의 `NES(Notebook Executor Service)` 연동 
+- `airflow.providers.sktvane.operators.nes` : AIDP 의 `NES` 연동
+    - `NesOperator` 
         ```python
         # import
         from airflow.providers.sktvane.operators.nes import NesOperator
         
         ...
         
         # usage
@@ -55,16 +58,16 @@
         	parameters={"current_date": "{{ ds }}", "channel": "#aim-statistics"},
         )
         ```
         
 
 ###### Sensors
 
-- `airflow.providers.sktvane.sensors.gcp`
-    - `BigqueryPartitionSensor` : AIDP 의 `BigQuery` 연동
+- `airflow.providers.sktvane.sensors.gcp` : AIDP 의 `GCP` 연동
+    - `BigqueryPartitionSensor`
         ```python
         # import
         from airflow.providers.sktvane.sensors.gcp import BigqueryPartitionSensor
         
         ...
         
         # usage
@@ -75,16 +78,16 @@
         	partition="dt = '{{ds}}'",
         )
         ```
         
 
 ###### Macros
 
-- `airflow.providers.sktvane.macros.slack`
-    - `send_fail_message` : AIDP 표준 포맷으로 에러 메시지를 `Slack` 으로 발송
+- `airflow.providers.sktvane.macros.slack` : AIDP 정의 규격으로 `Slack` 연동
+    - `send_fail_message`
         ```python
         # import
         from airflow.providers.sktvane.macros.slack import send_fail_message
         
         ...
         
         # usage
@@ -92,16 +95,16 @@
           send_fail_message(
             slack_channel="#aidp-airflow-monitoring",
             slack_username=f"Airflow-AlarmBot-{env}",
             slack_email=slack_email,
           )
         ```
         
-- `airflow.providers.sktvane.macros.gcp`
-    - `bigquery_client` : AIDP 관리 대상 `BigQuery` 연동
+- `airflow.providers.sktvane.macros.gcp` : AIDP 의 `GCP` 연동
+    - `bigquery_client`
         ```python
         # import
         from airflow.providers.sktvane.macros.gcp import bigquery_client
         
         ...
         
         # usage
@@ -113,16 +116,16 @@
             write_disposition="WRITE_TRUNCATE",
             destination=f"{bq_client.project}.prcpln_smp.{dest_table_name}",
           )
           job = bq_client.query(query, job_config=job_config)
           job.result()
         ```
         
-- `airflow.providers.sktvane.macros.vault`
-    - `get_secrets` : AIDP 의 `Vault` 를 사용, Secrets 관리
+- `airflow.providers.sktvane.macros.vault` : AIDP 의 `Vault` 연동
+    - `get_secrets`
         ```python
         # import
         from airflow.providers.sktvane.macros.vault import get_secrets
         
         ...
         
         # usage
@@ -133,16 +136,16 @@
           host = hiveserver2["ip"]
           port = hiveserver2["port"]
           user = hiveserver2["user"]
           conn = hive.connect(host, port=port, username=user)
           return conn
         ```
         
-- `airflow.providers.sktvane.macros.date`
-    - `ds_nodash_plus_days` : datetime 관련, 유틸리티성 용도
+- `airflow.providers.sktvane.macros.date` : AIDP 에서 제공하는 date 유틸리티
+    - `ds_nodash_plus_days`
         ```python
         # import
         from airflow.providers.sktvane.macros.date import ds_nodash_plus_days
         
         ...
         
         # usage
@@ -151,7 +154,8 @@
         ```
     - `ds_nodash_minus_days`
     - `ym_nodash_add_month`
     - `first_day_of_this_month`
     - `last_day_of_this_month`
     - `get_latest_loaded_dt`
 
+
```

### Comparing `apache-airflow-providers-sktvane-0.1.1/apache_airflow_providers_sktvane.egg-info/SOURCES.txt` & `apache-airflow-providers-sktvane-0.1.2/apache_airflow_providers_sktvane.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.1/setup.py` & `apache-airflow-providers-sktvane-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="apache-airflow-providers-sktvane",
-    version="0.1.1",
+    version="0.1.2",
     author="aidp",
     author_email="aidp@sktai.io",
     description="Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["airflow", "sktvane"],
     license="MIT",
```

