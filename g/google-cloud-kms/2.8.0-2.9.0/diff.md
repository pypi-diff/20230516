# Comparing `tmp/google-cloud-kms-2.8.0.tar.gz` & `tmp/google-cloud-kms-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/google-cloud-kms-2.8.0.tar", last modified: Thu Sep 30 21:02:50 2021, max compression
+gzip compressed data, was "google-cloud-kms-2.9.0.tar", last modified: Tue Oct 12 17:36:34 2021, max compression
```

## Comparing `google-cloud-kms-2.8.0.tar` & `google-cloud-kms-2.9.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 21:02:50.413723 google-cloud-kms-2.8.0/
--rw-rw-r--   0 root         (0)     1003    11358 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     3811 2021-09-30 21:02:50.413723 google-cloud-kms-2.8.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     2966 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 21:02:50.405719 google-cloud-kms-2.8.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 21:02:50.405719 google-cloud-kms-2.8.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 21:02:50.409721 google-cloud-kms-2.8.0/google/cloud/kms/
--rw-rw-r--   0 root         (0)     1003     5533 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/google/cloud/kms/__init__.py
--rw-rw-r--   0 root         (0)     1003       77 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/google/cloud/kms/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 21:02:50.409721 google-cloud-kms-2.8.0/google/cloud/kms_v1/
--rw-rw-r--   0 root         (0)     1003     4545 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/google/cloud/kms_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     7221 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/google/cloud/kms_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       77 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/google/cloud/kms_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 21:02:50.409721 google-cloud-kms-2.8.0/google/cloud/kms_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/google/cloud/kms_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 21:02:50.409721 google-cloud-kms-2.8.0/google/cloud/kms_v1/services/key_management_service/
--rw-rw-r--   0 root         (0)     1003      793 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/google/cloud/kms_v1/services/key_management_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   134307 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/google/cloud/kms_v1/services/key_management_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   141611 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/google/cloud/kms_v1/services/key_management_service/client.py
--rw-rw-r--   0 root         (0)     1003    20716 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/google/cloud/kms_v1/services/key_management_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 21:02:50.409721 google-cloud-kms-2.8.0/google/cloud/kms_v1/services/key_management_service/transports/
--rw-rw-r--   0 root         (0)     1003     1256 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/google/cloud/kms_v1/services/key_management_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    28583 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/google/cloud/kms_v1/services/key_management_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    49917 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/google/cloud/kms_v1/services/key_management_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    51062 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/google/cloud/kms_v1/services/key_management_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 21:02:50.409721 google-cloud-kms-2.8.0/google/cloud/kms_v1/types/
--rw-rw-r--   0 root         (0)     1003     3299 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/google/cloud/kms_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    32527 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/google/cloud/kms_v1/types/resources.py
--rw-rw-r--   0 root         (0)     1003    72715 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/google/cloud/kms_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 21:02:50.413723 google-cloud-kms-2.8.0/google_cloud_kms.egg-info/
--rw-r--r--   0 root         (0)     1003     3811 2021-09-30 21:02:50.000000 google-cloud-kms-2.8.0/google_cloud_kms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1421 2021-09-30 21:02:50.000000 google-cloud-kms-2.8.0/google_cloud_kms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2021-09-30 21:02:50.000000 google-cloud-kms-2.8.0/google_cloud_kms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2021-09-30 21:02:50.000000 google-cloud-kms-2.8.0/google_cloud_kms.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2021-09-30 21:02:50.000000 google-cloud-kms-2.8.0/google_cloud_kms.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      134 2021-09-30 21:02:50.000000 google-cloud-kms-2.8.0/google_cloud_kms.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2021-09-30 21:02:50.000000 google-cloud-kms-2.8.0/google_cloud_kms.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 21:02:50.413723 google-cloud-kms-2.8.0/scripts/
--rw-rw-r--   0 root         (0)     1003     8039 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/scripts/fixup_kms_v1_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2021-09-30 21:02:50.413723 google-cloud-kms-2.8.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2750 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 21:02:50.413723 google-cloud-kms-2.8.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 21:02:50.413723 google-cloud-kms-2.8.0/tests/system/
--rw-rw-r--   0 root         (0)     1003     1003 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/tests/system/test_system.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 21:02:50.413723 google-cloud-kms-2.8.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 21:02:50.413723 google-cloud-kms-2.8.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2021-09-30 21:02:50.413723 google-cloud-kms-2.8.0/tests/unit/gapic/kms_v1/
--rw-rw-r--   0 root         (0)     1003      600 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/tests/unit/gapic/kms_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   323553 2021-09-30 21:00:12.000000 google-cloud-kms-2.8.0/tests/unit/gapic/kms_v1/test_key_management_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-12 17:36:34.570785 google-cloud-kms-2.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     3811 2021-10-12 17:36:34.570785 google-cloud-kms-2.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     2966 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-12 17:36:34.562785 google-cloud-kms-2.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-12 17:36:34.562785 google-cloud-kms-2.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-12 17:36:34.562785 google-cloud-kms-2.9.0/google/cloud/kms/
+-rw-rw-r--   0 root         (0)     1003     5533 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/google/cloud/kms/__init__.py
+-rw-rw-r--   0 root         (0)     1003       77 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/google/cloud/kms/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-12 17:36:34.566785 google-cloud-kms-2.9.0/google/cloud/kms_v1/
+-rw-rw-r--   0 root         (0)     1003     4545 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/google/cloud/kms_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7221 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/google/cloud/kms_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       77 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/google/cloud/kms_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-12 17:36:34.566785 google-cloud-kms-2.9.0/google/cloud/kms_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/google/cloud/kms_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-12 17:36:34.566785 google-cloud-kms-2.9.0/google/cloud/kms_v1/services/key_management_service/
+-rw-rw-r--   0 root         (0)     1003      793 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/google/cloud/kms_v1/services/key_management_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   134448 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/google/cloud/kms_v1/services/key_management_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   141859 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/google/cloud/kms_v1/services/key_management_service/client.py
+-rw-rw-r--   0 root         (0)     1003    20716 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/google/cloud/kms_v1/services/key_management_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-12 17:36:34.566785 google-cloud-kms-2.9.0/google/cloud/kms_v1/services/key_management_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1256 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/google/cloud/kms_v1/services/key_management_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    28871 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/google/cloud/kms_v1/services/key_management_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    49973 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/google/cloud/kms_v1/services/key_management_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    51125 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/google/cloud/kms_v1/services/key_management_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-12 17:36:34.566785 google-cloud-kms-2.9.0/google/cloud/kms_v1/types/
+-rw-rw-r--   0 root         (0)     1003     3299 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/google/cloud/kms_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    32527 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/google/cloud/kms_v1/types/resources.py
+-rw-rw-r--   0 root         (0)     1003    72715 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/google/cloud/kms_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-12 17:36:34.570785 google-cloud-kms-2.9.0/google_cloud_kms.egg-info/
+-rw-r--r--   0 root         (0)     1003     3811 2021-10-12 17:36:34.000000 google-cloud-kms-2.9.0/google_cloud_kms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1421 2021-10-12 17:36:34.000000 google-cloud-kms-2.9.0/google_cloud_kms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2021-10-12 17:36:34.000000 google-cloud-kms-2.9.0/google_cloud_kms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2021-10-12 17:36:34.000000 google-cloud-kms-2.9.0/google_cloud_kms.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2021-10-12 17:36:34.000000 google-cloud-kms-2.9.0/google_cloud_kms.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      134 2021-10-12 17:36:34.000000 google-cloud-kms-2.9.0/google_cloud_kms.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2021-10-12 17:36:34.000000 google-cloud-kms-2.9.0/google_cloud_kms.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-12 17:36:34.570785 google-cloud-kms-2.9.0/scripts/
+-rw-rw-r--   0 root         (0)     1003     8039 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/scripts/fixup_kms_v1_keywords.py
+-rw-rw-r--   0 root         (0)     1003       67 2021-10-12 17:36:34.570785 google-cloud-kms-2.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2750 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-12 17:36:34.570785 google-cloud-kms-2.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-12 17:36:34.570785 google-cloud-kms-2.9.0/tests/system/
+-rw-rw-r--   0 root         (0)     1003     1003 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/tests/system/test_system.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-12 17:36:34.570785 google-cloud-kms-2.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-12 17:36:34.570785 google-cloud-kms-2.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2021-10-12 17:36:34.570785 google-cloud-kms-2.9.0/tests/unit/gapic/kms_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/tests/unit/gapic/kms_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   325058 2021-10-12 17:33:51.000000 google-cloud-kms-2.9.0/tests/unit/gapic/kms_v1/test_key_management_service.py
```

### Comparing `google-cloud-kms-2.8.0/LICENSE` & `google-cloud-kms-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-2.8.0/MANIFEST.in` & `google-cloud-kms-2.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-2.8.0/PKG-INFO` & `google-cloud-kms-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-kms
-Version: 2.8.0
+Version: 2.9.0
 Summary: Cloud Key Management Service (KMS) API client library
 Home-page: https://github.com/googleapis/python-kms
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-kms-2.8.0/README.rst` & `google-cloud-kms-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-2.8.0/google/cloud/kms/__init__.py` & `google-cloud-kms-2.9.0/google/cloud/kms/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-2.8.0/google/cloud/kms_v1/__init__.py` & `google-cloud-kms-2.9.0/google/cloud/kms_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-2.8.0/google/cloud/kms_v1/gapic_metadata.json` & `google-cloud-kms-2.9.0/google/cloud/kms_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-2.8.0/google/cloud/kms_v1/services/__init__.py` & `google-cloud-kms-2.9.0/google/cloud/kms_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-2.8.0/google/cloud/kms_v1/services/key_management_service/__init__.py` & `google-cloud-kms-2.9.0/google/cloud/kms_v1/services/key_management_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-2.8.0/google/cloud/kms_v1/services/key_management_service/async_client.py` & `google-cloud-kms-2.9.0/google/cloud/kms_v1/services/key_management_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3144,14 +3144,20 @@
 
         # Send the request.
         response = await rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
 
         # Done; return the response.
         return response
 
