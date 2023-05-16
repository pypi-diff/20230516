# Comparing `tmp/apache-airflow-providers-sktvane-0.1.2.tar.gz` & `tmp/apache-airflow-providers-sktvane-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-sktvane-0.1.2.tar", last modified: Tue May 16 01:39:22 2023, max compression
+gzip compressed data, was "apache-airflow-providers-sktvane-0.1.3.tar", last modified: Tue May 16 01:55:50 2023, max compression
```

## Comparing `apache-airflow-providers-sktvane-0.1.2.tar` & `apache-airflow-providers-sktvane-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:22.929234 apache-airflow-providers-sktvane-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-16 01:39:22.929234 apache-airflow-providers-sktvane-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:22.925234 apache-airflow-providers-sktvane-0.1.2/airflow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:22.925234 apache-airflow-providers-sktvane-0.1.2/airflow/providers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:22.925234 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:22.925234 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/macros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/macros/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/macros/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/macros/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/macros/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:22.925234 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/operators/nes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:22.925234 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/sensors/gcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:22.925234 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:39:22.929234 apache-airflow-providers-sktvane-0.1.2/apache_airflow_providers_sktvane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-16 01:39:22.000000 apache-airflow-providers-sktvane-0.1.2/apache_airflow_providers_sktvane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-16 01:39:22.000000 apache-airflow-providers-sktvane-0.1.2/apache_airflow_providers_sktvane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 01:39:22.000000 apache-airflow-providers-sktvane-0.1.2/apache_airflow_providers_sktvane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 01:39:22.000000 apache-airflow-providers-sktvane-0.1.2/apache_airflow_providers_sktvane.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 01:39:22.000000 apache-airflow-providers-sktvane-0.1.2/apache_airflow_providers_sktvane.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 01:39:22.929234 apache-airflow-providers-sktvane-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-16 01:39:16.000000 apache-airflow-providers-sktvane-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:55:50.368541 apache-airflow-providers-sktvane-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-16 01:55:50.368541 apache-airflow-providers-sktvane-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-16 01:55:44.000000 apache-airflow-providers-sktvane-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:55:50.360541 apache-airflow-providers-sktvane-0.1.3/airflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:55:50.360541 apache-airflow-providers-sktvane-0.1.3/airflow/providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:55:50.364541 apache-airflow-providers-sktvane-0.1.3/airflow/providers/sktvane/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 01:55:44.000000 apache-airflow-providers-sktvane-0.1.3/airflow/providers/sktvane/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:55:50.364541 apache-airflow-providers-sktvane-0.1.3/airflow/providers/sktvane/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:55:44.000000 apache-airflow-providers-sktvane-0.1.3/airflow/providers/sktvane/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-16 01:55:44.000000 apache-airflow-providers-sktvane-0.1.3/airflow/providers/sktvane/macros/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-16 01:55:44.000000 apache-airflow-providers-sktvane-0.1.3/airflow/providers/sktvane/macros/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-16 01:55:44.000000 apache-airflow-providers-sktvane-0.1.3/airflow/providers/sktvane/macros/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-16 01:55:44.000000 apache-airflow-providers-sktvane-0.1.3/airflow/providers/sktvane/macros/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:55:50.364541 apache-airflow-providers-sktvane-0.1.3/airflow/providers/sktvane/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:55:44.000000 apache-airflow-providers-sktvane-0.1.3/airflow/providers/sktvane/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-16 01:55:44.000000 apache-airflow-providers-sktvane-0.1.3/airflow/providers/sktvane/operators/nes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:55:50.368541 apache-airflow-providers-sktvane-0.1.3/airflow/providers/sktvane/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:55:44.000000 apache-airflow-providers-sktvane-0.1.3/airflow/providers/sktvane/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-16 01:55:44.000000 apache-airflow-providers-sktvane-0.1.3/airflow/providers/sktvane/sensors/gcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:55:50.368541 apache-airflow-providers-sktvane-0.1.3/airflow/providers/sktvane/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:55:44.000000 apache-airflow-providers-sktvane-0.1.3/airflow/providers/sktvane/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 01:55:44.000000 apache-airflow-providers-sktvane-0.1.3/airflow/providers/sktvane/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:55:50.368541 apache-airflow-providers-sktvane-0.1.3/apache_airflow_providers_sktvane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-16 01:55:50.000000 apache-airflow-providers-sktvane-0.1.3/apache_airflow_providers_sktvane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-16 01:55:50.000000 apache-airflow-providers-sktvane-0.1.3/apache_airflow_providers_sktvane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 01:55:50.000000 apache-airflow-providers-sktvane-0.1.3/apache_airflow_providers_sktvane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 01:55:50.000000 apache-airflow-providers-sktvane-0.1.3/apache_airflow_providers_sktvane.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 01:55:50.000000 apache-airflow-providers-sktvane-0.1.3/apache_airflow_providers_sktvane.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 01:55:50.372541 apache-airflow-providers-sktvane-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-16 01:55:44.000000 apache-airflow-providers-sktvane-0.1.3/setup.py
```

### Comparing `apache-airflow-providers-sktvane-0.1.2/PKG-INFO` & `apache-airflow-providers-sktvane-0.1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sktvane
-Version: 0.1.2
+Version: 0.1.3
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt
 Home-page: https://github.com/sktaiflow/sktvane-airflow-providers
 Author: aidp
 Author-email: aidp@sktai.io
 License: MIT
 Download-URL: https://github.com/sktaiflow/sktvane-airflow-providers
 Keywords: airflow,sktvane
