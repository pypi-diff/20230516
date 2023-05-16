# Comparing `tmp/alibabacloud_computenestsupplier20210521_py2-1.1.2.tar.gz` & `tmp/alibabacloud_computenestsupplier20210521_py2-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_computenestsupplier20210521_py2-1.1.2.tar", last modified: Mon Feb  6 08:12:33 2023, max compression
+gzip compressed data, was "dist/alibabacloud_computenestsupplier20210521_py2-1.1.3.tar", last modified: Tue May 16 09:56:51 2023, max compression
```

## Comparing `alibabacloud_computenestsupplier20210521_py2-1.1.2.tar` & `alibabacloud_computenestsupplier20210521_py2-1.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:12:33.000000 alibabacloud_computenestsupplier20210521_py2-1.1.2/
--rw-r--r--   0 root         (0) root         (0)      195 2023-02-06 08:12:33.000000 alibabacloud_computenestsupplier20210521_py2-1.1.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-02-06 08:12:33.000000 alibabacloud_computenestsupplier20210521_py2-1.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-02-06 08:12:33.000000 alibabacloud_computenestsupplier20210521_py2-1.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2568 2023-02-06 08:12:33.000000 alibabacloud_computenestsupplier20210521_py2-1.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1081 2023-02-06 08:12:33.000000 alibabacloud_computenestsupplier20210521_py2-1.1.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1164 2023-02-06 08:12:33.000000 alibabacloud_computenestsupplier20210521_py2-1.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:12:33.000000 alibabacloud_computenestsupplier20210521_py2-1.1.2/alibabacloud_computenestsupplier20210521/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-06 08:12:33.000000 alibabacloud_computenestsupplier20210521_py2-1.1.2/alibabacloud_computenestsupplier20210521/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15975 2023-02-06 08:12:33.000000 alibabacloud_computenestsupplier20210521_py2-1.1.2/alibabacloud_computenestsupplier20210521/client.py
--rw-r--r--   0 root         (0) root         (0)   116957 2023-02-06 08:12:33.000000 alibabacloud_computenestsupplier20210521_py2-1.1.2/alibabacloud_computenestsupplier20210521/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:12:33.000000 alibabacloud_computenestsupplier20210521_py2-1.1.2/alibabacloud_computenestsupplier20210521_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2568 2023-02-06 08:12:33.000000 alibabacloud_computenestsupplier20210521_py2-1.1.2/alibabacloud_computenestsupplier20210521_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      568 2023-02-06 08:12:33.000000 alibabacloud_computenestsupplier20210521_py2-1.1.2/alibabacloud_computenestsupplier20210521_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-06 08:12:33.000000 alibabacloud_computenestsupplier20210521_py2-1.1.2/alibabacloud_computenestsupplier20210521_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-02-06 08:12:33.000000 alibabacloud_computenestsupplier20210521_py2-1.1.2/alibabacloud_computenestsupplier20210521_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-02-06 08:12:33.000000 alibabacloud_computenestsupplier20210521_py2-1.1.2/alibabacloud_computenestsupplier20210521_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-02-06 08:12:33.000000 alibabacloud_computenestsupplier20210521_py2-1.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2983 2023-02-06 08:12:33.000000 alibabacloud_computenestsupplier20210521_py2-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:56:51.000000 alibabacloud_computenestsupplier20210521_py2-1.1.3/
+-rw-r--r--   0 root         (0) root         (0)      259 2023-05-16 09:56:51.000000 alibabacloud_computenestsupplier20210521_py2-1.1.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-16 09:56:51.000000 alibabacloud_computenestsupplier20210521_py2-1.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-16 09:56:51.000000 alibabacloud_computenestsupplier20210521_py2-1.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2568 2023-05-16 09:56:51.000000 alibabacloud_computenestsupplier20210521_py2-1.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-05-16 09:56:51.000000 alibabacloud_computenestsupplier20210521_py2-1.1.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1164 2023-05-16 09:56:51.000000 alibabacloud_computenestsupplier20210521_py2-1.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:56:51.000000 alibabacloud_computenestsupplier20210521_py2-1.1.3/alibabacloud_computenestsupplier20210521/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 09:56:51.000000 alibabacloud_computenestsupplier20210521_py2-1.1.3/alibabacloud_computenestsupplier20210521/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23095 2023-05-16 09:56:51.000000 alibabacloud_computenestsupplier20210521_py2-1.1.3/alibabacloud_computenestsupplier20210521/client.py
+-rw-r--r--   0 root         (0) root         (0)   155301 2023-05-16 09:56:51.000000 alibabacloud_computenestsupplier20210521_py2-1.1.3/alibabacloud_computenestsupplier20210521/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:56:51.000000 alibabacloud_computenestsupplier20210521_py2-1.1.3/alibabacloud_computenestsupplier20210521_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2568 2023-05-16 09:56:51.000000 alibabacloud_computenestsupplier20210521_py2-1.1.3/alibabacloud_computenestsupplier20210521_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      568 2023-05-16 09:56:51.000000 alibabacloud_computenestsupplier20210521_py2-1.1.3/alibabacloud_computenestsupplier20210521_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 09:56:51.000000 alibabacloud_computenestsupplier20210521_py2-1.1.3/alibabacloud_computenestsupplier20210521_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-16 09:56:51.000000 alibabacloud_computenestsupplier20210521_py2-1.1.3/alibabacloud_computenestsupplier20210521_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-05-16 09:56:51.000000 alibabacloud_computenestsupplier20210521_py2-1.1.3/alibabacloud_computenestsupplier20210521_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 09:56:51.000000 alibabacloud_computenestsupplier20210521_py2-1.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2983 2023-05-16 09:56:51.000000 alibabacloud_computenestsupplier20210521_py2-1.1.3/setup.py
```

### Comparing `alibabacloud_computenestsupplier20210521_py2-1.1.2/LICENSE` & `alibabacloud_computenestsupplier20210521_py2-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_computenestsupplier20210521_py2-1.1.2/PKG-INFO` & `alibabacloud_computenestsupplier20210521_py2-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_computenestsupplier20210521_py2
-Version: 1.1.2
+Version: 1.1.3
 Summary: Alibaba Cloud ComputeNestSupplier (20210521) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_computenestsupplier20210521_py2-1.1.2/README-CN.md` & `alibabacloud_computenestsupplier20210521_py2-1.1.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_computenestsupplier20210521_py2-1.1.2/README.md` & `alibabacloud_computenestsupplier20210521_py2-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_computenestsupplier20210521_py2-1.1.2/alibabacloud_computenestsupplier20210521/client.py` & `alibabacloud_computenestsupplier20210521_py2-1.1.3/alibabacloud_computenestsupplier20210521/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -70,14 +70,82 @@
             self.call_api(params, req, runtime)
         )
 
     def create_artifact(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_artifact_with_options(request, runtime)
 
+    def create_service_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.alarm_metadata):
+            query['AlarmMetadata'] = request.alarm_metadata
+        if not UtilClient.is_unset(request.approval_type):
+            query['ApprovalType'] = request.approval_type
+        if not UtilClient.is_unset(request.client_token):
+            query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.deploy_metadata):
+            query['DeployMetadata'] = request.deploy_metadata
+        if not UtilClient.is_unset(request.deploy_type):
+            query['DeployType'] = request.deploy_type
+        if not UtilClient.is_unset(request.duration):
+            query['Duration'] = request.duration
+        if not UtilClient.is_unset(request.is_support_operated):
+            query['IsSupportOperated'] = request.is_support_operated
+        if not UtilClient.is_unset(request.license_metadata):
+            query['LicenseMetadata'] = request.license_metadata
+        if not UtilClient.is_unset(request.operation_metadata):
+            query['OperationMetadata'] = request.operation_metadata
+        if not UtilClient.is_unset(request.policy_names):
+            query['PolicyNames'] = request.policy_names
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.service_id):
+            query['ServiceId'] = request.service_id
+        if not UtilClient.is_unset(request.service_info):
+            query['ServiceInfo'] = request.service_info
+        if not UtilClient.is_unset(request.service_type):
+            query['ServiceType'] = request.service_type
+        if not UtilClient.is_unset(request.share_type):
+            query['ShareType'] = request.share_type
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
+        if not UtilClient.is_unset(request.tenant_type):
+            query['TenantType'] = request.tenant_type
+        if not UtilClient.is_unset(request.trial_duration):
+            query['TrialDuration'] = request.trial_duration
+        if not UtilClient.is_unset(request.upgrade_metadata):
+            query['UpgradeMetadata'] = request.upgrade_metadata
+        if not UtilClient.is_unset(request.version_name):
+            query['VersionName'] = request.version_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateService',
+            version='2021-05-21',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            compute_nest_supplier_20210521_models.CreateServiceResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def create_service(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.create_service_with_options(request, runtime)
+
     def delete_artifact_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.artifact_id):
             query['ArtifactId'] = request.artifact_id
         if not UtilClient.is_unset(request.artifact_version):
             query['ArtifactVersion'] = request.artifact_version