+    async def __aenter__(self):
+        return self
+
+    async def __aexit__(self, exc_type, exc, tb):
+        await self.transport.close()
+
 
 try:
     DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
         gapic_version=pkg_resources.get_distribution("google-cloud-kms",).version,
     )
 except pkg_resources.DistributionNotFound:
     DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo()
```

### Comparing `google-cloud-kms-2.8.0/google/cloud/kms_v1/services/key_management_service/client.py` & `google-cloud-kms-2.9.0/google/cloud/kms_v1/services/key_management_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,18 +460,15 @@
                 credentials=credentials,
                 credentials_file=client_options.credentials_file,
                 host=api_endpoint,
                 scopes=client_options.scopes,
                 client_cert_source_for_mtls=client_cert_source_func,
                 quota_project_id=client_options.quota_project_id,
                 client_info=client_info,
-                always_use_jwt_access=(
-                    Transport == type(self).get_transport_class("grpc")
-                    or Transport == type(self).get_transport_class("grpc_asyncio")
-                ),
+                always_use_jwt_access=True,
             )
 
     def list_key_rings(
         self,
         request: Union[service.ListKeyRingsRequest, dict] = None,
         *,
         parent: str = None,
@@ -2905,14 +2902,27 @@
 
         # Send the request.
         response = rpc(request, retry=retry, timeout=timeout, metadata=metadata,)
 
         # Done; return the response.
         return response
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, type, value, traceback):
+        """Releases underlying transport's resources.
+
+        .. warning::
+            ONLY use as a context manager if the transport is NOT shared
+            with other clients! Exiting the with block will CLOSE the transport
+            and may cause errors in other clients!
+        """
+        self.transport.close()
+
     def set_iam_policy(
         self,
         request: iam_policy_pb2.SetIamPolicyRequest = None,
         *,
         retry: retries.Retry = gapic_v1.method.DEFAULT,
         timeout: float = None,
         metadata: Sequence[Tuple[str, str]] = (),
```

### Comparing `google-cloud-kms-2.8.0/google/cloud/kms_v1/services/key_management_service/pagers.py` & `google-cloud-kms-2.9.0/google/cloud/kms_v1/services/key_management_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-2.8.0/google/cloud/kms_v1/services/key_management_service/transports/__init__.py` & `google-cloud-kms-2.9.0/google/cloud/kms_v1/services/key_management_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-2.8.0/google/cloud/kms_v1/services/key_management_service/transports/base.py` & `google-cloud-kms-2.9.0/google/cloud/kms_v1/services/key_management_service/transports/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -526,14 +526,23 @@
                     deadline=60.0,
                 ),
                 default_timeout=60.0,
                 client_info=client_info,
             ),
         }
 
