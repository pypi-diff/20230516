# Comparing `tmp/dlhub_sdk-2.0.2.tar.gz` & `tmp/dlhub_sdk-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlhub_sdk-2.0.2.tar", last modified: Thu Apr 27 21:08:06 2023, max compression
+gzip compressed data, was "dlhub_sdk-2.0.3.tar", last modified: Tue May 16 18:24:52 2023, max compression
```

## Comparing `dlhub_sdk-2.0.2.tar` & `dlhub_sdk-2.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:08:06.376782 dlhub_sdk-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-27 21:08:06.376782 dlhub_sdk-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:08:06.372782 dlhub_sdk-2.0.2/dlhub_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/dlhub_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33939 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/dlhub_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/dlhub_sdk/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:08:06.372782 dlhub_sdk-2.0.2/dlhub_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (123)    18602 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/dlhub_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19337 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/dlhub_sdk/models/datacite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:08:06.372782 dlhub_sdk-2.0.2/dlhub_sdk/models/servables/
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/dlhub_sdk/models/servables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/dlhub_sdk/models/servables/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/dlhub_sdk/models/servables/python.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/dlhub_sdk/models/servables/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/dlhub_sdk/models/servables/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/dlhub_sdk/models/servables/tensorflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:08:06.376782 dlhub_sdk-2.0.2/dlhub_sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/dlhub_sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/dlhub_sdk/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/dlhub_sdk/utils/funcx_login_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/dlhub_sdk/utils/futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/dlhub_sdk/utils/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/dlhub_sdk/utils/publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/dlhub_sdk/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/dlhub_sdk/utils/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/dlhub_sdk/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/dlhub_sdk/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/dlhub_sdk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:08:06.372782 dlhub_sdk-2.0.2/dlhub_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-27 21:08:06.000000 dlhub_sdk-2.0.2/dlhub_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-27 21:08:06.000000 dlhub_sdk-2.0.2/dlhub_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:08:06.000000 dlhub_sdk-2.0.2/dlhub_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-27 21:08:06.000000 dlhub_sdk-2.0.2/dlhub_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 21:08:06.000000 dlhub_sdk-2.0.2/dlhub_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-27 21:08:06.376782 dlhub_sdk-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-27 21:07:57.000000 dlhub_sdk-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:24:52.104308 dlhub_sdk-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-16 18:24:52.104308 dlhub_sdk-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:24:52.104308 dlhub_sdk-2.0.3/dlhub_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/dlhub_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33939 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/dlhub_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/dlhub_sdk/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:24:52.104308 dlhub_sdk-2.0.3/dlhub_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    18602 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/dlhub_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19337 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/dlhub_sdk/models/datacite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:24:52.104308 dlhub_sdk-2.0.3/dlhub_sdk/models/servables/
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/dlhub_sdk/models/servables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/dlhub_sdk/models/servables/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/dlhub_sdk/models/servables/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/dlhub_sdk/models/servables/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/dlhub_sdk/models/servables/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/dlhub_sdk/models/servables/tensorflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:24:52.104308 dlhub_sdk-2.0.3/dlhub_sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/dlhub_sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/dlhub_sdk/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/dlhub_sdk/utils/funcx_login_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/dlhub_sdk/utils/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/dlhub_sdk/utils/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/dlhub_sdk/utils/publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/dlhub_sdk/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/dlhub_sdk/utils/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/dlhub_sdk/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/dlhub_sdk/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/dlhub_sdk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:24:52.104308 dlhub_sdk-2.0.3/dlhub_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-16 18:24:52.000000 dlhub_sdk-2.0.3/dlhub_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-16 18:24:52.000000 dlhub_sdk-2.0.3/dlhub_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:24:52.000000 dlhub_sdk-2.0.3/dlhub_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-16 18:24:52.000000 dlhub_sdk-2.0.3/dlhub_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 18:24:52.000000 dlhub_sdk-2.0.3/dlhub_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-16 18:24:52.108307 dlhub_sdk-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-16 18:24:44.000000 dlhub_sdk-2.0.3/setup.py
```

### Comparing `dlhub_sdk-2.0.2/LICENSE` & `dlhub_sdk-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-2.0.2/PKG-INFO` & `dlhub_sdk-2.0.3/dlhub_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dlhub_sdk
-Version: 2.0.2
+Name: dlhub-sdk
+Version: 2.0.3
 Summary: Python interface and utilities for DLHub
 Home-page: https://github.com/DLHub-Argonne/dlhub_sdk
 Author: Ben Blaiszik
 Author-email: bblaiszik@anl.gov
 License: Apache License, Version 2.0
 Keywords: DLHub,Data and Learning Hub for Science,machine learning,data publication,reproducibility
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dlhub_sdk-2.0.2/README.md` & `dlhub_sdk-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-2.0.2/dlhub_sdk/client.py` & `dlhub_sdk-2.0.3/dlhub_sdk/client.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-2.0.2/dlhub_sdk/config.py` & `dlhub_sdk-2.0.3/dlhub_sdk/config.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-2.0.2/dlhub_sdk/models/__init__.py` & `dlhub_sdk-2.0.3/dlhub_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-2.0.2/dlhub_sdk/models/datacite.py` & `dlhub_sdk-2.0.3/dlhub_sdk/models/datacite.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-2.0.2/dlhub_sdk/models/servables/__init__.py` & `dlhub_sdk-2.0.3/dlhub_sdk/models/servables/__init__.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-2.0.2/dlhub_sdk/models/servables/keras.py` & `dlhub_sdk-2.0.3/dlhub_sdk/models/servables/keras.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-2.0.2/dlhub_sdk/models/servables/python.py` & `dlhub_sdk-2.0.3/dlhub_sdk/models/servables/python.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-2.0.2/dlhub_sdk/models/servables/pytorch.py` & `dlhub_sdk-2.0.3/dlhub_sdk/models/servables/pytorch.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-2.0.2/dlhub_sdk/models/servables/sklearn.py` & `dlhub_sdk-2.0.3/dlhub_sdk/models/servables/sklearn.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-2.0.2/dlhub_sdk/models/servables/tensorflow.py` & `dlhub_sdk-2.0.3/dlhub_sdk/models/servables/tensorflow.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-2.0.2/dlhub_sdk/utils/__init__.py` & `dlhub_sdk-2.0.3/dlhub_sdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-2.0.2/dlhub_sdk/utils/funcx_login_manager.py` & `dlhub_sdk-2.0.3/dlhub_sdk/utils/funcx_login_manager.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-2.0.2/dlhub_sdk/utils/futures.py` & `dlhub_sdk-2.0.3/dlhub_sdk/utils/futures.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-2.0.2/dlhub_sdk/utils/inspect.py` & `dlhub_sdk-2.0.3/dlhub_sdk/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-2.0.2/dlhub_sdk/utils/publish.py` & `dlhub_sdk-2.0.3/dlhub_sdk/utils/publish.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,24 @@
     try:
         for k, v in metadata['dlhub']['dependencies']['python'].items():
             dependencies.append("{0}=={1}".format(k, v))
     except Exception:
         # There are no python dependencies
         pass
 
