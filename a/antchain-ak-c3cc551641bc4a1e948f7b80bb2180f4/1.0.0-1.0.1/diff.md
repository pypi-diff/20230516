# Comparing `tmp/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0.tar.gz` & `tmp/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0.tar", last modified: Tue May 16 05:43:41 2023, max compression
+gzip compressed data, was "dist/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1.tar", last modified: Tue May 16 06:00:01 2023, max compression
```

## Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0.tar` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 05:43:41.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-16 05:43:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 05:43:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 05:43:41.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-05-16 05:43:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-05-16 05:43:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 05:43:41.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 05:43:41.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-05-16 05:43:41.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 05:43:41.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-16 05:43:41.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-16 05:43:41.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 05:43:41.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 05:43:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28038 2023-05-16 05:43:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/client.py
--rw-r--r--   0 root         (0) root         (0)    23705 2023-05-16 05:43:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 05:43:41.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-05-16 05:43:40.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:00:01.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-16 06:00:00.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 06:00:00.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 06:00:01.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-05-16 06:00:00.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-05-16 06:00:00.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:00:01.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 06:00:01.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-16 06:00:01.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 06:00:01.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-16 06:00:01.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-16 06:00:01.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:00:01.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 06:00:00.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30248 2023-05-16 06:00:00.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/client.py
+-rw-r--r--   0 root         (0) root         (0)    25731 2023-05-16 06:00:00.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 06:00:01.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-05-16 06:00:00.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/setup.py
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/LICENSE` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/PKG-INFO` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4
-Version: 1.0.0
+Name: antchain-ak-c3cc551641bc4a1e948f7b80bb2180f4
+Version: 1.0.1
 Summary: Ant Chain Ak_c3cc551641bc4a1e948f7b80bb2180f4 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/README-CN.md` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/README.md` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain-ak-c3cc551641bc4a1e948f7b80bb2180f4