+    def close(self):
+        """Closes resources associated with the transport.
+
+       .. warning::
+            Only call this method if the transport is NOT shared
+            with other clients - this may cause errors in other clients!
+        """
+        raise NotImplementedError()
+
     @property
     def list_key_rings(
         self,
     ) -> Callable[
         [service.ListKeyRingsRequest],
         Union[service.ListKeyRingsResponse, Awaitable[service.ListKeyRingsResponse]],
     ]:
```

### Comparing `google-cloud-kms-2.8.0/google/cloud/kms_v1/services/key_management_service/transports/grpc.py` & `google-cloud-kms-2.9.0/google/cloud/kms_v1/services/key_management_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1109,9 +1109,12 @@
             self._stubs["test_iam_permissions"] = self.grpc_channel.unary_unary(
                 "/google.iam.v1.IAMPolicy/TestIamPermissions",
                 request_serializer=iam_policy_pb2.TestIamPermissionsRequest.SerializeToString,
                 response_deserializer=iam_policy_pb2.TestIamPermissionsResponse.FromString,
             )
         return self._stubs["test_iam_permissions"]
 
+    def close(self):
+        self.grpc_channel.close()
+
 
 __all__ = ("KeyManagementServiceGrpcTransport",)
```

### Comparing `google-cloud-kms-2.8.0/google/cloud/kms_v1/services/key_management_service/transports/grpc_asyncio.py` & `google-cloud-kms-2.9.0/google/cloud/kms_v1/services/key_management_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1144,9 +1144,12 @@
             self._stubs["test_iam_permissions"] = self.grpc_channel.unary_unary(
                 "/google.iam.v1.IAMPolicy/TestIamPermissions",
                 request_serializer=iam_policy_pb2.TestIamPermissionsRequest.SerializeToString,
                 response_deserializer=iam_policy_pb2.TestIamPermissionsResponse.FromString,
             )
         return self._stubs["test_iam_permissions"]
 