+    # If there's a requirements.txt in the payload, add it to the dependencies
+    fileslist = []
+    try:
+        fileslist = metadata['dlhub']['files']['other']
+    except KeyError:
+        pass
+
+    if 'requirements.txt' in fileslist:
+        dependencies.append("--requirement requirements.txt")
+
     model_location = None
     # If the model was uploaded using a signed URL, it will have a
     # transfer_method of S3 in its metadata.
     # If the model is being built from a repo, it will not have a
     # transfer_method, but will have a 'repository'
     if 'transfer_method' in metadata['dlhub']:
         if 'S3' in metadata['dlhub']['transfer_method']:
```

### Comparing `dlhub_sdk-2.0.2/dlhub_sdk/utils/schemas.py` & `dlhub_sdk-2.0.3/dlhub_sdk/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-2.0.2/dlhub_sdk/utils/search.py` & `dlhub_sdk-2.0.3/dlhub_sdk/utils/search.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-2.0.2/dlhub_sdk/utils/types.py` & `dlhub_sdk-2.0.3/dlhub_sdk/utils/types.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-2.0.2/dlhub_sdk/utils/validation.py` & `dlhub_sdk-2.0.3/dlhub_sdk/utils/validation.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-2.0.2/dlhub_sdk.egg-info/PKG-INFO` & `dlhub_sdk-2.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dlhub-sdk
-Version: 2.0.2
+Name: dlhub_sdk
+Version: 2.0.3
 Summary: Python interface and utilities for DLHub
 Home-page: https://github.com/DLHub-Argonne/dlhub_sdk
 Author: Ben Blaiszik
 Author-email: bblaiszik@anl.gov
 License: Apache License, Version 2.0
 Keywords: DLHub,Data and Learning Hub for Science,machine learning,data publication,reproducibility
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dlhub_sdk-2.0.2/dlhub_sdk.egg-info/SOURCES.txt` & `dlhub_sdk-2.0.3/dlhub_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-2.0.2/setup.py` & `dlhub_sdk-2.0.3/setup.py`

 * *Files identical despite different names*

