# Comparing `tmp/antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8.tar.gz` & `tmp/antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8.tar", last modified: Tue Aug 23 02:34:49 2022, max compression
+gzip compressed data, was "dist/antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9.tar", last modified: Wed May 10 09:18:06 2023, max compression
```

## Comparing `antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8.tar` & `antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 02:34:49.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      600 2022-08-23 02:34:48.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-08-23 02:34:48.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2022-08-23 02:34:49.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2022-08-23 02:34:48.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2022-08-23 02:34:48.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 02:34:49.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2022-08-23 02:34:48.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2022-08-23 02:34:48.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-23 02:34:48.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2022-08-23 02:34:48.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2022-08-23 02:34:48.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-23 02:34:49.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/antchain_sdk_ak_5bb1b66c4aab4cc998c05a36078e45c1/
--rw-r--r--   0 root         (0) root         (0)       21 2022-08-23 02:34:48.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/antchain_sdk_ak_5bb1b66c4aab4cc998c05a36078e45c1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51818 2022-08-23 02:34:48.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/antchain_sdk_ak_5bb1b66c4aab4cc998c05a36078e45c1/client.py
--rw-r--r--   0 root         (0) root         (0)    99210 2022-08-23 02:34:48.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/antchain_sdk_ak_5bb1b66c4aab4cc998c05a36078e45c1/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2022-08-23 02:34:49.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2022-08-23 02:34:48.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 09:18:06.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-10 09:18:06.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-10 09:18:06.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-10 09:18:06.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-05-10 09:18:06.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-05-10 09:18:06.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 09:18:06.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-10 09:18:06.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-10 09:18:06.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 09:18:06.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-10 09:18:06.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-10 09:18:06.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 09:18:06.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/antchain_sdk_ak_5bb1b66c4aab4cc998c05a36078e45c1/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-10 09:18:06.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/antchain_sdk_ak_5bb1b66c4aab4cc998c05a36078e45c1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49112 2023-05-10 09:18:06.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/antchain_sdk_ak_5bb1b66c4aab4cc998c05a36078e45c1/client.py
+-rw-r--r--   0 root         (0) root         (0)    96689 2023-05-10 09:18:06.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/antchain_sdk_ak_5bb1b66c4aab4cc998c05a36078e45c1/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-10 09:18:06.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-05-10 09:18:06.000000 antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/setup.py
```

### Comparing `antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/LICENSE` & `antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/PKG-INFO` & `antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1
-Version: 1.0.8
+Version: 1.0.9
 Summary: Ant Chain Ak_5bb1b66c4aab4cc998c05a36078e45c1 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/README-CN.md` & `antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/README.md` & `antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1.egg-info/PKG-INFO` & `antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-5bb1b66c4aab4cc998c05a36078e45c1
-Version: 1.0.8
+Version: 1.0.9
 Summary: Ant Chain Ak_5bb1b66c4aab4cc998c05a36078e45c1 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1.egg-info/SOURCES.txt` & `antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/antchain_sdk_ak_5bb1b66c4aab4cc998c05a36078e45c1/client.py` & `antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/antchain_sdk_ak_5bb1b66c4aab4cc998c05a36078e45c1/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.8',
+                    'sdk_version': '1.0.9',
                     '_prod_code': 'ak_5bb1b66c4aab4cc998c05a36078e45c1',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -198,15 +198,15 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.8',
