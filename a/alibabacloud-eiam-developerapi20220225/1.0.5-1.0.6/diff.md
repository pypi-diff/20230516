# Comparing `tmp/alibabacloud_eiam-developerapi20220225-1.0.5.tar.gz` & `tmp/alibabacloud_eiam-developerapi20220225-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_eiam-developerapi20220225-1.0.5.tar", last modified: Mon Nov 28 08:32:48 2022, max compression
+gzip compressed data, was "dist/alibabacloud_eiam-developerapi20220225-1.0.6.tar", last modified: Tue May 16 08:00:02 2023, max compression
```

## Comparing `alibabacloud_eiam-developerapi20220225-1.0.5.tar` & `alibabacloud_eiam-developerapi20220225-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-28 08:32:48.000000 alibabacloud_eiam-developerapi20220225-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      180 2022-11-28 08:32:47.000000 alibabacloud_eiam-developerapi20220225-1.0.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-11-28 08:32:47.000000 alibabacloud_eiam-developerapi20220225-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-11-28 08:32:47.000000 alibabacloud_eiam-developerapi20220225-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2412 2022-11-28 08:32:48.000000 alibabacloud_eiam-developerapi20220225-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1064 2022-11-28 08:32:47.000000 alibabacloud_eiam-developerapi20220225-1.0.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1149 2022-11-28 08:32:47.000000 alibabacloud_eiam-developerapi20220225-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-28 08:32:48.000000 alibabacloud_eiam-developerapi20220225-1.0.5/alibabacloud_eiam_developerapi20220225/
--rw-r--r--   0 root         (0) root         (0)       21 2022-11-28 08:32:47.000000 alibabacloud_eiam-developerapi20220225-1.0.5/alibabacloud_eiam_developerapi20220225/__init__.py
--rw-r--r--   0 root         (0) root         (0)   103074 2022-11-28 08:32:47.000000 alibabacloud_eiam-developerapi20220225-1.0.5/alibabacloud_eiam_developerapi20220225/client.py
--rw-r--r--   0 root         (0) root         (0)   110395 2022-11-28 08:32:47.000000 alibabacloud_eiam-developerapi20220225-1.0.5/alibabacloud_eiam_developerapi20220225/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-28 08:32:48.000000 alibabacloud_eiam-developerapi20220225-1.0.5/alibabacloud_eiam_developerapi20220225.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2412 2022-11-28 08:32:47.000000 alibabacloud_eiam-developerapi20220225-1.0.5/alibabacloud_eiam_developerapi20220225.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      532 2022-11-28 08:32:47.000000 alibabacloud_eiam-developerapi20220225-1.0.5/alibabacloud_eiam_developerapi20220225.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-28 08:32:47.000000 alibabacloud_eiam-developerapi20220225-1.0.5/alibabacloud_eiam_developerapi20220225.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-11-28 08:32:47.000000 alibabacloud_eiam-developerapi20220225-1.0.5/alibabacloud_eiam_developerapi20220225.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       39 2022-11-28 08:32:47.000000 alibabacloud_eiam-developerapi20220225-1.0.5/alibabacloud_eiam_developerapi20220225.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-11-28 08:32:48.000000 alibabacloud_eiam-developerapi20220225-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2682 2022-11-28 08:32:47.000000 alibabacloud_eiam-developerapi20220225-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:00:02.000000 alibabacloud_eiam-developerapi20220225-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      216 2023-05-16 08:00:02.000000 alibabacloud_eiam-developerapi20220225-1.0.6/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-16 08:00:02.000000 alibabacloud_eiam-developerapi20220225-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 08:00:02.000000 alibabacloud_eiam-developerapi20220225-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2412 2023-05-16 08:00:02.000000 alibabacloud_eiam-developerapi20220225-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-05-16 08:00:02.000000 alibabacloud_eiam-developerapi20220225-1.0.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-05-16 08:00:02.000000 alibabacloud_eiam-developerapi20220225-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:00:02.000000 alibabacloud_eiam-developerapi20220225-1.0.6/alibabacloud_eiam_developerapi20220225/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 08:00:02.000000 alibabacloud_eiam-developerapi20220225-1.0.6/alibabacloud_eiam_developerapi20220225/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   122106 2023-05-16 08:00:02.000000 alibabacloud_eiam-developerapi20220225-1.0.6/alibabacloud_eiam_developerapi20220225/client.py
+-rw-r--r--   0 root         (0) root         (0)   123179 2023-05-16 08:00:02.000000 alibabacloud_eiam-developerapi20220225-1.0.6/alibabacloud_eiam_developerapi20220225/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:00:02.000000 alibabacloud_eiam-developerapi20220225-1.0.6/alibabacloud_eiam_developerapi20220225.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2412 2023-05-16 08:00:02.000000 alibabacloud_eiam-developerapi20220225-1.0.6/alibabacloud_eiam_developerapi20220225.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      532 2023-05-16 08:00:02.000000 alibabacloud_eiam-developerapi20220225-1.0.6/alibabacloud_eiam_developerapi20220225.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 08:00:02.000000 alibabacloud_eiam-developerapi20220225-1.0.6/alibabacloud_eiam_developerapi20220225.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-16 08:00:02.000000 alibabacloud_eiam-developerapi20220225-1.0.6/alibabacloud_eiam_developerapi20220225.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-16 08:00:02.000000 alibabacloud_eiam-developerapi20220225-1.0.6/alibabacloud_eiam_developerapi20220225.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 08:00:02.000000 alibabacloud_eiam-developerapi20220225-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-05-16 08:00:02.000000 alibabacloud_eiam-developerapi20220225-1.0.6/setup.py
```

### Comparing `alibabacloud_eiam-developerapi20220225-1.0.5/LICENSE` & `alibabacloud_eiam-developerapi20220225-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_eiam-developerapi20220225-1.0.5/PKG-INFO` & `alibabacloud_eiam-developerapi20220225-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_eiam-developerapi20220225
-Version: 1.0.5
+Version: 1.0.6
 Summary: Alibaba Cloud Eiam-developerapi (20220225) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eiam-developerapi20220225-1.0.5/README-CN.md` & `alibabacloud_eiam-developerapi20220225-1.0.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eiam-developerapi20220225-1.0.5/README.md` & `alibabacloud_eiam-developerapi20220225-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eiam-developerapi20220225-1.0.5/alibabacloud_eiam_developerapi20220225/client.py` & `alibabacloud_eiam-developerapi20220225-1.0.6/alibabacloud_eiam_developerapi20220225/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,33 +38,111 @@
     ) -> str:
         if not UtilClient.empty(endpoint):
             return endpoint
         if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
             return endpoint_map.get(region_id)
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
-    def create_organizational_unit(
+    def add_user_to_organizational_units_with_options(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.CreateOrganizationalUnitRequest,
-    ) -> eiam_developerapi_20220225_models.CreateOrganizationalUnitResponse:
+        user_id: str,
+        request: eiam_developerapi_20220225_models.AddUserToOrganizationalUnitsRequest,
+        headers: eiam_developerapi_20220225_models.AddUserToOrganizationalUnitsHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> eiam_developerapi_20220225_models.AddUserToOrganizationalUnitsResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.organizational_unit_ids):
+            body['organizationalUnitIds'] = request.organizational_unit_ids
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AddUserToOrganizationalUnits',
+            version='2022-02-25',
+            protocol='HTTPS',
+            pathname=f'/v2/{OpenApiUtilClient.get_encode_param(instance_id)}/{OpenApiUtilClient.get_encode_param(application_id)}/users/{OpenApiUtilClient.get_encode_param(user_id)}/actions/addUserToOrganizationalUnits',
+            method='POST',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='json',
+            body_type='none'
+        )
+        return TeaCore.from_map(
+            eiam_developerapi_20220225_models.AddUserToOrganizationalUnitsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def add_user_to_organizational_units_with_options_async(
+        self,
+        instance_id: str,
+        application_id: str,
+        user_id: str,
+        request: eiam_developerapi_20220225_models.AddUserToOrganizationalUnitsRequest,
+        headers: eiam_developerapi_20220225_models.AddUserToOrganizationalUnitsHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> eiam_developerapi_20220225_models.AddUserToOrganizationalUnitsResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.organizational_unit_ids):
+            body['organizationalUnitIds'] = request.organizational_unit_ids
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='AddUserToOrganizationalUnits',
+            version='2022-02-25',
+            protocol='HTTPS',
+            pathname=f'/v2/{OpenApiUtilClient.get_encode_param(instance_id)}/{OpenApiUtilClient.get_encode_param(application_id)}/users/{OpenApiUtilClient.get_encode_param(user_id)}/actions/addUserToOrganizationalUnits',
+            method='POST',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='json',
+            body_type='none'
+        )
+        return TeaCore.from_map(
+            eiam_developerapi_20220225_models.AddUserToOrganizationalUnitsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def add_user_to_organizational_units(
+        self,
+        instance_id: str,
+        application_id: str,
+        user_id: str,
+        request: eiam_developerapi_20220225_models.AddUserToOrganizationalUnitsRequest,
+    ) -> eiam_developerapi_20220225_models.AddUserToOrganizationalUnitsResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.CreateOrganizationalUnitHeaders()
-        return self.create_organizational_unit_with_options(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.AddUserToOrganizationalUnitsHeaders()
+        return self.add_user_to_organizational_units_with_options(instance_id, application_id, user_id, request, headers, runtime)
 
-    async def create_organizational_unit_async(
+    async def add_user_to_organizational_units_async(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.CreateOrganizationalUnitRequest,
-    ) -> eiam_developerapi_20220225_models.CreateOrganizationalUnitResponse:
+        user_id: str,
+        request: eiam_developerapi_20220225_models.AddUserToOrganizationalUnitsRequest,
+    ) -> eiam_developerapi_20220225_models.AddUserToOrganizationalUnitsResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.CreateOrganizationalUnitHeaders()
-        return await self.create_organizational_unit_with_options_async(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.AddUserToOrganizationalUnitsHeaders()
+        return await self.add_user_to_organizational_units_with_options_async(instance_id, application_id, user_id, request, headers, runtime)
 
     def create_organizational_unit_with_options(
         self,
         instance_id: str,
         application_id: str,
         request: eiam_developerapi_20220225_models.CreateOrganizationalUnitRequest,
         headers: eiam_developerapi_20220225_models.CreateOrganizationalUnitHeaders,
@@ -144,33 +222,33 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.CreateOrganizationalUnitResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def create_user(
+    def create_organizational_unit(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.CreateUserRequest,
-    ) -> eiam_developerapi_20220225_models.CreateUserResponse:
+        request: eiam_developerapi_20220225_models.CreateOrganizationalUnitRequest,
+    ) -> eiam_developerapi_20220225_models.CreateOrganizationalUnitResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.CreateUserHeaders()
-        return self.create_user_with_options(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.CreateOrganizationalUnitHeaders()
+        return self.create_organizational_unit_with_options(instance_id, application_id, request, headers, runtime)
 
-    async def create_user_async(
+    async def create_organizational_unit_async(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.CreateUserRequest,
-    ) -> eiam_developerapi_20220225_models.CreateUserResponse:
+        request: eiam_developerapi_20220225_models.CreateOrganizationalUnitRequest,
+    ) -> eiam_developerapi_20220225_models.CreateOrganizationalUnitResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.CreateUserHeaders()
-        return await self.create_user_with_options_async(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.CreateOrganizationalUnitHeaders()
+        return await self.create_organizational_unit_with_options_async(instance_id, application_id, request, headers, runtime)
 
     def create_user_with_options(
         self,
         instance_id: str,
         application_id: str,
         request: eiam_developerapi_20220225_models.CreateUserRequest,
         headers: eiam_developerapi_20220225_models.CreateUserHeaders,
@@ -286,33 +364,33 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.CreateUserResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def delete_organizational_unit(
+    def create_user(
         self,
         instance_id: str,
         application_id: str,
-        organizational_unit_id: str,
-    ) -> eiam_developerapi_20220225_models.DeleteOrganizationalUnitResponse:
+        request: eiam_developerapi_20220225_models.CreateUserRequest,
+    ) -> eiam_developerapi_20220225_models.CreateUserResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.DeleteOrganizationalUnitHeaders()
-        return self.delete_organizational_unit_with_options(instance_id, application_id, organizational_unit_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.CreateUserHeaders()
+        return self.create_user_with_options(instance_id, application_id, request, headers, runtime)
 
-    async def delete_organizational_unit_async(
+    async def create_user_async(
         self,
         instance_id: str,
         application_id: str,
-        organizational_unit_id: str,
-    ) -> eiam_developerapi_20220225_models.DeleteOrganizationalUnitResponse:
+        request: eiam_developerapi_20220225_models.CreateUserRequest,
+    ) -> eiam_developerapi_20220225_models.CreateUserResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.DeleteOrganizationalUnitHeaders()
-        return await self.delete_organizational_unit_with_options_async(instance_id, application_id, organizational_unit_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.CreateUserHeaders()
+        return await self.create_user_with_options_async(instance_id, application_id, request, headers, runtime)
 
     def delete_organizational_unit_with_options(
         self,
         instance_id: str,
         application_id: str,
         organizational_unit_id: str,
         headers: eiam_developerapi_20220225_models.DeleteOrganizationalUnitHeaders,
@@ -370,33 +448,33 @@
             body_type='none'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.DeleteOrganizationalUnitResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def delete_user(
+    def delete_organizational_unit(
         self,
         instance_id: str,
         application_id: str,
-        user_id: str,
-    ) -> eiam_developerapi_20220225_models.DeleteUserResponse:
+        organizational_unit_id: str,
+    ) -> eiam_developerapi_20220225_models.DeleteOrganizationalUnitResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.DeleteUserHeaders()
-        return self.delete_user_with_options(instance_id, application_id, user_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.DeleteOrganizationalUnitHeaders()
+        return self.delete_organizational_unit_with_options(instance_id, application_id, organizational_unit_id, headers, runtime)
 
-    async def delete_user_async(
+    async def delete_organizational_unit_async(
         self,
         instance_id: str,
         application_id: str,
-        user_id: str,
-    ) -> eiam_developerapi_20220225_models.DeleteUserResponse:
+        organizational_unit_id: str,
+    ) -> eiam_developerapi_20220225_models.DeleteOrganizationalUnitResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.DeleteUserHeaders()
-        return await self.delete_user_with_options_async(instance_id, application_id, user_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.DeleteOrganizationalUnitHeaders()
+        return await self.delete_organizational_unit_with_options_async(instance_id, application_id, organizational_unit_id, headers, runtime)
 
     def delete_user_with_options(
         self,
         instance_id: str,
         application_id: str,
         user_id: str,
         headers: eiam_developerapi_20220225_models.DeleteUserHeaders,
@@ -454,33 +532,33 @@
             body_type='none'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.DeleteUserResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def disable_user(
+    def delete_user(
         self,
         instance_id: str,
         application_id: str,
         user_id: str,
-    ) -> eiam_developerapi_20220225_models.DisableUserResponse:
+    ) -> eiam_developerapi_20220225_models.DeleteUserResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.DisableUserHeaders()
-        return self.disable_user_with_options(instance_id, application_id, user_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.DeleteUserHeaders()
+        return self.delete_user_with_options(instance_id, application_id, user_id, headers, runtime)
 
-    async def disable_user_async(
+    async def delete_user_async(
         self,
         instance_id: str,
         application_id: str,
         user_id: str,
-    ) -> eiam_developerapi_20220225_models.DisableUserResponse:
+    ) -> eiam_developerapi_20220225_models.DeleteUserResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.DisableUserHeaders()
-        return await self.disable_user_with_options_async(instance_id, application_id, user_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.DeleteUserHeaders()
+        return await self.delete_user_with_options_async(instance_id, application_id, user_id, headers, runtime)
 
     def disable_user_with_options(
         self,
         instance_id: str,
         application_id: str,
         user_id: str,
         headers: eiam_developerapi_20220225_models.DisableUserHeaders,
@@ -538,33 +616,33 @@
             body_type='none'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.DisableUserResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def enable_user(
+    def disable_user(
         self,
         instance_id: str,
         application_id: str,
         user_id: str,
-    ) -> eiam_developerapi_20220225_models.EnableUserResponse:
+    ) -> eiam_developerapi_20220225_models.DisableUserResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.EnableUserHeaders()
-        return self.enable_user_with_options(instance_id, application_id, user_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.DisableUserHeaders()
+        return self.disable_user_with_options(instance_id, application_id, user_id, headers, runtime)
 
-    async def enable_user_async(
+    async def disable_user_async(
         self,
         instance_id: str,
         application_id: str,
         user_id: str,
-    ) -> eiam_developerapi_20220225_models.EnableUserResponse:
+    ) -> eiam_developerapi_20220225_models.DisableUserResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.EnableUserHeaders()
-        return await self.enable_user_with_options_async(instance_id, application_id, user_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.DisableUserHeaders()
+        return await self.disable_user_with_options_async(instance_id, application_id, user_id, headers, runtime)
 
     def enable_user_with_options(
         self,
         instance_id: str,
         application_id: str,
         user_id: str,
         headers: eiam_developerapi_20220225_models.EnableUserHeaders,
@@ -622,33 +700,33 @@
             body_type='none'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.EnableUserResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def generate_device_code(
+    def enable_user(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.GenerateDeviceCodeRequest,
-    ) -> eiam_developerapi_20220225_models.GenerateDeviceCodeResponse:
+        user_id: str,
+    ) -> eiam_developerapi_20220225_models.EnableUserResponse:
         runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.generate_device_code_with_options(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.EnableUserHeaders()
+        return self.enable_user_with_options(instance_id, application_id, user_id, headers, runtime)
 
-    async def generate_device_code_async(
+    async def enable_user_async(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.GenerateDeviceCodeRequest,
-    ) -> eiam_developerapi_20220225_models.GenerateDeviceCodeResponse:
+        user_id: str,
+    ) -> eiam_developerapi_20220225_models.EnableUserResponse:
         runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.generate_device_code_with_options_async(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.EnableUserHeaders()
+        return await self.enable_user_with_options_async(instance_id, application_id, user_id, headers, runtime)
 
     def generate_device_code_with_options(
         self,
         instance_id: str,
         application_id: str,
         request: eiam_developerapi_20220225_models.GenerateDeviceCodeRequest,
         headers: Dict[str, str],
@@ -706,33 +784,33 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.GenerateDeviceCodeResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def generate_token(
+    def generate_device_code(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.GenerateTokenRequest,
-    ) -> eiam_developerapi_20220225_models.GenerateTokenResponse:
+        request: eiam_developerapi_20220225_models.GenerateDeviceCodeRequest,
+    ) -> eiam_developerapi_20220225_models.GenerateDeviceCodeResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.generate_token_with_options(instance_id, application_id, request, headers, runtime)
+        return self.generate_device_code_with_options(instance_id, application_id, request, headers, runtime)
 
-    async def generate_token_async(
+    async def generate_device_code_async(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.GenerateTokenRequest,
-    ) -> eiam_developerapi_20220225_models.GenerateTokenResponse:
+        request: eiam_developerapi_20220225_models.GenerateDeviceCodeRequest,
+    ) -> eiam_developerapi_20220225_models.GenerateDeviceCodeResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.generate_token_with_options_async(instance_id, application_id, request, headers, runtime)
+        return await self.generate_device_code_with_options_async(instance_id, application_id, request, headers, runtime)
 
     def generate_token_with_options(
         self,
         instance_id: str,
         application_id: str,
         request: eiam_developerapi_20220225_models.GenerateTokenRequest,
         headers: Dict[str, str],
@@ -834,31 +912,33 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.GenerateTokenResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_application_provisioning_scope(
+    def generate_token(
         self,
         instance_id: str,
         application_id: str,
-    ) -> eiam_developerapi_20220225_models.GetApplicationProvisioningScopeResponse:
+        request: eiam_developerapi_20220225_models.GenerateTokenRequest,
+    ) -> eiam_developerapi_20220225_models.GenerateTokenResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetApplicationProvisioningScopeHeaders()
-        return self.get_application_provisioning_scope_with_options(instance_id, application_id, headers, runtime)
+        headers = {}
+        return self.generate_token_with_options(instance_id, application_id, request, headers, runtime)
 
-    async def get_application_provisioning_scope_async(
+    async def generate_token_async(
         self,
         instance_id: str,
         application_id: str,
-    ) -> eiam_developerapi_20220225_models.GetApplicationProvisioningScopeResponse:
+        request: eiam_developerapi_20220225_models.GenerateTokenRequest,
+    ) -> eiam_developerapi_20220225_models.GenerateTokenResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetApplicationProvisioningScopeHeaders()
-        return await self.get_application_provisioning_scope_with_options_async(instance_id, application_id, headers, runtime)
+        headers = {}
+        return await self.generate_token_with_options_async(instance_id, application_id, request, headers, runtime)
 
     def get_application_provisioning_scope_with_options(
         self,
         instance_id: str,
         application_id: str,
         headers: eiam_developerapi_20220225_models.GetApplicationProvisioningScopeHeaders,
         runtime: util_models.RuntimeOptions,
@@ -914,33 +994,31 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.GetApplicationProvisioningScopeResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_organizational_unit(
+    def get_application_provisioning_scope(
         self,
         instance_id: str,
         application_id: str,
-        organizational_unit_id: str,
-    ) -> eiam_developerapi_20220225_models.GetOrganizationalUnitResponse:
+    ) -> eiam_developerapi_20220225_models.GetApplicationProvisioningScopeResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetOrganizationalUnitHeaders()
-        return self.get_organizational_unit_with_options(instance_id, application_id, organizational_unit_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetApplicationProvisioningScopeHeaders()
+        return self.get_application_provisioning_scope_with_options(instance_id, application_id, headers, runtime)
 
-    async def get_organizational_unit_async(
+    async def get_application_provisioning_scope_async(
         self,
         instance_id: str,
         application_id: str,
-        organizational_unit_id: str,
-    ) -> eiam_developerapi_20220225_models.GetOrganizationalUnitResponse:
+    ) -> eiam_developerapi_20220225_models.GetApplicationProvisioningScopeResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetOrganizationalUnitHeaders()
-        return await self.get_organizational_unit_with_options_async(instance_id, application_id, organizational_unit_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetApplicationProvisioningScopeHeaders()
+        return await self.get_application_provisioning_scope_with_options_async(instance_id, application_id, headers, runtime)
 
     def get_organizational_unit_with_options(
         self,
         instance_id: str,
         application_id: str,
         organizational_unit_id: str,
         headers: eiam_developerapi_20220225_models.GetOrganizationalUnitHeaders,
@@ -998,33 +1076,33 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.GetOrganizationalUnitResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_organizational_unit_id_by_external_id(
+    def get_organizational_unit(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.GetOrganizationalUnitIdByExternalIdRequest,
-    ) -> eiam_developerapi_20220225_models.GetOrganizationalUnitIdByExternalIdResponse:
+        organizational_unit_id: str,
+    ) -> eiam_developerapi_20220225_models.GetOrganizationalUnitResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetOrganizationalUnitIdByExternalIdHeaders()
-        return self.get_organizational_unit_id_by_external_id_with_options(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetOrganizationalUnitHeaders()
+        return self.get_organizational_unit_with_options(instance_id, application_id, organizational_unit_id, headers, runtime)
 
-    async def get_organizational_unit_id_by_external_id_async(
+    async def get_organizational_unit_async(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.GetOrganizationalUnitIdByExternalIdRequest,
-    ) -> eiam_developerapi_20220225_models.GetOrganizationalUnitIdByExternalIdResponse:
+        organizational_unit_id: str,
+    ) -> eiam_developerapi_20220225_models.GetOrganizationalUnitResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetOrganizationalUnitIdByExternalIdHeaders()
-        return await self.get_organizational_unit_id_by_external_id_with_options_async(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetOrganizationalUnitHeaders()
+        return await self.get_organizational_unit_with_options_async(instance_id, application_id, organizational_unit_id, headers, runtime)
 
     def get_organizational_unit_id_by_external_id_with_options(
         self,
         instance_id: str,
         application_id: str,
         request: eiam_developerapi_20220225_models.GetOrganizationalUnitIdByExternalIdRequest,
         headers: eiam_developerapi_20220225_models.GetOrganizationalUnitIdByExternalIdHeaders,
@@ -1100,33 +1178,33 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.GetOrganizationalUnitIdByExternalIdResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_user(
+    def get_organizational_unit_id_by_external_id(
         self,
         instance_id: str,
         application_id: str,
-        user_id: str,
-    ) -> eiam_developerapi_20220225_models.GetUserResponse:
+        request: eiam_developerapi_20220225_models.GetOrganizationalUnitIdByExternalIdRequest,
+    ) -> eiam_developerapi_20220225_models.GetOrganizationalUnitIdByExternalIdResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetUserHeaders()
-        return self.get_user_with_options(instance_id, application_id, user_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetOrganizationalUnitIdByExternalIdHeaders()
+        return self.get_organizational_unit_id_by_external_id_with_options(instance_id, application_id, request, headers, runtime)
 
-    async def get_user_async(
+    async def get_organizational_unit_id_by_external_id_async(
         self,
         instance_id: str,
         application_id: str,
-        user_id: str,
-    ) -> eiam_developerapi_20220225_models.GetUserResponse:
+        request: eiam_developerapi_20220225_models.GetOrganizationalUnitIdByExternalIdRequest,
+    ) -> eiam_developerapi_20220225_models.GetOrganizationalUnitIdByExternalIdResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetUserHeaders()
-        return await self.get_user_with_options_async(instance_id, application_id, user_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetOrganizationalUnitIdByExternalIdHeaders()
+        return await self.get_organizational_unit_id_by_external_id_with_options_async(instance_id, application_id, request, headers, runtime)
 
     def get_user_with_options(
         self,
         instance_id: str,
         application_id: str,
         user_id: str,
         headers: eiam_developerapi_20220225_models.GetUserHeaders,
@@ -1184,33 +1262,33 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.GetUserResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_user_id_by_email(
+    def get_user(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.GetUserIdByEmailRequest,
-    ) -> eiam_developerapi_20220225_models.GetUserIdByEmailResponse:
+        user_id: str,
+    ) -> eiam_developerapi_20220225_models.GetUserResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetUserIdByEmailHeaders()
-        return self.get_user_id_by_email_with_options(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetUserHeaders()
+        return self.get_user_with_options(instance_id, application_id, user_id, headers, runtime)
 
-    async def get_user_id_by_email_async(
+    async def get_user_async(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.GetUserIdByEmailRequest,
-    ) -> eiam_developerapi_20220225_models.GetUserIdByEmailResponse:
+        user_id: str,
+    ) -> eiam_developerapi_20220225_models.GetUserResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetUserIdByEmailHeaders()
-        return await self.get_user_id_by_email_with_options_async(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetUserHeaders()
+        return await self.get_user_with_options_async(instance_id, application_id, user_id, headers, runtime)
 
     def get_user_id_by_email_with_options(
         self,
         instance_id: str,
         application_id: str,
         request: eiam_developerapi_20220225_models.GetUserIdByEmailRequest,
         headers: eiam_developerapi_20220225_models.GetUserIdByEmailHeaders,
@@ -1278,33 +1356,33 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.GetUserIdByEmailResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_user_id_by_phone_number(
+    def get_user_id_by_email(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.GetUserIdByPhoneNumberRequest,
-    ) -> eiam_developerapi_20220225_models.GetUserIdByPhoneNumberResponse:
+        request: eiam_developerapi_20220225_models.GetUserIdByEmailRequest,
+    ) -> eiam_developerapi_20220225_models.GetUserIdByEmailResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetUserIdByPhoneNumberHeaders()
-        return self.get_user_id_by_phone_number_with_options(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetUserIdByEmailHeaders()
+        return self.get_user_id_by_email_with_options(instance_id, application_id, request, headers, runtime)
 
-    async def get_user_id_by_phone_number_async(
+    async def get_user_id_by_email_async(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.GetUserIdByPhoneNumberRequest,
-    ) -> eiam_developerapi_20220225_models.GetUserIdByPhoneNumberResponse:
+        request: eiam_developerapi_20220225_models.GetUserIdByEmailRequest,
+    ) -> eiam_developerapi_20220225_models.GetUserIdByEmailResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetUserIdByPhoneNumberHeaders()
-        return await self.get_user_id_by_phone_number_with_options_async(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetUserIdByEmailHeaders()
+        return await self.get_user_id_by_email_with_options_async(instance_id, application_id, request, headers, runtime)
 
     def get_user_id_by_phone_number_with_options(
         self,
         instance_id: str,
         application_id: str,
         request: eiam_developerapi_20220225_models.GetUserIdByPhoneNumberRequest,
         headers: eiam_developerapi_20220225_models.GetUserIdByPhoneNumberHeaders,
@@ -1372,33 +1450,33 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.GetUserIdByPhoneNumberResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_user_id_by_user_external_id(
+    def get_user_id_by_phone_number(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.GetUserIdByUserExternalIdRequest,
-    ) -> eiam_developerapi_20220225_models.GetUserIdByUserExternalIdResponse:
+        request: eiam_developerapi_20220225_models.GetUserIdByPhoneNumberRequest,
+    ) -> eiam_developerapi_20220225_models.GetUserIdByPhoneNumberResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetUserIdByUserExternalIdHeaders()
-        return self.get_user_id_by_user_external_id_with_options(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetUserIdByPhoneNumberHeaders()
+        return self.get_user_id_by_phone_number_with_options(instance_id, application_id, request, headers, runtime)
 
-    async def get_user_id_by_user_external_id_async(
+    async def get_user_id_by_phone_number_async(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.GetUserIdByUserExternalIdRequest,
-    ) -> eiam_developerapi_20220225_models.GetUserIdByUserExternalIdResponse:
+        request: eiam_developerapi_20220225_models.GetUserIdByPhoneNumberRequest,
+    ) -> eiam_developerapi_20220225_models.GetUserIdByPhoneNumberResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetUserIdByUserExternalIdHeaders()
-        return await self.get_user_id_by_user_external_id_with_options_async(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetUserIdByPhoneNumberHeaders()
+        return await self.get_user_id_by_phone_number_with_options_async(instance_id, application_id, request, headers, runtime)
 
     def get_user_id_by_user_external_id_with_options(
         self,
         instance_id: str,
         application_id: str,
         request: eiam_developerapi_20220225_models.GetUserIdByUserExternalIdRequest,
         headers: eiam_developerapi_20220225_models.GetUserIdByUserExternalIdHeaders,
@@ -1474,33 +1552,33 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.GetUserIdByUserExternalIdResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_user_id_by_username(
+    def get_user_id_by_user_external_id(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.GetUserIdByUsernameRequest,
-    ) -> eiam_developerapi_20220225_models.GetUserIdByUsernameResponse:
+        request: eiam_developerapi_20220225_models.GetUserIdByUserExternalIdRequest,
+    ) -> eiam_developerapi_20220225_models.GetUserIdByUserExternalIdResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetUserIdByUsernameHeaders()
-        return self.get_user_id_by_username_with_options(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetUserIdByUserExternalIdHeaders()
+        return self.get_user_id_by_user_external_id_with_options(instance_id, application_id, request, headers, runtime)
 
-    async def get_user_id_by_username_async(
+    async def get_user_id_by_user_external_id_async(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.GetUserIdByUsernameRequest,
-    ) -> eiam_developerapi_20220225_models.GetUserIdByUsernameResponse:
+        request: eiam_developerapi_20220225_models.GetUserIdByUserExternalIdRequest,
+    ) -> eiam_developerapi_20220225_models.GetUserIdByUserExternalIdResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetUserIdByUsernameHeaders()
-        return await self.get_user_id_by_username_with_options_async(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetUserIdByUserExternalIdHeaders()
+        return await self.get_user_id_by_user_external_id_with_options_async(instance_id, application_id, request, headers, runtime)
 
     def get_user_id_by_username_with_options(
         self,
         instance_id: str,
         application_id: str,
         request: eiam_developerapi_20220225_models.GetUserIdByUsernameRequest,
         headers: eiam_developerapi_20220225_models.GetUserIdByUsernameHeaders,
@@ -1568,31 +1646,33 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.GetUserIdByUsernameResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def get_user_info(
+    def get_user_id_by_username(
         self,
         instance_id: str,
         application_id: str,
-    ) -> eiam_developerapi_20220225_models.GetUserInfoResponse:
+        request: eiam_developerapi_20220225_models.GetUserIdByUsernameRequest,
+    ) -> eiam_developerapi_20220225_models.GetUserIdByUsernameResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetUserInfoHeaders()
-        return self.get_user_info_with_options(instance_id, application_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetUserIdByUsernameHeaders()
+        return self.get_user_id_by_username_with_options(instance_id, application_id, request, headers, runtime)
 
-    async def get_user_info_async(
+    async def get_user_id_by_username_async(
         self,
         instance_id: str,
         application_id: str,
-    ) -> eiam_developerapi_20220225_models.GetUserInfoResponse:
+        request: eiam_developerapi_20220225_models.GetUserIdByUsernameRequest,
+    ) -> eiam_developerapi_20220225_models.GetUserIdByUsernameResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetUserInfoHeaders()
-        return await self.get_user_info_with_options_async(instance_id, application_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetUserIdByUsernameHeaders()
+        return await self.get_user_id_by_username_with_options_async(instance_id, application_id, request, headers, runtime)
 
     def get_user_info_with_options(
         self,
         instance_id: str,
         application_id: str,
         headers: eiam_developerapi_20220225_models.GetUserInfoHeaders,
         runtime: util_models.RuntimeOptions,
@@ -1648,33 +1728,31 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.GetUserInfoResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_organizational_unit_parent_ids(
+    def get_user_info(
         self,
         instance_id: str,
         application_id: str,
-        organizational_unit_id: str,
-    ) -> eiam_developerapi_20220225_models.ListOrganizationalUnitParentIdsResponse:
+    ) -> eiam_developerapi_20220225_models.GetUserInfoResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.ListOrganizationalUnitParentIdsHeaders()
-        return self.list_organizational_unit_parent_ids_with_options(instance_id, application_id, organizational_unit_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetUserInfoHeaders()
+        return self.get_user_info_with_options(instance_id, application_id, headers, runtime)
 
-    async def list_organizational_unit_parent_ids_async(
+    async def get_user_info_async(
         self,
         instance_id: str,
         application_id: str,
-        organizational_unit_id: str,
-    ) -> eiam_developerapi_20220225_models.ListOrganizationalUnitParentIdsResponse:
+    ) -> eiam_developerapi_20220225_models.GetUserInfoResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.ListOrganizationalUnitParentIdsHeaders()
-        return await self.list_organizational_unit_parent_ids_with_options_async(instance_id, application_id, organizational_unit_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetUserInfoHeaders()
+        return await self.get_user_info_with_options_async(instance_id, application_id, headers, runtime)
 
     def list_organizational_unit_parent_ids_with_options(
         self,
         instance_id: str,
         application_id: str,
         organizational_unit_id: str,
         headers: eiam_developerapi_20220225_models.ListOrganizationalUnitParentIdsHeaders,
@@ -1732,33 +1810,33 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.ListOrganizationalUnitParentIdsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_organizational_units(
+    def list_organizational_unit_parent_ids(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.ListOrganizationalUnitsRequest,
-    ) -> eiam_developerapi_20220225_models.ListOrganizationalUnitsResponse:
+        organizational_unit_id: str,
+    ) -> eiam_developerapi_20220225_models.ListOrganizationalUnitParentIdsResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.ListOrganizationalUnitsHeaders()
-        return self.list_organizational_units_with_options(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.ListOrganizationalUnitParentIdsHeaders()
+        return self.list_organizational_unit_parent_ids_with_options(instance_id, application_id, organizational_unit_id, headers, runtime)
 
-    async def list_organizational_units_async(
+    async def list_organizational_unit_parent_ids_async(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.ListOrganizationalUnitsRequest,
-    ) -> eiam_developerapi_20220225_models.ListOrganizationalUnitsResponse:
+        organizational_unit_id: str,
+    ) -> eiam_developerapi_20220225_models.ListOrganizationalUnitParentIdsResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.ListOrganizationalUnitsHeaders()
-        return await self.list_organizational_units_with_options_async(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.ListOrganizationalUnitParentIdsHeaders()
+        return await self.list_organizational_unit_parent_ids_with_options_async(instance_id, application_id, organizational_unit_id, headers, runtime)
 
     def list_organizational_units_with_options(
         self,
         instance_id: str,
         application_id: str,
         request: eiam_developerapi_20220225_models.ListOrganizationalUnitsRequest,
         headers: eiam_developerapi_20220225_models.ListOrganizationalUnitsHeaders,
@@ -1834,33 +1912,33 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.ListOrganizationalUnitsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_users(
+    def list_organizational_units(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.ListUsersRequest,
-    ) -> eiam_developerapi_20220225_models.ListUsersResponse:
+        request: eiam_developerapi_20220225_models.ListOrganizationalUnitsRequest,
+    ) -> eiam_developerapi_20220225_models.ListOrganizationalUnitsResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.ListUsersHeaders()
-        return self.list_users_with_options(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.ListOrganizationalUnitsHeaders()
+        return self.list_organizational_units_with_options(instance_id, application_id, request, headers, runtime)
 
-    async def list_users_async(
+    async def list_organizational_units_async(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.ListUsersRequest,
-    ) -> eiam_developerapi_20220225_models.ListUsersResponse:
+        request: eiam_developerapi_20220225_models.ListOrganizationalUnitsRequest,
+    ) -> eiam_developerapi_20220225_models.ListOrganizationalUnitsResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.ListUsersHeaders()
-        return await self.list_users_with_options_async(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.ListOrganizationalUnitsHeaders()
+        return await self.list_organizational_units_with_options_async(instance_id, application_id, request, headers, runtime)
 
     def list_users_with_options(
         self,
         instance_id: str,
         application_id: str,
         request: eiam_developerapi_20220225_models.ListUsersRequest,
         headers: eiam_developerapi_20220225_models.ListUsersHeaders,
@@ -1936,35 +2014,33 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.ListUsersResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def patch_organizational_unit(
+    def list_users(
         self,
         instance_id: str,
         application_id: str,
-        organizational_unit_id: str,
-        request: eiam_developerapi_20220225_models.PatchOrganizationalUnitRequest,
-    ) -> eiam_developerapi_20220225_models.PatchOrganizationalUnitResponse:
+        request: eiam_developerapi_20220225_models.ListUsersRequest,
+    ) -> eiam_developerapi_20220225_models.ListUsersResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.PatchOrganizationalUnitHeaders()
-        return self.patch_organizational_unit_with_options(instance_id, application_id, organizational_unit_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.ListUsersHeaders()
+        return self.list_users_with_options(instance_id, application_id, request, headers, runtime)
 
-    async def patch_organizational_unit_async(
+    async def list_users_async(
         self,
         instance_id: str,
         application_id: str,
-        organizational_unit_id: str,
-        request: eiam_developerapi_20220225_models.PatchOrganizationalUnitRequest,
-    ) -> eiam_developerapi_20220225_models.PatchOrganizationalUnitResponse:
+        request: eiam_developerapi_20220225_models.ListUsersRequest,
+    ) -> eiam_developerapi_20220225_models.ListUsersResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.PatchOrganizationalUnitHeaders()
-        return await self.patch_organizational_unit_with_options_async(instance_id, application_id, organizational_unit_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.ListUsersHeaders()
+        return await self.list_users_with_options_async(instance_id, application_id, request, headers, runtime)
 
     def patch_organizational_unit_with_options(
         self,
         instance_id: str,
         application_id: str,
         organizational_unit_id: str,
         request: eiam_developerapi_20220225_models.PatchOrganizationalUnitRequest,
@@ -2038,35 +2114,35 @@
             body_type='none'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.PatchOrganizationalUnitResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def patch_user(
+    def patch_organizational_unit(
         self,
         instance_id: str,
         application_id: str,
-        user_id: str,
-        request: eiam_developerapi_20220225_models.PatchUserRequest,
-    ) -> eiam_developerapi_20220225_models.PatchUserResponse:
+        organizational_unit_id: str,
+        request: eiam_developerapi_20220225_models.PatchOrganizationalUnitRequest,
+    ) -> eiam_developerapi_20220225_models.PatchOrganizationalUnitResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.PatchUserHeaders()
-        return self.patch_user_with_options(instance_id, application_id, user_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.PatchOrganizationalUnitHeaders()
+        return self.patch_organizational_unit_with_options(instance_id, application_id, organizational_unit_id, request, headers, runtime)
 
-    async def patch_user_async(
+    async def patch_organizational_unit_async(
         self,
         instance_id: str,
         application_id: str,
-        user_id: str,
-        request: eiam_developerapi_20220225_models.PatchUserRequest,
-    ) -> eiam_developerapi_20220225_models.PatchUserResponse:
+        organizational_unit_id: str,
+        request: eiam_developerapi_20220225_models.PatchOrganizationalUnitRequest,
+    ) -> eiam_developerapi_20220225_models.PatchOrganizationalUnitResponse:
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.PatchUserHeaders()
-        return await self.patch_user_with_options_async(instance_id, application_id, user_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.PatchOrganizationalUnitHeaders()
+        return await self.patch_organizational_unit_with_options_async(instance_id, application_id, organizational_unit_id, request, headers, runtime)
 
     def patch_user_with_options(
         self,
         instance_id: str,
         application_id: str,
         user_id: str,
         request: eiam_developerapi_20220225_models.PatchUserRequest,
@@ -2164,33 +2240,133 @@
             body_type='none'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.PatchUserResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def revoke_token(
+    def patch_user(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.RevokeTokenRequest,
-    ) -> eiam_developerapi_20220225_models.RevokeTokenResponse:
+        user_id: str,
+        request: eiam_developerapi_20220225_models.PatchUserRequest,
+    ) -> eiam_developerapi_20220225_models.PatchUserResponse:
         runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.revoke_token_with_options(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.PatchUserHeaders()
+        return self.patch_user_with_options(instance_id, application_id, user_id, request, headers, runtime)
 
-    async def revoke_token_async(
+    async def patch_user_async(
         self,
         instance_id: str,
         application_id: str,
-        request: eiam_developerapi_20220225_models.RevokeTokenRequest,
-    ) -> eiam_developerapi_20220225_models.RevokeTokenResponse:
+        user_id: str,
+        request: eiam_developerapi_20220225_models.PatchUserRequest,
+    ) -> eiam_developerapi_20220225_models.PatchUserResponse:
         runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.revoke_token_with_options_async(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.PatchUserHeaders()
+        return await self.patch_user_with_options_async(instance_id, application_id, user_id, request, headers, runtime)
+
+    def remove_user_from_organizational_units_with_options(
+        self,
+        instance_id: str,
+        application_id: str,
+        user_id: str,
+        request: eiam_developerapi_20220225_models.RemoveUserFromOrganizationalUnitsRequest,
+        headers: eiam_developerapi_20220225_models.RemoveUserFromOrganizationalUnitsHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> eiam_developerapi_20220225_models.RemoveUserFromOrganizationalUnitsResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.organizational_unit_ids):
+            body['organizationalUnitIds'] = request.organizational_unit_ids
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='RemoveUserFromOrganizationalUnits',
+            version='2022-02-25',
+            protocol='HTTPS',
+            pathname=f'/v2/{OpenApiUtilClient.get_encode_param(instance_id)}/{OpenApiUtilClient.get_encode_param(application_id)}/users/{OpenApiUtilClient.get_encode_param(user_id)}/actions/removeUserFromOrganizationalUnits',
+            method='POST',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='json',
+            body_type='none'
+        )
+        return TeaCore.from_map(
+            eiam_developerapi_20220225_models.RemoveUserFromOrganizationalUnitsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def remove_user_from_organizational_units_with_options_async(
+        self,
+        instance_id: str,
+        application_id: str,
+        user_id: str,
+        request: eiam_developerapi_20220225_models.RemoveUserFromOrganizationalUnitsRequest,
+        headers: eiam_developerapi_20220225_models.RemoveUserFromOrganizationalUnitsHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> eiam_developerapi_20220225_models.RemoveUserFromOrganizationalUnitsResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.organizational_unit_ids):
+            body['organizationalUnitIds'] = request.organizational_unit_ids
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='RemoveUserFromOrganizationalUnits',
+            version='2022-02-25',
+            protocol='HTTPS',
+            pathname=f'/v2/{OpenApiUtilClient.get_encode_param(instance_id)}/{OpenApiUtilClient.get_encode_param(application_id)}/users/{OpenApiUtilClient.get_encode_param(user_id)}/actions/removeUserFromOrganizationalUnits',
+            method='POST',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='json',
+            body_type='none'
+        )
+        return TeaCore.from_map(
+            eiam_developerapi_20220225_models.RemoveUserFromOrganizationalUnitsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def remove_user_from_organizational_units(
+        self,
+        instance_id: str,
+        application_id: str,
+        user_id: str,
+        request: eiam_developerapi_20220225_models.RemoveUserFromOrganizationalUnitsRequest,
+    ) -> eiam_developerapi_20220225_models.RemoveUserFromOrganizationalUnitsResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = eiam_developerapi_20220225_models.RemoveUserFromOrganizationalUnitsHeaders()
+        return self.remove_user_from_organizational_units_with_options(instance_id, application_id, user_id, request, headers, runtime)
+
+    async def remove_user_from_organizational_units_async(
+        self,
+        instance_id: str,
+        application_id: str,
+        user_id: str,
+        request: eiam_developerapi_20220225_models.RemoveUserFromOrganizationalUnitsRequest,
+    ) -> eiam_developerapi_20220225_models.RemoveUserFromOrganizationalUnitsResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = eiam_developerapi_20220225_models.RemoveUserFromOrganizationalUnitsHeaders()
+        return await self.remove_user_from_organizational_units_with_options_async(instance_id, application_id, user_id, request, headers, runtime)
 
     def revoke_token_with_options(
         self,
         instance_id: str,
         application_id: str,
         request: eiam_developerapi_20220225_models.RevokeTokenRequest,
         headers: Dict[str, str],
@@ -2259,7 +2435,223 @@
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.RevokeTokenResponse(),
             await self.call_api_async(params, req, runtime)
         )
+
+    def revoke_token(
+        self,
+        instance_id: str,
+        application_id: str,
+        request: eiam_developerapi_20220225_models.RevokeTokenRequest,
+    ) -> eiam_developerapi_20220225_models.RevokeTokenResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.revoke_token_with_options(instance_id, application_id, request, headers, runtime)
+
+    async def revoke_token_async(
+        self,
+        instance_id: str,
+        application_id: str,
+        request: eiam_developerapi_20220225_models.RevokeTokenRequest,
+    ) -> eiam_developerapi_20220225_models.RevokeTokenResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.revoke_token_with_options_async(instance_id, application_id, request, headers, runtime)
+
+    def set_user_primary_organizational_unit_with_options(
+        self,
+        instance_id: str,
+        application_id: str,
+        user_id: str,
+        request: eiam_developerapi_20220225_models.SetUserPrimaryOrganizationalUnitRequest,
+        headers: eiam_developerapi_20220225_models.SetUserPrimaryOrganizationalUnitHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> eiam_developerapi_20220225_models.SetUserPrimaryOrganizationalUnitResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.organizational_unit_id):
+            body['organizationalUnitId'] = request.organizational_unit_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='SetUserPrimaryOrganizationalUnit',
+            version='2022-02-25',
+            protocol='HTTPS',
+            pathname=f'/v2/{OpenApiUtilClient.get_encode_param(instance_id)}/{OpenApiUtilClient.get_encode_param(application_id)}/users/{OpenApiUtilClient.get_encode_param(user_id)}/actions/setUserPrimaryOrganizationalUnit',
+            method='POST',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='json',
+            body_type='none'
+        )
+        return TeaCore.from_map(
+            eiam_developerapi_20220225_models.SetUserPrimaryOrganizationalUnitResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def set_user_primary_organizational_unit_with_options_async(
+        self,
+        instance_id: str,
+        application_id: str,
+        user_id: str,
+        request: eiam_developerapi_20220225_models.SetUserPrimaryOrganizationalUnitRequest,
+        headers: eiam_developerapi_20220225_models.SetUserPrimaryOrganizationalUnitHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> eiam_developerapi_20220225_models.SetUserPrimaryOrganizationalUnitResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.organizational_unit_id):
+            body['organizationalUnitId'] = request.organizational_unit_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='SetUserPrimaryOrganizationalUnit',
+            version='2022-02-25',
+            protocol='HTTPS',
+            pathname=f'/v2/{OpenApiUtilClient.get_encode_param(instance_id)}/{OpenApiUtilClient.get_encode_param(application_id)}/users/{OpenApiUtilClient.get_encode_param(user_id)}/actions/setUserPrimaryOrganizationalUnit',
+            method='POST',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='json',
+            body_type='none'
+        )
+        return TeaCore.from_map(
+            eiam_developerapi_20220225_models.SetUserPrimaryOrganizationalUnitResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def set_user_primary_organizational_unit(
+        self,
+        instance_id: str,
+        application_id: str,
+        user_id: str,
+        request: eiam_developerapi_20220225_models.SetUserPrimaryOrganizationalUnitRequest,
+    ) -> eiam_developerapi_20220225_models.SetUserPrimaryOrganizationalUnitResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = eiam_developerapi_20220225_models.SetUserPrimaryOrganizationalUnitHeaders()
+        return self.set_user_primary_organizational_unit_with_options(instance_id, application_id, user_id, request, headers, runtime)
+
+    async def set_user_primary_organizational_unit_async(
+        self,
+        instance_id: str,
+        application_id: str,
+        user_id: str,
+        request: eiam_developerapi_20220225_models.SetUserPrimaryOrganizationalUnitRequest,
+    ) -> eiam_developerapi_20220225_models.SetUserPrimaryOrganizationalUnitResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = eiam_developerapi_20220225_models.SetUserPrimaryOrganizationalUnitHeaders()
+        return await self.set_user_primary_organizational_unit_with_options_async(instance_id, application_id, user_id, request, headers, runtime)
+
+    def update_user_password_with_options(
+        self,
+        instance_id: str,
+        application_id: str,
+        user_id: str,
+        request: eiam_developerapi_20220225_models.UpdateUserPasswordRequest,
+        headers: eiam_developerapi_20220225_models.UpdateUserPasswordHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> eiam_developerapi_20220225_models.UpdateUserPasswordResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.password):
+            body['password'] = request.password
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UpdateUserPassword',
+            version='2022-02-25',
+            protocol='HTTPS',
+            pathname=f'/v2/{OpenApiUtilClient.get_encode_param(instance_id)}/{OpenApiUtilClient.get_encode_param(application_id)}/users/{OpenApiUtilClient.get_encode_param(user_id)}/actions/updateUserPassword',
+            method='POST',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='json',
+            body_type='none'
+        )
+        return TeaCore.from_map(
+            eiam_developerapi_20220225_models.UpdateUserPasswordResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def update_user_password_with_options_async(
+        self,
+        instance_id: str,
+        application_id: str,
+        user_id: str,
+        request: eiam_developerapi_20220225_models.UpdateUserPasswordRequest,
+        headers: eiam_developerapi_20220225_models.UpdateUserPasswordHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> eiam_developerapi_20220225_models.UpdateUserPasswordResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.password):
+            body['password'] = request.password
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='UpdateUserPassword',
+            version='2022-02-25',
+            protocol='HTTPS',
+            pathname=f'/v2/{OpenApiUtilClient.get_encode_param(instance_id)}/{OpenApiUtilClient.get_encode_param(application_id)}/users/{OpenApiUtilClient.get_encode_param(user_id)}/actions/updateUserPassword',
+            method='POST',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='json',
+            body_type='none'
+        )
+        return TeaCore.from_map(
+            eiam_developerapi_20220225_models.UpdateUserPasswordResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def update_user_password(
+        self,
+        instance_id: str,
+        application_id: str,
+        user_id: str,
+        request: eiam_developerapi_20220225_models.UpdateUserPasswordRequest,
+    ) -> eiam_developerapi_20220225_models.UpdateUserPasswordResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = eiam_developerapi_20220225_models.UpdateUserPasswordHeaders()
+        return self.update_user_password_with_options(instance_id, application_id, user_id, request, headers, runtime)
+
+    async def update_user_password_async(
+        self,
+        instance_id: str,
+        application_id: str,
+        user_id: str,
+        request: eiam_developerapi_20220225_models.UpdateUserPasswordRequest,
+    ) -> eiam_developerapi_20220225_models.UpdateUserPasswordResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = eiam_developerapi_20220225_models.UpdateUserPasswordHeaders()
+        return await self.update_user_password_with_options_async(instance_id, application_id, user_id, request, headers, runtime)
```

### Comparing `alibabacloud_eiam-developerapi20220225-1.0.5/alibabacloud_eiam_developerapi20220225/models.py` & `alibabacloud_eiam-developerapi20220225-1.0.6/alibabacloud_eiam_developerapi20220225/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,107 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import Dict, List
 
 
+class AddUserToOrganizationalUnitsHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        authorization: str = None,
+    ):
+        self.common_headers = common_headers
+        self.authorization = authorization
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.authorization is not None:
+            result['Authorization'] = self.authorization
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('Authorization') is not None:
+            self.authorization = m.get('Authorization')
+        return self
+
+
+class AddUserToOrganizationalUnitsRequest(TeaModel):
+    def __init__(
+        self,
+        organizational_unit_ids: List[str] = None,
+    ):
+        self.organizational_unit_ids = organizational_unit_ids
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.organizational_unit_ids is not None:
+            result['organizationalUnitIds'] = self.organizational_unit_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('organizationalUnitIds') is not None:
+            self.organizational_unit_ids = m.get('organizationalUnitIds')
+        return self
+
+
+class AddUserToOrganizationalUnitsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        return self
+
+
 class CreateOrganizationalUnitHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         authorization: str = None,
     ):
         self.common_headers = common_headers
@@ -946,18 +1040,21 @@
         access_token: str = None,
         expires_at: int = None,
         expires_in: int = None,
         id_token: str = None,
         refresh_token: str = None,
         token_type: str = None,
     ):
+        # access_token。
         self.access_token = access_token
         self.expires_at = expires_at
         self.expires_in = expires_in
+        # id_token。
         self.id_token = id_token
+        # refresh_token。
         self.refresh_token = refresh_token
         self.token_type = token_type
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1508,14 +1605,53 @@
         if m.get('fieldName') is not None:
             self.field_name = m.get('fieldName')
         if m.get('fieldValue') is not None:
             self.field_value = m.get('fieldValue')
         return self
 
 
+class GetUserResponseBodyGroups(TeaModel):
+    def __init__(
+        self,
+        description: str = None,
+        group_id: str = None,
+        group_name: str = None,
+    ):
+        self.description = description
+        self.group_id = group_id
+        self.group_name = group_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.description is not None:
+            result['description'] = self.description
+        if self.group_id is not None:
+            result['groupId'] = self.group_id
+        if self.group_name is not None:
+            result['groupName'] = self.group_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('description') is not None:
+            self.description = m.get('description')
+        if m.get('groupId') is not None:
+            self.group_id = m.get('groupId')
+        if m.get('groupName') is not None:
+            self.group_name = m.get('groupName')
+        return self
+
+
 class GetUserResponseBodyOrganizationalUnits(TeaModel):
     def __init__(
         self,
         organizational_unit_id: str = None,
         organizational_unit_name: str = None,
         primary: bool = None,
     ):
@@ -1557,14 +1693,15 @@
         account_expire_time: int = None,
         create_time: int = None,
         custom_fields: List[GetUserResponseBodyCustomFields] = None,
         description: str = None,
         display_name: str = None,
         email: str = None,
         email_verified: bool = None,
+        groups: List[GetUserResponseBodyGroups] = None,
         instance_id: str = None,
         lock_expire_time: int = None,
         organizational_units: List[GetUserResponseBodyOrganizationalUnits] = None,
         password_set: bool = None,
         phone_number: str = None,
         phone_number_verified: bool = None,
         phone_region: str = None,
@@ -1581,14 +1718,15 @@
         self.account_expire_time = account_expire_time
         self.create_time = create_time
         self.custom_fields = custom_fields
         self.description = description
         self.display_name = display_name
         self.email = email
         self.email_verified = email_verified
+        self.groups = groups
         self.instance_id = instance_id
         self.lock_expire_time = lock_expire_time
         self.organizational_units = organizational_units
         self.password_set = password_set
         self.phone_number = phone_number
         self.phone_number_verified = phone_number_verified
         self.phone_region = phone_region
@@ -1603,14 +1741,18 @@
         self.username = username
 
     def validate(self):
         if self.custom_fields:
             for k in self.custom_fields:
                 if k:
                     k.validate()
+        if self.groups:
+            for k in self.groups:
+                if k:
+                    k.validate()
         if self.organizational_units:
             for k in self.organizational_units:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
@@ -1630,14 +1772,18 @@
             result['description'] = self.description
         if self.display_name is not None:
             result['displayName'] = self.display_name
         if self.email is not None:
             result['email'] = self.email
         if self.email_verified is not None:
             result['emailVerified'] = self.email_verified
+        result['groups'] = []
+        if self.groups is not None:
+            for k in self.groups:
+                result['groups'].append(k.to_map() if k else None)
         if self.instance_id is not None:
             result['instanceId'] = self.instance_id
         if self.lock_expire_time is not None:
             result['lockExpireTime'] = self.lock_expire_time
         result['organizationalUnits'] = []
         if self.organizational_units is not None:
             for k in self.organizational_units:
@@ -1685,14 +1831,19 @@
             self.description = m.get('description')
         if m.get('displayName') is not None:
             self.display_name = m.get('displayName')
         if m.get('email') is not None:
             self.email = m.get('email')
         if m.get('emailVerified') is not None:
             self.email_verified = m.get('emailVerified')
+        self.groups = []
+        if m.get('groups') is not None:
+            for k in m.get('groups'):
+                temp_model = GetUserResponseBodyGroups()
+                self.groups.append(temp_model.from_map(k))
         if m.get('instanceId') is not None:
             self.instance_id = m.get('instanceId')
         if m.get('lockExpireTime') is not None:
             self.lock_expire_time = m.get('lockExpireTime')
         self.organizational_units = []
         if m.get('organizationalUnits') is not None:
             for k in m.get('organizationalUnits'):
@@ -2823,14 +2974,15 @@
         self.create_time = create_time
         self.description = description
         self.display_name = display_name
         self.email = email
         self.email_verified = email_verified
         self.instance_id = instance_id
         self.lock_expire_time = lock_expire_time
+        # 密码是否已设置
         self.password_set = password_set
         self.phone_number = phone_number
         self.phone_number_verified = phone_number_verified
         self.phone_region = phone_region
         self.register_time = register_time
         self.status = status
         self.update_time = update_time
@@ -3155,18 +3307,24 @@
 
 
 class PatchUserRequestCustomFields(TeaModel):
     def __init__(
         self,
         field_name: str = None,
         field_value: str = None,
+        operation: str = None,
         operator: str = None,
     ):
         self.field_name = field_name
         self.field_value = field_value
+        # 字段操作类型，取值可选范围：
+        # - add：添加。
+        # - replace：替换。若对应扩展字段无设置值，会转换为add操作。
+        # - remove：移除。
+        self.operation = operation
         self.operator = operator
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3174,24 +3332,28 @@
             return _map
 
         result = dict()
         if self.field_name is not None:
             result['fieldName'] = self.field_name
         if self.field_value is not None:
             result['fieldValue'] = self.field_value
+        if self.operation is not None:
+            result['operation'] = self.operation
         if self.operator is not None:
             result['operator'] = self.operator
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('fieldName') is not None:
             self.field_name = m.get('fieldName')
         if m.get('fieldValue') is not None:
             self.field_value = m.get('fieldValue')
+        if m.get('operation') is not None:
+            self.operation = m.get('operation')
         if m.get('operator') is not None:
             self.operator = m.get('operator')
         return self
 
 
 class PatchUserRequest(TeaModel):
     def __init__(
@@ -3300,14 +3462,108 @@
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         return self
 
 
+class RemoveUserFromOrganizationalUnitsHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        authorization: str = None,
+    ):
+        self.common_headers = common_headers
+        self.authorization = authorization
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.authorization is not None:
+            result['Authorization'] = self.authorization
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('Authorization') is not None:
+            self.authorization = m.get('Authorization')
+        return self
+
+
+class RemoveUserFromOrganizationalUnitsRequest(TeaModel):
+    def __init__(
+        self,
+        organizational_unit_ids: List[str] = None,
+    ):
+        self.organizational_unit_ids = organizational_unit_ids
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.organizational_unit_ids is not None:
+            result['organizationalUnitIds'] = self.organizational_unit_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('organizationalUnitIds') is not None:
+            self.organizational_unit_ids = m.get('organizationalUnitIds')
+        return self
+
+
+class RemoveUserFromOrganizationalUnitsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        return self
+
+
 class RevokeTokenRequest(TeaModel):
     def __init__(
         self,
         client_id: str = None,
         client_secret: str = None,
         token: str = None,
         token_type_hint: str = None,
@@ -3386,7 +3642,195 @@
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             self.body = m.get('body')
         return self
 
 
+class SetUserPrimaryOrganizationalUnitHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        authorization: str = None,
+    ):
+        self.common_headers = common_headers
+        self.authorization = authorization
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.authorization is not None:
+            result['Authorization'] = self.authorization
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('Authorization') is not None:
+            self.authorization = m.get('Authorization')
+        return self
+
+
+class SetUserPrimaryOrganizationalUnitRequest(TeaModel):
+    def __init__(
+        self,
+        organizational_unit_id: str = None,
+    ):
+        self.organizational_unit_id = organizational_unit_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.organizational_unit_id is not None:
+            result['organizationalUnitId'] = self.organizational_unit_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('organizationalUnitId') is not None:
+            self.organizational_unit_id = m.get('organizationalUnitId')
+        return self
+
+
+class SetUserPrimaryOrganizationalUnitResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        return self
+
+
+class UpdateUserPasswordHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        authorization: str = None,
+    ):
+        self.common_headers = common_headers
+        self.authorization = authorization
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.authorization is not None:
+            result['Authorization'] = self.authorization
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('Authorization') is not None:
+            self.authorization = m.get('Authorization')
+        return self
+
+
+class UpdateUserPasswordRequest(TeaModel):
+    def __init__(
+        self,
+        password: str = None,
+    ):
+        self.password = password
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.password is not None:
+            result['password'] = self.password
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('password') is not None:
+            self.password = m.get('password')
+        return self
+
+
+class UpdateUserPasswordResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        return self
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_eiam-developerapi20220225-1.0.5/alibabacloud_eiam_developerapi20220225.egg-info/PKG-INFO` & `alibabacloud_eiam-developerapi20220225-1.0.6/alibabacloud_eiam_developerapi20220225.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-eiam-developerapi20220225
-Version: 1.0.5
+Version: 1.0.6
 Summary: Alibaba Cloud Eiam-developerapi (20220225) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eiam-developerapi20220225-1.0.5/alibabacloud_eiam_developerapi20220225.egg-info/SOURCES.txt` & `alibabacloud_eiam-developerapi20220225-1.0.6/alibabacloud_eiam_developerapi20220225.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_eiam-developerapi20220225-1.0.5/setup.py` & `alibabacloud_eiam-developerapi20220225-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_eiam-developerapi20220225.
 
-Created on 28/11/2022
+Created on 16/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_eiam_developerapi20220225"
 NAME = "alibabacloud_eiam-developerapi20220225" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Eiam-developerapi (20220225) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
-    "alibabacloud_openapi_util>=0.2.0, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

