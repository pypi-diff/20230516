# Comparing `tmp/antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5.tar.gz` & `tmp/antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5.tar", last modified: Tue May 16 03:21:03 2023, max compression
+gzip compressed data, was "dist/antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6.tar", last modified: Tue May 16 03:48:23 2023, max compression
```

## Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5.tar` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:21:03.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-16 03:21:03.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 03:21:03.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 03:21:03.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-05-16 03:21:03.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-05-16 03:21:03.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:21:03.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 03:21:03.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-05-16 03:21:03.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 03:21:03.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-16 03:21:03.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-16 03:21:03.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:21:03.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 03:21:03.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34424 2023-05-16 03:21:03.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/client.py
--rw-r--r--   0 root         (0) root         (0)    39027 2023-05-16 03:21:03.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 03:21:03.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-05-16 03:21:03.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:48:23.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-16 03:48:22.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 03:48:22.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 03:48:23.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-05-16 03:48:22.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-05-16 03:48:22.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:48:23.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 03:48:23.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-16 03:48:23.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 03:48:23.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-16 03:48:23.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-16 03:48:23.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 03:48:23.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 03:48:22.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27662 2023-05-16 03:48:22.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/client.py
+-rw-r--r--   0 root         (0) root         (0)    23788 2023-05-16 03:48:22.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 03:48:23.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-05-16 03:48:22.000000 antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/setup.py
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/LICENSE` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/PKG-INFO` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_68b3ee3230284cddaa19740dcaf251d8
-Version: 1.0.5
+Version: 1.0.6
 Summary: Ant Chain Ak_68b3ee3230284cddaa19740dcaf251d8 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/README-CN.md` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/README.md` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/PKG-INFO` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-68b3ee3230284cddaa19740dcaf251d8
-Version: 1.0.5
+Version: 1.0.6
 Summary: Ant Chain Ak_68b3ee3230284cddaa19740dcaf251d8 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/SOURCES.txt` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_ak_68b3ee3230284cddaa19740dcaf251d8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/client.py` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/client.py`

 * *Files 24% similar despite different names*

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
+            # 键值对，兼容map用
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
-                    'sdk_version': '1.0.5',
+                    'sdk_version': '1.0.6',
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
-            # api信息结构体
+            # 键值对，兼容map用
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
-                    'sdk_version': '1.0.5',
+                    'sdk_version': '1.0.6',
                     '_prod_code': 'ak_68b3ee3230284cddaa19740dcaf251d8',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -271,180 +271,180 @@
             except Exception as e:
                 if TeaCore.is_retryable(e):
                     _last_exception = e
                     continue
                 raise e
         raise UnretryableException(_last_request, _last_exception)
 