+                    'sdk_version': '1.0.9',
                     '_prod_code': 'ak_5bb1b66c4aab4cc998c05a36078e45c1',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -607,70 +607,14 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.VerifyAntchainBbpMetaResponse(),
             await self.do_request_async('1.0', 'antchain.bbp.meta.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    def bind_demo_aaa_bbb_ccc(
-        self,
-        request: ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.BindDemoAaaBbbCccRequest,
-    ) -> ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.BindDemoAaaBbbCccResponse:
-        """
-        Description: 自动化测试创建，用于测试新建&修改功能
-        Summary: 自动化测试创建，用于测试新建&修改功能
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.bind_demo_aaa_bbb_ccc_ex(request, headers, runtime)
-
-    async def bind_demo_aaa_bbb_ccc_async(
-        self,
-        request: ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.BindDemoAaaBbbCccRequest,
-    ) -> ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.BindDemoAaaBbbCccResponse:
-        """
-        Description: 自动化测试创建，用于测试新建&修改功能
-        Summary: 自动化测试创建，用于测试新建&修改功能
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.bind_demo_aaa_bbb_ccc_ex_async(request, headers, runtime)
-
-    def bind_demo_aaa_bbb_ccc_ex(
-        self,
-        request: ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.BindDemoAaaBbbCccRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.BindDemoAaaBbbCccResponse:
-        """
-        Description: 自动化测试创建，用于测试新建&修改功能
-        Summary: 自动化测试创建，用于测试新建&修改功能
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.BindDemoAaaBbbCccResponse(),
-            self.do_request('1.0', 'demo.aaa.bbb.ccc.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def bind_demo_aaa_bbb_ccc_ex_async(
-        self,
-        request: ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.BindDemoAaaBbbCccRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.BindDemoAaaBbbCccResponse:
-        """
-        Description: 自动化测试创建，用于测试新建&修改功能
-        Summary: 自动化测试创建，用于测试新建&修改功能
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.BindDemoAaaBbbCccResponse(),
-            await self.do_request_async('1.0', 'demo.aaa.bbb.ccc.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
     def check_saas_security_infosec_holoxcontentcheckservice(
         self,
         request: ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.CheckSaasSecurityInfosecHoloxcontentcheckserviceRequest,
     ) -> ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.CheckSaasSecurityInfosecHoloxcontentcheckserviceResponse:
         """
         Description: 大安全接口
         Summary: 大安全接口
@@ -837,41 +781,41 @@
 
     def query_saas_security_infosec_holoxcontentcheckqueryservice(
         self,
         request: ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.QuerySaasSecurityInfosecHoloxcontentcheckqueryserviceRequest,
     ) -> ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.QuerySaasSecurityInfosecHoloxcontentcheckqueryserviceResponse:
         """
         Description: 123
-        Summary: 大安全接口
+        Summary: 大安全内容风控接口
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.query_saas_security_infosec_holoxcontentcheckqueryservice_ex(request, headers, runtime)
 
     async def query_saas_security_infosec_holoxcontentcheckqueryservice_async(
         self,
         request: ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.QuerySaasSecurityInfosecHoloxcontentcheckqueryserviceRequest,
     ) -> ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.QuerySaasSecurityInfosecHoloxcontentcheckqueryserviceResponse:
         """
         Description: 123
-        Summary: 大安全接口
+        Summary: 大安全内容风控接口
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.query_saas_security_infosec_holoxcontentcheckqueryservice_ex_async(request, headers, runtime)
 
     def query_saas_security_infosec_holoxcontentcheckqueryservice_ex(
         self,
         request: ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.QuerySaasSecurityInfosecHoloxcontentcheckqueryserviceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.QuerySaasSecurityInfosecHoloxcontentcheckqueryserviceResponse:
         """
         Description: 123
-        Summary: 大安全接口
+        Summary: 大安全内容风控接口
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.QuerySaasSecurityInfosecHoloxcontentcheckqueryserviceResponse(),
             self.do_request('1.0', 'saas.security.infosec.holoxcontentcheckqueryservice.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
@@ -879,15 +823,15 @@
         self,
         request: ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.QuerySaasSecurityInfosecHoloxcontentcheckqueryserviceRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.QuerySaasSecurityInfosecHoloxcontentcheckqueryserviceResponse:
         """
         Description: 123
-        Summary: 大安全接口
+        Summary: 大安全内容风控接口
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak__5bb_1b_66c_4aab_4cc_998c_05a_36078e_45c_1_models.QuerySaasSecurityInfosecHoloxcontentcheckqueryserviceResponse(),
             await self.do_request_async('1.0', 'saas.security.infosec.holoxcontentcheckqueryservice.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
```

### Comparing `antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/antchain_sdk_ak_5bb1b66c4aab4cc998c05a36078e45c1/models.py` & `antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/antchain_sdk_ak_5bb1b66c4aab4cc998c05a36078e45c1/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2043,97 +2043,14 @@
             self.result_msg = m.get('result_msg')
         if m.get('result') is not None:
             temp_model = CustomerAuthResult()
             self.result = temp_model.from_map(m['result'])
         return self
 
 
-class BindDemoAaaBbbCccRequest(TeaModel):
-    def __init__(
-        self,
-        auth_token: str = None,
-        product_instance_id: str = None,
-        data: str = None,
-    ):
-        # OAuth模式下的授权token
-        self.auth_token = auth_token
-        self.product_instance_id = product_instance_id
-        # 123
-        self.data = data
-
-    def validate(self):
-        self.validate_required(self.data, 'data')
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
-        if self.data is not None:
-            result['data'] = self.data
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('auth_token') is not None:
-            self.auth_token = m.get('auth_token')
-        if m.get('product_instance_id') is not None:
-            self.product_instance_id = m.get('product_instance_id')
-        if m.get('data') is not None:
-            self.data = m.get('data')
-        return self
-
-
-class BindDemoAaaBbbCccResponse(TeaModel):
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
 class CheckSaasSecurityInfosecHoloxcontentcheckserviceRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         holox_check_event: HoloxCheckEvent = None,
         service_version: str = None,
```

### Comparing `antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.8/setup.py` & `antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1.
 
-Created on 23/08/2022
+Created on 10/05/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_ak_5bb1b66c4aab4cc998c05a36078e45c1"
 NAME = "antchain_ak_5bb1b66c4aab4cc998c05a36078e45c1" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain Ak_5bb1b66c4aab4cc998c05a36078e45c1 SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

