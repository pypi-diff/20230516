# Comparing `tmp/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2.tar.gz` & `tmp/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2.tar", last modified: Tue May 16 06:08:40 2023, max compression
+gzip compressed data, was "dist/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3.tar", last modified: Tue May 16 06:20:13 2023, max compression
```

## Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2.tar` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:08:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-16 06:08:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 06:08:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 06:08:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-05-16 06:08:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-05-16 06:08:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:08:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 06:08:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-05-16 06:08:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 06:08:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-16 06:08:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-16 06:08:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:08:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 06:08:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33668 2023-05-16 06:08:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/client.py
--rw-r--r--   0 root         (0) root         (0)    38221 2023-05-16 06:08:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 06:08:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-05-16 06:08:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:20:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 06:20:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:20:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:20:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35756 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/client.py
+-rw-r--r--   0 root         (0) root         (0)    41149 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 06:20:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/setup.py
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/LICENSE` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/PKG-INFO` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4
-Version: 1.0.2
+Version: 1.0.3
 Summary: Ant Chain Ak_c3cc551641bc4a1e948f7b80bb2180f4 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/README-CN.md` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/README.md` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-c3cc551641bc4a1e948f7b80bb2180f4
-Version: 1.0.2
+Version: 1.0.3
 Summary: Ant Chain Ak_c3cc551641bc4a1e948f7b80bb2180f4 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/client.py` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -106,15 +106,15 @@
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
                 'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
                 'period': UtilClient.default_number(runtime.backoff_period, 1)
             },
             'ignoreSSL': runtime.ignore_ssl,
-            # api信息结构体
+            # 子结构体
         }
         _last_request = None
         _last_exception = None
         _now = time.time()
         _retry_times = 0
         while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
             if _retry_times > 0:
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.2',
+                    'sdk_version': '1.0.3',
                     '_prod_code': 'ak_c3cc551641bc4a1e948f7b80bb2180f4',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -210,15 +210,15 @@
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
                 'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
                 'period': UtilClient.default_number(runtime.backoff_period, 1)
             },
             'ignoreSSL': runtime.ignore_ssl,
-            # api信息结构体
+            # 子结构体
         }
         _last_request = None
         _last_exception = None
         _now = time.time()
         _retry_times = 0
         while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
             if _retry_times > 0:
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.2',
+                    'sdk_version': '1.0.3',
                     '_prod_code': 'ak_c3cc551641bc4a1e948f7b80bb2180f4',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -327,14 +327,104 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.StatusDemoGatewayCheckResponse(),
             await self.do_request_async('1.0', 'demo.gateway.check.status', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def preview_antchain_abc_demo(
+        self,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.PreviewAntchainAbcDemoRequest,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.PreviewAntchainAbcDemoResponse:
+        """
+        Description: 录入演示111
+        Summary: 录入演示API
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.preview_antchain_abc_demo_ex(request, headers, runtime)
+
+    async def preview_antchain_abc_demo_async(
+        self,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.PreviewAntchainAbcDemoRequest,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.PreviewAntchainAbcDemoResponse:
+        """
+        Description: 录入演示111
+        Summary: 录入演示API
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.preview_antchain_abc_demo_ex_async(request, headers, runtime)
+
+    def preview_antchain_abc_demo_ex(
+        self,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.PreviewAntchainAbcDemoRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.PreviewAntchainAbcDemoResponse:
+        """
+        Description: 录入演示111
+        Summary: 录入演示API
+        """
+        if not UtilClient.is_unset(request.file_object):
+            upload_req = ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.CreateAntcloudGatewayxFileUploadRequest(
+                auth_token=request.auth_token,
+                api_code='antchain.abc.demo.preview',
+                file_name=request.file_object_name
+            )
+            upload_resp = self.create_antcloud_gatewayx_file_upload_ex(upload_req, headers, runtime)
+            if not AntchainUtils.is_success(upload_resp.result_code, 'ok'):
+                preview_antchain_abc_demo_response = ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.PreviewAntchainAbcDemoResponse(
+                    req_msg_id=upload_resp.req_msg_id,
+                    result_code=upload_resp.result_code,
+                    result_msg=upload_resp.result_msg
+                )
+                return preview_antchain_abc_demo_response
+            upload_headers = AntchainUtils.parse_upload_headers(upload_resp.upload_headers)
+            AntchainUtils.put_object(request.file_object, upload_headers, upload_resp.upload_url)
+            request.file_id = upload_resp.file_id
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.PreviewAntchainAbcDemoResponse(),
+            self.do_request('1.0', 'antchain.abc.demo.preview', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def preview_antchain_abc_demo_ex_async(
+        self,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.PreviewAntchainAbcDemoRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.PreviewAntchainAbcDemoResponse:
+        """
+        Description: 录入演示111
+        Summary: 录入演示API
+        """
+        if not UtilClient.is_unset(request.file_object):
+            upload_req = ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.CreateAntcloudGatewayxFileUploadRequest(
+                auth_token=request.auth_token,
+                api_code='antchain.abc.demo.preview',
+                file_name=request.file_object_name
+            )
+            upload_resp = await self.create_antcloud_gatewayx_file_upload_ex_async(upload_req, headers, runtime)
+            if not AntchainUtils.is_success(upload_resp.result_code, 'ok'):
+                preview_antchain_abc_demo_response = ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.PreviewAntchainAbcDemoResponse(
+                    req_msg_id=upload_resp.req_msg_id,
+                    result_code=upload_resp.result_code,
+                    result_msg=upload_resp.result_msg
+                )
+                return preview_antchain_abc_demo_response
+            upload_headers = AntchainUtils.parse_upload_headers(upload_resp.upload_headers)
+            await AntchainUtils.put_object_async(request.file_object, upload_headers, upload_resp.upload_url)
+            request.file_id = upload_resp.file_id
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.PreviewAntchainAbcDemoResponse(),
+            await self.do_request_async('1.0', 'antchain.abc.demo.preview', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def query_demo_gateway_test(
         self,
         request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayTestRequest,
     ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayTestResponse:
         """
         Description: 测试用aaa
         Summary: 测试001
@@ -383,68 +473,68 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayTestResponse(),
             await self.do_request_async('1.0', 'demo.gateway.test.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    def bind_antchain_saas_ability(
+    def query_antchain_abc_abcda_abcddaa(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.BindAntchainSaasAbilityRequest,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.BindAntchainSaasAbilityResponse:
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainAbcAbcdaAbcddaaRequest,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainAbcAbcdaAbcddaaResponse:
         """
-        Description: 绑定API
-        Summary: 绑定能力与API关系
+        Description: 调试a s dddd
+        Summary: 调试1
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.bind_antchain_saas_ability_ex(request, headers, runtime)
+        return self.query_antchain_abc_abcda_abcddaa_ex(request, headers, runtime)
 
-    async def bind_antchain_saas_ability_async(
+    async def query_antchain_abc_abcda_abcddaa_async(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.BindAntchainSaasAbilityRequest,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.BindAntchainSaasAbilityResponse:
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainAbcAbcdaAbcddaaRequest,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainAbcAbcdaAbcddaaResponse:
         """
-        Description: 绑定API
-        Summary: 绑定能力与API关系
+        Description: 调试a s dddd
+        Summary: 调试1
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.bind_antchain_saas_ability_ex_async(request, headers, runtime)
+        return await self.query_antchain_abc_abcda_abcddaa_ex_async(request, headers, runtime)
 
-    def bind_antchain_saas_ability_ex(
+    def query_antchain_abc_abcda_abcddaa_ex(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.BindAntchainSaasAbilityRequest,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainAbcAbcdaAbcddaaRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.BindAntchainSaasAbilityResponse:
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainAbcAbcdaAbcddaaResponse:
         """
-        Description: 绑定API
-        Summary: 绑定能力与API关系
+        Description: 调试a s dddd
+        Summary: 调试1
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.BindAntchainSaasAbilityResponse(),
-            self.do_request('1.0', 'antchain.saas.ability.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainAbcAbcdaAbcddaaResponse(),
+            self.do_request('1.0', 'antchain.abc.abcda.abcddaa.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    async def bind_antchain_saas_ability_ex_async(
+    async def query_antchain_abc_abcda_abcddaa_ex_async(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.BindAntchainSaasAbilityRequest,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainAbcAbcdaAbcddaaRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.BindAntchainSaasAbilityResponse:
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainAbcAbcdaAbcddaaResponse:
         """
-        Description: 绑定API
-        Summary: 绑定能力与API关系
+        Description: 调试a s dddd
+        Summary: 调试1
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.BindAntchainSaasAbilityResponse(),
-            await self.do_request_async('1.0', 'antchain.saas.ability.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainAbcAbcdaAbcddaaResponse(),
+            await self.do_request_async('1.0', 'antchain.abc.abcda.abcddaa.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def upload_demo_gateway_file(
         self,
         request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.UploadDemoGatewayFileRequest,
     ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.UploadDemoGatewayFileResponse:
         """
@@ -529,124 +619,68 @@
             request.file_id = upload_resp.file_id
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.UploadDemoGatewayFileResponse(),
             await self.do_request_async('1.0', 'demo.gateway.file.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    def bind_antchain_saas_ability_api(
-        self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.BindAntchainSaasAbilityApiRequest,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.BindAntchainSaasAbilityApiResponse:
-        """
-        Description: 绑定能力的api信息
-        Summary: 绑定能力的api信息
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.bind_antchain_saas_ability_api_ex(request, headers, runtime)
-
-    async def bind_antchain_saas_ability_api_async(
-        self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.BindAntchainSaasAbilityApiRequest,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.BindAntchainSaasAbilityApiResponse:
-        """
-        Description: 绑定能力的api信息
-        Summary: 绑定能力的api信息
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.bind_antchain_saas_ability_api_ex_async(request, headers, runtime)
-
-    def bind_antchain_saas_ability_api_ex(
-        self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.BindAntchainSaasAbilityApiRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.BindAntchainSaasAbilityApiResponse:
-        """
-        Description: 绑定能力的api信息
-        Summary: 绑定能力的api信息
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.BindAntchainSaasAbilityApiResponse(),
-            self.do_request('1.0', 'antchain.saas.ability.api.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def bind_antchain_saas_ability_api_ex_async(
-        self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.BindAntchainSaasAbilityApiRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.BindAntchainSaasAbilityApiResponse:
-        """
-        Description: 绑定能力的api信息
-        Summary: 绑定能力的api信息
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.BindAntchainSaasAbilityApiResponse(),
-            await self.do_request_async('1.0', 'antchain.saas.ability.api.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    def query_antchain_saas_ability_businesscode(
+    def query_antchain_abc_approval_test(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainSaasAbilityBusinesscodeRequest,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainSaasAbilityBusinesscodeResponse:
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainAbcApprovalTestRequest,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainAbcApprovalTestResponse:
         """
-        Description: 根据商业产品编码查询能力信息
-        Summary: 根据商业产品编码查询能力信息
+        Description: 用于测试api评审接入SDL/修改后的评审/0323
+        Summary: api评审测试/修改后再次发起/0323
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.query_antchain_saas_ability_businesscode_ex(request, headers, runtime)
+        return self.query_antchain_abc_approval_test_ex(request, headers, runtime)
 
-    async def query_antchain_saas_ability_businesscode_async(
+    async def query_antchain_abc_approval_test_async(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainSaasAbilityBusinesscodeRequest,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainSaasAbilityBusinesscodeResponse:
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainAbcApprovalTestRequest,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainAbcApprovalTestResponse:
         """
-        Description: 根据商业产品编码查询能力信息
-        Summary: 根据商业产品编码查询能力信息
+        Description: 用于测试api评审接入SDL/修改后的评审/0323
+        Summary: api评审测试/修改后再次发起/0323
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.query_antchain_saas_ability_businesscode_ex_async(request, headers, runtime)
+        return await self.query_antchain_abc_approval_test_ex_async(request, headers, runtime)
 
-    def query_antchain_saas_ability_businesscode_ex(
+    def query_antchain_abc_approval_test_ex(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainSaasAbilityBusinesscodeRequest,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainAbcApprovalTestRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainSaasAbilityBusinesscodeResponse:
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainAbcApprovalTestResponse:
         """
-        Description: 根据商业产品编码查询能力信息
-        Summary: 根据商业产品编码查询能力信息
+        Description: 用于测试api评审接入SDL/修改后的评审/0323
+        Summary: api评审测试/修改后再次发起/0323
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainSaasAbilityBusinesscodeResponse(),
-            self.do_request('1.0', 'antchain.saas.ability.businesscode.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainAbcApprovalTestResponse(),
+            self.do_request('1.0', 'antchain.abc.approval.test.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    async def query_antchain_saas_ability_businesscode_ex_async(
+    async def query_antchain_abc_approval_test_ex_async(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainSaasAbilityBusinesscodeRequest,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainAbcApprovalTestRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainSaasAbilityBusinesscodeResponse:
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainAbcApprovalTestResponse:
         """
-        Description: 根据商业产品编码查询能力信息
-        Summary: 根据商业产品编码查询能力信息
+        Description: 用于测试api评审接入SDL/修改后的评审/0323
+        Summary: api评审测试/修改后再次发起/0323
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainSaasAbilityBusinesscodeResponse(),
-            await self.do_request_async('1.0', 'antchain.saas.ability.businesscode.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryAntchainAbcApprovalTestResponse(),
+            await self.do_request_async('1.0', 'antchain.abc.approval.test.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def create_antcloud_gatewayx_file_upload(
         self,
         request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.CreateAntcloudGatewayxFileUploadRequest,
     ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.CreateAntcloudGatewayxFileUploadResponse:
         """
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/models.py` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -150,179 +150,139 @@
         if m.get('maxRequests') is not None:
             self.max_requests = m.get('maxRequests')
         if m.get('maxRequestsPerHost') is not None:
             self.max_requests_per_host = m.get('maxRequestsPerHost')
         return self
 
 