-    def publish_demo_saas_test_testc(
+    def init_demo_bbp_insurance_user(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.PublishDemoSaasTestTestcRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.PublishDemoSaasTestTestcResponse:
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoBbpInsuranceUserRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoBbpInsuranceUserResponse:
         """
-        Description: testc
-        Summary: 测试用api
+        Description: 保司用户埋点信息
+        Summary: 用户登陆页面埋点
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.publish_demo_saas_test_testc_ex(request, headers, runtime)
+        return self.init_demo_bbp_insurance_user_ex(request, headers, runtime)
 
-    async def publish_demo_saas_test_testc_async(
+    async def init_demo_bbp_insurance_user_async(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.PublishDemoSaasTestTestcRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.PublishDemoSaasTestTestcResponse:
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoBbpInsuranceUserRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoBbpInsuranceUserResponse:
         """
-        Description: testc
-        Summary: 测试用api
+        Description: 保司用户埋点信息
+        Summary: 用户登陆页面埋点
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.publish_demo_saas_test_testc_ex_async(request, headers, runtime)
+        return await self.init_demo_bbp_insurance_user_ex_async(request, headers, runtime)
 
-    def publish_demo_saas_test_testc_ex(
+    def init_demo_bbp_insurance_user_ex(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.PublishDemoSaasTestTestcRequest,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoBbpInsuranceUserRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.PublishDemoSaasTestTestcResponse:
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoBbpInsuranceUserResponse:
         """
-        Description: testc
-        Summary: 测试用api
+        Description: 保司用户埋点信息
+        Summary: 用户登陆页面埋点
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.PublishDemoSaasTestTestcResponse(),
-            self.do_request('1.0', 'demo.saas.test.testc.publish', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoBbpInsuranceUserResponse(),
+            self.do_request('1.0', 'demo.bbp.insurance.user.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    async def publish_demo_saas_test_testc_ex_async(
+    async def init_demo_bbp_insurance_user_ex_async(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.PublishDemoSaasTestTestcRequest,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoBbpInsuranceUserRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.PublishDemoSaasTestTestcResponse:
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoBbpInsuranceUserResponse:
         """
-        Description: testc
-        Summary: 测试用api
+        Description: 保司用户埋点信息
+        Summary: 用户登陆页面埋点
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.PublishDemoSaasTestTestcResponse(),
-            await self.do_request_async('1.0', 'demo.saas.test.testc.publish', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoBbpInsuranceUserResponse(),
+            await self.do_request_async('1.0', 'demo.bbp.insurance.user.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    def bind_antchain_saas_ability(
+    def query_demo_ad_asd_asd(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityResponse:
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoAdAsdAsdRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoAdAsdAsdResponse:
         """
-        Description: 绑定API
-        Summary: 绑定能力与API关系
+        Description: asd
+        Summary: asd1
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.bind_antchain_saas_ability_ex(request, headers, runtime)
+        return self.query_demo_ad_asd_asd_ex(request, headers, runtime)
 
-    async def bind_antchain_saas_ability_async(
+    async def query_demo_ad_asd_asd_async(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityResponse:
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoAdAsdAsdRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoAdAsdAsdResponse:
         """
-        Description: 绑定API
-        Summary: 绑定能力与API关系
+        Description: asd
+        Summary: asd1
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.bind_antchain_saas_ability_ex_async(request, headers, runtime)
+        return await self.query_demo_ad_asd_asd_ex_async(request, headers, runtime)
 
-    def bind_antchain_saas_ability_ex(
+    def query_demo_ad_asd_asd_ex(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityRequest,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoAdAsdAsdRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityResponse:
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoAdAsdAsdResponse:
         """
-        Description: 绑定API
-        Summary: 绑定能力与API关系
+        Description: asd
+        Summary: asd1
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityResponse(),
-            self.do_request('1.0', 'antchain.saas.ability.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoAdAsdAsdResponse(),
+            self.do_request('1.0', 'demo.ad.asd.asd.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    async def bind_antchain_saas_ability_ex_async(
+    async def query_demo_ad_asd_asd_ex_async(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityRequest,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoAdAsdAsdRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityResponse:
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoAdAsdAsdResponse:
         """
-        Description: 绑定API
-        Summary: 绑定能力与API关系
+        Description: asd
+        Summary: asd1
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindAntchainSaasAbilityResponse(),
-            await self.do_request_async('1.0', 'antchain.saas.ability.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoAdAsdAsdResponse(),
+            await self.do_request_async('1.0', 'demo.ad.asd.asd.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    def query_antchain_saas_ability_withapiname(
+    def bind_demo_asd_asd_asd(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityWithapinameRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityWithapinameResponse:
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAsdAsdAsdRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAsdAsdAsdResponse:
         """
-        Description: 根据api名称列表查询能力标签列表
-        Summary: 根据api名称列表查询能力标签列表
+        Description: asd
+        Summary: asd
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.query_antchain_saas_ability_withapiname_ex(request, headers, runtime)
+        return self.bind_demo_asd_asd_asd_ex(request, headers, runtime)
 
-    async def query_antchain_saas_ability_withapiname_async(
+    async def bind_demo_asd_asd_asd_async(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityWithapinameRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityWithapinameResponse:
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAsdAsdAsdRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAsdAsdAsdResponse:
         """
-        Description: 根据api名称列表查询能力标签列表
-        Summary: 根据api名称列表查询能力标签列表
+        Description: asd
+        Summary: asd
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.query_antchain_saas_ability_withapiname_ex_async(request, headers, runtime)
+        return await self.bind_demo_asd_asd_asd_ex_async(request, headers, runtime)
 
-    def query_antchain_saas_ability_withapiname_ex(
+    def bind_demo_asd_asd_asd_ex(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityWithapinameRequest,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAsdAsdAsdRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityWithapinameResponse:
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAsdAsdAsdResponse:
         """
-        Description: 根据api名称列表查询能力标签列表
-        Summary: 根据api名称列表查询能力标签列表
+        Description: asd
+        Summary: asd
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityWithapinameResponse(),
-            self.do_request('1.0', 'antchain.saas.ability.withapiname.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAsdAsdAsdResponse(),
+            self.do_request('1.0', 'demo.asd.asd.asd.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    async def query_antchain_saas_ability_withapiname_ex_async(
+    async def bind_demo_asd_asd_asd_ex_async(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityWithapinameRequest,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAsdAsdAsdRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityWithapinameResponse:
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAsdAsdAsdResponse:
         """
-        Description: 根据api名称列表查询能力标签列表
-        Summary: 根据api名称列表查询能力标签列表
+        Description: asd
+        Summary: asd
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityWithapinameResponse(),
-            await self.do_request_async('1.0', 'antchain.saas.ability.withapiname.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoAsdAsdAsdResponse(),
+            await self.do_request_async('1.0', 'demo.asd.asd.asd.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def bind_demo_center_ability(
         self,
         request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoCenterAbilityRequest,
     ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoCenterAbilityResponse:
         """
@@ -495,230 +495,118 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoCenterAbilityResponse(),
             await self.do_request_async('1.0', 'demo.center.ability.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    def bind_demo_more_ability_testabc(
+    def query_demo_approval_test(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoMoreAbilityTestabcRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoMoreAbilityTestabcResponse:
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoApprovalTestRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoApprovalTestResponse:
         """
-        Description: 测试API绑定多个标签时的情况
-        Summary: API绑定多个标签
+        Description: 用于测试api评审接入SDL的测试使用
+        Summary: api评审测试
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.bind_demo_more_ability_testabc_ex(request, headers, runtime)
+        return self.query_demo_approval_test_ex(request, headers, runtime)
 
-    async def bind_demo_more_ability_testabc_async(
+    async def query_demo_approval_test_async(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoMoreAbilityTestabcRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoMoreAbilityTestabcResponse:
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoApprovalTestRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoApprovalTestResponse:
         """
-        Description: 测试API绑定多个标签时的情况
-        Summary: API绑定多个标签
+        Description: 用于测试api评审接入SDL的测试使用
+        Summary: api评审测试
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.bind_demo_more_ability_testabc_ex_async(request, headers, runtime)
+        return await self.query_demo_approval_test_ex_async(request, headers, runtime)
 
-    def bind_demo_more_ability_testabc_ex(
+    def query_demo_approval_test_ex(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoMoreAbilityTestabcRequest,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoApprovalTestRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoMoreAbilityTestabcResponse:
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoApprovalTestResponse:
         """
-        Description: 测试API绑定多个标签时的情况
-        Summary: API绑定多个标签
+        Description: 用于测试api评审接入SDL的测试使用
+        Summary: api评审测试
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoMoreAbilityTestabcResponse(),
-            self.do_request('1.0', 'demo.more.ability.testabc.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoApprovalTestResponse(),
+            self.do_request('1.0', 'demo.approval.test.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    async def bind_demo_more_ability_testabc_ex_async(
+    async def query_demo_approval_test_ex_async(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoMoreAbilityTestabcRequest,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoApprovalTestRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoMoreAbilityTestabcResponse:
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoApprovalTestResponse:
         """
-        Description: 测试API绑定多个标签时的情况
-        Summary: API绑定多个标签
+        Description: 用于测试api评审接入SDL的测试使用
+        Summary: api评审测试
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.BindDemoMoreAbilityTestabcResponse(),
-            await self.do_request_async('1.0', 'demo.more.ability.testabc.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryDemoApprovalTestResponse(),
+            await self.do_request_async('1.0', 'demo.approval.test.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    def callback_antchain_saas_ability(
+    def init_demo_cjtest_acopm_res(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.CallbackAntchainSaasAbilityRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.CallbackAntchainSaasAbilityResponse:
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoCjtestAcopmResRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoCjtestAcopmResResponse:
         """
-        Description: api上线回调接口
-        Summary: api上线回调接口
+        Description: cj test
+        Summary: cj test
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.callback_antchain_saas_ability_ex(request, headers, runtime)
+        return self.init_demo_cjtest_acopm_res_ex(request, headers, runtime)
 
-    async def callback_antchain_saas_ability_async(
+    async def init_demo_cjtest_acopm_res_async(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.CallbackAntchainSaasAbilityRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.CallbackAntchainSaasAbilityResponse:
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoCjtestAcopmResRequest,
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoCjtestAcopmResResponse:
         """
-        Description: api上线回调接口
-        Summary: api上线回调接口
+        Description: cj test
+        Summary: cj test
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.callback_antchain_saas_ability_ex_async(request, headers, runtime)
+        return await self.init_demo_cjtest_acopm_res_ex_async(request, headers, runtime)
 
-    def callback_antchain_saas_ability_ex(
+    def init_demo_cjtest_acopm_res_ex(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.CallbackAntchainSaasAbilityRequest,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoCjtestAcopmResRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.CallbackAntchainSaasAbilityResponse:
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoCjtestAcopmResResponse:
         """
-        Description: api上线回调接口
-        Summary: api上线回调接口
+        Description: cj test
+        Summary: cj test
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.CallbackAntchainSaasAbilityResponse(),
-            self.do_request('1.0', 'antchain.saas.ability.callback', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoCjtestAcopmResResponse(),
+            self.do_request('1.0', 'demo.cjtest.acopm.res.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
-    async def callback_antchain_saas_ability_ex_async(
+    async def init_demo_cjtest_acopm_res_ex_async(
         self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.CallbackAntchainSaasAbilityRequest,
+        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoCjtestAcopmResRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.CallbackAntchainSaasAbilityResponse:
+    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoCjtestAcopmResResponse:
         """
-        Description: api上线回调接口
-        Summary: api上线回调接口
+        Description: cj test
+        Summary: cj test
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.CallbackAntchainSaasAbilityResponse(),
-            await self.do_request_async('1.0', 'antchain.saas.ability.callback', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    def query_antchain_saas_foundation_protobuf(
-        self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasFoundationProtobufRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasFoundationProtobufResponse:
-        """
-        Description: 根据产品码+api code查询api protobuf信息
-        Summary: 查询api protobuf信息（勿删）
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.query_antchain_saas_foundation_protobuf_ex(request, headers, runtime)
-
-    async def query_antchain_saas_foundation_protobuf_async(
-        self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasFoundationProtobufRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasFoundationProtobufResponse:
-        """
-        Description: 根据产品码+api code查询api protobuf信息
-        Summary: 查询api protobuf信息（勿删）
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.query_antchain_saas_foundation_protobuf_ex_async(request, headers, runtime)
-
-    def query_antchain_saas_foundation_protobuf_ex(
-        self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasFoundationProtobufRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasFoundationProtobufResponse:
-        """
-        Description: 根据产品码+api code查询api protobuf信息
-        Summary: 查询api protobuf信息（勿删）
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasFoundationProtobufResponse(),
-            self.do_request('1.0', 'antchain.saas.foundation.protobuf.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def query_antchain_saas_foundation_protobuf_ex_async(
-        self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasFoundationProtobufRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasFoundationProtobufResponse:
-        """
-        Description: 根据产品码+api code查询api protobuf信息
-        Summary: 查询api protobuf信息（勿删）
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasFoundationProtobufResponse(),
-            await self.do_request_async('1.0', 'antchain.saas.foundation.protobuf.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    def query_antchain_saas_ability_resultcode(
-        self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityResultcodeRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityResultcodeResponse:
-        """
-        Description: 测试网关结果码和计量接口
-        Summary: 网关结果码测试接口
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return self.query_antchain_saas_ability_resultcode_ex(request, headers, runtime)
-
-    async def query_antchain_saas_ability_resultcode_async(
-        self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityResultcodeRequest,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityResultcodeResponse:
-        """
-        Description: 测试网关结果码和计量接口
-        Summary: 网关结果码测试接口
-        """
-        runtime = util_models.RuntimeOptions()
-        headers = {}
-        return await self.query_antchain_saas_ability_resultcode_ex_async(request, headers, runtime)
-
-    def query_antchain_saas_ability_resultcode_ex(
-        self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityResultcodeRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityResultcodeResponse:
-        """
-        Description: 测试网关结果码和计量接口
-        Summary: 网关结果码测试接口
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityResultcodeResponse(),
-            self.do_request('1.0', 'antchain.saas.ability.resultcode.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
-        )
-
-    async def query_antchain_saas_ability_resultcode_ex_async(
-        self,
-        request: ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityResultcodeRequest,
-        headers: Dict[str, str],
-        runtime: util_models.RuntimeOptions,
-    ) -> ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityResultcodeResponse:
-        """
-        Description: 测试网关结果码和计量接口
-        Summary: 网关结果码测试接口
-        """
-        UtilClient.validate_model(request)
-        return TeaCore.from_map(
-            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.QueryAntchainSaasAbilityResultcodeResponse(),
-            await self.do_request_async('1.0', 'antchain.saas.ability.resultcode.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+            ak__68b_3ee_3230284cddaa_19740dcaf_251d_8_models.InitDemoCjtestAcopmResResponse(),
+            await self.do_request_async('1.0', 'demo.cjtest.acopm.res.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/models.py` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/antchain_sdk_ak_68b3ee3230284cddaa19740dcaf251d8/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -150,570 +150,204 @@
         if m.get('maxRequests') is not None:
             self.max_requests = m.get('maxRequests')
         if m.get('maxRequestsPerHost') is not None:
             self.max_requests_per_host = m.get('maxRequestsPerHost')
         return self
 
 
-class ApiInfoModel(TeaModel):
+class NameValuePair(TeaModel):
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
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
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
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
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
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
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
-        return self
-
-
-class AbilityApiRelation(TeaModel):
-    def __init__(
-        self,
-        api_name: str = None,
-        ability_info_list: List[AbilityInfo] = None,
-    ):
-        # api名称
-        self.api_name = api_name
-        # 能力列表
-        self.ability_info_list = ability_info_list
-
-    def validate(self):
-        self.validate_required(self.api_name, 'api_name')
-        self.validate_required(self.ability_info_list, 'ability_info_list')
-        if self.ability_info_list:
-            for k in self.ability_info_list:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.api_name is not None:
-            result['api_name'] = self.api_name
-        result['ability_info_list'] = []
-        if self.ability_info_list is not None:
-            for k in self.ability_info_list:
-                result['ability_info_list'].append(k.to_map() if k else None)
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('api_name') is not None:
-            self.api_name = m.get('api_name')
-        self.ability_info_list = []
-        if m.get('ability_info_list') is not None:
-            for k in m.get('ability_info_list'):
-                temp_model = AbilityInfo()
-                self.ability_info_list.append(temp_model.from_map(k))
-        return self
-
-
-class ApiInfo(TeaModel):
-    def __init__(
-        self,
-        api_code: str = None,
-        api_protobuf_definition: str = None,
-    ):
-        # 查询不动产接口
-        self.api_code = api_code
-        # api pb文件定义
-        self.api_protobuf_definition = api_protobuf_definition
-
-    def validate(self):
-        self.validate_required(self.api_code, 'api_code')
-        self.validate_required(self.api_protobuf_definition, 'api_protobuf_definition')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.api_code is not None:
-            result['api_code'] = self.api_code
-        if self.api_protobuf_definition is not None:
-            result['api_protobuf_definition'] = self.api_protobuf_definition
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('api_code') is not None:
-            self.api_code = m.get('api_code')
-        if m.get('api_protobuf_definition') is not None:
-            self.api_protobuf_definition = m.get('api_protobuf_definition')
-        return self
-
-
-class PublishDemoSaasTestTestcRequest(TeaModel):
-    def __init__(
-        self,
-        auth_token: str = None,
-        product_instance_id: str = None,
         name: str = None,
-        age: int = None,
+        value: str = None,
     ):
-        # OAuth模式下的授权token
-        self.auth_token = auth_token
-        self.product_instance_id = product_instance_id
-        # 张三
+        # 键名
         self.name = name
-        # 14
-        self.age = age
+        # 键值
+        self.value = value
 
     def validate(self):
         self.validate_required(self.name, 'name')
-        self.validate_required(self.age, 'age')
+        self.validate_required(self.value, 'value')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.auth_token is not None:
-            result['auth_token'] = self.auth_token
-        if self.product_instance_id is not None:
-            result['product_instance_id'] = self.product_instance_id
         if self.name is not None:
             result['name'] = self.name
-        if self.age is not None:
-            result['age'] = self.age
+        if self.value is not None:
+            result['value'] = self.value
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('auth_token') is not None:
-            self.auth_token = m.get('auth_token')
-        if m.get('product_instance_id') is not None:
-            self.product_instance_id = m.get('product_instance_id')
         if m.get('name') is not None:
             self.name = m.get('name')
-        if m.get('age') is not None:
-            self.age = m.get('age')
+        if m.get('value') is not None:
+            self.value = m.get('value')
         return self
 
 
-class PublishDemoSaasTestTestcResponse(TeaModel):
+class QueryMap(TeaModel):
     def __init__(
         self,
-        req_msg_id: str = None,
-        result_code: str = None,
-        result_msg: str = None,
-        sex: str = None,
-    ):
-        # 请求唯一ID，用于链路跟踪和问题排查
-        self.req_msg_id = req_msg_id
-        # 结果码，一般OK表示调用成功
-        self.result_code = result_code
-        # 异常信息的文本描述
-        self.result_msg = result_msg
-        # 男
-        self.sex = sex
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
-        if self.sex is not None:
-            result['sex'] = self.sex
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
-        if m.get('sex') is not None:
-            self.sex = m.get('sex')
-        return self
-
-
-class BindAntchainSaasAbilityRequest(TeaModel):
-    def __init__(
-        self,
-        auth_token: str = None,
-        product_instance_id: str = None,
-        api_name: str = None,
-        ability_ids: List[str] = None,
-        operator_id: str = None,
-        api_info_model: ApiInfoModel = None,
-    ):
-        # OAuth模式下的授权token
-        self.auth_token = auth_token
-        self.product_instance_id = product_instance_id
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
-        if self.api_name is not None:
-            result['api_name'] = self.api_name
-        if self.ability_ids is not None:
-            result['ability_ids'] = self.ability_ids
-        if self.operator_id is not None:
-            result['operator_id'] = self.operator_id
-        if self.api_info_model is not None:
-            result['api_info_model'] = self.api_info_model.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('auth_token') is not None:
-            self.auth_token = m.get('auth_token')
-        if m.get('product_instance_id') is not None:
-            self.product_instance_id = m.get('product_instance_id')
-        if m.get('api_name') is not None:
-            self.api_name = m.get('api_name')
-        if m.get('ability_ids') is not None:
-            self.ability_ids = m.get('ability_ids')
-        if m.get('operator_id') is not None:
-            self.operator_id = m.get('operator_id')
-        if m.get('api_info_model') is not None:
-            temp_model = ApiInfoModel()
-            self.api_info_model = temp_model.from_map(m['api_info_model'])
-        return self
-
-
-class BindAntchainSaasAbilityResponse(TeaModel):
-    def __init__(
-        self,
-        req_msg_id: str = None,
-        result_code: str = None,
-        result_msg: str = None,
+        name: str = None,
+        value: List[NameValuePair] = None,
     ):
-        # 请求唯一ID，用于链路跟踪和问题排查
-        self.req_msg_id = req_msg_id
-        # 结果码，一般OK表示调用成功
-        self.result_code = result_code
-        # 异常信息的文本描述
-        self.result_msg = result_msg
+        # 键值
+        self.name = name
+        # 额外用户信息
+        self.value = value
 
     def validate(self):
-        pass
+        self.validate_required(self.name, 'name')
+        if self.value:
+            for k in self.value:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.req_msg_id is not None:
-            result['req_msg_id'] = self.req_msg_id
-        if self.result_code is not None:
-            result['result_code'] = self.result_code
-        if self.result_msg is not None:
-            result['result_msg'] = self.result_msg
+        if self.name is not None:
+            result['name'] = self.name
+        result['value'] = []
+        if self.value is not None:
+            for k in self.value:
+                result['value'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('req_msg_id') is not None:
-            self.req_msg_id = m.get('req_msg_id')
-        if m.get('result_code') is not None:
-            self.result_code = m.get('result_code')
-        if m.get('result_msg') is not None:
-            self.result_msg = m.get('result_msg')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        self.value = []
+        if m.get('value') is not None:
+            for k in m.get('value'):
+                temp_model = NameValuePair()
+                self.value.append(temp_model.from_map(k))
         return self
 
 
-class QueryAntchainSaasAbilityWithapinameRequest(TeaModel):
+class InitDemoBbpInsuranceUserRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        api_name_list: List[str] = None,
+        business_code: str = None,
+        third_part_id: str = None,
+        channel: str = None,
+        burieds: QueryMap = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # api名称列表
-        self.api_name_list = api_name_list
+        # 保司编码
+        self.business_code = business_code
+        # 第三方id，此处为天猫uid
+        self.third_part_id = third_part_id
+        # 来源渠道
+        self.channel = channel
+        # 埋点信息
+        self.burieds = burieds
 
     def validate(self):
-        self.validate_required(self.api_name_list, 'api_name_list')
+        self.validate_required(self.business_code, 'business_code')
+        self.validate_required(self.third_part_id, 'third_part_id')
+        self.validate_required(self.channel, 'channel')
+        if self.burieds:
+            self.burieds.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.api_name_list is not None:
-            result['api_name_list'] = self.api_name_list
+        if self.business_code is not None:
+            result['business_code'] = self.business_code
+        if self.third_part_id is not None:
+            result['third_part_id'] = self.third_part_id
+        if self.channel is not None:
+            result['channel'] = self.channel
+        if self.burieds is not None:
+            result['burieds'] = self.burieds.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('api_name_list') is not None:
-            self.api_name_list = m.get('api_name_list')
+        if m.get('business_code') is not None:
+            self.business_code = m.get('business_code')
+        if m.get('third_part_id') is not None:
+            self.third_part_id = m.get('third_part_id')
+        if m.get('channel') is not None:
+            self.channel = m.get('channel')
+        if m.get('burieds') is not None:
+            temp_model = QueryMap()
+            self.burieds = temp_model.from_map(m['burieds'])
         return self
 
 
-class QueryAntchainSaasAbilityWithapinameResponse(TeaModel):
+class InitDemoBbpInsuranceUserResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
-        ability_api_relation_list: List[AbilityApiRelation] = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
-        # api与能力信息关联列表
-        self.ability_api_relation_list = ability_api_relation_list
 
     def validate(self):
-        if self.ability_api_relation_list:
-            for k in self.ability_api_relation_list:
-                if k:
-                    k.validate()
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
-        result['ability_api_relation_list'] = []
-        if self.ability_api_relation_list is not None:
-            for k in self.ability_api_relation_list:
-                result['ability_api_relation_list'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
-        self.ability_api_relation_list = []
-        if m.get('ability_api_relation_list') is not None:
-            for k in m.get('ability_api_relation_list'):
-                temp_model = AbilityApiRelation()
-                self.ability_api_relation_list.append(temp_model.from_map(k))
         return self
 
 
-class BindDemoCenterAbilityRequest(TeaModel):
+class QueryDemoAdAsdAsdRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
@@ -739,15 +373,15 @@
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
         return self
 
 
-class BindDemoCenterAbilityResponse(TeaModel):
+class QueryDemoAdAsdAsdResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
@@ -781,15 +415,15 @@
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         return self
 
 
-class BindDemoMoreAbilityTestabcRequest(TeaModel):
+class BindDemoAsdAsdAsdRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
@@ -815,15 +449,15 @@
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
         return self
 
 
-class BindDemoMoreAbilityTestabcResponse(TeaModel):
+class BindDemoAsdAsdAsdResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
@@ -857,56 +491,49 @@
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         return self
 
 
-class CallbackAntchainSaasAbilityRequest(TeaModel):
+class BindDemoCenterAbilityRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        api_names: List[str] = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # api名称集合
-        self.api_names = api_names
 
     def validate(self):
-        self.validate_required(self.api_names, 'api_names')
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
-        if self.api_names is not None:
-            result['api_names'] = self.api_names
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('api_names') is not None:
-            self.api_names = m.get('api_names')
         return self
 
 
-class CallbackAntchainSaasAbilityResponse(TeaModel):
+class BindDemoCenterAbilityResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
@@ -940,162 +567,139 @@
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         return self
 
 
-class QueryAntchainSaasFoundationProtobufRequest(TeaModel):
+class QueryDemoApprovalTestRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        product_code: str = None,
-        api_code_list: List[str] = None,
+        input: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 产品码
-        self.product_code = product_code
-        # api code列表信息
-        self.api_code_list = api_code_list
+        # 字符串
+        self.input = input
 
     def validate(self):
-        self.validate_required(self.product_code, 'product_code')
-        self.validate_required(self.api_code_list, 'api_code_list')
+        self.validate_required(self.input, 'input')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.product_code is not None:
-            result['product_code'] = self.product_code
-        if self.api_code_list is not None:
-            result['api_code_list'] = self.api_code_list
+        if self.input is not None:
+            result['input'] = self.input
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('product_code') is not None:
-            self.product_code = m.get('product_code')
-        if m.get('api_code_list') is not None:
-            self.api_code_list = m.get('api_code_list')
+        if m.get('input') is not None:
+            self.input = m.get('input')
         return self
 
 
-class QueryAntchainSaasFoundationProtobufResponse(TeaModel):
+class QueryDemoApprovalTestResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
-        api_info_list: List[ApiInfo] = None,
+        msg: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
-        # api probuf信息
-        self.api_info_list = api_info_list
+        # 回参
+        self.msg = msg
 
     def validate(self):
-        if self.api_info_list:
-            for k in self.api_info_list:
-                if k:
-                    k.validate()
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
-        result['api_info_list'] = []
-        if self.api_info_list is not None:
-            for k in self.api_info_list:
-                result['api_info_list'].append(k.to_map() if k else None)
+        if self.msg is not None:
+            result['msg'] = self.msg
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
-        self.api_info_list = []
-        if m.get('api_info_list') is not None:
-            for k in m.get('api_info_list'):
-                temp_model = ApiInfo()
-                self.api_info_list.append(temp_model.from_map(k))
+        if m.get('msg') is not None:
+            self.msg = m.get('msg')
         return self
 
 
-class QueryAntchainSaasAbilityResultcodeRequest(TeaModel):
+class InitDemoCjtestAcopmResRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        index: int = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 1-INTERNAL_ERROR，2-TOO_MANY_REQUESTS，3-UNKNOW_ERROR，4-ACCESS_DENIED，5-OK，6-CUSTOM_RESULT_CODE_ONE，7-CUSTOM_RESULT_CODE_TWO
-        self.index = index
 
     def validate(self):
-        self.validate_required(self.index, 'index')
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
-        if self.index is not None:
-            result['index'] = self.index
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('index') is not None:
-            self.index = m.get('index')
         return self
 
 
-class QueryAntchainSaasAbilityResultcodeResponse(TeaModel):
+class InitDemoCjtestAcopmResResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
```

### Comparing `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.5/setup.py` & `antchain_ak_68b3ee3230284cddaa19740dcaf251d8-1.0.6/setup.py`

 * *Files identical despite different names*

