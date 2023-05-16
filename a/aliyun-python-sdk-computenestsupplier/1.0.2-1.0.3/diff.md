# Comparing `tmp/aliyun-python-sdk-computenestsupplier-1.0.2.tar.gz` & `tmp/aliyun-python-sdk-computenestsupplier-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-computenestsupplier-1.0.2.tar", last modified: Thu Apr 20 09:41:48 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-computenestsupplier-1.0.3.tar", last modified: Tue May 16 05:56:22 2023, max compression
```

## Comparing `aliyun-python-sdk-computenestsupplier-1.0.2.tar` & `aliyun-python-sdk-computenestsupplier-1.0.3.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      575 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1617 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      559 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyun_python_sdk_computenestsupplier.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1617 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyun_python_sdk_computenestsupplier.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1369 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyun_python_sdk_computenestsupplier.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyun_python_sdk_computenestsupplier.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyun_python_sdk_computenestsupplier.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyun_python_sdk_computenestsupplier.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/
--rw-r--r--   0 root         (0) root         (0)     2778 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/CreateArtifactRequest.py
--rw-r--r--   0 root         (0) root         (0)     1708 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/DeleteArtifactRequest.py
--rw-r--r--   0 root         (0) root         (0)     1750 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRepositoryCredentialsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1702 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRequest.py
--rw-r--r--   0 root         (0) root         (0)     1537 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1869 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactVersionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2217 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2845 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2223 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceUsagesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/ReleaseArtifactRequest.py
--rw-r--r--   0 root         (0) root         (0)     2420 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/UpdateArtifactRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2532 2023-04-20 09:41:48.000000 aliyun-python-sdk-computenestsupplier-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      559 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyun_python_sdk_computenestsupplier.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyun_python_sdk_computenestsupplier.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyun_python_sdk_computenestsupplier.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyun_python_sdk_computenestsupplier.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyun_python_sdk_computenestsupplier.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyun_python_sdk_computenestsupplier.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/
+-rw-r--r--   0 root         (0) root         (0)     2778 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/CreateArtifactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6253 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/CreateServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/DeleteArtifactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1750 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRepositoryCredentialsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2536 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceEstimateCostRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactVersionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2217 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2845 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceUsagesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/ListServicesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/ReleaseArtifactRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/UpdateArtifactRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2532 2023-05-16 05:56:22.000000 aliyun-python-sdk-computenestsupplier-1.0.3/setup.py
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.2/LICENSE` & `aliyun-python-sdk-computenestsupplier-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.2/PKG-INFO` & `aliyun-python-sdk-computenestsupplier-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-computenestsupplier
-Version: 1.0.2
+Version: 1.0.3
 Summary: The computenestsupplier module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-computenestsupplier
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.2/README.rst` & `aliyun-python-sdk-computenestsupplier-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.2/aliyun_python_sdk_computenestsupplier.egg-info/PKG-INFO` & `aliyun-python-sdk-computenestsupplier-1.0.3/aliyun_python_sdk_computenestsupplier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-computenestsupplier
-Version: 1.0.2
+Version: 1.0.3
 Summary: The computenestsupplier module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-computenestsupplier
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.2/aliyun_python_sdk_computenestsupplier.egg-info/SOURCES.txt` & `aliyun-python-sdk-computenestsupplier-1.0.3/aliyun_python_sdk_computenestsupplier.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,21 @@
 aliyun_python_sdk_computenestsupplier.egg-info/dependency_links.txt
 aliyun_python_sdk_computenestsupplier.egg-info/requires.txt
 aliyun_python_sdk_computenestsupplier.egg-info/top_level.txt
 aliyunsdkcomputenestsupplier/__init__.py
 aliyunsdkcomputenestsupplier/endpoint.py
 aliyunsdkcomputenestsupplier/request/__init__.py
 aliyunsdkcomputenestsupplier/request/v20210521/CreateArtifactRequest.py
+aliyunsdkcomputenestsupplier/request/v20210521/CreateServiceRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/DeleteArtifactRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRepositoryCredentialsRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRequest.py
+aliyunsdkcomputenestsupplier/request/v20210521/GetServiceEstimateCostRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/GetServiceInstanceRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactVersionsRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactsRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/ListServiceInstancesRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/ListServiceUsagesRequest.py
+aliyunsdkcomputenestsupplier/request/v20210521/ListServicesRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/ReleaseArtifactRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/UpdateArtifactRequest.py
 aliyunsdkcomputenestsupplier/request/v20210521/__init__.py
```

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/endpoint.py` & `aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/CreateArtifactRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/CreateArtifactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/DeleteArtifactRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/DeleteArtifactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRepositoryCredentialsRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRepositoryCredentialsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/GetArtifactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceInstanceRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/GetServiceInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactVersionsRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactVersionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactsRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/ListArtifactsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceInstancesRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceUsagesRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/ListServiceUsagesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/ReleaseArtifactRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/ReleaseArtifactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.2/aliyunsdkcomputenestsupplier/request/v20210521/UpdateArtifactRequest.py` & `aliyun-python-sdk-computenestsupplier-1.0.3/aliyunsdkcomputenestsupplier/request/v20210521/UpdateArtifactRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenestsupplier-1.0.2/setup.py` & `aliyun-python-sdk-computenestsupplier-1.0.3/setup.py`

 * *Files identical despite different names*