@@ -39,123 +39,99 @@
     $ rm -rf build dist apache_airflow_providers_sktvane.egg-info 
     ```
 
 ## Components
 
 ###### Operators
 
-- `airflow.providers.sktvane.operators.nes` : AIDP 의 `NES` 연동
-    - `NesOperator` 
-        ```python
-        # import
-        from airflow.providers.sktvane.operators.nes import NesOperator
-        
-        ...
-        
-        # usage
-        NesOperator(
-        	task_id="jupyter_daily_count",
-        	input_nb="https://github.com/sktaiflow/notebooks/blob/master/statistics/jupyter_daily_count.ipynb",
-        	parameters={"current_date": "{{ ds }}", "channel": "#aim-statistics"},
-        )
-        ```
+- `airflow.providers.sktvane.operators.nes.NesOperator` : AIDP 의 `NES` 사용
+    ```python
+    from airflow.providers.sktvane.operators.nes import NesOperator
+    
+    ...
+    
+    NesOperator(
+        task_id="jupyter_daily_count",
+        input_nb="https://github.com/sktaiflow/notebooks/blob/master/statistics/jupyter_daily_count.ipynb",
+        parameters={"current_date": "{{ ds }}", "channel": "#aim-statistics"},
+    )
+    ```
         
 
 ###### Sensors
 
-- `airflow.providers.sktvane.sensors.gcp` : AIDP 의 `GCP` 연동
-    - `BigqueryPartitionSensor`
-        ```python
-        # import
-        from airflow.providers.sktvane.sensors.gcp import BigqueryPartitionSensor
-        
-        ...
-        
-        # usage
-        BigqueryPartitionSensor(
-        	task_id=f"{table}_partition_sensor",
-        	dataset_id="wind_tmt",
-        	table_id=table,
-        	partition="dt = '{{ds}}'",
-        )
-        ```
-        
+- `airflow.providers.sktvane.sensors.gcp.BigqueryPartitionSensor` : AIDP 의 `BigQuery` 파티션 체크
+
+    ```python
+    from airflow.providers.sktvane.sensors.gcp import BigqueryPartitionSensor
+    
+    ...
+    
+    BigqueryPartitionSensor(
+        task_id=f"{table}_partition_sensor",
+        dataset_id="wind_tmt",
+        table_id=table,
+        partition="dt = '{{ds}}'",
+    )
+    ``` 
 
 ###### Macros
 
-- `airflow.providers.sktvane.macros.slack` : AIDP 정의 규격으로 `Slack` 연동
-    - `send_fail_message`
-        ```python
-        # import
-        from airflow.providers.sktvane.macros.slack import send_fail_message
-        
-        ...
-        
-        # usage
-        def send_aidp_fail_message(slack_email: str) -> None:
-          send_fail_message(
-            slack_channel="#aidp-airflow-monitoring",
-            slack_username=f"Airflow-AlarmBot-{env}",
-            slack_email=slack_email,
-          )
-        ```
-        
-- `airflow.providers.sktvane.macros.gcp` : AIDP 의 `GCP` 연동
-    - `bigquery_client`
-        ```python
-        # import
-        from airflow.providers.sktvane.macros.gcp import bigquery_client
-        
-        ...
-        
-        # usage
-        def bq_query_to_bq(query, dest_table_name, **kwarg):
-        	bq_client = bigquery_client()
-        
-          job_config = QueryJobConfig(
-            create_disposition="CREATE_IF_NEEDED",
-            write_disposition="WRITE_TRUNCATE",
-            destination=f"{bq_client.project}.prcpln_smp.{dest_table_name}",
-          )
-          job = bq_client.query(query, job_config=job_config)
-          job.result()
-        ```
-        
-- `airflow.providers.sktvane.macros.vault` : AIDP 의 `Vault` 연동
-    - `get_secrets`
-        ```python
-        # import
-        from airflow.providers.sktvane.macros.vault import get_secrets
-        
-        ...
-        
-        # usage
-        def get_hive_conn():
-          from pyhive import hive
-        
-          hiveserver2 = get_secrets(path="ye/hiveserver2")
-          host = hiveserver2["ip"]
-          port = hiveserver2["port"]
-          user = hiveserver2["user"]
-          conn = hive.connect(host, port=port, username=user)
-          return conn
-        ```
+- `airflow.providers.sktvane.macros.slack.send_fail_message` : AIDP 정의 포맷으로 `Slack` 에러 메시지 발송
+    ```python
+    from airflow.providers.sktvane.macros.slack import send_fail_message
+    
+    ...
+    
+    def send_aidp_fail_message(slack_email: str) -> None:
+      send_fail_message(
+        slack_channel="#aidp-airflow-monitoring",
+        slack_username=f"Airflow-AlarmBot-{env}",
+        slack_email=slack_email,
+      )
+    ```
         
-- `airflow.providers.sktvane.macros.date` : AIDP 에서 제공하는 date 유틸리티
-    - `ds_nodash_plus_days`
-        ```python
-        # import
-        from airflow.providers.sktvane.macros.date import ds_nodash_plus_days
+- `airflow.providers.sktvane.macros.gcp.bigquery_client` : AIDP 의 `BigQuery` 사용
+    ```python
+    from airflow.providers.sktvane.macros.gcp import bigquery_client
+    
+    ...
+    
+    def bq_query_to_bq(query, dest_table_name, **kwarg):
+      bq_client = bigquery_client()
+      job = bq_client.query(query)
+      job.result()
+    ```
         