@@ -160,14 +228,58 @@
             self.call_api(params, req, runtime)
         )
 
     def get_artifact_repository_credentials(self, request):
         runtime = util_models.RuntimeOptions()
         return self.get_artifact_repository_credentials_with_options(request, runtime)
 
+    def get_service_estimate_cost_with_options(self, tmp_req, runtime):
+        UtilClient.validate_model(tmp_req)
+        request = compute_nest_supplier_20210521_models.GetServiceEstimateCostShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.parameters):
+            request.parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.parameters, 'Parameters', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.client_token):
+            query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.parameters_shrink):
+            query['Parameters'] = request.parameters_shrink
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.service_id):
+            query['ServiceId'] = request.service_id
+        if not UtilClient.is_unset(request.service_instance_id):
+            query['ServiceInstanceId'] = request.service_instance_id
+        if not UtilClient.is_unset(request.service_version):
+            query['ServiceVersion'] = request.service_version
+        if not UtilClient.is_unset(request.template_name):
+            query['TemplateName'] = request.template_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetServiceEstimateCost',
+            version='2021-05-21',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            compute_nest_supplier_20210521_models.GetServiceEstimateCostResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def get_service_estimate_cost(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.get_service_estimate_cost_with_options(request, runtime)
+
     def get_service_instance_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.service_instance_id):
             query['ServiceInstanceId'] = request.service_instance_id
