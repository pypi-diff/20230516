# Comparing `tmp/data_loader_xyz-0.0.1.tar.gz` & `tmp/data_loader_xyz-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_loader_xyz-0.0.1.tar", last modified: Tue May 16 13:46:18 2023, max compression
+gzip compressed data, was "data_loader_xyz-0.0.2.tar", last modified: Tue May 16 14:09:37 2023, max compression
```

## Comparing `data_loader_xyz-0.0.1.tar` & `data_loader_xyz-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 13:46:18.150810 data_loader_xyz-0.0.1/
--rw-rw-r--   0 zied      (1000) zied      (1000)     1073 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.1/LICENCE
--rw-rw-r--   0 zied      (1000) zied      (1000)     4061 2023-05-16 13:46:18.150810 data_loader_xyz-0.0.1/PKG-INFO
--rw-rw-r--   0 zied      (1000) zied      (1000)     3357 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.1/README.md
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 13:46:18.150810 data_loader_xyz-0.0.1/configs/
--rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.1/configs/__init__.py
--rw-rw-r--   0 zied      (1000) zied      (1000)      237 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.1/configs/base_config.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 13:46:18.150810 data_loader_xyz-0.0.1/data_loader_xyz/
--rw-rw-r--   0 zied      (1000) zied      (1000)       51 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.1/data_loader_xyz/__init__.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 13:46:18.150810 data_loader_xyz-0.0.1/data_loader_xyz/src/
--rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.1/data_loader_xyz/src/__init__.py
--rw-rw-r--   0 zied      (1000) zied      (1000)     2418 2023-05-16 11:11:50.000000 data_loader_xyz-0.0.1/data_loader_xyz/src/mount.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 13:46:18.150810 data_loader_xyz-0.0.1/data_loader_xyz.egg-info/
--rw-rw-r--   0 zied      (1000) zied      (1000)     4061 2023-05-16 13:46:18.000000 data_loader_xyz-0.0.1/data_loader_xyz.egg-info/PKG-INFO
--rw-rw-r--   0 zied      (1000) zied      (1000)      444 2023-05-16 13:46:18.000000 data_loader_xyz-0.0.1/data_loader_xyz.egg-info/SOURCES.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)        1 2023-05-16 13:46:18.000000 data_loader_xyz-0.0.1/data_loader_xyz.egg-info/dependency_links.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       62 2023-05-16 13:46:18.000000 data_loader_xyz-0.0.1/data_loader_xyz.egg-info/entry_points.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       34 2023-05-16 13:46:18.000000 data_loader_xyz-0.0.1/data_loader_xyz.egg-info/requires.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       82 2023-05-16 13:46:18.000000 data_loader_xyz-0.0.1/data_loader_xyz.egg-info/top_level.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       79 2023-05-16 13:46:18.150810 data_loader_xyz-0.0.1/setup.cfg
--rw-rw-r--   0 zied      (1000) zied      (1000)     2019 2023-05-16 13:44:07.000000 data_loader_xyz-0.0.1/setup.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 13:46:18.150810 data_loader_xyz-0.0.1/utils/
--rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.1/utils/__init__.py
--rw-rw-r--   0 zied      (1000) zied      (1000)     1758 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.1/utils/util.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 14:09:37.851290 data_loader_xyz-0.0.2/
+-rw-rw-r--   0 zied      (1000) zied      (1000)     1073 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.2/LICENCE
+-rw-rw-r--   0 zied      (1000) zied      (1000)     4061 2023-05-16 14:09:37.851290 data_loader_xyz-0.0.2/PKG-INFO
+-rw-rw-r--   0 zied      (1000) zied      (1000)     3357 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.2/README.md
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 14:09:37.847290 data_loader_xyz-0.0.2/configs/
+-rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.2/configs/__init__.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)      237 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.2/configs/base_config.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 14:09:37.851290 data_loader_xyz-0.0.2/data_loader_xyz/
+-rw-rw-r--   0 zied      (1000) zied      (1000)       51 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.2/data_loader_xyz/__init__.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 14:09:37.851290 data_loader_xyz-0.0.2/data_loader_xyz/src/
+-rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.2/data_loader_xyz/src/__init__.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)     2443 2023-05-16 14:09:36.000000 data_loader_xyz-0.0.2/data_loader_xyz/src/mount.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 14:09:37.851290 data_loader_xyz-0.0.2/data_loader_xyz.egg-info/
+-rw-rw-r--   0 zied      (1000) zied      (1000)     4061 2023-05-16 14:09:37.000000 data_loader_xyz-0.0.2/data_loader_xyz.egg-info/PKG-INFO
+-rw-rw-r--   0 zied      (1000) zied      (1000)      444 2023-05-16 14:09:37.000000 data_loader_xyz-0.0.2/data_loader_xyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)        1 2023-05-16 14:09:37.000000 data_loader_xyz-0.0.2/data_loader_xyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       62 2023-05-16 14:09:37.000000 data_loader_xyz-0.0.2/data_loader_xyz.egg-info/entry_points.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       34 2023-05-16 14:09:37.000000 data_loader_xyz-0.0.2/data_loader_xyz.egg-info/requires.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       82 2023-05-16 14:09:37.000000 data_loader_xyz-0.0.2/data_loader_xyz.egg-info/top_level.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       79 2023-05-16 14:09:37.851290 data_loader_xyz-0.0.2/setup.cfg
+-rw-rw-r--   0 zied      (1000) zied      (1000)     2019 2023-05-16 13:44:07.000000 data_loader_xyz-0.0.2/setup.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 14:09:37.847290 data_loader_xyz-0.0.2/utils/
+-rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.2/utils/__init__.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)     1758 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.2/utils/util.py
```

### Comparing `data_loader_xyz-0.0.1/LICENCE` & `data_loader_xyz-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `data_loader_xyz-0.0.1/PKG-INFO` & `data_loader_xyz-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_loader_xyz
-Version: 0.0.1
+Version: 0.0.2
 Summary: to work with aws S3
 Home-page: https://github.com/Proxia-ai/data_loader
 Author: Zied
 Author-email: ziedici@gmail.com
 License: BSD
 Project-URL: url0, https://github.com/Proxia-ai/
 Keywords: working with aws S3
```