-        ...
+- `airflow.providers.sktvane.macros.vault.get_secrets` : AIDP 의 `Vault` 사용
+    ```python
+    from airflow.providers.sktvane.macros.vault import get_secrets
+    
+    ...
+    
+    def get_hive_conn():
+      from pyhive import hive
+    
+      hiveserver2 = get_secrets(path="ye/hiveserver2")
+      host = hiveserver2["ip"]
+      port = hiveserver2["port"]
+      user = hiveserver2["user"]
+      conn = hive.connect(host, port=port, username=user)
+      return conn
+    ```
         
-        # usage
-        def ds_nodash_tomorrow(ds):
-            ds_nodash_plus_days(ds, 1)
-        ```
-    - `ds_nodash_minus_days`
-    - `ym_nodash_add_month`
-    - `first_day_of_this_month`
-    - `last_day_of_this_month`
-    - `get_latest_loaded_dt`
+- `airflow.providers.sktvane.macros.date.ds_nodash_plus_days` : AIDP 에서 제공하는 `date` 유틸리티
+    ```python
+    from airflow.providers.sktvane.macros.date import ds_nodash_plus_days
+    
+    ...
+    
+    def ds_nodash_tomorrow(ds):
+        ds_nodash_plus_days(ds, 1)
+    ```
+- `airflow.providers.sktvane.macros.date.ds_nodash_minus_days` : `ds_nodash_plus_days` 와 동일
+- `airflow.providers.sktvane.macros.date.ym_nodash_add_month` : `ds_nodash_plus_days` 와 동일
+- `airflow.providers.sktvane.macros.date.first_day_of_this_month` : `ds_nodash_plus_days` 와 동일
+- `airflow.providers.sktvane.macros.date.last_day_of_this_month` : `ds_nodash_plus_days` 와 동일
+- `airflow.providers.sktvane.macros.date.get_latest_loaded_dt` : `ds_nodash_plus_days` 와 동일
```

### Comparing `apache-airflow-providers-sktvane-0.1.2/README.md` & `apache-airflow-providers-sktvane-0.1.3/apache_airflow_providers_sktvane.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: apache-airflow-providers-sktvane
+Version: 0.1.3
+Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt
+Home-page: https://github.com/sktaiflow/sktvane-airflow-providers
+Author: aidp
+Author-email: aidp@sktai.io
+License: MIT
+Download-URL: https://github.com/sktaiflow/sktvane-airflow-providers
+Keywords: airflow,sktvane
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
 # apache-airflow-providers-sktvane
 
 - AIDP 가 제공하는 자원들에 접근하는 용도
   - `NES`
   - `BigQuery`
   - `Vault`
 - 기타 공용 목적의 코드
