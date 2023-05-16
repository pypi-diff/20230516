# Comparing `tmp/antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6.tar.gz` & `tmp/antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6.tar", last modified: Tue May 16 03:48:23 2023, max compression
+gzip compressed data, was "dist/antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8.tar", last modified: Tue May 16 03:58:19 2023, max compression
```

## Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6.tar` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:48:23.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-16 03:48:22.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 03:48:22.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 03:48:23.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-05-16 03:48:22.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-05-16 03:48:22.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:48:23.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 03:48:23.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-05-16 03:48:23.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 03:48:23.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-16 03:48:23.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-16 03:48:23.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:48:23.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 03:48:22.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27662 2023-05-16 03:48:22.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/client.py
--rw-r--r--   0 root         (0) root         (0)    23788 2023-05-16 03:48:22.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 03:48:23.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-05-16 03:48:22.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31410 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/client.py
+-rw-r--r--   0 root         (0) root         (0)    36763 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-05-16 03:58:19.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/setup.py
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/LICENSE` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/PKG-INFO` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_68b3ee3230284cddaa19740dcaf251d8
-Version: 1.0.6
+Version: 1.0.8
 Summary: Ant Chain Ak_68b3ee3230284cddaa19740dcaf251d8 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/README-CN.md` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/README.md` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/PKG-INFO` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-68b3ee3230284cddaa19740dcaf251d8
-Version: 1.0.6
+Version: 1.0.8
 Summary: Ant Chain Ak_68b3ee3230284cddaa19740dcaf251d8 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/SOURCES.txt` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/client.py` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -106,15 +106,15 @@
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
                 'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
                 'period': UtilClient.default_number(runtime.backoff_period, 1)
             },
             'ignoreSSL': runtime.ignore_ssl,
-            # 键值对，兼容map用
+            # api信息结构体
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
-                    'sdk_version': '1.0.6',
+                    'sdk_version': '1.0.8',
                     '_prod_code': 'ak_68b3ee3230284cddaa19740dcaf251d8',
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
-            # 键值对，兼容map用
+            # api信息结构体
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
-                    'sdk_version': '1.0.6',
+                    'sdk_version': '1.0.8',
                     '_prod_code': 'ak_68b3ee3230284cddaa19740dcaf251d8',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -271,342 +271,398 @@
             except Exception as e:
                 if TeaCore.is_retryable(e):
                     _last_exception = e
                     continue
                 raise e
         raise UnretryableException(_last_request, _last_exception)
 
-    def init_demo_bbp_insurance_user(
+    def update_demo_cjtest_cj(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoBbpInsuranceUserRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoBbpInsuranceUserResponse:
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.UpdateDemoCjtestCjRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.UpdateDemoCjtestCjResponse:
         """
-        Description: 保司用户埋点信息
-        Summary: 用户登陆页面埋点
+        Description: 测试网关评审能力
+        Summary: 评审测试
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.init_demo_bbp_insurance_user_ex(request, headers, runtime)
+        return self.update_demo_cjtest_cj_ex(request, headers, runtime)
 
-    async def init_demo_bbp_insurance_user_async(
+    async def update_demo_cjtest_cj_async(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoBbpInsuranceUserRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoBbpInsuranceUserResponse:
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.UpdateDemoCjtestCjRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.UpdateDemoCjtestCjResponse:
         """
-        Description: 保司用户埋点信息
-        Summary: 用户登陆页面埋点
+        Description: 测试网关评审能力
+        Summary: 评审测试
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.init_demo_bbp_insurance_user_ex_async(request, headers, runtime)
+        return await self.update_demo_cjtest_cj_ex_async(request, headers, runtime)
 
-    def init_demo_bbp_insurance_user_ex(
+    def update_demo_cjtest_cj_ex(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoBbpInsuranceUserRequest,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.UpdateDemoCjtestCjRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoBbpInsuranceUserResponse:
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.UpdateDemoCjtestCjResponse:
         """
-        Description: 保司用户埋点信息
-        Summary: 用户登陆页面埋点
+        Description: 测试网关评审能力
+        Summary: 评审测试
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoBbpInsuranceUserResponse(),
-            self.do_request('1.0', 'demo.bbp.insurance.user.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.UpdateDemoCjtestCjResponse(),
+            self.do_request('1.0', 'demo.cjtest.cj.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    async def init_demo_bbp_insurance_user_ex_async(
+    async def update_demo_cjtest_cj_ex_async(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoBbpInsuranceUserRequest,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.UpdateDemoCjtestCjRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoBbpInsuranceUserResponse:
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.UpdateDemoCjtestCjResponse:
         """
-        Description: 保司用户埋点信息
-        Summary: 用户登陆页面埋点
+        Description: 测试网关评审能力
+        Summary: 评审测试
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoBbpInsuranceUserResponse(),
-            await self.do_request_async('1.0', 'demo.bbp.insurance.user.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.UpdateDemoCjtestCjResponse(),
+            await self.do_request_async('1.0', 'demo.cjtest.cj.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    def query_demo_ad_asd_asd(
+    def pagequery_antchain_saas_ability(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoAdAsdAsdRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoAdAsdAsdResponse:
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.PagequeryAntchainSaasAbilityRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.PagequeryAntchainSaasAbilityResponse:
         """
-        Description: asd
-        Summary: asd1
+        Description: 分页查询能力数据
+        Summary: 分页查询能力数据
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.query_demo_ad_asd_asd_ex(request, headers, runtime)
+        return self.pagequery_antchain_saas_ability_ex(request, headers, runtime)
 
-    async def query_demo_ad_asd_asd_async(
+    async def pagequery_antchain_saas_ability_async(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoAdAsdAsdRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoAdAsdAsdResponse:
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.PagequeryAntchainSaasAbilityRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.PagequeryAntchainSaasAbilityResponse:
         """
-        Description: asd
-        Summary: asd1
+        Description: 分页查询能力数据
+        Summary: 分页查询能力数据
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.query_demo_ad_asd_asd_ex_async(request, headers, runtime)
+        return await self.pagequery_antchain_saas_ability_ex_async(request, headers, runtime)
 
-    def query_demo_ad_asd_asd_ex(
+    def pagequery_antchain_saas_ability_ex(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoAdAsdAsdRequest,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.PagequeryAntchainSaasAbilityRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoAdAsdAsdResponse:
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.PagequeryAntchainSaasAbilityResponse:
         """
-        Description: asd
-        Summary: asd1
+        Description: 分页查询能力数据
+        Summary: 分页查询能力数据
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoAdAsdAsdResponse(),
-            self.do_request('1.0', 'demo.ad.asd.asd.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.PagequeryAntchainSaasAbilityResponse(),
+            self.do_request('1.0', 'antchain.saas.ability.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    async def query_demo_ad_asd_asd_ex_async(
+    async def pagequery_antchain_saas_ability_ex_async(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoAdAsdAsdRequest,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.PagequeryAntchainSaasAbilityRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoAdAsdAsdResponse:
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.PagequeryAntchainSaasAbilityResponse:
         """
-        Description: asd
-        Summary: asd1
+        Description: 分页查询能力数据
+        Summary: 分页查询能力数据
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoAdAsdAsdResponse(),
-            await self.do_request_async('1.0', 'demo.ad.asd.asd.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.PagequeryAntchainSaasAbilityResponse(),
+            await self.do_request_async('1.0', 'antchain.saas.ability.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    def bind_demo_asd_asd_asd(
+    def bind_antchain_saas_ability(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAsdAsdAsdRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAsdAsdAsdResponse:
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityResponse:
         """
-        Description: asd
-        Summary: asd
+        Description: 绑定API
+        Summary: 绑定能力与API关系
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.bind_demo_asd_asd_asd_ex(request, headers, runtime)
+        return self.bind_antchain_saas_ability_ex(request, headers, runtime)
 
-    async def bind_demo_asd_asd_asd_async(
+    async def bind_antchain_saas_ability_async(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAsdAsdAsdRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAsdAsdAsdResponse:
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityResponse:
         """
-        Description: asd
-        Summary: asd
+        Description: 绑定API
+        Summary: 绑定能力与API关系
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.bind_demo_asd_asd_asd_ex_async(request, headers, runtime)
+        return await self.bind_antchain_saas_ability_ex_async(request, headers, runtime)
 
-    def bind_demo_asd_asd_asd_ex(
+    def bind_antchain_saas_ability_ex(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAsdAsdAsdRequest,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAsdAsdAsdResponse:
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityResponse:
         """
-        Description: asd
-        Summary: asd
+        Description: 绑定API
+        Summary: 绑定能力与API关系
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAsdAsdAsdResponse(),
-            self.do_request('1.0', 'demo.asd.asd.asd.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityResponse(),
+            self.do_request('1.0', 'antchain.saas.ability.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    async def bind_demo_asd_asd_asd_ex_async(
+    async def bind_antchain_saas_ability_ex_async(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAsdAsdAsdRequest,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAsdAsdAsdResponse:
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityResponse:
         """
-        Description: asd
-        Summary: asd
+        Description: 绑定API
+        Summary: 绑定能力与API关系
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAsdAsdAsdResponse(),
-            await self.do_request_async('1.0', 'demo.asd.asd.asd.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityResponse(),
+            await self.do_request_async('1.0', 'antchain.saas.ability.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    def bind_demo_center_ability(
+    def callback_antchain_saas_ability(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoCenterAbilityRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoCenterAbilityResponse:
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.CallbackAntchainSaasAbilityRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.CallbackAntchainSaasAbilityResponse:
         """
-        Description: 测试能力中心九期API打标&能力绑定API使用
-        Summary: 能力中心九期测试
+        Description: api上线回调接口
+        Summary: api上线回调接口
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.bind_demo_center_ability_ex(request, headers, runtime)
+        return self.callback_antchain_saas_ability_ex(request, headers, runtime)
 
-    async def bind_demo_center_ability_async(
+    async def callback_antchain_saas_ability_async(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoCenterAbilityRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoCenterAbilityResponse:
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.CallbackAntchainSaasAbilityRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.CallbackAntchainSaasAbilityResponse:
         """
-        Description: 测试能力中心九期API打标&能力绑定API使用
-        Summary: 能力中心九期测试
+        Description: api上线回调接口
+        Summary: api上线回调接口
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.bind_demo_center_ability_ex_async(request, headers, runtime)
+        return await self.callback_antchain_saas_ability_ex_async(request, headers, runtime)
 
-    def bind_demo_center_ability_ex(
+    def callback_antchain_saas_ability_ex(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoCenterAbilityRequest,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.CallbackAntchainSaasAbilityRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoCenterAbilityResponse:
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.CallbackAntchainSaasAbilityResponse:
         """
-        Description: 测试能力中心九期API打标&能力绑定API使用
-        Summary: 能力中心九期测试
+        Description: api上线回调接口
+        Summary: api上线回调接口
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoCenterAbilityResponse(),
-            self.do_request('1.0', 'demo.center.ability.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.CallbackAntchainSaasAbilityResponse(),
+            self.do_request('1.0', 'antchain.saas.ability.callback', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    async def bind_demo_center_ability_ex_async(
+    async def callback_antchain_saas_ability_ex_async(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoCenterAbilityRequest,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.CallbackAntchainSaasAbilityRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoCenterAbilityResponse:
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.CallbackAntchainSaasAbilityResponse:
         """
-        Description: 测试能力中心九期API打标&能力绑定API使用
-        Summary: 能力中心九期测试
+        Description: api上线回调接口
+        Summary: api上线回调接口
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoCenterAbilityResponse(),
-            await self.do_request_async('1.0', 'demo.center.ability.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.CallbackAntchainSaasAbilityResponse(),
+            await self.do_request_async('1.0', 'antchain.saas.ability.callback', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    def query_demo_approval_test(
+    def query_antchain_saas_ability_resultcode(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoApprovalTestRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoApprovalTestResponse:
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityResultcodeRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityResultcodeResponse:
         """
-        Description: 用于测试api评审接入SDL的测试使用
-        Summary: api评审测试
+        Description: 测试网关结果码和计量接口
+        Summary: 网关结果码测试接口
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.query_demo_approval_test_ex(request, headers, runtime)
+        return self.query_antchain_saas_ability_resultcode_ex(request, headers, runtime)
 
-    async def query_demo_approval_test_async(
+    async def query_antchain_saas_ability_resultcode_async(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoApprovalTestRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoApprovalTestResponse:
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityResultcodeRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityResultcodeResponse:
         """
-        Description: 用于测试api评审接入SDL的测试使用
-        Summary: api评审测试
+        Description: 测试网关结果码和计量接口
+        Summary: 网关结果码测试接口
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.query_demo_approval_test_ex_async(request, headers, runtime)
+        return await self.query_antchain_saas_ability_resultcode_ex_async(request, headers, runtime)
 
-    def query_demo_approval_test_ex(
+    def query_antchain_saas_ability_resultcode_ex(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoApprovalTestRequest,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityResultcodeRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoApprovalTestResponse:
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityResultcodeResponse:
         """
-        Description: 用于测试api评审接入SDL的测试使用
-        Summary: api评审测试
+        Description: 测试网关结果码和计量接口
+        Summary: 网关结果码测试接口
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoApprovalTestResponse(),
-            self.do_request('1.0', 'demo.approval.test.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityResultcodeResponse(),
+            self.do_request('1.0', 'antchain.saas.ability.resultcode.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    async def query_demo_approval_test_ex_async(
+    async def query_antchain_saas_ability_resultcode_ex_async(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoApprovalTestRequest,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityResultcodeRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoApprovalTestResponse:
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityResultcodeResponse:
         """
-        Description: 用于测试api评审接入SDL的测试使用
-        Summary: api评审测试
+        Description: 测试网关结果码和计量接口
+        Summary: 网关结果码测试接口
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoApprovalTestResponse(),
-            await self.do_request_async('1.0', 'demo.approval.test.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityResultcodeResponse(),
+            await self.do_request_async('1.0', 'antchain.saas.ability.resultcode.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    def init_demo_cjtest_acopm_res(
+    def bind_antchain_saas_ability_api(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoCjtestAcopmResRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoCjtestAcopmResResponse:
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityApiRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityApiResponse:
         """
-        Description: cj test
-        Summary: cj test
+        Description: 绑定能力的api信息
+        Summary: 绑定能力的api信息
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.init_demo_cjtest_acopm_res_ex(request, headers, runtime)
+        return self.bind_antchain_saas_ability_api_ex(request, headers, runtime)
 
-    async def init_demo_cjtest_acopm_res_async(
+    async def bind_antchain_saas_ability_api_async(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoCjtestAcopmResRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoCjtestAcopmResResponse:
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityApiRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityApiResponse:
         """
-        Description: cj test
-        Summary: cj test
+        Description: 绑定能力的api信息
+        Summary: 绑定能力的api信息
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.init_demo_cjtest_acopm_res_ex_async(request, headers, runtime)
+        return await self.bind_antchain_saas_ability_api_ex_async(request, headers, runtime)
 
-    def init_demo_cjtest_acopm_res_ex(
+    def bind_antchain_saas_ability_api_ex(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoCjtestAcopmResRequest,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityApiRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoCjtestAcopmResResponse:
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityApiResponse:
         """
-        Description: cj test
-        Summary: cj test
+        Description: 绑定能力的api信息
+        Summary: 绑定能力的api信息
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoCjtestAcopmResResponse(),
-            self.do_request('1.0', 'demo.cjtest.acopm.res.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityApiResponse(),
+            self.do_request('1.0', 'antchain.saas.ability.api.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    async def init_demo_cjtest_acopm_res_ex_async(
+    async def bind_antchain_saas_ability_api_ex_async(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoCjtestAcopmResRequest,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityApiRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoCjtestAcopmResResponse:
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityApiResponse:
         """
-        Description: cj test
-        Summary: cj test
+        Description: 绑定能力的api信息
+        Summary: 绑定能力的api信息
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoCjtestAcopmResResponse(),
-            await self.do_request_async('1.0', 'demo.cjtest.acopm.res.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityApiResponse(),
+            await self.do_request_async('1.0', 'antchain.saas.ability.api.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_antchain_saas_ability_businesscode(
+        self,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityBusinesscodeRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityBusinesscodeResponse:
+        """
+        Description: 根据商业产品编码查询能力信息
+        Summary: 根据商业产品编码查询能力信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_antchain_saas_ability_businesscode_ex(request, headers, runtime)
+
+    async def query_antchain_saas_ability_businesscode_async(
+        self,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityBusinesscodeRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityBusinesscodeResponse:
+        """
+        Description: 根据商业产品编码查询能力信息
+        Summary: 根据商业产品编码查询能力信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_antchain_saas_ability_businesscode_ex_async(request, headers, runtime)
+
+    def query_antchain_saas_ability_businesscode_ex(
+        self,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityBusinesscodeRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityBusinesscodeResponse:
+        """
+        Description: 根据商业产品编码查询能力信息
+        Summary: 根据商业产品编码查询能力信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityBusinesscodeResponse(),
+            self.do_request('1.0', 'antchain.saas.ability.businesscode.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_antchain_saas_ability_businesscode_ex_async(
+        self,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityBusinesscodeRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityBusinesscodeResponse:
+        """
+        Description: 根据商业产品编码查询能力信息
+        Summary: 根据商业产品编码查询能力信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityBusinesscodeResponse(),
+            await self.do_request_async('1.0', 'antchain.saas.ability.businesscode.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/models.py` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -150,174 +150,254 @@
         if m.get('maxRequests') is not None:
             self.max_requests = m.get('maxRequests')
         if m.get('maxRequestsPerHost') is not None:
             self.max_requests_per_host = m.get('maxRequestsPerHost')
         return self
 
 