### Comparing `data_loader_xyz-0.0.1/README.md` & `data_loader_xyz-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `data_loader_xyz-0.0.1/data_loader_xyz/src/mount.py` & `data_loader_xyz-0.0.2/data_loader_xyz/src/mount.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,29 +16,29 @@
 
 # import asset config
 yaml_asset_config = read_yaml_data(YAML_CONFIG_FILE_PATH)
 
 # Load crediantials
 credential_file = PROJECT_EMPL + yaml_asset_config[2]["asset_default_data"]["credentials"]
 
-# load params
-bucket_name = yaml_asset_config[1]["asset_parameters"][0]["s3"]["bucket_name"]
-region = yaml_asset_config[1]["asset_parameters"][0]["s3"]["region"]
-
 # Load environement variables
 load_dotenv(credential_file)
 config = dotenv_values(credential_file)
 
 # exporter vos identifiants
 AWS_ACCESS_KEY_ID = config["AWS_ACCESS_KEY"]
 AWS_SECRET_ACCESS_KEY = config["AWS_SECRET_KEY"]
 
 
 @get_log
-def upload_pandas_df(df):
+def upload_pandas_df(df, yaml_file=yaml_asset_config):
+    # load params
+    bucket_name = yaml_file[1]["asset_parameters"][0]["s3"]["bucket_name"]
+    region = yaml_file[1]["asset_parameters"][0]["s3"]["region"]
+
     # creer une session boto3
     session = boto3.session.Session()
 
     # configurer votre client
     s3_client = session.client(
         service_name='s3',
         region_name=region,
```

### Comparing `data_loader_xyz-0.0.1/data_loader_xyz.egg-info/PKG-INFO` & `data_loader_xyz-0.0.2/data_loader_xyz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-loader-xyz
-Version: 0.0.1
+Version: 0.0.2
 Summary: to work with aws S3
 Home-page: https://github.com/Proxia-ai/data_loader
 Author: Zied
 Author-email: ziedici@gmail.com
 License: BSD
 Project-URL: url0, https://github.com/Proxia-ai/
 Keywords: working with aws S3
```

### Comparing `data_loader_xyz-0.0.1/setup.py` & `data_loader_xyz-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `data_loader_xyz-0.0.1/utils/util.py` & `data_loader_xyz-0.0.2/utils/util.py`

 * *Files identical despite different names*