@@ -22,121 +39,99 @@
     $ rm -rf build dist apache_airflow_providers_sktvane.egg-info 
     ```
 
 ## Components
 
 ###### Operators
 
-- `airflow.providers.sktvane.operators.nes` : AIDP 의 `NES` 연동
-    - `NesOperator` 
-        ```python
-        # import
-        from airflow.providers.sktvane.operators.nes import NesOperator
-        
-        ...
-        
-        # usage
-        NesOperator(
-        	task_id="jupyter_daily_count",
-        	input_nb="https://github.com/sktaiflow/notebooks/blob/master/statistics/jupyter_daily_count.ipynb",
-        	parameters={"current_date": "{{ ds }}", "channel": "#aim-statistics"},
-        )
-        ```
+- `airflow.providers.sktvane.operators.nes.NesOperator` : AIDP 의 `NES` 사용
+    ```python
+    from airflow.providers.sktvane.operators.nes import NesOperator
+    
+    ...
+    
+    NesOperator(
+        task_id="jupyter_daily_count",
+        input_nb="https://github.com/sktaiflow/notebooks/blob/master/statistics/jupyter_daily_count.ipynb",
+        parameters={"current_date": "{{ ds }}", "channel": "#aim-statistics"},
+    )
+    ```
         
 
 ###### Sensors
 
-- `airflow.providers.sktvane.sensors.gcp` : AIDP 의 `GCP` 연동
-    - `BigqueryPartitionSensor`
-        ```python
-        # import
-        from airflow.providers.sktvane.sensors.gcp import BigqueryPartitionSensor
-        
-        ...
-        
-        # usage
-        BigqueryPartitionSensor(
-        	task_id=f"{table}_partition_sensor",
-        	dataset_id="wind_tmt",
-        	table_id=table,
-        	partition="dt = '{{ds}}'",
-        )
-        ```
-        
+- `airflow.providers.sktvane.sensors.gcp.BigqueryPartitionSensor` : AIDP 의 `BigQuery` 파티션 체크
+
+    ```python
+    from airflow.providers.sktvane.sensors.gcp import BigqueryPartitionSensor
+    
+    ...
+    
+    BigqueryPartitionSensor(
+        task_id=f"{table}_partition_sensor",
+        dataset_id="wind_tmt",
+        table_id=table,
+        partition="dt = '{{ds}}'",
+    )
+    ``` 
 
 ###### Macros
 
-- `airflow.providers.sktvane.macros.slack` : AIDP 정의 규격으로 `Slack` 연동
-    - `send_fail_message`
-        ```python
-        # import
-        from airflow.providers.sktvane.macros.slack import send_fail_message
-        
-        ...
-        
-        # usage
-        def send_aidp_fail_message(slack_email: str) -> None:
-          send_fail_message(
-            slack_channel="#aidp-airflow-monitoring",
-            slack_username=f"Airflow-AlarmBot-{env}",
-            slack_email=slack_email,
-          )
-        ```
-        
-- `airflow.providers.sktvane.macros.gcp` : AIDP 의 `GCP` 연동
-    - `bigquery_client`
-        ```python
-        # import
-        from airflow.providers.sktvane.macros.gcp import bigquery_client
-        
-        ...
-        
-        # usage
-        def bq_query_to_bq(query, dest_table_name, **kwarg):
-        	bq_client = bigquery_client()
-        
-          job_config = QueryJobConfig(
-            create_disposition="CREATE_IF_NEEDED",
-            write_disposition="WRITE_TRUNCATE",
-            destination=f"{bq_client.project}.prcpln_smp.{dest_table_name}",
-          )
-          job = bq_client.query(query, job_config=job_config)
-          job.result()
-        ```
-        
-- `airflow.providers.sktvane.macros.vault` : AIDP 의 `Vault` 연동
-    - `get_secrets`
-        ```python
-        # import
-        from airflow.providers.sktvane.macros.vault import get_secrets
-        
-        ...
-        
-        # usage
-        def get_hive_conn():
-          from pyhive import hive
-        
-          hiveserver2 = get_secrets(path="ye/hiveserver2")
-          host = hiveserver2["ip"]
-          port = hiveserver2["port"]
-          user = hiveserver2["user"]
-          conn = hive.connect(host, port=port, username=user)
-          return conn
-        ```
+- `airflow.providers.sktvane.macros.slack.send_fail_message` : AIDP 정의 포맷으로 `Slack` 에러 메시지 발송
+    ```python
+    from airflow.providers.sktvane.macros.slack import send_fail_message
+    
+    ...
+    
+    def send_aidp_fail_message(slack_email: str) -> None:
+      send_fail_message(
+        slack_channel="#aidp-airflow-monitoring",
+        slack_username=f"Airflow-AlarmBot-{env}",
+        slack_email=slack_email,
+      )
+    ```
         
-- `airflow.providers.sktvane.macros.date` : AIDP 에서 제공하는 date 유틸리티
-    - `ds_nodash_plus_days`
-        ```python
-        # import
-        from airflow.providers.sktvane.macros.date import ds_nodash_plus_days
+- `airflow.providers.sktvane.macros.gcp.bigquery_client` : AIDP 의 `BigQuery` 사용
+    ```python
+    from airflow.providers.sktvane.macros.gcp import bigquery_client
+    
+    ...
+    
+    def bq_query_to_bq(query, dest_table_name, **kwarg):
+      bq_client = bigquery_client()
+      job = bq_client.query(query)
+      job.result()
+    ```
         
