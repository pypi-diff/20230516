# Comparing `tmp/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4.tar.gz` & `tmp/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4.tar", last modified: Tue May 16 06:52:43 2023, max compression
+gzip compressed data, was "dist/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5.tar", last modified: Tue May 16 07:38:11 2023, max compression
```

## Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4.tar` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:52:43.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 06:52:43.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:52:43.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:52:43.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22004 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/client.py
--rw-r--r--   0 root         (0) root         (0)    15216 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 06:52:43.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:38:11.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-16 07:38:10.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 07:38:10.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 07:38:11.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-05-16 07:38:10.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-05-16 07:38:10.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:38:11.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 07:38:10.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-16 07:38:10.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 07:38:10.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-16 07:38:10.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-16 07:38:10.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:38:11.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 07:38:10.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18046 2023-05-16 07:38:10.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/client.py
+-rw-r--r--   0 root         (0) root         (0)    11175 2023-05-16 07:38:10.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 07:38:11.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-05-16 07:38:10.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/setup.py
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/LICENSE` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/PKG-INFO` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4
-Version: 1.0.4
+Version: 1.0.5
 Summary: Ant Chain Ak_c3cc551641bc4a1e948f7b80bb2180f4 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/README-CN.md` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/README.md` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-c3cc551641bc4a1e948f7b80bb2180f4