-class NameValuePair(TeaModel):
+class ApiInfoModel(TeaModel):
     def __init__(
         self,
-        name: str = None,
-        value: str = None,
+        api_name: str = None,
+        prod_code: str = None,
+        internal: int = None,
+        api_version: str = None,
+        api_desc: str = None,
+        provider_id: str = None,
     ):
-        # 键名
-        self.name = name
-        # 键值
-        self.value = value
+        # api名称
+        self.api_name = api_name
+        # 产品码
+        self.prod_code = prod_code
+        # 是否是内部接口 0对外 1对内
+        self.internal = internal
+        # api版本号
+        self.api_version = api_version
+        # api描述
+        self.api_desc = api_desc
+        # api所属网关产品id
+        self.provider_id = provider_id
 
     def validate(self):
-        self.validate_required(self.name, 'name')
-        self.validate_required(self.value, 'value')
+        self.validate_required(self.api_name, 'api_name')
+        self.validate_required(self.prod_code, 'prod_code')
+        self.validate_required(self.internal, 'internal')
+        self.validate_required(self.api_version, 'api_version')
+        self.validate_required(self.api_desc, 'api_desc')
+        self.validate_required(self.provider_id, 'provider_id')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.name is not None:
-            result['name'] = self.name
-        if self.value is not None:
-            result['value'] = self.value
+        if self.api_name is not None:
+            result['api_name'] = self.api_name
+        if self.prod_code is not None:
+            result['prod_code'] = self.prod_code
+        if self.internal is not None:
+            result['internal'] = self.internal
+        if self.api_version is not None:
+            result['api_version'] = self.api_version
+        if self.api_desc is not None:
+            result['api_desc'] = self.api_desc
+        if self.provider_id is not None:
+            result['provider_id'] = self.provider_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('name') is not None:
-            self.name = m.get('name')
-        if m.get('value') is not None:
-            self.value = m.get('value')
+        if m.get('api_name') is not None:
+            self.api_name = m.get('api_name')
+        if m.get('prod_code') is not None:
+            self.prod_code = m.get('prod_code')
+        if m.get('internal') is not None:
+            self.internal = m.get('internal')
+        if m.get('api_version') is not None:
+            self.api_version = m.get('api_version')
+        if m.get('api_desc') is not None:
+            self.api_desc = m.get('api_desc')
+        if m.get('provider_id') is not None:
+            self.provider_id = m.get('provider_id')
         return self
 
 