-class ApiInfoModel(TeaModel):
+class SubDemoStruct(TeaModel):
     def __init__(
         self,
-        api_name: str = None,
-        prod_code: str = None,
-        internal: int = None,
-        api_version: str = None,
-        api_desc: str = None,
-        provider_id: str = None,
-    ):
-        # api名称
-        self.api_name = api_name
-        # 产品码
-        self.prod_code = prod_code
-        # 是否是内部接口 0对外 1对内
-        self.internal = internal
-        # api版本号
-        self.api_version = api_version
-        # api描述
-        self.api_desc = api_desc
-        # api所属网关产品id
-        self.provider_id = provider_id
-
-    def validate(self):
-        self.validate_required(self.api_name, 'api_name')
-        self.validate_required(self.prod_code, 'prod_code')
-        self.validate_required(self.internal, 'internal')
-        self.validate_required(self.api_version, 'api_version')
-        self.validate_required(self.api_desc, 'api_desc')
-        self.validate_required(self.provider_id, 'provider_id')
+        name: str = None,
+        value: str = None,
+    ):
+        # name
+        self.name = name
+        # value
+        self.value = value
+
+    def validate(self):
+        self.validate_required(self.name, 'name')
+        self.validate_required(self.value, 'value')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.api_name is not None:
-            result['api_name'] = self.api_name
-        if self.prod_code is not None:
-            result['prod_code'] = self.prod_code
-        if self.internal is not None:
-            result['internal'] = self.internal
-        if self.api_version is not None:
-            result['api_version'] = self.api_version
-        if self.api_desc is not None:
-            result['api_desc'] = self.api_desc
-        if self.provider_id is not None:
-            result['provider_id'] = self.provider_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('api_name') is not None:
-            self.api_name = m.get('api_name')
-        if m.get('prod_code') is not None:
-            self.prod_code = m.get('prod_code')
-        if m.get('internal') is not None:
-            self.internal = m.get('internal')
-        if m.get('api_version') is not None:
-            self.api_version = m.get('api_version')
-        if m.get('api_desc') is not None:
-            self.api_desc = m.get('api_desc')
-        if m.get('provider_id') is not None:
-            self.provider_id = m.get('provider_id')
-        return self
-
-
-class AbilityInfo(TeaModel):
-    def __init__(
-        self,
-        ability_id: str = None,
-        ability_name: str = None,
-        dev_owner: str = None,
-        gmt_create: str = None,
-        description: str = None,
-        dev_owner_prefix_email: str = None,
-        product_owner: str = None,
-        business_code: str = None,
-        api_info_models: List[ApiInfoModel] = None,
-    ):
-        # 能力编号
-        self.ability_id = ability_id
-        # 能力名称
-        self.ability_name = ability_name
-        # 研发负责人
-        self.dev_owner = dev_owner
-        # 创建时间
-        self.gmt_create = gmt_create
-        # 描述信息
-        self.description = description
-        # 研发负责人邮箱前缀
-        self.dev_owner_prefix_email = dev_owner_prefix_email
-        # 产品负责人
-        self.product_owner = product_owner
-        # 能力对应商业中台L5Code
-        self.business_code = business_code
-        # apiInfoModels列表
-        self.api_info_models = api_info_models
-
-    def validate(self):
-        self.validate_required(self.ability_id, 'ability_id')
-        self.validate_required(self.ability_name, 'ability_name')
-        self.validate_required(self.dev_owner, 'dev_owner')
-        self.validate_required(self.gmt_create, 'gmt_create')
-        self.validate_required(self.description, 'description')
-        self.validate_required(self.dev_owner_prefix_email, 'dev_owner_prefix_email')
-        self.validate_required(self.product_owner, 'product_owner')
-        self.validate_required(self.api_info_models, 'api_info_models')
-        if self.api_info_models:
-            for k in self.api_info_models:
+        if self.name is not None:
+            result['name'] = self.name
+        if self.value is not None:
+            result['value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('value') is not None:
+            self.value = m.get('value')
+        return self
+
+
+class AbcDemoStruct(TeaModel):
+    def __init__(
+        self,
+        some_string: str = None,
+        some_number: int = None,
+        some_boolean: bool = None,
+        some_date: str = None,
+        some_string_list: List[str] = None,
+        some_struct: SubDemoStruct = None,
+        some_struct_list: List[SubDemoStruct] = None,
+    ):
+        # 字符串属性
+        self.some_string = some_string
+        # Long型属性
+        self.some_number = some_number
+        # 布尔型
+        self.some_boolean = some_boolean
+        # ISO8601格式字符串：yyyy-MM-dd_T_HH:mm:ss_Z_
+        self.some_date = some_date
+        # 字符串数组
+        self.some_string_list = some_string_list
+        # 子结构体
+        self.some_struct = some_struct
+        # 结构体数组
+        self.some_struct_list = some_struct_list
+
+    def validate(self):
+        if self.some_string is not None:
+            self.validate_max_length(self.some_string, 'some_string', 100)
+        self.validate_required(self.some_number, 'some_number')
+        if self.some_number is not None:
+            self.validate_maximum(self.some_number, 'some_number', 100)
+            self.validate_minimum(self.some_number, 'some_number', 1)
+        self.validate_required(self.some_boolean, 'some_boolean')
+        if self.some_date is not None:
+            self.validate_pattern(self.some_date, 'some_date', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
+        self.validate_required(self.some_struct, 'some_struct')
+        if self.some_struct:
+            self.some_struct.validate()
+        self.validate_required(self.some_struct_list, 'some_struct_list')
+        if self.some_struct_list:
+            for k in self.some_struct_list:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.ability_id is not None:
-            result['ability_id'] = self.ability_id
-        if self.ability_name is not None:
-            result['ability_name'] = self.ability_name
-        if self.dev_owner is not None:
-            result['dev_owner'] = self.dev_owner
-        if self.gmt_create is not None:
-            result['gmt_create'] = self.gmt_create
-        if self.description is not None:
-            result['description'] = self.description
-        if self.dev_owner_prefix_email is not None:
-            result['dev_owner_prefix_email'] = self.dev_owner_prefix_email
-        if self.product_owner is not None:
-            result['product_owner'] = self.product_owner
-        if self.business_code is not None:
-            result['business_code'] = self.business_code
-        result['api_info_models'] = []
-        if self.api_info_models is not None:
-            for k in self.api_info_models:
-                result['api_info_models'].append(k.to_map() if k else None)
+        if self.some_string is not None:
+            result['some_string'] = self.some_string
+        if self.some_number is not None:
+            result['some_number'] = self.some_number
+        if self.some_boolean is not None:
+            result['some_boolean'] = self.some_boolean
+        if self.some_date is not None:
+            result['some_date'] = self.some_date
+        if self.some_string_list is not None:
+            result['some_string_list'] = self.some_string_list
+        if self.some_struct is not None:
+            result['some_struct'] = self.some_struct.to_map()
+        result['some_struct_list'] = []
+        if self.some_struct_list is not None:
+            for k in self.some_struct_list:
+                result['some_struct_list'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ability_id') is not None:
-            self.ability_id = m.get('ability_id')
-        if m.get('ability_name') is not None:
-            self.ability_name = m.get('ability_name')
-        if m.get('dev_owner') is not None:
-            self.dev_owner = m.get('dev_owner')
-        if m.get('gmt_create') is not None:
-            self.gmt_create = m.get('gmt_create')
-        if m.get('description') is not None:
-            self.description = m.get('description')
-        if m.get('dev_owner_prefix_email') is not None:
-            self.dev_owner_prefix_email = m.get('dev_owner_prefix_email')
-        if m.get('product_owner') is not None:
-            self.product_owner = m.get('product_owner')
-        if m.get('business_code') is not None:
-            self.business_code = m.get('business_code')
-        self.api_info_models = []
-        if m.get('api_info_models') is not None:
-            for k in m.get('api_info_models'):
-                temp_model = ApiInfoModel()
-                self.api_info_models.append(temp_model.from_map(k))
+        if m.get('some_string') is not None:
+            self.some_string = m.get('some_string')
+        if m.get('some_number') is not None:
+            self.some_number = m.get('some_number')
+        if m.get('some_boolean') is not None:
+            self.some_boolean = m.get('some_boolean')
+        if m.get('some_date') is not None:
+            self.some_date = m.get('some_date')
+        if m.get('some_string_list') is not None:
+            self.some_string_list = m.get('some_string_list')
+        if m.get('some_struct') is not None:
+            temp_model = SubDemoStruct()
+            self.some_struct = temp_model.from_map(m['some_struct'])
+        self.some_struct_list = []
+        if m.get('some_struct_list') is not None:
+            for k in m.get('some_struct_list'):
+                temp_model = SubDemoStruct()
+                self.some_struct_list.append(temp_model.from_map(k))
         return self
 
 
 class XNameValuePair(TeaModel):
     def __init__(
         self,
         name: str = None,
@@ -437,159 +397,280 @@
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('status') is not None:
             self.status = m.get('status')
         return self
 
 
-class QueryDemoGatewayTestRequest(TeaModel):
+class PreviewAntchainAbcDemoRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
+        input_string: str = None,
+        input_number: int = None,
+        input_boolean: bool = None,
+        input_date: str = None,
+        input_string_list: List[str] = None,
+        input_struct: AbcDemoStruct = None,
+        input_struct_list: List[AbcDemoStruct] = None,
+        file_object: BinaryIO = None,
+        file_object_name: str = None,
+        file_id: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
+        # 字符串入参
+        self.input_string = input_string
+        # Long型入参
+        self.input_number = input_number
+        # 布尔型入参
+        self.input_boolean = input_boolean
+        # ISO8601格式字符串：yyyy-MM-dd_T_HH:mm:ss_Z_
+        self.input_date = input_date
+        # 字符串列表入参
+        self.input_string_list = input_string_list
+        # 示例结构体入参
+        self.input_struct = input_struct
+        # 结构体数组入参
+        self.input_struct_list = input_struct_list
+        # 123
+        # 待上传文件
+        self.file_object = file_object
+        # 待上传文件名
+        self.file_object_name = file_object_name
+        self.file_id = file_id
 
     def validate(self):
-        pass
+        self.validate_required(self.input_string, 'input_string')
+        if self.input_string is not None:
+            self.validate_max_length(self.input_string, 'input_string', 1000)
+        if self.input_number is not None:
+            self.validate_maximum(self.input_number, 'input_number', 10000)
+            self.validate_minimum(self.input_number, 'input_number', 10)
+        self.validate_required(self.input_boolean, 'input_boolean')
+        if self.input_date is not None:
+            self.validate_pattern(self.input_date, 'input_date', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
+        self.validate_required(self.input_struct, 'input_struct')
+        if self.input_struct:
+            self.input_struct.validate()
+        self.validate_required(self.input_struct_list, 'input_struct_list')
+        if self.input_struct_list:
+            for k in self.input_struct_list:
+                if k:
+                    k.validate()
+        self.validate_required(self.file_id, 'file_id')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
+        if self.input_string is not None:
+            result['input_string'] = self.input_string
+        if self.input_number is not None:
+            result['input_number'] = self.input_number
+        if self.input_boolean is not None:
+            result['input_boolean'] = self.input_boolean
+        if self.input_date is not None:
+            result['input_date'] = self.input_date
+        if self.input_string_list is not None:
+            result['input_string_list'] = self.input_string_list
+        if self.input_struct is not None:
+            result['input_struct'] = self.input_struct.to_map()
+        result['input_struct_list'] = []
+        if self.input_struct_list is not None:
+            for k in self.input_struct_list:
+                result['input_struct_list'].append(k.to_map() if k else None)
+        if self.file_object is not None:
+            result['fileObject'] = self.file_object
+        if self.file_object_name is not None:
+            result['fileObjectName'] = self.file_object_name
+        if self.file_id is not None:
+            result['file_id'] = self.file_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
+        if m.get('input_string') is not None:
+            self.input_string = m.get('input_string')
+        if m.get('input_number') is not None:
+            self.input_number = m.get('input_number')
+        if m.get('input_boolean') is not None:
+            self.input_boolean = m.get('input_boolean')
+        if m.get('input_date') is not None:
+            self.input_date = m.get('input_date')
+        if m.get('input_string_list') is not None:
+            self.input_string_list = m.get('input_string_list')
+        if m.get('input_struct') is not None:
+            temp_model = AbcDemoStruct()
+            self.input_struct = temp_model.from_map(m['input_struct'])
+        self.input_struct_list = []
+        if m.get('input_struct_list') is not None:
+            for k in m.get('input_struct_list'):
+                temp_model = AbcDemoStruct()
+                self.input_struct_list.append(temp_model.from_map(k))
+        if m.get('fileObject') is not None:
+            self.file_object = m.get('fileObject')
+        if m.get('fileObjectName') is not None:
+            self.file_object_name = m.get('fileObjectName')
+        if m.get('file_id') is not None:
+            self.file_id = m.get('file_id')
         return self
 
 
-class QueryDemoGatewayTestResponse(TeaModel):
+class PreviewAntchainAbcDemoResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
+        output_string: str = None,
+        output_number: int = None,
+        output_boolean: bool = None,
+        output_date: str = None,
+        output_string_list: List[str] = None,
+        output_struct: AbcDemoStruct = None,
+        output_struct_list: List[AbcDemoStruct] = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
-
-    def validate(self):
-        pass
+        # 字符串回参
+        self.output_string = output_string
+        # Long型回参
+        self.output_number = output_number
+        # 布尔型回参
+        self.output_boolean = output_boolean
+        # ISO8602格式字符串：yyyy-MM-dd_T_HH:mm:ss_Z_
+        self.output_date = output_date
+        # 字符串数组
+        self.output_string_list = output_string_list
+        # 结构体回参
+        self.output_struct = output_struct
+        # 结构体列表回参
+        self.output_struct_list = output_struct_list
+
+    def validate(self):
+        if self.output_date is not None:
+            self.validate_pattern(self.output_date, 'output_date', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
+        if self.output_struct:
+            self.output_struct.validate()
+        if self.output_struct_list:
+            for k in self.output_struct_list:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
+        if self.output_string is not None:
+            result['output_string'] = self.output_string
+        if self.output_number is not None:
+            result['output_number'] = self.output_number
+        if self.output_boolean is not None:
+            result['output_boolean'] = self.output_boolean
+        if self.output_date is not None:
+            result['output_date'] = self.output_date
+        if self.output_string_list is not None:
+            result['output_string_list'] = self.output_string_list
+        if self.output_struct is not None:
+            result['output_struct'] = self.output_struct.to_map()
+        result['output_struct_list'] = []
+        if self.output_struct_list is not None:
+            for k in self.output_struct_list:
+                result['output_struct_list'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
+        if m.get('output_string') is not None:
+            self.output_string = m.get('output_string')
+        if m.get('output_number') is not None:
+            self.output_number = m.get('output_number')
+        if m.get('output_boolean') is not None:
+            self.output_boolean = m.get('output_boolean')
+        if m.get('output_date') is not None:
+            self.output_date = m.get('output_date')
+        if m.get('output_string_list') is not None:
+            self.output_string_list = m.get('output_string_list')
+        if m.get('output_struct') is not None:
+            temp_model = AbcDemoStruct()
+            self.output_struct = temp_model.from_map(m['output_struct'])
+        self.output_struct_list = []
+        if m.get('output_struct_list') is not None:
+            for k in m.get('output_struct_list'):
+                temp_model = AbcDemoStruct()
+                self.output_struct_list.append(temp_model.from_map(k))
         return self
 
 
-class BindAntchainSaasAbilityRequest(TeaModel):
+class QueryDemoGatewayTestRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        api_name: str = None,
-        ability_ids: List[str] = None,
-        operator_id: str = None,
-        api_info_model: ApiInfoModel = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # api名称
-        self.api_name = api_name
-        # 能力id列表
-        self.ability_ids = ability_ids
-        # 操作人的域账号
-        self.operator_id = operator_id
-        # api信息
-        self.api_info_model = api_info_model
-
-    def validate(self):
-        self.validate_required(self.api_name, 'api_name')
-        self.validate_required(self.ability_ids, 'ability_ids')
-        self.validate_required(self.operator_id, 'operator_id')
-        self.validate_required(self.api_info_model, 'api_info_model')
-        if self.api_info_model:
-            self.api_info_model.validate()
+
+    def validate(self):
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.api_name is not None:
-            result['api_name'] = self.api_name
-        if self.ability_ids is not None:
-            result['ability_ids'] = self.ability_ids
-        if self.operator_id is not None:
-            result['operator_id'] = self.operator_id
-        if self.api_info_model is not None:
-            result['api_info_model'] = self.api_info_model.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('api_name') is not None:
-            self.api_name = m.get('api_name')
-        if m.get('ability_ids') is not None:
-            self.ability_ids = m.get('ability_ids')
-        if m.get('operator_id') is not None:
-            self.operator_id = m.get('operator_id')
-        if m.get('api_info_model') is not None:
-            temp_model = ApiInfoModel()
-            self.api_info_model = temp_model.from_map(m['api_info_model'])
         return self
 
 
-class BindAntchainSaasAbilityResponse(TeaModel):
+class QueryDemoGatewayTestResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
@@ -623,78 +704,49 @@
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         return self
 
 
-class UploadDemoGatewayFileRequest(TeaModel):
+class QueryAntchainAbcAbcdaAbcddaaRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        file_object: BinaryIO = None,
-        file_object_name: str = None,
-        file_id: str = None,
-        data: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 123
-        # 待上传文件
-        self.file_object = file_object
-        # 待上传文件名
-        self.file_object_name = file_object_name
-        self.file_id = file_id
-        # 123
-        self.data = data
 
     def validate(self):
-        self.validate_required(self.file_id, 'file_id')
-        self.validate_required(self.data, 'data')
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.file_object is not None:
-            result['fileObject'] = self.file_object
-        if self.file_object_name is not None:
-            result['fileObjectName'] = self.file_object_name
-        if self.file_id is not None:
-            result['file_id'] = self.file_id
-        if self.data is not None:
-            result['data'] = self.data
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('fileObject') is not None:
-            self.file_object = m.get('fileObject')
-        if m.get('fileObjectName') is not None:
-            self.file_object_name = m.get('fileObjectName')
-        if m.get('file_id') is not None:
-            self.file_id = m.get('file_id')
-        if m.get('data') is not None:
-            self.data = m.get('data')
         return self
 
 
-class UploadDemoGatewayFileResponse(TeaModel):
+class QueryAntchainAbcAbcdaAbcddaaResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
@@ -728,81 +780,78 @@
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         return self
 
 
-class BindAntchainSaasAbilityApiRequest(TeaModel):
+class UploadDemoGatewayFileRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        ability_id: str = None,
-        operator_id: str = None,
-        api_info_models: List[ApiInfoModel] = None,
+        file_object: BinaryIO = None,
+        file_object_name: str = None,
+        file_id: str = None,
+        data: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 共享能力id
-        self.ability_id = ability_id
-        # qiujianglong.qjl
-        self.operator_id = operator_id
-        # api模型集合
-        self.api_info_models = api_info_models
+        # 123
+        # 待上传文件
+        self.file_object = file_object
+        # 待上传文件名
+        self.file_object_name = file_object_name
+        self.file_id = file_id
+        # 123
+        self.data = data
 
     def validate(self):
-        self.validate_required(self.ability_id, 'ability_id')
-        self.validate_required(self.operator_id, 'operator_id')
-        self.validate_required(self.api_info_models, 'api_info_models')
-        if self.api_info_models:
-            for k in self.api_info_models:
-                if k:
-                    k.validate()
+        self.validate_required(self.file_id, 'file_id')
+        self.validate_required(self.data, 'data')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.ability_id is not None:
-            result['ability_id'] = self.ability_id
-        if self.operator_id is not None:
-            result['operator_id'] = self.operator_id
-        result['api_info_models'] = []
-        if self.api_info_models is not None:
-            for k in self.api_info_models:
-                result['api_info_models'].append(k.to_map() if k else None)
+        if self.file_object is not None:
+            result['fileObject'] = self.file_object
+        if self.file_object_name is not None:
+            result['fileObjectName'] = self.file_object_name
+        if self.file_id is not None:
+            result['file_id'] = self.file_id
+        if self.data is not None:
+            result['data'] = self.data
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('ability_id') is not None:
-            self.ability_id = m.get('ability_id')
-        if m.get('operator_id') is not None:
-            self.operator_id = m.get('operator_id')
-        self.api_info_models = []
-        if m.get('api_info_models') is not None:
-            for k in m.get('api_info_models'):
-                temp_model = ApiInfoModel()
-                self.api_info_models.append(temp_model.from_map(k))
+        if m.get('fileObject') is not None:
+            self.file_object = m.get('fileObject')
+        if m.get('fileObjectName') is not None:
+            self.file_object_name = m.get('fileObjectName')
+        if m.get('file_id') is not None:
+            self.file_id = m.get('file_id')
+        if m.get('data') is not None:
+            self.data = m.get('data')
         return self
 
 
-class BindAntchainSaasAbilityApiResponse(TeaModel):
+class UploadDemoGatewayFileResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
@@ -836,103 +885,116 @@
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         return self
 
 
-class QueryAntchainSaasAbilityBusinesscodeRequest(TeaModel):
+class QueryAntchainAbcApprovalTestRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        business_code: str = None,
+        input: str = None,
+        delete: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 商业产品编码，L5编码
-        self.business_code = business_code
+        # 入参
+        self.input = input
+        # 新增字段
+        self.delete = delete
 
     def validate(self):
-        self.validate_required(self.business_code, 'business_code')
+        self.validate_required(self.input, 'input')
+        self.validate_required(self.delete, 'delete')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.business_code is not None:
-            result['business_code'] = self.business_code
+        if self.input is not None:
+            result['input'] = self.input
+        if self.delete is not None:
+            result['delete'] = self.delete
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('business_code') is not None:
-            self.business_code = m.get('business_code')
+        if m.get('input') is not None:
+            self.input = m.get('input')
+        if m.get('delete') is not None:
+            self.delete = m.get('delete')
         return self
 
 
-class QueryAntchainSaasAbilityBusinesscodeResponse(TeaModel):
+class QueryAntchainAbcApprovalTestResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
-        ability_info: AbilityInfo = None,
+        msg: str = None,
+        code: int = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
-        # 能力信息
-        self.ability_info = ability_info
+        # 回参
+        self.msg = msg
+        # 新增字段
+        self.code = code
 
     def validate(self):
-        if self.ability_info:
-            self.ability_info.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
-        if self.ability_info is not None:
-            result['ability_info'] = self.ability_info.to_map()
+        if self.msg is not None:
+            result['msg'] = self.msg
+        if self.code is not None:
+            result['code'] = self.code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
-        if m.get('ability_info') is not None:
-            temp_model = AbilityInfo()
-            self.ability_info = temp_model.from_map(m['ability_info'])
+        if m.get('msg') is not None:
+            self.msg = m.get('msg')
+        if m.get('code') is not None:
+            self.code = m.get('code')
         return self
 
 
 class CreateAntcloudGatewayxFileUploadRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.2/setup.py` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/setup.py`

 * *Files identical despite different names*

