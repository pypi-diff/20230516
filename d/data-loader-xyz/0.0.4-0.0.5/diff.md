# Comparing `tmp/data_loader_xyz-0.0.4.tar.gz` & `tmp/data_loader_xyz-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_loader_xyz-0.0.4.tar", last modified: Tue May 16 16:12:07 2023, max compression
+gzip compressed data, was "data_loader_xyz-0.0.5.tar", last modified: Tue May 16 16:50:41 2023, max compression
```

## Comparing `data_loader_xyz-0.0.4.tar` & `data_loader_xyz-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 16:12:07.901656 data_loader_xyz-0.0.4/
--rw-rw-r--   0 zied      (1000) zied      (1000)     1073 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.4/LICENCE
--rw-rw-r--   0 zied      (1000) zied      (1000)     4061 2023-05-16 16:12:07.901656 data_loader_xyz-0.0.4/PKG-INFO
--rw-rw-r--   0 zied      (1000) zied      (1000)     3357 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.4/README.md
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 16:12:07.897656 data_loader_xyz-0.0.4/configs/
--rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.4/configs/__init__.py
--rw-rw-r--   0 zied      (1000) zied      (1000)      237 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.4/configs/base_config.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 16:12:07.897656 data_loader_xyz-0.0.4/data_loader_xyz/
--rw-rw-r--   0 zied      (1000) zied      (1000)       51 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.4/data_loader_xyz/__init__.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 16:12:07.901656 data_loader_xyz-0.0.4/data_loader_xyz/src/
--rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.4/data_loader_xyz/src/__init__.py
--rw-rw-r--   0 zied      (1000) zied      (1000)     4877 2023-05-16 16:11:56.000000 data_loader_xyz-0.0.4/data_loader_xyz/src/mount.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 16:12:07.901656 data_loader_xyz-0.0.4/data_loader_xyz.egg-info/
--rw-rw-r--   0 zied      (1000) zied      (1000)     4061 2023-05-16 16:12:07.000000 data_loader_xyz-0.0.4/data_loader_xyz.egg-info/PKG-INFO
--rw-rw-r--   0 zied      (1000) zied      (1000)      444 2023-05-16 16:12:07.000000 data_loader_xyz-0.0.4/data_loader_xyz.egg-info/SOURCES.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)        1 2023-05-16 16:12:07.000000 data_loader_xyz-0.0.4/data_loader_xyz.egg-info/dependency_links.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       62 2023-05-16 16:12:07.000000 data_loader_xyz-0.0.4/data_loader_xyz.egg-info/entry_points.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       34 2023-05-16 16:12:07.000000 data_loader_xyz-0.0.4/data_loader_xyz.egg-info/requires.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       82 2023-05-16 16:12:07.000000 data_loader_xyz-0.0.4/data_loader_xyz.egg-info/top_level.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       79 2023-05-16 16:12:07.901656 data_loader_xyz-0.0.4/setup.cfg
--rw-rw-r--   0 zied      (1000) zied      (1000)     2019 2023-05-16 13:44:07.000000 data_loader_xyz-0.0.4/setup.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 16:12:07.897656 data_loader_xyz-0.0.4/utils/
--rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.4/utils/__init__.py
--rw-rw-r--   0 zied      (1000) zied      (1000)     1758 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.4/utils/util.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 16:50:41.411272 data_loader_xyz-0.0.5/
+-rw-rw-r--   0 zied      (1000) zied      (1000)     1073 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.5/LICENCE
+-rw-rw-r--   0 zied      (1000) zied      (1000)     4061 2023-05-16 16:50:41.411272 data_loader_xyz-0.0.5/PKG-INFO
+-rw-rw-r--   0 zied      (1000) zied      (1000)     3357 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.5/README.md
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 16:50:41.407272 data_loader_xyz-0.0.5/configs/
+-rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.5/configs/__init__.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)      237 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.5/configs/base_config.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 16:50:41.407272 data_loader_xyz-0.0.5/data_loader_xyz/
+-rw-rw-r--   0 zied      (1000) zied      (1000)       51 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.5/data_loader_xyz/__init__.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 16:50:41.411272 data_loader_xyz-0.0.5/data_loader_xyz/src/
+-rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.5/data_loader_xyz/src/__init__.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)     4453 2023-05-16 16:49:11.000000 data_loader_xyz-0.0.5/data_loader_xyz/src/mount.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 16:50:41.407272 data_loader_xyz-0.0.5/data_loader_xyz.egg-info/
+-rw-rw-r--   0 zied      (1000) zied      (1000)     4061 2023-05-16 16:50:41.000000 data_loader_xyz-0.0.5/data_loader_xyz.egg-info/PKG-INFO
+-rw-rw-r--   0 zied      (1000) zied      (1000)      444 2023-05-16 16:50:41.000000 data_loader_xyz-0.0.5/data_loader_xyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)        1 2023-05-16 16:50:41.000000 data_loader_xyz-0.0.5/data_loader_xyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       62 2023-05-16 16:50:41.000000 data_loader_xyz-0.0.5/data_loader_xyz.egg-info/entry_points.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       34 2023-05-16 16:50:41.000000 data_loader_xyz-0.0.5/data_loader_xyz.egg-info/requires.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       82 2023-05-16 16:50:41.000000 data_loader_xyz-0.0.5/data_loader_xyz.egg-info/top_level.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       79 2023-05-16 16:50:41.411272 data_loader_xyz-0.0.5/setup.cfg
+-rw-rw-r--   0 zied      (1000) zied      (1000)     2019 2023-05-16 13:44:07.000000 data_loader_xyz-0.0.5/setup.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 16:50:41.407272 data_loader_xyz-0.0.5/utils/
+-rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.5/utils/__init__.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)     1758 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.5/utils/util.py
```

### Comparing `data_loader_xyz-0.0.4/LICENCE` & `data_loader_xyz-0.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `data_loader_xyz-0.0.4/PKG-INFO` & `data_loader_xyz-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_loader_xyz
-Version: 0.0.4
+Version: 0.0.5
 Summary: to work with aws S3
 Home-page: https://github.com/Proxia-ai/data_loader
 Author: Zied
 Author-email: ziedici@gmail.com
 License: BSD
 Project-URL: url0, https://github.com/Proxia-ai/
 Keywords: working with aws S3
```