+    def close(self):
+        return self.grpc_channel.close()
+
 
 __all__ = ("KeyManagementServiceGrpcAsyncIOTransport",)
```

### Comparing `google-cloud-kms-2.8.0/google/cloud/kms_v1/types/__init__.py` & `google-cloud-kms-2.9.0/google/cloud/kms_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-2.8.0/google/cloud/kms_v1/types/resources.py` & `google-cloud-kms-2.9.0/google/cloud/kms_v1/types/resources.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-2.8.0/google/cloud/kms_v1/types/service.py` & `google-cloud-kms-2.9.0/google/cloud/kms_v1/types/service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-2.8.0/google_cloud_kms.egg-info/PKG-INFO` & `google-cloud-kms-2.9.0/google_cloud_kms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-kms
-Version: 2.8.0
+Version: 2.9.0
 Summary: Cloud Key Management Service (KMS) API client library
 Home-page: https://github.com/googleapis/python-kms
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-kms-2.8.0/google_cloud_kms.egg-info/SOURCES.txt` & `google-cloud-kms-2.9.0/google_cloud_kms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-2.8.0/scripts/fixup_kms_v1_keywords.py` & `google-cloud-kms-2.9.0/scripts/fixup_kms_v1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-2.8.0/setup.py` & `google-cloud-kms-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import io
 import os
 
 import setuptools
 
 name = "google-cloud-kms"
 description = "Cloud Key Management Service (KMS) API client library"