-Version: 1.0.4
+Version: 1.0.5
 Summary: Ant Chain Ak_c3cc551641bc4a1e948f7b80bb2180f4 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/client.py` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.4',
+                    'sdk_version': '1.0.5',
                     '_prod_code': 'ak_c3cc551641bc4a1e948f7b80bb2180f4',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -233,15 +233,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.4',
+                    'sdk_version': '1.0.5',
                     '_prod_code': 'ak_c3cc551641bc4a1e948f7b80bb2180f4',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -269,230 +269,118 @@
             except Exception as e:
                 if TeaCore.is_retryable(e):
                     _last_exception = e
                     continue
                 raise e
         raise UnretryableException(_last_request, _last_exception)
 
-    def query_demo_testyy_q(
+    def status_demo_gateway_check(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestyyQRequest,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestyyQResponse:
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.StatusDemoGatewayCheckRequest,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.StatusDemoGatewayCheckResponse:
         """
-        Description: 2
-        Summary: 2
+        Description: Demo接口，返回当前服务器当前状态1
+        Summary: 检查服务状态
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.query_demo_testyy_qex(request, headers, runtime)
+        return self.status_demo_gateway_check_ex(request, headers, runtime)
 
-    async def query_demo_testyy_q_async(
+    async def status_demo_gateway_check_async(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestyyQRequest,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestyyQResponse:
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.StatusDemoGatewayCheckRequest,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.StatusDemoGatewayCheckResponse:
         """
-        Description: 2
-        Summary: 2
+        Description: Demo接口，返回当前服务器当前状态1
+        Summary: 检查服务状态
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.query_demo_testyy_qex_async(request, headers, runtime)
+        return await self.status_demo_gateway_check_ex_async(request, headers, runtime)
 
-    def query_demo_testyy_qex(
+    def status_demo_gateway_check_ex(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestyyQRequest,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.StatusDemoGatewayCheckRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestyyQResponse:
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.StatusDemoGatewayCheckResponse:
         """
-        Description: 2
-        Summary: 2
+        Description: Demo接口，返回当前服务器当前状态1
+        Summary: 检查服务状态
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestyyQResponse(),
-            self.do_request('1.0', 'demo.testyy.q.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.StatusDemoGatewayCheckResponse(),
+            self.do_request('1.0', 'demo.gateway.check.status', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    async def query_demo_testyy_qex_async(
+    async def status_demo_gateway_check_ex_async(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestyyQRequest,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.StatusDemoGatewayCheckRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestyyQResponse:
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.StatusDemoGatewayCheckResponse:
         """
-        Description: 2
-        Summary: 2
+        Description: Demo接口，返回当前服务器当前状态1
+        Summary: 检查服务状态
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestyyQResponse(),
-            await self.do_request_async('1.0', 'demo.testyy.q.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.StatusDemoGatewayCheckResponse(),
+            await self.do_request_async('1.0', 'demo.gateway.check.status', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    def query_demo_testzz_q(
+    def query_demo_gateway_embed(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestzzQRequest,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestzzQResponse:
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayEmbedRequest,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayEmbedResponse:
         """
-        Description: 1
-        Summary: 1
+        Description: 近端网关测试接口
+        Summary: 近端网关测试接口（勿删）
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.query_demo_testzz_qex(request, headers, runtime)
+        return self.query_demo_gateway_embed_ex(request, headers, runtime)
 
-    async def query_demo_testzz_q_async(
+    async def query_demo_gateway_embed_async(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestzzQRequest,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestzzQResponse:
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayEmbedRequest,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayEmbedResponse:
         """
-        Description: 1
-        Summary: 1
+        Description: 近端网关测试接口
+        Summary: 近端网关测试接口（勿删）
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.query_demo_testzz_qex_async(request, headers, runtime)
+        return await self.query_demo_gateway_embed_ex_async(request, headers, runtime)
 
-    def query_demo_testzz_qex(
+    def query_demo_gateway_embed_ex(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestzzQRequest,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayEmbedRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestzzQResponse:
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayEmbedResponse:
         """
-        Description: 1
-        Summary: 1
+        Description: 近端网关测试接口
+        Summary: 近端网关测试接口（勿删）
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestzzQResponse(),
-            self.do_request('1.0', 'demo.testzz.q.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayEmbedResponse(),
+            self.do_request('1.0', 'demo.gateway.embed.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    async def query_demo_testzz_qex_async(
+    async def query_demo_gateway_embed_ex_async(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestzzQRequest,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayEmbedRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestzzQResponse:
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayEmbedResponse:
         """
-        Description: 1
-        Summary: 1
+        Description: 近端网关测试接口
+        Summary: 近端网关测试接口（勿删）
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestzzQResponse(),
-            await self.do_request_async('1.0', 'demo.testzz.q.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    def query_demo_testzzz_q(
-        self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestzzzQRequest,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestzzzQResponse:
-        """
-        Description: 1
-        Summary: 1
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.query_demo_testzzz_qex(request, headers, runtime)
-
-    async def query_demo_testzzz_q_async(
-        self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestzzzQRequest,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestzzzQResponse:
-        """
-        Description: 1
-        Summary: 1
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.query_demo_testzzz_qex_async(request, headers, runtime)
-
-    def query_demo_testzzz_qex(
-        self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestzzzQRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestzzzQResponse:
-        """
-        Description: 1
-        Summary: 1
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestzzzQResponse(),
-            self.do_request('1.0', 'demo.testzzz.q.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def query_demo_testzzz_qex_async(
-        self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestzzzQRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestzzzQResponse:
-        """
-        Description: 1
-        Summary: 1
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoTestzzzQResponse(),
-            await self.do_request_async('1.0', 'demo.testzzz.q.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    def query_demo_xyz_demo_xxx(
-        self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoXyzDemoXxxRequest,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoXyzDemoXxxResponse:
-        """
-        Description: test
-        Summary: test
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.query_demo_xyz_demo_xxx_ex(request, headers, runtime)
-
-    async def query_demo_xyz_demo_xxx_async(
-        self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoXyzDemoXxxRequest,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoXyzDemoXxxResponse:
-        """
-        Description: test
-        Summary: test
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.query_demo_xyz_demo_xxx_ex_async(request, headers, runtime)
-
-    def query_demo_xyz_demo_xxx_ex(
-        self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoXyzDemoXxxRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoXyzDemoXxxResponse:
-        """
-        Description: test
-        Summary: test
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoXyzDemoXxxResponse(),
-            self.do_request('1.0', 'demo.xyz.demo.xxx.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def query_demo_xyz_demo_xxx_ex_async(
-        self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoXyzDemoXxxRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoXyzDemoXxxResponse:
-        """
-        Description: test
-        Summary: test
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoXyzDemoXxxResponse(),
-            await self.do_request_async('1.0', 'demo.xyz.demo.xxx.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayEmbedResponse(),
+            await self.do_request_async('1.0', 'demo.gateway.embed.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/models.py` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         if m.get('maxRequests') is not None:
             self.max_requests = m.get('maxRequests')
         if m.get('maxRequestsPerHost') is not None:
             self.max_requests_per_host = m.get('maxRequestsPerHost')
         return self
 
 