-Version: 1.0.0
+Name: antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4
+Version: 1.0.1
 Summary: Ant Chain Ak_c3cc551641bc4a1e948f7b80bb2180f4 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/client.py` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.0',
+                    'sdk_version': '1.0.1',
                     '_prod_code': 'ak_c3cc551641bc4a1e948f7b80bb2180f4',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.0',
+                    'sdk_version': '1.0.1',
                     '_prod_code': 'ak_c3cc551641bc4a1e948f7b80bb2180f4',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -327,124 +327,180 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.StatusDemoGatewayCheckResponse(),
             await self.do_request_async('1.0', 'demo.gateway.check.status', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    def query_demo_gateway_my(
+    def query_demo_gateway_check(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayMyRequest,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayMyResponse:
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayCheckRequest,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayCheckResponse:
         """
-        Description: aaa
-        Summary: 测试demo
+        Description: ceshi
+        Summary: ss
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.query_demo_gateway_my_ex(request, headers, runtime)
+        return self.query_demo_gateway_check_ex(request, headers, runtime)
 
-    async def query_demo_gateway_my_async(
+    async def query_demo_gateway_check_async(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayMyRequest,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayMyResponse:
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayCheckRequest,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayCheckResponse:
         """
-        Description: aaa
-        Summary: 测试demo
+        Description: ceshi
+        Summary: ss
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.query_demo_gateway_my_ex_async(request, headers, runtime)
+        return await self.query_demo_gateway_check_ex_async(request, headers, runtime)
 
-    def query_demo_gateway_my_ex(
+    def query_demo_gateway_check_ex(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayMyRequest,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayCheckRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayMyResponse:
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayCheckResponse:
         """
-        Description: aaa
-        Summary: 测试demo
+        Description: ceshi
+        Summary: ss
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayMyResponse(),
-            self.do_request('1.0', 'demo.gateway.my.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayCheckResponse(),
+            self.do_request('1.0', 'demo.gateway.check.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    async def query_demo_gateway_my_ex_async(
+    async def query_demo_gateway_check_ex_async(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayMyRequest,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayCheckRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayMyResponse:
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayCheckResponse:
         """
-        Description: aaa
-        Summary: 测试demo
+        Description: ceshi
+        Summary: ss
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayMyResponse(),
-            await self.do_request_async('1.0', 'demo.gateway.my.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayCheckResponse(),
+            await self.do_request_async('1.0', 'demo.gateway.check.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_demo_gateway_test(
+        self,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayTestRequest,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayTestResponse:
+        """
+        Description: 测试用aaa
+        Summary: 测试001
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_demo_gateway_test_ex(request, headers, runtime)
+
+    async def query_demo_gateway_test_async(
+        self,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayTestRequest,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayTestResponse:
+        """
+        Description: 测试用aaa
+        Summary: 测试001
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_demo_gateway_test_ex_async(request, headers, runtime)
+
+    def query_demo_gateway_test_ex(
+        self,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayTestRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayTestResponse:
+        """
+        Description: 测试用aaa
+        Summary: 测试001
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayTestResponse(),
+            self.do_request('1.0', 'demo.gateway.test.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    def query_demo_gateway_embed(
+    async def query_demo_gateway_test_ex_async(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayEmbedRequest,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayEmbedResponse:
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayTestRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayTestResponse:
         """
-        Description: 近端网关测试接口
-        Summary: 近端网关测试接口（勿删）
+        Description: 测试用aaa
+        Summary: 测试001
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayTestResponse(),
+            await self.do_request_async('1.0', 'demo.gateway.test.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_demo_gateway_my(
+        self,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayMyRequest,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayMyResponse:
+        """
+        Description: aaa
+        Summary: 测试demo
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.query_demo_gateway_embed_ex(request, headers, runtime)
+        return self.query_demo_gateway_my_ex(request, headers, runtime)
 
-    async def query_demo_gateway_embed_async(
+    async def query_demo_gateway_my_async(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayEmbedRequest,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayEmbedResponse:
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayMyRequest,
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayMyResponse:
         """
-        Description: 近端网关测试接口
-        Summary: 近端网关测试接口（勿删）
+        Description: aaa
+        Summary: 测试demo
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.query_demo_gateway_embed_ex_async(request, headers, runtime)
+        return await self.query_demo_gateway_my_ex_async(request, headers, runtime)
 
-    def query_demo_gateway_embed_ex(
+    def query_demo_gateway_my_ex(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayEmbedRequest,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayMyRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayEmbedResponse:
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayMyResponse:
         """
-        Description: 近端网关测试接口
-        Summary: 近端网关测试接口（勿删）
+        Description: aaa
+        Summary: 测试demo
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayEmbedResponse(),
-            self.do_request('1.0', 'demo.gateway.embed.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayMyResponse(),
+            self.do_request('1.0', 'demo.gateway.my.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    async def query_demo_gateway_embed_ex_async(
+    async def query_demo_gateway_my_ex_async(
         self,
-        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayEmbedRequest,
+        request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayMyRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayEmbedResponse:
+    ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayMyResponse:
         """
-        Description: 近端网关测试接口
-        Summary: 近端网关测试接口（勿删）
+        Description: aaa
+        Summary: 测试demo
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayEmbedResponse(),
-            await self.do_request_async('1.0', 'demo.gateway.embed.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.QueryDemoGatewayMyResponse(),
+            await self.do_request_async('1.0', 'demo.gateway.my.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def upload_demo_gateway_file(
         self,
         request: ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.UploadDemoGatewayFileRequest,
     ) -> ak_c_3cc_551641bc_4a_1e_948f_7b_80bb_2180f_4_models.UploadDemoGatewayFileResponse:
         """
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/models.py` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,15 +269,15 @@
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('status') is not None:
             self.status = m.get('status')
         return self
 
 
-class QueryDemoGatewayMyRequest(TeaModel):
+class QueryDemoGatewayCheckRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
@@ -303,15 +303,91 @@
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
         return self
 
 
-class QueryDemoGatewayMyResponse(TeaModel):
+class QueryDemoGatewayCheckResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class QueryDemoGatewayTestRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
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
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        return self
+
+
+class QueryDemoGatewayTestResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
@@ -345,56 +421,49 @@
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         return self
 
 
-class QueryDemoGatewayEmbedRequest(TeaModel):
+class QueryDemoGatewayMyRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        timeout: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 实例参数
-        self.timeout = timeout
 
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
-        if self.timeout is not None:
-            result['timeout'] = self.timeout
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('timeout') is not None:
-            self.timeout = m.get('timeout')
         return self
 
 
-class QueryDemoGatewayEmbedResponse(TeaModel):
+class QueryDemoGatewayMyResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.0/setup.py` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.1/setup.py`

 * *Files identical despite different names*