-class QueryMap(TeaModel):
+class AbilityInfo(TeaModel):
     def __init__(
         self,
-        name: str = None,
-        value: List[NameValuePair] = None,
+        ability_id: str = None,
+        ability_name: str = None,
+        dev_owner: str = None,
+        gmt_create: str = None,
+        description: str = None,
+        dev_owner_prefix_email: str = None,
+        product_owner: str = None,
+        business_code: str = None,
+        api_info_models: List[ApiInfoModel] = None,
     ):
-        # 键值
-        self.name = name
-        # 额外用户信息
-        self.value = value
+        # 能力编号
+        self.ability_id = ability_id
+        # 能力名称
+        self.ability_name = ability_name
+        # 研发负责人
+        self.dev_owner = dev_owner
+        # 创建时间
+        self.gmt_create = gmt_create
+        # 描述信息
+        self.description = description
+        # 研发负责人邮箱前缀
+        self.dev_owner_prefix_email = dev_owner_prefix_email
+        # 产品负责人
+        self.product_owner = product_owner
+        # 能力对应商业中台L5Code
+        self.business_code = business_code
+        # apiInfoModels列表
+        self.api_info_models = api_info_models
 
     def validate(self):
-        self.validate_required(self.name, 'name')
-        if self.value:
-            for k in self.value:
+        self.validate_required(self.ability_id, 'ability_id')
+        self.validate_required(self.ability_name, 'ability_name')
+        self.validate_required(self.dev_owner, 'dev_owner')
+        self.validate_required(self.gmt_create, 'gmt_create')
+        self.validate_required(self.description, 'description')
+        self.validate_required(self.dev_owner_prefix_email, 'dev_owner_prefix_email')
+        self.validate_required(self.product_owner, 'product_owner')
+        self.validate_required(self.api_info_models, 'api_info_models')
+        if self.api_info_models:
+            for k in self.api_info_models:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.name is not None:
-            result['name'] = self.name
-        result['value'] = []
-        if self.value is not None:
-            for k in self.value:
-                result['value'].append(k.to_map() if k else None)
+        if self.ability_id is not None:
+            result['ability_id'] = self.ability_id
+        if self.ability_name is not None:
+            result['ability_name'] = self.ability_name
+        if self.dev_owner is not None:
+            result['dev_owner'] = self.dev_owner
+        if self.gmt_create is not None:
+            result['gmt_create'] = self.gmt_create
+        if self.description is not None:
+            result['description'] = self.description
+        if self.dev_owner_prefix_email is not None:
+            result['dev_owner_prefix_email'] = self.dev_owner_prefix_email
+        if self.product_owner is not None:
+            result['product_owner'] = self.product_owner
+        if self.business_code is not None:
+            result['business_code'] = self.business_code
+        result['api_info_models'] = []
+        if self.api_info_models is not None:
+            for k in self.api_info_models:
+                result['api_info_models'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('name') is not None:
-            self.name = m.get('name')
-        self.value = []
-        if m.get('value') is not None:
-            for k in m.get('value'):
-                temp_model = NameValuePair()
-                self.value.append(temp_model.from_map(k))
+        if m.get('ability_id') is not None:
+            self.ability_id = m.get('ability_id')
+        if m.get('ability_name') is not None:
+            self.ability_name = m.get('ability_name')
+        if m.get('dev_owner') is not None:
+            self.dev_owner = m.get('dev_owner')
+        if m.get('gmt_create') is not None:
+            self.gmt_create = m.get('gmt_create')
+        if m.get('description') is not None:
+            self.description = m.get('description')
+        if m.get('dev_owner_prefix_email') is not None:
+            self.dev_owner_prefix_email = m.get('dev_owner_prefix_email')
+        if m.get('product_owner') is not None:
+            self.product_owner = m.get('product_owner')
+        if m.get('business_code') is not None:
+            self.business_code = m.get('business_code')
+        self.api_info_models = []
+        if m.get('api_info_models') is not None:
+            for k in m.get('api_info_models'):
+                temp_model = ApiInfoModel()
+                self.api_info_models.append(temp_model.from_map(k))
         return self
 
 
-class InitDemoBbpInsuranceUserRequest(TeaModel):
+class UpdateDemoCjtestCjRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        business_code: str = None,
-        third_part_id: str = None,
-        channel: str = None,
-        burieds: QueryMap = None,
+        var_1: str = None,
+        var_2: str = None,
+        subject: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 保司编码
-        self.business_code = business_code
-        # 第三方id，此处为天猫uid
-        self.third_part_id = third_part_id
-        # 来源渠道
-        self.channel = channel
-        # 埋点信息
-        self.burieds = burieds
+        # 测试参数
+        self.var_1 = var_1
+        # 测试参数2
+        self.var_2 = var_2
+        # 被授权机构did
+        self.subject = subject
 
     def validate(self):
-        self.validate_required(self.business_code, 'business_code')
-        self.validate_required(self.third_part_id, 'third_part_id')
-        self.validate_required(self.channel, 'channel')
-        if self.burieds:
-            self.burieds.validate()
+        self.validate_required(self.var_1, 'var_1')
+        self.validate_required(self.var_2, 'var_2')
 
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
-        if self.third_part_id is not None:
-            result['third_part_id'] = self.third_part_id
-        if self.channel is not None:
-            result['channel'] = self.channel
-        if self.burieds is not None:
-            result['burieds'] = self.burieds.to_map()
+        if self.var_1 is not None:
+            result['var1'] = self.var_1
+        if self.var_2 is not None:
+            result['var2'] = self.var_2
+        if self.subject is not None:
+            result['subject'] = self.subject
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('business_code') is not None:
-            self.business_code = m.get('business_code')
-        if m.get('third_part_id') is not None:
-            self.third_part_id = m.get('third_part_id')
-        if m.get('channel') is not None:
-            self.channel = m.get('channel')
-        if m.get('burieds') is not None:
-            temp_model = QueryMap()
-            self.burieds = temp_model.from_map(m['burieds'])
+        if m.get('var1') is not None:
+            self.var_1 = m.get('var1')
+        if m.get('var2') is not None:
+            self.var_2 = m.get('var2')
+        if m.get('subject') is not None:
+            self.subject = m.get('subject')
         return self
 
 
-class InitDemoBbpInsuranceUserResponse(TeaModel):
+class UpdateDemoCjtestCjResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
+        return_1: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
+        # 测试返回参数1
+        self.return_1 = return_1
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -326,138 +406,324 @@
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
+        if self.return_1 is not None:
+            result['return1'] = self.return_1
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
+        if m.get('return1') is not None:
+            self.return_1 = m.get('return1')
         return self
 
 
-class QueryDemoAdAsdAsdRequest(TeaModel):
+class PagequeryAntchainSaasAbilityRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
+        current: int = None,
+        page_size: int = None,
+        keyword: str = None,
+        prod_code: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
+        # 当前页码
+        self.current = current
+        # 每页大小
+        self.page_size = page_size
+        # 用于能力的搜索标签
+        self.keyword = keyword
+        # 网关产品码
+        self.prod_code = prod_code
 
     def validate(self):
-        pass
+        self.validate_required(self.current, 'current')
+        self.validate_required(self.page_size, 'page_size')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
+        if self.current is not None:
+            result['current'] = self.current
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        if self.keyword is not None:
+            result['keyword'] = self.keyword
+        if self.prod_code is not None:
+            result['prod_code'] = self.prod_code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
+        if m.get('current') is not None:
+            self.current = m.get('current')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        if m.get('keyword') is not None:
+            self.keyword = m.get('keyword')
+        if m.get('prod_code') is not None:
+            self.prod_code = m.get('prod_code')
         return self
 
 
-class QueryDemoAdAsdAsdResponse(TeaModel):
+class PagequeryAntchainSaasAbilityResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
+        current: int = None,
+        page_size: int = None,
+        total: int = None,
+        ability_info_list: List[AbilityInfo] = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
+        # 当前页码
+        self.current = current
+        # 当前页大小
+        self.page_size = page_size
+        # 总数
+        self.total = total
+        # 能力信息列表
+        self.ability_info_list = ability_info_list
 
     def validate(self):
-        pass
+        if self.ability_info_list:
+            for k in self.ability_info_list:
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
+        if self.current is not None:
+            result['current'] = self.current
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        if self.total is not None:
+            result['total'] = self.total
+        result['ability_info_list'] = []
+        if self.ability_info_list is not None:
+            for k in self.ability_info_list:
+                result['ability_info_list'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
+        if m.get('current') is not None:
+            self.current = m.get('current')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        if m.get('total') is not None:
+            self.total = m.get('total')
+        self.ability_info_list = []
+        if m.get('ability_info_list') is not None:
+            for k in m.get('ability_info_list'):
+                temp_model = AbilityInfo()
+                self.ability_info_list.append(temp_model.from_map(k))
         return self
 
 
-class BindDemoAsdAsdAsdRequest(TeaModel):
+class BindAntchainSaasAbilityRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
+        api_name: str = None,
+        ability_ids: List[str] = None,
+        operator_id: str = None,
+        api_info_model: ApiInfoModel = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
+        # api名称
+        self.api_name = api_name
+        # 能力id列表
+        self.ability_ids = ability_ids
+        # 操作人的域账号
+        self.operator_id = operator_id
+        # api信息
+        self.api_info_model = api_info_model
+
+    def validate(self):
+        self.validate_required(self.api_name, 'api_name')
+        self.validate_required(self.ability_ids, 'ability_ids')
+        self.validate_required(self.operator_id, 'operator_id')
+        self.validate_required(self.api_info_model, 'api_info_model')
+        if self.api_info_model:
+            self.api_info_model.validate()
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
+        if self.api_name is not None:
+            result['api_name'] = self.api_name
+        if self.ability_ids is not None:
+            result['ability_ids'] = self.ability_ids
+        if self.operator_id is not None:
+            result['operator_id'] = self.operator_id
+        if self.api_info_model is not None:
+            result['api_info_model'] = self.api_info_model.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('api_name') is not None:
+            self.api_name = m.get('api_name')
+        if m.get('ability_ids') is not None:
+            self.ability_ids = m.get('ability_ids')
+        if m.get('operator_id') is not None:
+            self.operator_id = m.get('operator_id')
+        if m.get('api_info_model') is not None:
+            temp_model = ApiInfoModel()
+            self.api_info_model = temp_model.from_map(m['api_info_model'])
+        return self
+
+
+class BindAntchainSaasAbilityResponse(TeaModel):
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
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
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
+class CallbackAntchainSaasAbilityRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        api_names: List[str] = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # api名称集合
+        self.api_names = api_names
+
+    def validate(self):
+        self.validate_required(self.api_names, 'api_names')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
+        if self.api_names is not None:
+            result['api_names'] = self.api_names
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
+        if m.get('api_names') is not None:
+            self.api_names = m.get('api_names')
         return self
 
 
-class BindDemoAsdAsdAsdResponse(TeaModel):
+class CallbackAntchainSaasAbilityResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
@@ -491,49 +757,56 @@
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         return self
 
 
-class BindDemoCenterAbilityRequest(TeaModel):
+class QueryAntchainSaasAbilityResultcodeRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
+        index: int = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
+        # 1-INTERNAL_ERROR，2-TOO_MANY_REQUESTS，3-UNKNOW_ERROR，4-ACCESS_DENIED，5-OK，6-CUSTOM_RESULT_CODE_ONE，7-CUSTOM_RESULT_CODE_TWO
+        self.index = index
 
     def validate(self):
-        pass
+        self.validate_required(self.index, 'index')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
+        if self.index is not None:
+            result['index'] = self.index
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
+        if m.get('index') is not None:
+            self.index = m.get('index')
         return self
 
 
-class BindDemoCenterAbilityResponse(TeaModel):
+class QueryAntchainSaasAbilityResultcodeResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
@@ -567,71 +840,93 @@
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         return self
 
 
-class QueryDemoApprovalTestRequest(TeaModel):
+class BindAntchainSaasAbilityApiRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        input: str = None,
+        ability_id: str = None,
+        operator_id: str = None,
+        api_info_models: List[ApiInfoModel] = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 字符串
-        self.input = input
+        # 共享能力id
+        self.ability_id = ability_id
+        # qiujianglong.qjl
+        self.operator_id = operator_id
+        # api模型集合
+        self.api_info_models = api_info_models
 
     def validate(self):
-        self.validate_required(self.input, 'input')
+        self.validate_required(self.ability_id, 'ability_id')
+        self.validate_required(self.operator_id, 'operator_id')
+        self.validate_required(self.api_info_models, 'api_info_models')
+        if self.api_info_models:
+            for k in self.api_info_models:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.input is not None:
-            result['input'] = self.input
+        if self.ability_id is not None:
+            result['ability_id'] = self.ability_id
+        if self.operator_id is not None:
+            result['operator_id'] = self.operator_id
+        result['api_info_models'] = []
+        if self.api_info_models is not None:
+            for k in self.api_info_models:
+                result['api_info_models'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('input') is not None:
-            self.input = m.get('input')
+        if m.get('ability_id') is not None:
+            self.ability_id = m.get('ability_id')
+        if m.get('operator_id') is not None:
+            self.operator_id = m.get('operator_id')
+        self.api_info_models = []
+        if m.get('api_info_models') is not None:
+            for k in m.get('api_info_models'):
+                temp_model = ApiInfoModel()
+                self.api_info_models.append(temp_model.from_map(k))
         return self
 
 
-class QueryDemoApprovalTestResponse(TeaModel):
+class BindAntchainSaasAbilityApiResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
-        msg: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
-        # 回参
-        self.msg = msg
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -640,100 +935,112 @@
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
-        if self.msg is not None:
-            result['msg'] = self.msg
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
-        if m.get('msg') is not None:
-            self.msg = m.get('msg')
         return self
 
 
-class InitDemoCjtestAcopmResRequest(TeaModel):
+class QueryAntchainSaasAbilityBusinesscodeRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
+        business_code: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
+        # 商业产品编码，L5编码
+        self.business_code = business_code
 
     def validate(self):
-        pass
+        self.validate_required(self.business_code, 'business_code')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
+        if self.business_code is not None:
+            result['business_code'] = self.business_code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
+        if m.get('business_code') is not None:
+            self.business_code = m.get('business_code')
         return self
 
 
-class InitDemoCjtestAcopmResResponse(TeaModel):
+class QueryAntchainSaasAbilityBusinesscodeResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
+        ability_info: AbilityInfo = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
+        # 能力信息
+        self.ability_info = ability_info
 
     def validate(self):
-        pass
+        if self.ability_info:
+            self.ability_info.validate()
 
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
+        if self.ability_info is not None:
+            result['ability_info'] = self.ability_info.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
+        if m.get('ability_info') is not None:
+            temp_model = AbilityInfo()
+            self.ability_info = temp_model.from_map(m['ability_info'])
         return self
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/setup.py` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.8/setup.py`

 * *Files identical despite different names*