-class QueryDemoTestyyQRequest(TeaModel):
+class StatusDemoGatewayCheckRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
@@ -183,27 +183,30 @@
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
         return self
 
 
-class QueryDemoTestyyQResponse(TeaModel):
+class StatusDemoGatewayCheckResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
+        status: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
+        # OK
+        self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -212,214 +215,73 @@
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
+        if self.status is not None:
+            result['status'] = self.status
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
+        if m.get('status') is not None:
+            self.status = m.get('status')
         return self
 
 
-class QueryDemoTestzzQRequest(TeaModel):
+class QueryDemoGatewayEmbedRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
+        timeout: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
+        # 实例参数
+        self.timeout = timeout
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
+        if self.timeout is not None:
+            result['timeout'] = self.timeout
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
+        if m.get('timeout') is not None:
+            self.timeout = m.get('timeout')
         return self
 
 
-class QueryDemoTestzzQResponse(TeaModel):
-    def __init__(
-        self,
-        req_msg_id: str = None,
-        result_code: str = None,
-        result_msg: str = None,
-    ):
-        # 请求唯一ID，用于链路跟踪和问题排查
-        self.req_msg_id = req_msg_id
-        # 结果码，一般OK表示调用成功
-        self.result_code = result_code
-        # 异常信息的文本描述
-        self.result_msg = result_msg
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.req_msg_id is not None:
-            result['req_msg_id'] = self.req_msg_id
-        if self.result_code is not None:
-            result['result_code'] = self.result_code
-        if self.result_msg is not None:
-            result['result_msg'] = self.result_msg
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('req_msg_id') is not None:
-            self.req_msg_id = m.get('req_msg_id')
-        if m.get('result_code') is not None:
-            self.result_code = m.get('result_code')
-        if m.get('result_msg') is not None:
-            self.result_msg = m.get('result_msg')
-        return self
-
-
-class QueryDemoTestzzzQRequest(TeaModel):
-    def __init__(
-        self,
-        auth_token: str = None,
-        product_instance_id: str = None,
-    ):
-        # OAuth模式下的授权token
-        self.auth_token = auth_token
-        self.product_instance_id = product_instance_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.auth_token is not None:
-            result['auth_token'] = self.auth_token
-        if self.product_instance_id is not None:
-            result['product_instance_id'] = self.product_instance_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('auth_token') is not None:
-            self.auth_token = m.get('auth_token')
-        if m.get('product_instance_id') is not None:
-            self.product_instance_id = m.get('product_instance_id')
-        return self
-
-
-class QueryDemoTestzzzQResponse(TeaModel):
-    def __init__(
-        self,
-        req_msg_id: str = None,
-        result_code: str = None,
-        result_msg: str = None,
-    ):
-        # 请求唯一ID，用于链路跟踪和问题排查
-        self.req_msg_id = req_msg_id
-        # 结果码，一般OK表示调用成功
-        self.result_code = result_code
-        # 异常信息的文本描述
-        self.result_msg = result_msg
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.req_msg_id is not None:
-            result['req_msg_id'] = self.req_msg_id
-        if self.result_code is not None:
-            result['result_code'] = self.result_code
-        if self.result_msg is not None:
-            result['result_msg'] = self.result_msg
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('req_msg_id') is not None:
-            self.req_msg_id = m.get('req_msg_id')
-        if m.get('result_code') is not None:
-            self.result_code = m.get('result_code')
-        if m.get('result_msg') is not None:
-            self.result_msg = m.get('result_msg')
-        return self
-
-
-class QueryDemoXyzDemoXxxRequest(TeaModel):
-    def __init__(
-        self,
-        auth_token: str = None,
-        product_instance_id: str = None,
-    ):
-        # OAuth模式下的授权token
-        self.auth_token = auth_token
-        self.product_instance_id = product_instance_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.auth_token is not None:
-            result['auth_token'] = self.auth_token
-        if self.product_instance_id is not None:
-            result['product_instance_id'] = self.product_instance_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('auth_token') is not None:
-            self.auth_token = m.get('auth_token')
-        if m.get('product_instance_id') is not None:
-            self.product_instance_id = m.get('product_instance_id')
-        return self
-
-
-class QueryDemoXyzDemoXxxResponse(TeaModel):
+class QueryDemoGatewayEmbedResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/setup.py` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.5/setup.py`

 * *Files identical despite different names*