### Comparing `data_loader_xyz-0.0.4/README.md` & `data_loader_xyz-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `data_loader_xyz-0.0.4/data_loader_xyz/src/mount.py` & `data_loader_xyz-0.0.5/data_loader_xyz/src/mount.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # importer les librairies
 import boto3
 import io
 import pandas as pd
 import time
 from dotenv import load_dotenv, dotenv_values
+from boto3.session import Session
 
 # import internal packages
 from utils.util import read_yaml_data, get_log
 from configs import base_config
 
 # import config emplacement files of the project
 PROJECT_EMPL = base_config.project_empl
@@ -67,71 +68,51 @@
                 status = f"Successful S3 put_object response. Status - {status}"
             else:
                 status = f"Unsuccessful S3 put_object response. Status - {status}"
             print(status)
             return status
 
     @get_log
-    def download_file(self, file_name_on_s3, local_file_emplacement):
+    def download_file(self, file_name_on_s3, local_folder_emplacement):
         # creer une session boto3
-        session = boto3.session.Session()
-
-        # configurer votre client
-        s3_client = session.client(
-            service_name='s3',
-            region_name=self.region,
-            use_ssl=False,
-            aws_access_key_id=self.AWS_ACCESS_KEY_ID,
-            aws_secret_access_key=self.AWS_SECRET_ACCESS_KEY
-        )
-
-        response = s3_client.resource('s3').Bucket(self.bucket_name).download_file(file_name_on_s3,
-                                                                                   local_file_emplacement)
-
-        # Avoir la reponse
-        status = response.get("ResponseMetadata", {}).get("HTTPStatusCode")
-
-        # Afficher la reponse
-        if status == 200:
-            status = f"Successful S3 download_file response. Status - {status}"
-        else:
-            status = f"Unsuccessful S3 download_file response. Status - {status}"
-        print(status)
-        return status
+        session = Session(aws_access_key_id=self.AWS_ACCESS_KEY_ID,
+                          aws_secret_access_key=self.AWS_SECRET_ACCESS_KEY,
+                          region_name=self.region,
+                          )
+
+        # session is authenticated and can access the resource in question
+        try:
+            session.resource('s3').Bucket(self.bucket_name).download_file(file_name_on_s3,
+                                                                          local_folder_emplacement + str(
+                                                                              file_name_on_s3))
+            msg = "successful Download"
+        except Exception as e:
+            msg = "Unsuccessful Download with error: {}".format(e)
+        print(msg)
+        return msg
 
     @get_log
     def upload_file(self, local_file_emplacement, file_name_on_s3):
         # creer une session boto3