@@ -265,14 +377,16 @@
             query['Filter'] = request.filter
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.show_deleted):
+            query['ShowDeleted'] = request.show_deleted
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListServiceInstances',
@@ -322,14 +436,54 @@
             self.call_api(params, req, runtime)
         )
 
     def list_service_usages(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_service_usages_with_options(request, runtime)
 
+    def list_services_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.all_versions):
+            query['AllVersions'] = request.all_versions
+        if not UtilClient.is_unset(request.filter):
+            query['Filter'] = request.filter
+        if not UtilClient.is_unset(request.max_results):
+            query['MaxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListServices',
+            version='2021-05-21',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            compute_nest_supplier_20210521_models.ListServicesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def list_services(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_services_with_options(request, runtime)
+
     def release_artifact_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.artifact_id):
             query['ArtifactId'] = request.artifact_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
```

### Comparing `alibabacloud_computenestsupplier20210521_py2-1.1.2/alibabacloud_computenestsupplier20210521/models.py` & `alibabacloud_computenestsupplier20210521_py2-1.1.3/alibabacloud_computenestsupplier20210521/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -286,14 +286,305 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateArtifactResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateServiceRequestServiceInfo(TeaModel):
+    def __init__(self, image=None, locale=None, name=None, short_description=None):
+        self.image = image  # type: str
+        self.locale = locale  # type: str
+        self.name = name  # type: str
+        self.short_description = short_description  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateServiceRequestServiceInfo, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.image is not None:
+            result['Image'] = self.image
+        if self.locale is not None:
+            result['Locale'] = self.locale
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.short_description is not None:
+            result['ShortDescription'] = self.short_description
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Image') is not None:
+            self.image = m.get('Image')
+        if m.get('Locale') is not None:
+            self.locale = m.get('Locale')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('ShortDescription') is not None:
+            self.short_description = m.get('ShortDescription')
+        return self
+
+
+class CreateServiceRequestTag(TeaModel):
+    def __init__(self, key=None, value=None):
+        self.key = key  # type: str
+        self.value = value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateServiceRequestTag, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class CreateServiceRequest(TeaModel):
+    def __init__(self, alarm_metadata=None, approval_type=None, client_token=None, deploy_metadata=None,
+                 deploy_type=None, duration=None, is_support_operated=None, license_metadata=None, operation_metadata=None,
+                 policy_names=None, region_id=None, resource_group_id=None, service_id=None, service_info=None,
+                 service_type=None, share_type=None, tag=None, tenant_type=None, trial_duration=None, upgrade_metadata=None,
+                 version_name=None):
+        self.alarm_metadata = alarm_metadata  # type: str
+        self.approval_type = approval_type  # type: str
+        self.client_token = client_token  # type: str
+        self.deploy_metadata = deploy_metadata  # type: str
+        self.deploy_type = deploy_type  # type: str
+        self.duration = duration  # type: long
+        self.is_support_operated = is_support_operated  # type: bool
+        self.license_metadata = license_metadata  # type: str
+        self.operation_metadata = operation_metadata  # type: str
+        self.policy_names = policy_names  # type: str
+        self.region_id = region_id  # type: str
+        self.resource_group_id = resource_group_id  # type: str
+        self.service_id = service_id  # type: str
+        self.service_info = service_info  # type: list[CreateServiceRequestServiceInfo]
+        self.service_type = service_type  # type: str
+        self.share_type = share_type  # type: str
+        self.tag = tag  # type: list[CreateServiceRequestTag]
+        self.tenant_type = tenant_type  # type: str
+        self.trial_duration = trial_duration  # type: long
+        self.upgrade_metadata = upgrade_metadata  # type: str
+        self.version_name = version_name  # type: str
+
+    def validate(self):
+        if self.service_info:
+            for k in self.service_info:
+                if k:
+                    k.validate()
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(CreateServiceRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.alarm_metadata is not None:
+            result['AlarmMetadata'] = self.alarm_metadata
+        if self.approval_type is not None:
+            result['ApprovalType'] = self.approval_type
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        if self.deploy_metadata is not None:
+            result['DeployMetadata'] = self.deploy_metadata
+        if self.deploy_type is not None:
+            result['DeployType'] = self.deploy_type
+        if self.duration is not None:
+            result['Duration'] = self.duration
+        if self.is_support_operated is not None:
+            result['IsSupportOperated'] = self.is_support_operated
+        if self.license_metadata is not None:
+            result['LicenseMetadata'] = self.license_metadata
+        if self.operation_metadata is not None:
+            result['OperationMetadata'] = self.operation_metadata
+        if self.policy_names is not None:
+            result['PolicyNames'] = self.policy_names
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
+        if self.service_id is not None:
+            result['ServiceId'] = self.service_id
+        result['ServiceInfo'] = []
+        if self.service_info is not None:
+            for k in self.service_info:
+                result['ServiceInfo'].append(k.to_map() if k else None)
+        if self.service_type is not None:
+            result['ServiceType'] = self.service_type
+        if self.share_type is not None:
+            result['ShareType'] = self.share_type
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
+        if self.tenant_type is not None:
+            result['TenantType'] = self.tenant_type
+        if self.trial_duration is not None:
+            result['TrialDuration'] = self.trial_duration
+        if self.upgrade_metadata is not None:
+            result['UpgradeMetadata'] = self.upgrade_metadata
+        if self.version_name is not None:
+            result['VersionName'] = self.version_name
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AlarmMetadata') is not None:
+            self.alarm_metadata = m.get('AlarmMetadata')
+        if m.get('ApprovalType') is not None:
+            self.approval_type = m.get('ApprovalType')
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        if m.get('DeployMetadata') is not None:
+            self.deploy_metadata = m.get('DeployMetadata')
+        if m.get('DeployType') is not None:
+            self.deploy_type = m.get('DeployType')
+        if m.get('Duration') is not None:
+            self.duration = m.get('Duration')
+        if m.get('IsSupportOperated') is not None:
+            self.is_support_operated = m.get('IsSupportOperated')
+        if m.get('LicenseMetadata') is not None:
+            self.license_metadata = m.get('LicenseMetadata')
+        if m.get('OperationMetadata') is not None:
+            self.operation_metadata = m.get('OperationMetadata')
+        if m.get('PolicyNames') is not None:
+            self.policy_names = m.get('PolicyNames')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
+        if m.get('ServiceId') is not None:
+            self.service_id = m.get('ServiceId')
+        self.service_info = []
+        if m.get('ServiceInfo') is not None:
+            for k in m.get('ServiceInfo'):
+                temp_model = CreateServiceRequestServiceInfo()
+                self.service_info.append(temp_model.from_map(k))
+        if m.get('ServiceType') is not None:
+            self.service_type = m.get('ServiceType')
+        if m.get('ShareType') is not None:
+            self.share_type = m.get('ShareType')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = CreateServiceRequestTag()
+                self.tag.append(temp_model.from_map(k))
+        if m.get('TenantType') is not None:
+            self.tenant_type = m.get('TenantType')
+        if m.get('TrialDuration') is not None:
+            self.trial_duration = m.get('TrialDuration')
+        if m.get('UpgradeMetadata') is not None:
+            self.upgrade_metadata = m.get('UpgradeMetadata')
+        if m.get('VersionName') is not None:
+            self.version_name = m.get('VersionName')
+        return self
+
+
+class CreateServiceResponseBody(TeaModel):
+    def __init__(self, request_id=None, service_id=None, status=None, version=None):
+        self.request_id = request_id  # type: str
+        self.service_id = service_id  # type: str
+        self.status = status  # type: str
+        self.version = version  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateServiceResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.service_id is not None:
+            result['ServiceId'] = self.service_id
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.version is not None:
+            result['Version'] = self.version
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('ServiceId') is not None:
+            self.service_id = m.get('ServiceId')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('Version') is not None:
+            self.version = m.get('Version')
+        return self
+
+
+class CreateServiceResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: CreateServiceResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(CreateServiceResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateServiceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteArtifactRequest(TeaModel):
     def __init__(self, artifact_id=None, artifact_version=None):
         self.artifact_id = artifact_id  # type: str
         self.artifact_version = artifact_version  # type: str
 
     def validate(self):
         pass
@@ -729,14 +1020,192 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetArtifactRepositoryCredentialsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetServiceEstimateCostRequest(TeaModel):
+    def __init__(self, client_token=None, parameters=None, region_id=None, service_id=None,
+                 service_instance_id=None, service_version=None, template_name=None):
+        self.client_token = client_token  # type: str
+        self.parameters = parameters  # type: dict[str, any]
+        self.region_id = region_id  # type: str
+        self.service_id = service_id  # type: str
+        self.service_instance_id = service_instance_id  # type: str
+        self.service_version = service_version  # type: str
+        self.template_name = template_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetServiceEstimateCostRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        if self.parameters is not None:
+            result['Parameters'] = self.parameters
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.service_id is not None:
+            result['ServiceId'] = self.service_id
+        if self.service_instance_id is not None:
+            result['ServiceInstanceId'] = self.service_instance_id
+        if self.service_version is not None:
+            result['ServiceVersion'] = self.service_version
+        if self.template_name is not None:
+            result['TemplateName'] = self.template_name
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        if m.get('Parameters') is not None:
+            self.parameters = m.get('Parameters')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ServiceId') is not None:
+            self.service_id = m.get('ServiceId')
+        if m.get('ServiceInstanceId') is not None:
+            self.service_instance_id = m.get('ServiceInstanceId')
+        if m.get('ServiceVersion') is not None:
+            self.service_version = m.get('ServiceVersion')
+        if m.get('TemplateName') is not None:
+            self.template_name = m.get('TemplateName')
+        return self
+
+
+class GetServiceEstimateCostShrinkRequest(TeaModel):
+    def __init__(self, client_token=None, parameters_shrink=None, region_id=None, service_id=None,
+                 service_instance_id=None, service_version=None, template_name=None):
+        self.client_token = client_token  # type: str
+        self.parameters_shrink = parameters_shrink  # type: str
+        self.region_id = region_id  # type: str
+        self.service_id = service_id  # type: str
+        self.service_instance_id = service_instance_id  # type: str
+        self.service_version = service_version  # type: str
+        self.template_name = template_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetServiceEstimateCostShrinkRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        if self.parameters_shrink is not None:
+            result['Parameters'] = self.parameters_shrink
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.service_id is not None:
+            result['ServiceId'] = self.service_id
+        if self.service_instance_id is not None:
+            result['ServiceInstanceId'] = self.service_instance_id
+        if self.service_version is not None:
+            result['ServiceVersion'] = self.service_version
+        if self.template_name is not None:
+            result['TemplateName'] = self.template_name
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        if m.get('Parameters') is not None:
+            self.parameters_shrink = m.get('Parameters')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ServiceId') is not None:
+            self.service_id = m.get('ServiceId')
+        if m.get('ServiceInstanceId') is not None:
+            self.service_instance_id = m.get('ServiceInstanceId')
+        if m.get('ServiceVersion') is not None:
+            self.service_version = m.get('ServiceVersion')
+        if m.get('TemplateName') is not None:
+            self.template_name = m.get('TemplateName')
+        return self
+
+
+class GetServiceEstimateCostResponseBody(TeaModel):
+    def __init__(self, request_id=None, resources=None):
+        self.request_id = request_id  # type: str
+        self.resources = resources  # type: dict[str, any]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetServiceEstimateCostResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.resources is not None:
+            result['Resources'] = self.resources
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Resources') is not None:
+            self.resources = m.get('Resources')
+        return self
+
+
+class GetServiceEstimateCostResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetServiceEstimateCostResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GetServiceEstimateCostResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetServiceEstimateCostResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetServiceInstanceRequest(TeaModel):
     def __init__(self, region_id=None, service_instance_id=None):
         self.region_id = region_id  # type: str
         self.service_instance_id = service_instance_id  # type: str
 
     def validate(self):
         pass
@@ -759,16 +1228,18 @@
             self.region_id = m.get('RegionId')
         if m.get('ServiceInstanceId') is not None:
             self.service_instance_id = m.get('ServiceInstanceId')
         return self
 
 
 class GetServiceInstanceResponseBodyNetworkConfigPrivateVpcConnectionsConnectionConfigs(TeaModel):
-    def __init__(self, endpoint_ips=None, ingress_endpoint_status=None, network_service_status=None,
-                 security_groups=None, v_switches=None, vpc_id=None):
+    def __init__(self, connect_bandwidth=None, domain_name=None, endpoint_ips=None, ingress_endpoint_status=None,
+                 network_service_status=None, security_groups=None, v_switches=None, vpc_id=None):
+        self.connect_bandwidth = connect_bandwidth  # type: int
+        self.domain_name = domain_name  # type: str
         self.endpoint_ips = endpoint_ips  # type: list[str]
         self.ingress_endpoint_status = ingress_endpoint_status  # type: str
         self.network_service_status = network_service_status  # type: str
         self.security_groups = security_groups  # type: list[str]
         self.v_switches = v_switches  # type: list[str]
         self.vpc_id = vpc_id  # type: str
 
@@ -777,14 +1248,18 @@
 
     def to_map(self):
         _map = super(GetServiceInstanceResponseBodyNetworkConfigPrivateVpcConnectionsConnectionConfigs, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.connect_bandwidth is not None:
+            result['ConnectBandwidth'] = self.connect_bandwidth
+        if self.domain_name is not None:
+            result['DomainName'] = self.domain_name
         if self.endpoint_ips is not None:
             result['EndpointIps'] = self.endpoint_ips
         if self.ingress_endpoint_status is not None:
             result['IngressEndpointStatus'] = self.ingress_endpoint_status
         if self.network_service_status is not None:
             result['NetworkServiceStatus'] = self.network_service_status
         if self.security_groups is not None:
@@ -793,14 +1268,18 @@
             result['VSwitches'] = self.v_switches
         if self.vpc_id is not None:
             result['VpcId'] = self.vpc_id
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('ConnectBandwidth') is not None:
+            self.connect_bandwidth = m.get('ConnectBandwidth')
+        if m.get('DomainName') is not None:
+            self.domain_name = m.get('DomainName')
         if m.get('EndpointIps') is not None:
             self.endpoint_ips = m.get('EndpointIps')
         if m.get('IngressEndpointStatus') is not None:
             self.ingress_endpoint_status = m.get('IngressEndpointStatus')
         if m.get('NetworkServiceStatus') is not None:
             self.network_service_status = m.get('NetworkServiceStatus')
         if m.get('SecurityGroups') is not None:
@@ -983,26 +1462,27 @@
             self.short_description = m.get('ShortDescription')
         return self
 
 
 class GetServiceInstanceResponseBodyService(TeaModel):
     def __init__(self, deploy_metadata=None, deploy_type=None, publish_time=None, service_doc_url=None,
                  service_id=None, service_infos=None, service_product_url=None, service_type=None, status=None,
-                 supplier_name=None, supplier_url=None, version=None, version_name=None):
+                 supplier_name=None, supplier_url=None, upgradable_service_versions=None, version=None, version_name=None):
         self.deploy_metadata = deploy_metadata  # type: str
         self.deploy_type = deploy_type  # type: str
         self.publish_time = publish_time  # type: str
         self.service_doc_url = service_doc_url  # type: str
         self.service_id = service_id  # type: str
         self.service_infos = service_infos  # type: list[GetServiceInstanceResponseBodyServiceServiceInfos]
         self.service_product_url = service_product_url  # type: str
         self.service_type = service_type  # type: str
         self.status = status  # type: str
         self.supplier_name = supplier_name  # type: str
         self.supplier_url = supplier_url  # type: str
+        self.upgradable_service_versions = upgradable_service_versions  # type: list[str]
         self.version = version  # type: str
         self.version_name = version_name  # type: str
 
     def validate(self):
         if self.service_infos:
             for k in self.service_infos:
                 if k:
@@ -1034,14 +1514,16 @@
             result['ServiceType'] = self.service_type
         if self.status is not None:
             result['Status'] = self.status
         if self.supplier_name is not None:
             result['SupplierName'] = self.supplier_name
         if self.supplier_url is not None:
             result['SupplierUrl'] = self.supplier_url
+        if self.upgradable_service_versions is not None:
+            result['UpgradableServiceVersions'] = self.upgradable_service_versions
         if self.version is not None:
             result['Version'] = self.version
         if self.version_name is not None:
             result['VersionName'] = self.version_name
         return result
 
     def from_map(self, m=None):
@@ -1067,14 +1549,16 @@
             self.service_type = m.get('ServiceType')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('SupplierName') is not None:
             self.supplier_name = m.get('SupplierName')
         if m.get('SupplierUrl') is not None:
             self.supplier_url = m.get('SupplierUrl')
+        if m.get('UpgradableServiceVersions') is not None:
+            self.upgradable_service_versions = m.get('UpgradableServiceVersions')
         if m.get('Version') is not None:
             self.version = m.get('Version')
         if m.get('VersionName') is not None:
             self.version_name = m.get('VersionName')
         return self
 
 
@@ -1104,33 +1588,36 @@
             self.key = m.get('Key')
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class GetServiceInstanceResponseBody(TeaModel):
-    def __init__(self, create_time=None, enable_instance_ops=None, end_time=None, is_operated=None,
-                 license_metadata=None, name=None, network_config=None, operated_service_instance_id=None, operation_end_time=None,
-                 operation_start_time=None, outputs=None, parameters=None, pay_type=None, progress=None, request_id=None, resources=None,
-                 service=None, service_instance_id=None, service_type=None, source=None, status=None, status_detail=None,
-                 supplier_uid=None, tags=None, template_name=None, update_time=None, user_id=None):
+    def __init__(self, create_time=None, enable_instance_ops=None, enable_user_prometheus=None, end_time=None,
+                 is_operated=None, license_metadata=None, name=None, network_config=None, operated_service_instance_id=None,
+                 operation_end_time=None, operation_start_time=None, outputs=None, parameters=None, pay_type=None, progress=None,
+                 rd_account_login_url=None, request_id=None, resources=None, service=None, service_instance_id=None, service_type=None,
+                 source=None, status=None, status_detail=None, supplier_uid=None, tags=None, template_name=None,
+                 update_time=None, user_id=None):
         self.create_time = create_time  # type: str
         self.enable_instance_ops = enable_instance_ops  # type: bool
+        self.enable_user_prometheus = enable_user_prometheus  # type: str
         self.end_time = end_time  # type: str
         self.is_operated = is_operated  # type: bool
         self.license_metadata = license_metadata  # type: str
         self.name = name  # type: str
         self.network_config = network_config  # type: GetServiceInstanceResponseBodyNetworkConfig
         self.operated_service_instance_id = operated_service_instance_id  # type: str
         self.operation_end_time = operation_end_time  # type: str
         self.operation_start_time = operation_start_time  # type: str
         self.outputs = outputs  # type: str
         self.parameters = parameters  # type: str
         self.pay_type = pay_type  # type: str
         self.progress = progress  # type: long
+        self.rd_account_login_url = rd_account_login_url  # type: str
         self.request_id = request_id  # type: str
         self.resources = resources  # type: str
         self.service = service  # type: GetServiceInstanceResponseBodyService
         self.service_instance_id = service_instance_id  # type: str
         self.service_type = service_type  # type: str
         self.source = source  # type: str
         self.status = status  # type: str
@@ -1157,14 +1644,16 @@
             return _map
 
         result = dict()
         if self.create_time is not None:
             result['CreateTime'] = self.create_time
         if self.enable_instance_ops is not None:
             result['EnableInstanceOps'] = self.enable_instance_ops
+        if self.enable_user_prometheus is not None:
+            result['EnableUserPrometheus'] = self.enable_user_prometheus
         if self.end_time is not None:
             result['EndTime'] = self.end_time
         if self.is_operated is not None:
             result['IsOperated'] = self.is_operated
         if self.license_metadata is not None:
             result['LicenseMetadata'] = self.license_metadata
         if self.name is not None:
@@ -1181,14 +1670,16 @@
             result['Outputs'] = self.outputs
         if self.parameters is not None:
             result['Parameters'] = self.parameters
         if self.pay_type is not None:
             result['PayType'] = self.pay_type
         if self.progress is not None:
             result['Progress'] = self.progress
+        if self.rd_account_login_url is not None:
+            result['RdAccountLoginUrl'] = self.rd_account_login_url
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.resources is not None:
             result['Resources'] = self.resources
         if self.service is not None:
             result['Service'] = self.service.to_map()
         if self.service_instance_id is not None:
@@ -1217,14 +1708,16 @@
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
         if m.get('EnableInstanceOps') is not None:
             self.enable_instance_ops = m.get('EnableInstanceOps')
+        if m.get('EnableUserPrometheus') is not None:
+            self.enable_user_prometheus = m.get('EnableUserPrometheus')
         if m.get('EndTime') is not None:
             self.end_time = m.get('EndTime')
         if m.get('IsOperated') is not None:
             self.is_operated = m.get('IsOperated')
         if m.get('LicenseMetadata') is not None:
             self.license_metadata = m.get('LicenseMetadata')
         if m.get('Name') is not None:
@@ -1242,14 +1735,16 @@
             self.outputs = m.get('Outputs')
         if m.get('Parameters') is not None:
             self.parameters = m.get('Parameters')
         if m.get('PayType') is not None:
             self.pay_type = m.get('PayType')
         if m.get('Progress') is not None:
             self.progress = m.get('Progress')
+        if m.get('RdAccountLoginUrl') is not None:
+            self.rd_account_login_url = m.get('RdAccountLoginUrl')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         if m.get('Resources') is not None:
             self.resources = m.get('Resources')
         if m.get('Service') is not None:
             temp_model = GetServiceInstanceResponseBodyService()
             self.service = temp_model.from_map(m['Service'])
@@ -1801,19 +2296,20 @@
             self.key = m.get('Key')
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class ListServiceInstancesRequest(TeaModel):
-    def __init__(self, filter=None, max_results=None, next_token=None, region_id=None, tag=None):
+    def __init__(self, filter=None, max_results=None, next_token=None, region_id=None, show_deleted=None, tag=None):
         self.filter = filter  # type: list[ListServiceInstancesRequestFilter]
         self.max_results = max_results  # type: str
         self.next_token = next_token  # type: str
         self.region_id = region_id  # type: str
+        self.show_deleted = show_deleted  # type: bool
         self.tag = tag  # type: list[ListServiceInstancesRequestTag]
 
     def validate(self):
         if self.filter:
             for k in self.filter:
                 if k:
                     k.validate()
@@ -1834,14 +2330,16 @@
                 result['Filter'].append(k.to_map() if k else None)
         if self.max_results is not None:
             result['MaxResults'] = self.max_results
         if self.next_token is not None:
             result['NextToken'] = self.next_token
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.show_deleted is not None:
+            result['ShowDeleted'] = self.show_deleted
         result['Tag'] = []
         if self.tag is not None:
             for k in self.tag:
                 result['Tag'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m=None):
@@ -1853,14 +2351,16 @@
                 self.filter.append(temp_model.from_map(k))
         if m.get('MaxResults') is not None:
             self.max_results = m.get('MaxResults')
         if m.get('NextToken') is not None:
             self.next_token = m.get('NextToken')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('ShowDeleted') is not None:
+            self.show_deleted = m.get('ShowDeleted')
         self.tag = []
         if m.get('Tag') is not None:
             for k in m.get('Tag'):
                 temp_model = ListServiceInstancesRequestTag()
                 self.tag.append(temp_model.from_map(k))
         return self
 
@@ -1901,19 +2401,20 @@
             self.name = m.get('Name')
         if m.get('ShortDescription') is not None:
             self.short_description = m.get('ShortDescription')
         return self
 
 
 class ListServiceInstancesResponseBodyServiceInstancesService(TeaModel):
-    def __init__(self, deploy_metadata=None, deploy_type=None, publish_time=None, service_id=None,
-                 service_infos=None, service_type=None, status=None, supplier_name=None, supplier_url=None, version=None,
-                 version_name=None):
+    def __init__(self, deploy_metadata=None, deploy_type=None, enable_private_vpc_connection=None,
+                 publish_time=None, service_id=None, service_infos=None, service_type=None, status=None, supplier_name=None,
+                 supplier_url=None, version=None, version_name=None):
         self.deploy_metadata = deploy_metadata  # type: str
         self.deploy_type = deploy_type  # type: str
+        self.enable_private_vpc_connection = enable_private_vpc_connection  # type: bool
         self.publish_time = publish_time  # type: str
         self.service_id = service_id  # type: str
         self.service_infos = service_infos  # type: list[ListServiceInstancesResponseBodyServiceInstancesServiceServiceInfos]
         self.service_type = service_type  # type: str
         self.status = status  # type: str
         self.supplier_name = supplier_name  # type: str
         self.supplier_url = supplier_url  # type: str
@@ -1932,14 +2433,16 @@
             return _map
 
         result = dict()
         if self.deploy_metadata is not None:
             result['DeployMetadata'] = self.deploy_metadata
         if self.deploy_type is not None:
             result['DeployType'] = self.deploy_type
+        if self.enable_private_vpc_connection is not None:
+            result['EnablePrivateVpcConnection'] = self.enable_private_vpc_connection
         if self.publish_time is not None:
             result['PublishTime'] = self.publish_time
         if self.service_id is not None:
             result['ServiceId'] = self.service_id
         result['ServiceInfos'] = []
         if self.service_infos is not None:
             for k in self.service_infos:
@@ -1960,14 +2463,16 @@
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('DeployMetadata') is not None:
             self.deploy_metadata = m.get('DeployMetadata')
         if m.get('DeployType') is not None:
             self.deploy_type = m.get('DeployType')
+        if m.get('EnablePrivateVpcConnection') is not None:
+            self.enable_private_vpc_connection = m.get('EnablePrivateVpcConnection')
         if m.get('PublishTime') is not None:
             self.publish_time = m.get('PublishTime')
         if m.get('ServiceId') is not None:
             self.service_id = m.get('ServiceId')
         self.service_infos = []
         if m.get('ServiceInfos') is not None:
             for k in m.get('ServiceInfos'):
@@ -2531,14 +3036,463 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListServiceUsagesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListServicesRequestFilter(TeaModel):
+    def __init__(self, name=None, value=None):
+        self.name = name  # type: str
+        self.value = value  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListServicesRequestFilter, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class ListServicesRequestTag(TeaModel):
+    def __init__(self, key=None, value=None):
+        self.key = key  # type: str
+        self.value = value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListServicesRequestTag, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class ListServicesRequest(TeaModel):
+    def __init__(self, all_versions=None, filter=None, max_results=None, next_token=None, region_id=None,
+                 resource_group_id=None, tag=None):
+        self.all_versions = all_versions  # type: bool
+        self.filter = filter  # type: list[ListServicesRequestFilter]
+        self.max_results = max_results  # type: str
+        self.next_token = next_token  # type: str
+        self.region_id = region_id  # type: str
+        self.resource_group_id = resource_group_id  # type: str
+        self.tag = tag  # type: list[ListServicesRequestTag]
+
+    def validate(self):
+        if self.filter:
+            for k in self.filter:
+                if k:
+                    k.validate()
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListServicesRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.all_versions is not None:
+            result['AllVersions'] = self.all_versions
+        result['Filter'] = []
+        if self.filter is not None:
+            for k in self.filter:
+                result['Filter'].append(k.to_map() if k else None)
+        if self.max_results is not None:
+            result['MaxResults'] = self.max_results
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AllVersions') is not None:
+            self.all_versions = m.get('AllVersions')
+        self.filter = []
+        if m.get('Filter') is not None:
+            for k in m.get('Filter'):
+                temp_model = ListServicesRequestFilter()
+                self.filter.append(temp_model.from_map(k))
+        if m.get('MaxResults') is not None:
+            self.max_results = m.get('MaxResults')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = ListServicesRequestTag()
+                self.tag.append(temp_model.from_map(k))
+        return self
+
+
+class ListServicesResponseBodyServicesServiceInfos(TeaModel):
+    def __init__(self, image=None, locale=None, name=None, short_description=None):
+        self.image = image  # type: str
+        self.locale = locale  # type: str
+        self.name = name  # type: str
+        self.short_description = short_description  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListServicesResponseBodyServicesServiceInfos, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.image is not None:
+            result['Image'] = self.image
+        if self.locale is not None:
+            result['Locale'] = self.locale
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.short_description is not None:
+            result['ShortDescription'] = self.short_description
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Image') is not None:
+            self.image = m.get('Image')
+        if m.get('Locale') is not None:
+            self.locale = m.get('Locale')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('ShortDescription') is not None:
+            self.short_description = m.get('ShortDescription')
+        return self
+
+
+class ListServicesResponseBodyServicesTags(TeaModel):
+    def __init__(self, key=None, value=None):
+        self.key = key  # type: str
+        self.value = value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListServicesResponseBodyServicesTags, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class ListServicesResponseBodyServices(TeaModel):
+    def __init__(self, approval_type=None, artifact_id=None, artifact_version=None, commodity_code=None,
+                 create_time=None, default_version=None, deploy_type=None, publish_time=None, relation_type=None,
+                 resource_group_id=None, service_id=None, service_infos=None, service_type=None, share_type=None, source_image=None,
+                 status=None, supplier_name=None, supplier_url=None, tags=None, tenant_type=None, trial_type=None,
+                 update_time=None, version=None, version_name=None):
+        self.approval_type = approval_type  # type: str
+        self.artifact_id = artifact_id  # type: str
+        self.artifact_version = artifact_version  # type: str
+        self.commodity_code = commodity_code  # type: str
+        self.create_time = create_time  # type: str
+        self.default_version = default_version  # type: bool
+        self.deploy_type = deploy_type  # type: str
+        self.publish_time = publish_time  # type: str
+        self.relation_type = relation_type  # type: str
+        self.resource_group_id = resource_group_id  # type: str
+        self.service_id = service_id  # type: str
+        self.service_infos = service_infos  # type: list[ListServicesResponseBodyServicesServiceInfos]
+        self.service_type = service_type  # type: str
+        self.share_type = share_type  # type: str
+        self.source_image = source_image  # type: str
+        self.status = status  # type: str
+        self.supplier_name = supplier_name  # type: str
+        self.supplier_url = supplier_url  # type: str
+        self.tags = tags  # type: list[ListServicesResponseBodyServicesTags]
+        self.tenant_type = tenant_type  # type: str
+        self.trial_type = trial_type  # type: str
+        self.update_time = update_time  # type: str
+        self.version = version  # type: str
+        self.version_name = version_name  # type: str
+
+    def validate(self):
+        if self.service_infos:
+            for k in self.service_infos:
+                if k:
+                    k.validate()
+        if self.tags:
+            for k in self.tags:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListServicesResponseBodyServices, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.approval_type is not None:
+            result['ApprovalType'] = self.approval_type
+        if self.artifact_id is not None:
+            result['ArtifactId'] = self.artifact_id
+        if self.artifact_version is not None:
+            result['ArtifactVersion'] = self.artifact_version
+        if self.commodity_code is not None:
+            result['CommodityCode'] = self.commodity_code
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.default_version is not None:
+            result['DefaultVersion'] = self.default_version
+        if self.deploy_type is not None:
+            result['DeployType'] = self.deploy_type
+        if self.publish_time is not None:
+            result['PublishTime'] = self.publish_time
+        if self.relation_type is not None:
+            result['RelationType'] = self.relation_type
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
+        if self.service_id is not None:
+            result['ServiceId'] = self.service_id
+        result['ServiceInfos'] = []
+        if self.service_infos is not None:
+            for k in self.service_infos:
+                result['ServiceInfos'].append(k.to_map() if k else None)
+        if self.service_type is not None:
+            result['ServiceType'] = self.service_type
+        if self.share_type is not None:
+            result['ShareType'] = self.share_type
+        if self.source_image is not None:
+            result['SourceImage'] = self.source_image
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.supplier_name is not None:
+            result['SupplierName'] = self.supplier_name
+        if self.supplier_url is not None:
+            result['SupplierUrl'] = self.supplier_url
+        result['Tags'] = []
+        if self.tags is not None:
+            for k in self.tags:
+                result['Tags'].append(k.to_map() if k else None)
+        if self.tenant_type is not None:
+            result['TenantType'] = self.tenant_type
+        if self.trial_type is not None:
+            result['TrialType'] = self.trial_type
+        if self.update_time is not None:
+            result['UpdateTime'] = self.update_time
+        if self.version is not None:
+            result['Version'] = self.version
+        if self.version_name is not None:
+            result['VersionName'] = self.version_name
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ApprovalType') is not None:
+            self.approval_type = m.get('ApprovalType')
+        if m.get('ArtifactId') is not None:
+            self.artifact_id = m.get('ArtifactId')
+        if m.get('ArtifactVersion') is not None:
+            self.artifact_version = m.get('ArtifactVersion')
+        if m.get('CommodityCode') is not None:
+            self.commodity_code = m.get('CommodityCode')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('DefaultVersion') is not None:
+            self.default_version = m.get('DefaultVersion')
+        if m.get('DeployType') is not None:
+            self.deploy_type = m.get('DeployType')
+        if m.get('PublishTime') is not None:
+            self.publish_time = m.get('PublishTime')
+        if m.get('RelationType') is not None:
+            self.relation_type = m.get('RelationType')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
+        if m.get('ServiceId') is not None:
+            self.service_id = m.get('ServiceId')
+        self.service_infos = []
+        if m.get('ServiceInfos') is not None:
+            for k in m.get('ServiceInfos'):
+                temp_model = ListServicesResponseBodyServicesServiceInfos()
+                self.service_infos.append(temp_model.from_map(k))
+        if m.get('ServiceType') is not None:
+            self.service_type = m.get('ServiceType')
+        if m.get('ShareType') is not None:
+            self.share_type = m.get('ShareType')
+        if m.get('SourceImage') is not None:
+            self.source_image = m.get('SourceImage')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('SupplierName') is not None:
+            self.supplier_name = m.get('SupplierName')
+        if m.get('SupplierUrl') is not None:
+            self.supplier_url = m.get('SupplierUrl')
+        self.tags = []
+        if m.get('Tags') is not None:
+            for k in m.get('Tags'):
+                temp_model = ListServicesResponseBodyServicesTags()
+                self.tags.append(temp_model.from_map(k))
+        if m.get('TenantType') is not None:
+            self.tenant_type = m.get('TenantType')
+        if m.get('TrialType') is not None:
+            self.trial_type = m.get('TrialType')
+        if m.get('UpdateTime') is not None:
+            self.update_time = m.get('UpdateTime')
+        if m.get('Version') is not None:
+            self.version = m.get('Version')
+        if m.get('VersionName') is not None:
+            self.version_name = m.get('VersionName')
+        return self
+
+
+class ListServicesResponseBody(TeaModel):
+    def __init__(self, max_results=None, next_token=None, request_id=None, services=None, total_count=None):
+        self.max_results = max_results  # type: int
+        self.next_token = next_token  # type: str
+        self.request_id = request_id  # type: str
+        self.services = services  # type: list[ListServicesResponseBodyServices]
+        self.total_count = total_count  # type: str
+
+    def validate(self):
+        if self.services:
+            for k in self.services:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListServicesResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.max_results is not None:
+            result['MaxResults'] = self.max_results
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['Services'] = []
+        if self.services is not None:
+            for k in self.services:
+                result['Services'].append(k.to_map() if k else None)
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('MaxResults') is not None:
+            self.max_results = m.get('MaxResults')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.services = []
+        if m.get('Services') is not None:
+            for k in m.get('Services'):
+                temp_model = ListServicesResponseBodyServices()
+                self.services.append(temp_model.from_map(k))
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListServicesResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListServicesResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListServicesResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListServicesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ReleaseArtifactRequest(TeaModel):
     def __init__(self, artifact_id=None):
         self.artifact_id = artifact_id  # type: str
 
     def validate(self):
         pass
```

### Comparing `alibabacloud_computenestsupplier20210521_py2-1.1.2/alibabacloud_computenestsupplier20210521_py2.egg-info/PKG-INFO` & `alibabacloud_computenestsupplier20210521_py2-1.1.3/alibabacloud_computenestsupplier20210521_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-computenestsupplier20210521-py2
-Version: 1.1.2
+Version: 1.1.3
 Summary: Alibaba Cloud ComputeNestSupplier (20210521) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_computenestsupplier20210521_py2-1.1.2/alibabacloud_computenestsupplier20210521_py2.egg-info/SOURCES.txt` & `alibabacloud_computenestsupplier20210521_py2-1.1.3/alibabacloud_computenestsupplier20210521_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_computenestsupplier20210521_py2-1.1.2/setup.py` & `alibabacloud_computenestsupplier20210521_py2-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_computenestsupplier20210521_py2.
 
-Created on 06/02/2023
+Created on 16/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_computenestsupplier20210521"
 NAME = "alibabacloud_computenestsupplier20210521_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ComputeNestSupplier (20210521) SDK Library for Python2"
```

