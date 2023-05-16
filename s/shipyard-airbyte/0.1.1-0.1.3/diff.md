# Comparing `tmp/shipyard_airbyte-0.1.1.tar.gz` & `tmp/shipyard_airbyte-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_airbyte-0.1.1.tar", max compression
+gzip compressed data, was "shipyard_airbyte-0.1.3.tar", max compression
```

## Comparing `shipyard_airbyte-0.1.1.tar` & `shipyard_airbyte-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      931 2023-04-11 15:20:51.411716 shipyard_airbyte-0.1.1/README.md
--rw-r--r--   0        0        0      484 2023-04-12 01:26:25.848146 shipyard_airbyte-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       34 2023-04-07 13:56:29.886314 shipyard_airbyte-0.1.1/shipyard_airbyte/__init__.py
--rw-r--r--   0        0        0     4014 2023-04-11 15:20:00.786501 shipyard_airbyte-0.1.1/shipyard_airbyte/airbyte.py
--rw-r--r--   0        0        0     1212 2023-04-11 14:38:40.429784 shipyard_airbyte-0.1.1/shipyard_airbyte/cli/cli_determine_sync_status.py
--rw-r--r--   0        0        0     1249 2023-04-11 15:21:21.959665 shipyard_airbyte-0.1.1/shipyard_airbyte/cli/cli_trigger_sync.py
--rw-r--r--   0        0        0     1627 1970-01-01 00:00:00.000000 shipyard_airbyte-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      931 2023-04-18 15:33:24.337867 shipyard_airbyte-0.1.3/README.md
+-rw-r--r--   0        0        0      571 2023-05-16 03:54:15.724326 shipyard_airbyte-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-04-18 15:33:24.339180 shipyard_airbyte-0.1.3/shipyard_airbyte/__init__.py
+-rw-r--r--   0        0        0     4658 2023-05-15 22:33:53.992063 shipyard_airbyte-0.1.3/shipyard_airbyte/airbyte.py
+-rw-r--r--   0        0        0      403 2023-05-10 22:55:38.724312 shipyard_airbyte-0.1.3/shipyard_airbyte/cli/authtest.py
+-rw-r--r--   0        0        0     1196 2023-04-18 15:33:24.339946 shipyard_airbyte-0.1.3/shipyard_airbyte/cli/cli_determine_sync_status.py
+-rw-r--r--   0        0        0     1094 2023-04-18 15:33:24.340255 shipyard_airbyte-0.1.3/shipyard_airbyte/cli/cli_trigger_sync.py
+-rw-r--r--   0        0        0     1526 1970-01-01 00:00:00.000000 shipyard_airbyte-0.1.3/PKG-INFO
```

### Comparing `shipyard_airbyte-0.1.1/README.md` & `shipyard_airbyte-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `shipyard_airbyte-0.1.1/shipyard_airbyte/airbyte.py` & `shipyard_airbyte-0.1.3/shipyard_airbyte/airbyte.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,14 +30,18 @@
             'authorization': f'Bearer {self.access_token}',
             'User-Agent': 'Shipyard User 1.0'
         }
         try:
             response = requests.post(url, json=payload, headers=headers)
             if response.status_code == 200:
                 self.logger.info("Airbyte sync successfully triggered")
+            else:
+                self.logger.warn("Airbyte sync could not be triggerd")
+                self.logger.warn(f"Response from the Airbyte API: {response.json()}")
+                sys.exit(self.EXIT_CODE_SYNC_REFRESH_ERROR)
         except Exception as e:
             self.logger.error(
                 f"Error occurred when attempting to trigger sync. Check to see that the connection id and api token are valid ")
             sys.exit(self.EXIT_CODE_BAD_REQUEST)
         return response
 
     def trigger_sync(self, connection_id: str) -> dict:
@@ -97,8 +101,20 @@
             return self.EXIT_CODE_FINAL_STATUS_ERRORED
         elif job_status == 'succeeded':
             self.logger.info(
                 f"Airbyte job succeeded. Completed at {job_response['lastUpdatedAt']} with {job_response['rowsSynced']} rows synced")
             return self.EXIT_CODE_FINAL_STATUS_COMPLETED
         elif job_status == 'cancelled':
             self.logger.info('Airbyte job was cancelled')
-            return self.EXIT_CODE_SYNC_CANCELLED
+            return self.EXIT_CODE_FINAL_STATUS_CANCELLED 
+
+    def connect(self):
+        """ Connects to the Airbyte API
+
+        Returns: The HTTP response from the API
+            
+        """
+        url = "https://api.airbyte.com/v1/sources"
+        headers = {'authorization': f'Bearer {self.access_token}',
+                   'User-Agent': 'Shipyard User 1.0'}
+        response = requests.get(url, headers=headers)
+        return response.status_code
```

### Comparing `shipyard_airbyte-0.1.1/shipyard_airbyte/cli/cli_determine_sync_status.py` & `shipyard_airbyte-0.1.3/shipyard_airbyte/cli/cli_determine_sync_status.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     artifact_subfolder_paths = shipyard.logs.determine_artifact_subfolders(
         base_folder_name)
     shipyard.logs.create_artifacts_folders(artifact_subfolder_paths)
     # check if a job id was provided, otherwise look for it in the artifact folders
     if job_id is None:
         response = shipyard.logs.read_pickle_file(
             artifact_subfolder_paths, 'sync_response')
-        job_id = response.json()['jobId']
+        job_id = response
     job_status = client.get_sync_status(job_id=job_id)
     sync_status = client.determine_sync_status(job_status)
     sys.exit(sync_status)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_airbyte-0.1.1/shipyard_airbyte/cli/cli_trigger_sync.py` & `shipyard_airbyte-0.1.3/shipyard_airbyte/cli/cli_trigger_sync.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,24 +3,21 @@
 import shipyard_bp_utils as shipyard
 
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("--connection-id", dest='connection_id', required=True)
     parser.add_argument("--api-token", dest='api_token', required=True)
-    parser.add_argument('--check_status', dest='check_status',
-                        default=False, required=False)
     args = parser.parse_args()
     return args
 
 
 def main():
     args = get_args()
     connection_id = args.connection_id
-    check_status = args.check_status
     api_token = args.api_token
     client = AirbyteClient(access_token=api_token)
     resp = client.trigger_sync(
         connection_id=connection_id)
     # create artifacts folder to save response
     base_folder_name = shipyard.logs.determine_base_artifact_folder(
         'airbyte')
```

### Comparing `shipyard_airbyte-0.1.1/PKG-INFO` & `shipyard_airbyte-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: shipyard-airbyte
-Version: 0.1.1
+Version: 0.1.3
 Summary: A local client to work with Airbyte Cloud
 License: Apache-2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pytest (>=7.2.2,<8.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: shipyard-bp-utils (>=0.1.0,<0.2.0)
-Requires-Dist: shipyard-templates (>=0.1.0,<0.2.0)
+Requires-Dist: requests (>=2.28.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # shipyard-airbyte
 
 ## Description 
 A local client to trigger Airbyte syncs and check statuses of past jobs
```