-        session = boto3.session.Session()
-
-        # configurer votre client
-        s3_client = session.client(
-            service_name='s3',
-            region_name=self.region,
-            use_ssl=False,
-            aws_access_key_id=self.AWS_ACCESS_KEY_ID,
-            aws_secret_access_key=self.AWS_SECRET_ACCESS_KEY
-        )
-
-        response = s3_client.resource('s3').Bucket(self.bucket_name).upload_file(local_file_emplacement,
-                                                                                 file_name_on_s3)
-
-        # Avoir la reponse
-        status = response.get("ResponseMetadata", {}).get("HTTPStatusCode")
-
-        # Afficher la reponse
-        if status == 200:
-            status = f"Successful S3 upload_file response. Status - {status}"
-        else:
-            status = f"Unsuccessful S3 upload_file response. Status - {status}"
-        print(status)
-        return status
+        session = Session(aws_access_key_id=self.AWS_ACCESS_KEY_ID,
+                          aws_secret_access_key=self.AWS_SECRET_ACCESS_KEY,
+                          region_name=self.region,
+                          )
+
+        # session is authenticated and can access the resource in question
+        try:
+            session.resource('s3').Bucket(self.bucket_name).upload_file(local_file_emplacement, file_name_on_s3)
+            msg = "successful upload"
+        except Exception as e:
+            msg = "Unsuccessful upload with error: {}".format(e)
+        print(msg)
+        return msg
 
 
 if __name__ == "__main__":
     YAML_CONFIG_FILE_PATH = base_config.yaml_config_empl
-    _mount = _mount(YAML_CONFIG_FILE_PATH)
+    mount = _mount(YAML_CONFIG_FILE_PATH)
     books_df = pd.DataFrame(
         data={"Title": ["Book I", "Book II", "Book III"], "Price": [56.6, 59.87, 74.54]},
         columns=["Title", "Price"],
     )
-    _mount.upload_pandas_df(books_df)
+    mount.upload_pandas_df(books_df)
```

### Comparing `data_loader_xyz-0.0.4/data_loader_xyz.egg-info/PKG-INFO` & `data_loader_xyz-0.0.5/data_loader_xyz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-loader-xyz
-Version: 0.0.4
+Version: 0.0.5
 Summary: to work with aws S3
 Home-page: https://github.com/Proxia-ai/data_loader
 Author: Zied
 Author-email: ziedici@gmail.com
 License: BSD
 Project-URL: url0, https://github.com/Proxia-ai/
 Keywords: working with aws S3
```

### Comparing `data_loader_xyz-0.0.4/setup.py` & `data_loader_xyz-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `data_loader_xyz-0.0.4/utils/util.py` & `data_loader_xyz-0.0.5/utils/util.py`

 * *Files identical despite different names*