-        ...
+- `airflow.providers.sktvane.macros.vault.get_secrets` : AIDP 의 `Vault` 사용
+    ```python
+    from airflow.providers.sktvane.macros.vault import get_secrets
+    
+    ...
+    
+    def get_hive_conn():
+      from pyhive import hive
+    
+      hiveserver2 = get_secrets(path="ye/hiveserver2")
+      host = hiveserver2["ip"]
+      port = hiveserver2["port"]
+      user = hiveserver2["user"]
+      conn = hive.connect(host, port=port, username=user)
+      return conn
+    ```
         
-        # usage
-        def ds_nodash_tomorrow(ds):
-            ds_nodash_plus_days(ds, 1)
-        ```
-    - `ds_nodash_minus_days`
-    - `ym_nodash_add_month`
-    - `first_day_of_this_month`
-    - `last_day_of_this_month`
-    - `get_latest_loaded_dt`
+- `airflow.providers.sktvane.macros.date.ds_nodash_plus_days` : AIDP 에서 제공하는 `date` 유틸리티
+    ```python
+    from airflow.providers.sktvane.macros.date import ds_nodash_plus_days
+    
+    ...
+    
+    def ds_nodash_tomorrow(ds):
+        ds_nodash_plus_days(ds, 1)
+    ```
+- `airflow.providers.sktvane.macros.date.ds_nodash_minus_days` : `ds_nodash_plus_days` 와 동일
+- `airflow.providers.sktvane.macros.date.ym_nodash_add_month` : `ds_nodash_plus_days` 와 동일
+- `airflow.providers.sktvane.macros.date.first_day_of_this_month` : `ds_nodash_plus_days` 와 동일
+- `airflow.providers.sktvane.macros.date.last_day_of_this_month` : `ds_nodash_plus_days` 와 동일
+- `airflow.providers.sktvane.macros.date.get_latest_loaded_dt` : `ds_nodash_plus_days` 와 동일
+
+
```

### Comparing `apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/macros/date.py` & `apache-airflow-providers-sktvane-0.1.3/airflow/providers/sktvane/macros/date.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/macros/gcp.py` & `apache-airflow-providers-sktvane-0.1.3/airflow/providers/sktvane/macros/gcp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/macros/slack.py` & `apache-airflow-providers-sktvane-0.1.3/airflow/providers/sktvane/macros/slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/operators/nes.py` & `apache-airflow-providers-sktvane-0.1.3/airflow/providers/sktvane/operators/nes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.2/airflow/providers/sktvane/sensors/gcp.py` & `apache-airflow-providers-sktvane-0.1.3/airflow/providers/sktvane/sensors/gcp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.2/apache_airflow_providers_sktvane.egg-info/SOURCES.txt` & `apache-airflow-providers-sktvane-0.1.3/apache_airflow_providers_sktvane.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.2/setup.py` & `apache-airflow-providers-sktvane-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="apache-airflow-providers-sktvane",
-    version="0.1.2",
+    version="0.1.3",
     author="aidp",
     author_email="aidp@sktai.io",
     description="Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["airflow", "sktvane"],
     license="MIT",
```

