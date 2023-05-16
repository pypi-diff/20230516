# Comparing `tmp/alibabacloud_eiam-developerapi20220225_py2-1.0.5.tar.gz` & `tmp/alibabacloud_eiam-developerapi20220225_py2-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_eiam-developerapi20220225_py2-1.0.5.tar", last modified: Mon Nov 28 08:32:25 2022, max compression
+gzip compressed data, was "dist/alibabacloud_eiam-developerapi20220225_py2-1.0.6.tar", last modified: Tue May 16 07:59:37 2023, max compression
```

## Comparing `alibabacloud_eiam-developerapi20220225_py2-1.0.5.tar` & `alibabacloud_eiam-developerapi20220225_py2-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-28 08:32:25.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      180 2022-11-28 08:32:25.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-11-28 08:32:25.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-11-28 08:32:25.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2556 2022-11-28 08:32:25.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1075 2022-11-28 08:32:25.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1158 2022-11-28 08:32:25.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-28 08:32:25.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.5/alibabacloud_eiam_developerapi20220225/
--rw-r--r--   0 root         (0) root         (0)       21 2022-11-28 08:32:25.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.5/alibabacloud_eiam_developerapi20220225/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43931 2022-11-28 08:32:25.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.5/alibabacloud_eiam_developerapi20220225/client.py
--rw-r--r--   0 root         (0) root         (0)   111052 2022-11-28 08:32:25.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.5/alibabacloud_eiam_developerapi20220225/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-28 08:32:25.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.5/alibabacloud_eiam_developerapi20220225_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2556 2022-11-28 08:32:25.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.5/alibabacloud_eiam_developerapi20220225_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      552 2022-11-28 08:32:25.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.5/alibabacloud_eiam_developerapi20220225_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-28 08:32:25.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.5/alibabacloud_eiam_developerapi20220225_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-11-28 08:32:25.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.5/alibabacloud_eiam_developerapi20220225_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       39 2022-11-28 08:32:25.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.5/alibabacloud_eiam_developerapi20220225_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-11-28 08:32:25.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2975 2022-11-28 08:32:25.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:59:37.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      216 2023-05-16 07:59:37.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.6/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-16 07:59:37.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-16 07:59:37.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-05-16 07:59:37.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-05-16 07:59:37.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1158 2023-05-16 07:59:37.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:59:37.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.6/alibabacloud_eiam_developerapi20220225/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 07:59:37.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.6/alibabacloud_eiam_developerapi20220225/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51572 2023-05-16 07:59:37.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.6/alibabacloud_eiam_developerapi20220225/client.py
+-rw-r--r--   0 root         (0) root         (0)   124011 2023-05-16 07:59:37.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.6/alibabacloud_eiam_developerapi20220225/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:59:37.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.6/alibabacloud_eiam_developerapi20220225_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-05-16 07:59:37.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.6/alibabacloud_eiam_developerapi20220225_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      552 2023-05-16 07:59:37.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.6/alibabacloud_eiam_developerapi20220225_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 07:59:37.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.6/alibabacloud_eiam_developerapi20220225_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-16 07:59:37.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.6/alibabacloud_eiam_developerapi20220225_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-16 07:59:37.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.6/alibabacloud_eiam_developerapi20220225_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 07:59:37.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2975 2023-05-16 07:59:37.000000 alibabacloud_eiam-developerapi20220225_py2-1.0.6/setup.py
```

### Comparing `alibabacloud_eiam-developerapi20220225_py2-1.0.5/LICENSE` & `alibabacloud_eiam-developerapi20220225_py2-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_eiam-developerapi20220225_py2-1.0.5/PKG-INFO` & `alibabacloud_eiam-developerapi20220225_py2-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_eiam-developerapi20220225_py2
-Version: 1.0.5
+Version: 1.0.6
 Summary: Alibaba Cloud Eiam-developerapi (20220225) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eiam-developerapi20220225_py2-1.0.5/README-CN.md` & `alibabacloud_eiam-developerapi20220225_py2-1.0.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eiam-developerapi20220225_py2-1.0.5/README.md` & `alibabacloud_eiam-developerapi20220225_py2-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eiam-developerapi20220225_py2-1.0.5/alibabacloud_eiam_developerapi20220225/client.py` & `alibabacloud_eiam-developerapi20220225_py2-1.0.6/alibabacloud_eiam_developerapi20220225/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,18 +28,48 @@
     def get_endpoint(self, product_id, region_id, endpoint_rule, network, suffix, endpoint_map, endpoint):
         if not UtilClient.empty(endpoint):
             return endpoint
         if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
             return endpoint_map.get(region_id)
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
-    def create_organizational_unit(self, instance_id, application_id, request):
+    def add_user_to_organizational_units_with_options(self, instance_id, application_id, user_id, request, headers, runtime):
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
+            pathname='/v2/%s/%s/users/%s/actions/addUserToOrganizationalUnits' % (TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(instance_id)), TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(application_id)), TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(user_id))),
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
+    def add_user_to_organizational_units(self, instance_id, application_id, user_id, request):
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.CreateOrganizationalUnitHeaders()
-        return self.create_organizational_unit_with_options(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.AddUserToOrganizationalUnitsHeaders()
+        return self.add_user_to_organizational_units_with_options(instance_id, application_id, user_id, request, headers, runtime)
 
     def create_organizational_unit_with_options(self, instance_id, application_id, request, headers, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.description):
             body['description'] = request.description
         if not UtilClient.is_unset(request.organizational_unit_external_id):
@@ -69,18 +99,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.CreateOrganizationalUnitResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def create_user(self, instance_id, application_id, request):
+    def create_organizational_unit(self, instance_id, application_id, request):
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.CreateUserHeaders()
-        return self.create_user_with_options(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.CreateOrganizationalUnitHeaders()
+        return self.create_organizational_unit_with_options(instance_id, application_id, request, headers, runtime)
 
     def create_user_with_options(self, instance_id, application_id, request, headers, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.custom_fields):
             body['customFields'] = request.custom_fields
         if not UtilClient.is_unset(request.description):
@@ -128,18 +158,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.CreateUserResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def delete_organizational_unit(self, instance_id, application_id, organizational_unit_id):
+    def create_user(self, instance_id, application_id, request):
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.DeleteOrganizationalUnitHeaders()
-        return self.delete_organizational_unit_with_options(instance_id, application_id, organizational_unit_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.CreateUserHeaders()
+        return self.create_user_with_options(instance_id, application_id, request, headers, runtime)
 
     def delete_organizational_unit_with_options(self, instance_id, application_id, organizational_unit_id, headers, runtime):
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.authorization):
             real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
@@ -158,18 +188,18 @@
             body_type='none'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.DeleteOrganizationalUnitResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def delete_user(self, instance_id, application_id, user_id):
+    def delete_organizational_unit(self, instance_id, application_id, organizational_unit_id):
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.DeleteUserHeaders()
-        return self.delete_user_with_options(instance_id, application_id, user_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.DeleteOrganizationalUnitHeaders()
+        return self.delete_organizational_unit_with_options(instance_id, application_id, organizational_unit_id, headers, runtime)
 
     def delete_user_with_options(self, instance_id, application_id, user_id, headers, runtime):
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.authorization):
             real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
@@ -188,18 +218,18 @@
             body_type='none'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.DeleteUserResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def disable_user(self, instance_id, application_id, user_id):
+    def delete_user(self, instance_id, application_id, user_id):
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.DisableUserHeaders()
-        return self.disable_user_with_options(instance_id, application_id, user_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.DeleteUserHeaders()
+        return self.delete_user_with_options(instance_id, application_id, user_id, headers, runtime)
 
     def disable_user_with_options(self, instance_id, application_id, user_id, headers, runtime):
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.authorization):
             real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
@@ -218,18 +248,18 @@
             body_type='none'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.DisableUserResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def enable_user(self, instance_id, application_id, user_id):
+    def disable_user(self, instance_id, application_id, user_id):
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.EnableUserHeaders()
-        return self.enable_user_with_options(instance_id, application_id, user_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.DisableUserHeaders()
+        return self.disable_user_with_options(instance_id, application_id, user_id, headers, runtime)
 
     def enable_user_with_options(self, instance_id, application_id, user_id, headers, runtime):
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.authorization):
             real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
@@ -248,18 +278,18 @@
             body_type='none'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.EnableUserResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def generate_device_code(self, instance_id, application_id, request):
+    def enable_user(self, instance_id, application_id, user_id):
         runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.generate_device_code_with_options(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.EnableUserHeaders()
+        return self.enable_user_with_options(instance_id, application_id, user_id, headers, runtime)
 
     def generate_device_code_with_options(self, instance_id, application_id, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.scope):
             query['scope'] = request.scope
         req = open_api_models.OpenApiRequest(
@@ -278,18 +308,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.GenerateDeviceCodeResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def generate_token(self, instance_id, application_id, request):
+    def generate_device_code(self, instance_id, application_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.generate_token_with_options(instance_id, application_id, request, headers, runtime)
+        return self.generate_device_code_with_options(instance_id, application_id, request, headers, runtime)
 
     def generate_token_with_options(self, instance_id, application_id, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_id):
             query['client_id'] = request.client_id
         if not UtilClient.is_unset(request.client_secret):
@@ -330,18 +360,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.GenerateTokenResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_application_provisioning_scope(self, instance_id, application_id):
+    def generate_token(self, instance_id, application_id, request):
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetApplicationProvisioningScopeHeaders()
-        return self.get_application_provisioning_scope_with_options(instance_id, application_id, headers, runtime)
+        headers = {}
+        return self.generate_token_with_options(instance_id, application_id, request, headers, runtime)
 
     def get_application_provisioning_scope_with_options(self, instance_id, application_id, headers, runtime):
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.authorization):
             real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
@@ -360,18 +390,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.GetApplicationProvisioningScopeResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_organizational_unit(self, instance_id, application_id, organizational_unit_id):
+    def get_application_provisioning_scope(self, instance_id, application_id):
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetOrganizationalUnitHeaders()
-        return self.get_organizational_unit_with_options(instance_id, application_id, organizational_unit_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetApplicationProvisioningScopeHeaders()
+        return self.get_application_provisioning_scope_with_options(instance_id, application_id, headers, runtime)
 
     def get_organizational_unit_with_options(self, instance_id, application_id, organizational_unit_id, headers, runtime):
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.authorization):
             real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
@@ -390,18 +420,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.GetOrganizationalUnitResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_organizational_unit_id_by_external_id(self, instance_id, application_id, request):
+    def get_organizational_unit(self, instance_id, application_id, organizational_unit_id):
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetOrganizationalUnitIdByExternalIdHeaders()
-        return self.get_organizational_unit_id_by_external_id_with_options(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetOrganizationalUnitHeaders()
+        return self.get_organizational_unit_with_options(instance_id, application_id, organizational_unit_id, headers, runtime)
 
     def get_organizational_unit_id_by_external_id_with_options(self, instance_id, application_id, request, headers, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.organizational_unit_external_id):
             body['organizationalUnitExternalId'] = request.organizational_unit_external_id
         if not UtilClient.is_unset(request.organizational_unit_source_id):
@@ -429,18 +459,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.GetOrganizationalUnitIdByExternalIdResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_user(self, instance_id, application_id, user_id):
+    def get_organizational_unit_id_by_external_id(self, instance_id, application_id, request):
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetUserHeaders()
-        return self.get_user_with_options(instance_id, application_id, user_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetOrganizationalUnitIdByExternalIdHeaders()
+        return self.get_organizational_unit_id_by_external_id_with_options(instance_id, application_id, request, headers, runtime)
 
     def get_user_with_options(self, instance_id, application_id, user_id, headers, runtime):
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.authorization):
             real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
@@ -459,18 +489,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.GetUserResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_user_id_by_email(self, instance_id, application_id, request):
+    def get_user(self, instance_id, application_id, user_id):
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetUserIdByEmailHeaders()
-        return self.get_user_id_by_email_with_options(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetUserHeaders()
+        return self.get_user_with_options(instance_id, application_id, user_id, headers, runtime)
 
     def get_user_id_by_email_with_options(self, instance_id, application_id, request, headers, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.email):
             body['email'] = request.email
         real_headers = {}
@@ -494,18 +524,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.GetUserIdByEmailResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_user_id_by_phone_number(self, instance_id, application_id, request):
+    def get_user_id_by_email(self, instance_id, application_id, request):
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetUserIdByPhoneNumberHeaders()
-        return self.get_user_id_by_phone_number_with_options(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetUserIdByEmailHeaders()
+        return self.get_user_id_by_email_with_options(instance_id, application_id, request, headers, runtime)
 
     def get_user_id_by_phone_number_with_options(self, instance_id, application_id, request, headers, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.phone_number):
             body['phoneNumber'] = request.phone_number
         real_headers = {}
@@ -529,18 +559,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.GetUserIdByPhoneNumberResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_user_id_by_user_external_id(self, instance_id, application_id, request):
+    def get_user_id_by_phone_number(self, instance_id, application_id, request):
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetUserIdByUserExternalIdHeaders()
-        return self.get_user_id_by_user_external_id_with_options(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetUserIdByPhoneNumberHeaders()
+        return self.get_user_id_by_phone_number_with_options(instance_id, application_id, request, headers, runtime)
 
     def get_user_id_by_user_external_id_with_options(self, instance_id, application_id, request, headers, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.user_external_id):
             body['userExternalId'] = request.user_external_id
         if not UtilClient.is_unset(request.user_source_id):
@@ -568,18 +598,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.GetUserIdByUserExternalIdResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_user_id_by_username(self, instance_id, application_id, request):
+    def get_user_id_by_user_external_id(self, instance_id, application_id, request):
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetUserIdByUsernameHeaders()
-        return self.get_user_id_by_username_with_options(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetUserIdByUserExternalIdHeaders()
+        return self.get_user_id_by_user_external_id_with_options(instance_id, application_id, request, headers, runtime)
 
     def get_user_id_by_username_with_options(self, instance_id, application_id, request, headers, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.username):
             body['username'] = request.username
         real_headers = {}
@@ -603,18 +633,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.GetUserIdByUsernameResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def get_user_info(self, instance_id, application_id):
+    def get_user_id_by_username(self, instance_id, application_id, request):
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.GetUserInfoHeaders()
-        return self.get_user_info_with_options(instance_id, application_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetUserIdByUsernameHeaders()
+        return self.get_user_id_by_username_with_options(instance_id, application_id, request, headers, runtime)
 
     def get_user_info_with_options(self, instance_id, application_id, headers, runtime):
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.authorization):
             real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
@@ -633,18 +663,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.GetUserInfoResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def list_organizational_unit_parent_ids(self, instance_id, application_id, organizational_unit_id):
+    def get_user_info(self, instance_id, application_id):
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.ListOrganizationalUnitParentIdsHeaders()
-        return self.list_organizational_unit_parent_ids_with_options(instance_id, application_id, organizational_unit_id, headers, runtime)
+        headers = eiam_developerapi_20220225_models.GetUserInfoHeaders()
+        return self.get_user_info_with_options(instance_id, application_id, headers, runtime)
 
     def list_organizational_unit_parent_ids_with_options(self, instance_id, application_id, organizational_unit_id, headers, runtime):
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.authorization):
             real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
@@ -663,18 +693,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.ListOrganizationalUnitParentIdsResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def list_organizational_units(self, instance_id, application_id, request):
+    def list_organizational_unit_parent_ids(self, instance_id, application_id, organizational_unit_id):
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.ListOrganizationalUnitsHeaders()
-        return self.list_organizational_units_with_options(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.ListOrganizationalUnitParentIdsHeaders()
+        return self.list_organizational_unit_parent_ids_with_options(instance_id, application_id, organizational_unit_id, headers, runtime)
 
     def list_organizational_units_with_options(self, instance_id, application_id, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['pageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -702,18 +732,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.ListOrganizationalUnitsResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def list_users(self, instance_id, application_id, request):
+    def list_organizational_units(self, instance_id, application_id, request):
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.ListUsersHeaders()
-        return self.list_users_with_options(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.ListOrganizationalUnitsHeaders()
+        return self.list_organizational_units_with_options(instance_id, application_id, request, headers, runtime)
 
     def list_users_with_options(self, instance_id, application_id, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.organizational_unit_id):
             query['organizationalUnitId'] = request.organizational_unit_id
         if not UtilClient.is_unset(request.page_number):
@@ -741,18 +771,18 @@
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.ListUsersResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def patch_organizational_unit(self, instance_id, application_id, organizational_unit_id, request):
+    def list_users(self, instance_id, application_id, request):
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.PatchOrganizationalUnitHeaders()
-        return self.patch_organizational_unit_with_options(instance_id, application_id, organizational_unit_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.ListUsersHeaders()
+        return self.list_users_with_options(instance_id, application_id, request, headers, runtime)
 
     def patch_organizational_unit_with_options(self, instance_id, application_id, organizational_unit_id, request, headers, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.description):
             body['description'] = request.description
         if not UtilClient.is_unset(request.organizational_unit_name):
@@ -778,18 +808,18 @@
             body_type='none'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.PatchOrganizationalUnitResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def patch_user(self, instance_id, application_id, user_id, request):
+    def patch_organizational_unit(self, instance_id, application_id, organizational_unit_id, request):
         runtime = util_models.RuntimeOptions()
-        headers = eiam_developerapi_20220225_models.PatchUserHeaders()
-        return self.patch_user_with_options(instance_id, application_id, user_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.PatchOrganizationalUnitHeaders()
+        return self.patch_organizational_unit_with_options(instance_id, application_id, organizational_unit_id, request, headers, runtime)
 
     def patch_user_with_options(self, instance_id, application_id, user_id, request, headers, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.custom_fields):
             body['customFields'] = request.custom_fields
         if not UtilClient.is_unset(request.display_name):
@@ -827,18 +857,53 @@
             body_type='none'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.PatchUserResponse(),
             self.call_api(params, req, runtime)
         )
 
-    def revoke_token(self, instance_id, application_id, request):
+    def patch_user(self, instance_id, application_id, user_id, request):
         runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.revoke_token_with_options(instance_id, application_id, request, headers, runtime)
+        headers = eiam_developerapi_20220225_models.PatchUserHeaders()
+        return self.patch_user_with_options(instance_id, application_id, user_id, request, headers, runtime)
+
+    def remove_user_from_organizational_units_with_options(self, instance_id, application_id, user_id, request, headers, runtime):
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
+            pathname='/v2/%s/%s/users/%s/actions/removeUserFromOrganizationalUnits' % (TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(instance_id)), TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(application_id)), TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(user_id))),
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
+    def remove_user_from_organizational_units(self, instance_id, application_id, user_id, request):
+        runtime = util_models.RuntimeOptions()
+        headers = eiam_developerapi_20220225_models.RemoveUserFromOrganizationalUnitsHeaders()
+        return self.remove_user_from_organizational_units_with_options(instance_id, application_id, user_id, request, headers, runtime)
 
     def revoke_token_with_options(self, instance_id, application_id, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_id):
             query['client_id'] = request.client_id
         if not UtilClient.is_unset(request.client_secret):
@@ -862,7 +927,82 @@
             req_body_type='json',
             body_type='json'
         )
         return TeaCore.from_map(
             eiam_developerapi_20220225_models.RevokeTokenResponse(),
             self.call_api(params, req, runtime)
         )
+
+    def revoke_token(self, instance_id, application_id, request):
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.revoke_token_with_options(instance_id, application_id, request, headers, runtime)
+
+    def set_user_primary_organizational_unit_with_options(self, instance_id, application_id, user_id, request, headers, runtime):
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
+            pathname='/v2/%s/%s/users/%s/actions/setUserPrimaryOrganizationalUnit' % (TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(instance_id)), TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(application_id)), TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(user_id))),
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
+    def set_user_primary_organizational_unit(self, instance_id, application_id, user_id, request):
+        runtime = util_models.RuntimeOptions()
+        headers = eiam_developerapi_20220225_models.SetUserPrimaryOrganizationalUnitHeaders()
+        return self.set_user_primary_organizational_unit_with_options(instance_id, application_id, user_id, request, headers, runtime)
+
+    def update_user_password_with_options(self, instance_id, application_id, user_id, request, headers, runtime):
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
+            pathname='/v2/%s/%s/users/%s/actions/updateUserPassword' % (TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(instance_id)), TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(application_id)), TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(user_id))),
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
+    def update_user_password(self, instance_id, application_id, user_id, request):
+        runtime = util_models.RuntimeOptions()
+        headers = eiam_developerapi_20220225_models.UpdateUserPasswordHeaders()
+        return self.update_user_password_with_options(instance_id, application_id, user_id, request, headers, runtime)
```

### Comparing `alibabacloud_eiam-developerapi20220225_py2-1.0.5/alibabacloud_eiam_developerapi20220225/models.py` & `alibabacloud_eiam-developerapi20220225_py2-1.0.6/alibabacloud_eiam_developerapi20220225/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,95 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 
 
+class AddUserToOrganizationalUnitsHeaders(TeaModel):
+    def __init__(self, common_headers=None, authorization=None):
+        self.common_headers = common_headers  # type: dict[str, str]
+        self.authorization = authorization  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(AddUserToOrganizationalUnitsHeaders, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('Authorization') is not None:
+            self.authorization = m.get('Authorization')
+        return self
+
+
+class AddUserToOrganizationalUnitsRequest(TeaModel):
+    def __init__(self, organizational_unit_ids=None):
+        self.organizational_unit_ids = organizational_unit_ids  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(AddUserToOrganizationalUnitsRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.organizational_unit_ids is not None:
+            result['organizationalUnitIds'] = self.organizational_unit_ids
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('organizationalUnitIds') is not None:
+            self.organizational_unit_ids = m.get('organizationalUnitIds')
+        return self
+
+
+class AddUserToOrganizationalUnitsResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+
+    def to_map(self):
+        _map = super(AddUserToOrganizationalUnitsResponse, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        return self
+
+
 class CreateOrganizationalUnitHeaders(TeaModel):
     def __init__(self, common_headers=None, authorization=None):
         self.common_headers = common_headers  # type: dict[str, str]
         self.authorization = authorization  # type: str
 
     def validate(self):
         pass
@@ -827,18 +910,21 @@
             self.username = m.get('username')
         return self
 
 
 class GenerateTokenResponseBody(TeaModel):
     def __init__(self, access_token=None, expires_at=None, expires_in=None, id_token=None, refresh_token=None,
                  token_type=None):
+        # access_token。
         self.access_token = access_token  # type: str
         self.expires_at = expires_at  # type: long
         self.expires_in = expires_in  # type: long
+        # id_token。
         self.id_token = id_token  # type: str
+        # refresh_token。
         self.refresh_token = refresh_token  # type: str
         self.token_type = token_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1329,14 +1415,48 @@
         if m.get('fieldName') is not None:
             self.field_name = m.get('fieldName')
         if m.get('fieldValue') is not None:
             self.field_value = m.get('fieldValue')
         return self
 
 
+class GetUserResponseBodyGroups(TeaModel):
+    def __init__(self, description=None, group_id=None, group_name=None):
+        self.description = description  # type: str
+        self.group_id = group_id  # type: str
+        self.group_name = group_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetUserResponseBodyGroups, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, organizational_unit_id=None, organizational_unit_name=None, primary=None):
         self.organizational_unit_id = organizational_unit_id  # type: str
         self.organizational_unit_name = organizational_unit_name  # type: str
         self.primary = primary  # type: bool
 
     def validate(self):
@@ -1365,25 +1485,26 @@
         if m.get('primary') is not None:
             self.primary = m.get('primary')
         return self
 
 
 class GetUserResponseBody(TeaModel):
     def __init__(self, account_expire_time=None, create_time=None, custom_fields=None, description=None,
-                 display_name=None, email=None, email_verified=None, instance_id=None, lock_expire_time=None,
+                 display_name=None, email=None, email_verified=None, groups=None, instance_id=None, lock_expire_time=None,
                  organizational_units=None, password_set=None, phone_number=None, phone_number_verified=None, phone_region=None,
                  primary_organizational_unit_id=None, register_time=None, status=None, update_time=None, user_external_id=None, user_id=None,
                  user_source_id=None, user_source_type=None, username=None):
         self.account_expire_time = account_expire_time  # type: long
         self.create_time = create_time  # type: long
         self.custom_fields = custom_fields  # type: list[GetUserResponseBodyCustomFields]
         self.description = description  # type: str
         self.display_name = display_name  # type: str
         self.email = email  # type: str
         self.email_verified = email_verified  # type: bool
+        self.groups = groups  # type: list[GetUserResponseBodyGroups]
         self.instance_id = instance_id  # type: str
         self.lock_expire_time = lock_expire_time  # type: long
         self.organizational_units = organizational_units  # type: list[GetUserResponseBodyOrganizationalUnits]
         self.password_set = password_set  # type: bool
         self.phone_number = phone_number  # type: str
         self.phone_number_verified = phone_number_verified  # type: bool
         self.phone_region = phone_region  # type: str
@@ -1398,14 +1519,18 @@
         self.username = username  # type: str
 
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
         _map = super(GetUserResponseBody, self).to_map()
@@ -1425,14 +1550,18 @@
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
@@ -1480,14 +1609,19 @@
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
@@ -2474,14 +2608,15 @@
         self.create_time = create_time  # type: long
         self.description = description  # type: str
         self.display_name = display_name  # type: str
         self.email = email  # type: str
         self.email_verified = email_verified  # type: bool
         self.instance_id = instance_id  # type: str
         self.lock_expire_time = lock_expire_time  # type: long
+        # 密码是否已设置
         self.password_set = password_set  # type: bool
         self.phone_number = phone_number  # type: str
         self.phone_number_verified = phone_number_verified  # type: bool
         self.phone_region = phone_region  # type: str
         self.register_time = register_time  # type: long
         self.status = status  # type: str
         self.update_time = update_time  # type: long
@@ -2777,17 +2912,22 @@
             self.common_headers = m.get('commonHeaders')
         if m.get('Authorization') is not None:
             self.authorization = m.get('Authorization')
         return self
 
 
 class PatchUserRequestCustomFields(TeaModel):
-    def __init__(self, field_name=None, field_value=None, operator=None):
+    def __init__(self, field_name=None, field_value=None, operation=None, operator=None):
         self.field_name = field_name  # type: str
         self.field_value = field_value  # type: str
+        # 字段操作类型，取值可选范围：
+        # - add：添加。
+        # - replace：替换。若对应扩展字段无设置值，会转换为add操作。
+        # - remove：移除。
+        self.operation = operation  # type: str
         self.operator = operator  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(PatchUserRequestCustomFields, self).to_map()
@@ -2795,24 +2935,28 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, custom_fields=None, display_name=None, email=None, email_verified=None, phone_number=None,
@@ -2908,14 +3052,97 @@
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         return self
 
 
+class RemoveUserFromOrganizationalUnitsHeaders(TeaModel):
+    def __init__(self, common_headers=None, authorization=None):
+        self.common_headers = common_headers  # type: dict[str, str]
+        self.authorization = authorization  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(RemoveUserFromOrganizationalUnitsHeaders, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('Authorization') is not None:
+            self.authorization = m.get('Authorization')
+        return self
+
+
+class RemoveUserFromOrganizationalUnitsRequest(TeaModel):
+    def __init__(self, organizational_unit_ids=None):
+        self.organizational_unit_ids = organizational_unit_ids  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(RemoveUserFromOrganizationalUnitsRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.organizational_unit_ids is not None:
+            result['organizationalUnitIds'] = self.organizational_unit_ids
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('organizationalUnitIds') is not None:
+            self.organizational_unit_ids = m.get('organizationalUnitIds')
+        return self
+
+
+class RemoveUserFromOrganizationalUnitsResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+
+    def to_map(self):
+        _map = super(RemoveUserFromOrganizationalUnitsResponse, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        return self
+
+
 class RevokeTokenRequest(TeaModel):
     def __init__(self, client_id=None, client_secret=None, token=None, token_type_hint=None):
         self.client_id = client_id  # type: str
         self.client_secret = client_secret  # type: str
         self.token = token  # type: str
         self.token_type_hint = token_type_hint  # type: str
 
@@ -2983,7 +3210,173 @@
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             self.body = m.get('body')
         return self
 
 
+class SetUserPrimaryOrganizationalUnitHeaders(TeaModel):
+    def __init__(self, common_headers=None, authorization=None):
+        self.common_headers = common_headers  # type: dict[str, str]
+        self.authorization = authorization  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetUserPrimaryOrganizationalUnitHeaders, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('Authorization') is not None:
+            self.authorization = m.get('Authorization')
+        return self
+
+
+class SetUserPrimaryOrganizationalUnitRequest(TeaModel):
+    def __init__(self, organizational_unit_id=None):
+        self.organizational_unit_id = organizational_unit_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetUserPrimaryOrganizationalUnitRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.organizational_unit_id is not None:
+            result['organizationalUnitId'] = self.organizational_unit_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('organizationalUnitId') is not None:
+            self.organizational_unit_id = m.get('organizationalUnitId')
+        return self
+
+
+class SetUserPrimaryOrganizationalUnitResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+
+    def to_map(self):
+        _map = super(SetUserPrimaryOrganizationalUnitResponse, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        return self
+
+
+class UpdateUserPasswordHeaders(TeaModel):
+    def __init__(self, common_headers=None, authorization=None):
+        self.common_headers = common_headers  # type: dict[str, str]
+        self.authorization = authorization  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UpdateUserPasswordHeaders, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('Authorization') is not None:
+            self.authorization = m.get('Authorization')
+        return self
+
+
+class UpdateUserPasswordRequest(TeaModel):
+    def __init__(self, password=None):
+        self.password = password  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(UpdateUserPasswordRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.password is not None:
+            result['password'] = self.password
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('password') is not None:
+            self.password = m.get('password')
+        return self
+
+
+class UpdateUserPasswordResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+
+    def to_map(self):
+        _map = super(UpdateUserPasswordResponse, self).to_map()
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
+    def from_map(self, m=None):
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

### Comparing `alibabacloud_eiam-developerapi20220225_py2-1.0.5/alibabacloud_eiam_developerapi20220225_py2.egg-info/PKG-INFO` & `alibabacloud_eiam-developerapi20220225_py2-1.0.6/alibabacloud_eiam_developerapi20220225_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-eiam-developerapi20220225-py2
-Version: 1.0.5
+Version: 1.0.6
 Summary: Alibaba Cloud Eiam-developerapi (20220225) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eiam-developerapi20220225_py2-1.0.5/alibabacloud_eiam_developerapi20220225_py2.egg-info/SOURCES.txt` & `alibabacloud_eiam-developerapi20220225_py2-1.0.6/alibabacloud_eiam_developerapi20220225_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_eiam-developerapi20220225_py2-1.0.5/setup.py` & `alibabacloud_eiam-developerapi20220225_py2-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_eiam-developerapi20220225_py2.
 
-Created on 28/11/2022
+Created on 16/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_eiam_developerapi20220225"
 NAME = "alibabacloud_eiam-developerapi20220225_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Eiam-developerapi (20220225) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.1.0, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