-version = "2.8.0"
+version = "2.9.0"
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     # NOTE: Maintainers, please do not require google-api-core>=2.x.x
     # Until this issue is closed
     # https://github.com/googleapis/google-cloud-python/issues/10566
     "google-api-core[grpc] >= 1.26.0, <3.0.0dev",
     "grpc-google-iam-v1 >= 0.12.3, < 0.13dev",
```

### Comparing `google-cloud-kms-2.8.0/tests/__init__.py` & `google-cloud-kms-2.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-2.8.0/tests/system/test_system.py` & `google-cloud-kms-2.9.0/tests/system/test_system.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-2.8.0/tests/unit/__init__.py` & `google-cloud-kms-2.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-2.8.0/tests/unit/gapic/__init__.py` & `google-cloud-kms-2.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-2.8.0/tests/unit/gapic/kms_v1/__init__.py` & `google-cloud-kms-2.9.0/tests/unit/gapic/kms_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-kms-2.8.0/tests/unit/gapic/kms_v1/test_key_management_service.py` & `google-cloud-kms-2.9.0/tests/unit/gapic/kms_v1/test_key_management_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 
 from google.api_core import client_options
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import grpc_helpers
 from google.api_core import grpc_helpers_async
+from google.api_core import path_template
 from google.auth import credentials as ga_credentials
 from google.auth.exceptions import MutualTLSChannelError
 from google.cloud.kms_v1.services.key_management_service import (
     KeyManagementServiceAsyncClient,
 )
 from google.cloud.kms_v1.services.key_management_service import (
     KeyManagementServiceClient,
@@ -7409,14 +7410,17 @@
         "get_iam_policy",
         "test_iam_permissions",
     )
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
+    with pytest.raises(NotImplementedError):
+        transport.close()
+
 
 @requires_google_auth_gte_1_25_0
 def test_key_management_service_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
@@ -8513,7 +8517,53 @@
         response = await client.test_iam_permissions(
             request={
                 "resource": "resource_value",
                 "permissions": ["permissions_value"],
             }
         )
         call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_transport_close_async():
+    client = KeyManagementServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(), transport="grpc_asyncio",
+    )
+    with mock.patch.object(
+        type(getattr(client.transport, "grpc_channel")), "close"
+    ) as close:
+        async with client:
+            close.assert_not_called()
+        close.assert_called_once()
+
+
+def test_transport_close():
+    transports = {
+        "grpc": "_grpc_channel",
+    }
+
+    for transport, close_name in transports.items():
+        client = KeyManagementServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(), transport=transport
+        )
+        with mock.patch.object(
+            type(getattr(client.transport, close_name)), "close"
+        ) as close:
+            with client:
+                close.assert_not_called()
+            close.assert_called_once()
+
+
+def test_client_ctx():
+    transports = [
+        "grpc",
+    ]
+    for transport in transports:
+        client = KeyManagementServiceClient(
+            credentials=ga_credentials.AnonymousCredentials(), transport=transport
+        )
+        # Test client calls underlying transport.
+        with mock.patch.object(type(client.transport), "close") as close:
+            close.assert_not_called()
+            with client:
+                pass
+            close.assert_called()
```

