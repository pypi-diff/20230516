# Comparing `tmp/alibabacloud_computenestsupplier20210521-1.2.0.tar.gz` & `tmp/alibabacloud_computenestsupplier20210521-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_computenestsupplier20210521-1.2.0.tar", last modified: Fri Apr 28 07:45:17 2023, max compression
+gzip compressed data, was "dist/alibabacloud_computenestsupplier20210521-1.2.1.tar", last modified: Tue May 16 09:57:18 2023, max compression
```

## Comparing `alibabacloud_computenestsupplier20210521-1.2.0.tar` & `alibabacloud_computenestsupplier20210521-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/
--rw-r--r--   0 root         (0) root         (0)      259 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2424 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1070 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1155 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54641 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521/client.py
--rw-r--r--   0 root         (0) root         (0)   153003 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2424 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      548 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2690 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:57:18.000000 alibabacloud_computenestsupplier20210521-1.2.1/
+-rw-r--r--   0 root         (0) root         (0)      328 2023-05-16 09:57:18.000000 alibabacloud_computenestsupplier20210521-1.2.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-16 09:57:18.000000 alibabacloud_computenestsupplier20210521-1.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 09:57:18.000000 alibabacloud_computenestsupplier20210521-1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2424 2023-05-16 09:57:18.000000 alibabacloud_computenestsupplier20210521-1.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-05-16 09:57:18.000000 alibabacloud_computenestsupplier20210521-1.2.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-05-16 09:57:18.000000 alibabacloud_computenestsupplier20210521-1.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:57:18.000000 alibabacloud_computenestsupplier20210521-1.2.1/alibabacloud_computenestsupplier20210521/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 09:57:18.000000 alibabacloud_computenestsupplier20210521-1.2.1/alibabacloud_computenestsupplier20210521/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55153 2023-05-16 09:57:18.000000 alibabacloud_computenestsupplier20210521-1.2.1/alibabacloud_computenestsupplier20210521/client.py
+-rw-r--r--   0 root         (0) root         (0)   154250 2023-05-16 09:57:18.000000 alibabacloud_computenestsupplier20210521-1.2.1/alibabacloud_computenestsupplier20210521/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:57:18.000000 alibabacloud_computenestsupplier20210521-1.2.1/alibabacloud_computenestsupplier20210521.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2424 2023-05-16 09:57:18.000000 alibabacloud_computenestsupplier20210521-1.2.1/alibabacloud_computenestsupplier20210521.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      548 2023-05-16 09:57:18.000000 alibabacloud_computenestsupplier20210521-1.2.1/alibabacloud_computenestsupplier20210521.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 09:57:18.000000 alibabacloud_computenestsupplier20210521-1.2.1/alibabacloud_computenestsupplier20210521.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-16 09:57:18.000000 alibabacloud_computenestsupplier20210521-1.2.1/alibabacloud_computenestsupplier20210521.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-05-16 09:57:18.000000 alibabacloud_computenestsupplier20210521-1.2.1/alibabacloud_computenestsupplier20210521.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 09:57:18.000000 alibabacloud_computenestsupplier20210521-1.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2690 2023-05-16 09:57:18.000000 alibabacloud_computenestsupplier20210521-1.2.1/setup.py
```

### Comparing `alibabacloud_computenestsupplier20210521-1.2.0/LICENSE` & `alibabacloud_computenestsupplier20210521-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_computenestsupplier20210521-1.2.0/PKG-INFO` & `alibabacloud_computenestsupplier20210521-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_computenestsupplier20210521
-Version: 1.2.0
+Version: 1.2.1
 Summary: Alibaba Cloud ComputeNestSupplier (20210521) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_computenestsupplier20210521-1.2.0/README-CN.md` & `alibabacloud_computenestsupplier20210521-1.2.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_computenestsupplier20210521-1.2.0/README.md` & `alibabacloud_computenestsupplier20210521-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521/client.py` & `alibabacloud_computenestsupplier20210521-1.2.1/alibabacloud_computenestsupplier20210521/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,16 @@
             query['LicenseMetadata'] = request.license_metadata
         if not UtilClient.is_unset(request.operation_metadata):
             query['OperationMetadata'] = request.operation_metadata
         if not UtilClient.is_unset(request.policy_names):
             query['PolicyNames'] = request.policy_names
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.service_id):
             query['ServiceId'] = request.service_id
         if not UtilClient.is_unset(request.service_info):
             query['ServiceInfo'] = request.service_info
         if not UtilClient.is_unset(request.service_type):
             query['ServiceType'] = request.service_type
         if not UtilClient.is_unset(request.share_type):
@@ -234,14 +236,16 @@
             query['LicenseMetadata'] = request.license_metadata
         if not UtilClient.is_unset(request.operation_metadata):
             query['OperationMetadata'] = request.operation_metadata
         if not UtilClient.is_unset(request.policy_names):
             query['PolicyNames'] = request.policy_names
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.service_id):
             query['ServiceId'] = request.service_id
         if not UtilClient.is_unset(request.service_info):
             query['ServiceInfo'] = request.service_info
         if not UtilClient.is_unset(request.service_type):
             query['ServiceType'] = request.service_type
         if not UtilClient.is_unset(request.share_type):
@@ -1024,14 +1028,16 @@
             query['Filter'] = request.filter
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListServices',
@@ -1062,14 +1068,16 @@
             query['Filter'] = request.filter
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListServices',
```

### Comparing `alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521/models.py` & `alibabacloud_computenestsupplier20210521-1.2.1/alibabacloud_computenestsupplier20210521/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,14 +420,15 @@
         deploy_type: str = None,
         duration: int = None,
         is_support_operated: bool = None,
         license_metadata: str = None,
         operation_metadata: str = None,
         policy_names: str = None,
         region_id: str = None,
+        resource_group_id: str = None,
         service_id: str = None,
         service_info: List[CreateServiceRequestServiceInfo] = None,
         service_type: str = None,
         share_type: str = None,
         tag: List[CreateServiceRequestTag] = None,
         tenant_type: str = None,
         trial_duration: int = None,
@@ -441,14 +442,15 @@
         self.deploy_type = deploy_type
         self.duration = duration
         self.is_support_operated = is_support_operated
         self.license_metadata = license_metadata
         self.operation_metadata = operation_metadata
         self.policy_names = policy_names
         self.region_id = region_id
+        self.resource_group_id = resource_group_id
         self.service_id = service_id
         self.service_info = service_info
         self.service_type = service_type
         self.share_type = share_type
         self.tag = tag
         self.tenant_type = tenant_type
         self.trial_duration = trial_duration
@@ -489,14 +491,16 @@
             result['LicenseMetadata'] = self.license_metadata
         if self.operation_metadata is not None:
             result['OperationMetadata'] = self.operation_metadata
         if self.policy_names is not None:
             result['PolicyNames'] = self.policy_names
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
         if self.service_id is not None:
             result['ServiceId'] = self.service_id
         result['ServiceInfo'] = []
         if self.service_info is not None:
             for k in self.service_info:
                 result['ServiceInfo'].append(k.to_map() if k else None)
         if self.service_type is not None:
@@ -537,14 +541,16 @@
             self.license_metadata = m.get('LicenseMetadata')
         if m.get('OperationMetadata') is not None:
             self.operation_metadata = m.get('OperationMetadata')
         if m.get('PolicyNames') is not None:
             self.policy_names = m.get('PolicyNames')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
         if m.get('ServiceId') is not None:
             self.service_id = m.get('ServiceId')
         self.service_info = []
         if m.get('ServiceInfo') is not None:
             for k in m.get('ServiceInfo'):
                 temp_model = CreateServiceRequestServiceInfo()
                 self.service_info.append(temp_model.from_map(k))
@@ -1395,22 +1401,24 @@
             self.service_instance_id = m.get('ServiceInstanceId')
         return self
 
 
 class GetServiceInstanceResponseBodyNetworkConfigPrivateVpcConnectionsConnectionConfigs(TeaModel):
     def __init__(
         self,
+        connect_bandwidth: int = None,
         domain_name: str = None,
         endpoint_ips: List[str] = None,
         ingress_endpoint_status: str = None,
         network_service_status: str = None,
         security_groups: List[str] = None,
         v_switches: List[str] = None,
         vpc_id: str = None,
     ):
+        self.connect_bandwidth = connect_bandwidth
         self.domain_name = domain_name
         self.endpoint_ips = endpoint_ips
         self.ingress_endpoint_status = ingress_endpoint_status
         self.network_service_status = network_service_status
         self.security_groups = security_groups
         self.v_switches = v_switches
         self.vpc_id = vpc_id
@@ -1420,14 +1428,16 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.connect_bandwidth is not None:
+            result['ConnectBandwidth'] = self.connect_bandwidth
         if self.domain_name is not None:
             result['DomainName'] = self.domain_name
         if self.endpoint_ips is not None:
             result['EndpointIps'] = self.endpoint_ips
         if self.ingress_endpoint_status is not None:
             result['IngressEndpointStatus'] = self.ingress_endpoint_status
         if self.network_service_status is not None:
@@ -1438,14 +1448,16 @@
             result['VSwitches'] = self.v_switches
         if self.vpc_id is not None:
             result['VpcId'] = self.vpc_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('ConnectBandwidth') is not None:
+            self.connect_bandwidth = m.get('ConnectBandwidth')
         if m.get('DomainName') is not None:
             self.domain_name = m.get('DomainName')
         if m.get('EndpointIps') is not None:
             self.endpoint_ips = m.get('EndpointIps')
         if m.get('IngressEndpointStatus') is not None:
             self.ingress_endpoint_status = m.get('IngressEndpointStatus')
         if m.get('NetworkServiceStatus') is not None:
@@ -3517,21 +3529,23 @@
     def __init__(
         self,
         all_versions: bool = None,
         filter: List[ListServicesRequestFilter] = None,
         max_results: str = None,
         next_token: str = None,
         region_id: str = None,
+        resource_group_id: str = None,
         tag: List[ListServicesRequestTag] = None,
     ):
         self.all_versions = all_versions
         self.filter = filter
         self.max_results = max_results
         self.next_token = next_token
         self.region_id = region_id
+        self.resource_group_id = resource_group_id
         self.tag = tag
 
     def validate(self):
         if self.filter:
             for k in self.filter:
                 if k:
                     k.validate()
@@ -3554,14 +3568,16 @@
                 result['Filter'].append(k.to_map() if k else None)
         if self.max_results is not None:
             result['MaxResults'] = self.max_results
         if self.next_token is not None:
             result['NextToken'] = self.next_token
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
         result['Tag'] = []
         if self.tag is not None:
             for k in self.tag:
                 result['Tag'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
@@ -3575,14 +3591,16 @@
                 self.filter.append(temp_model.from_map(k))
         if m.get('MaxResults') is not None:
             self.max_results = m.get('MaxResults')
         if m.get('NextToken') is not None:
             self.next_token = m.get('NextToken')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
         self.tag = []
         if m.get('Tag') is not None:
             for k in m.get('Tag'):
                 temp_model = ListServicesRequestTag()
                 self.tag.append(temp_model.from_map(k))
         return self
 
@@ -3673,14 +3691,15 @@
         artifact_version: str = None,
         commodity_code: str = None,
         create_time: str = None,
         default_version: bool = None,
         deploy_type: str = None,
         publish_time: str = None,
         relation_type: str = None,
+        resource_group_id: str = None,
         service_id: str = None,
         service_infos: List[ListServicesResponseBodyServicesServiceInfos] = None,
         service_type: str = None,
         share_type: str = None,
         source_image: str = None,
         status: str = None,
         supplier_name: str = None,
@@ -3697,14 +3716,15 @@
         self.artifact_version = artifact_version
         self.commodity_code = commodity_code
         self.create_time = create_time
         self.default_version = default_version
         self.deploy_type = deploy_type
         self.publish_time = publish_time
         self.relation_type = relation_type
+        self.resource_group_id = resource_group_id
         self.service_id = service_id
         self.service_infos = service_infos
         self.service_type = service_type
         self.share_type = share_type
         self.source_image = source_image
         self.status = status
         self.supplier_name = supplier_name
@@ -3746,14 +3766,16 @@
             result['DefaultVersion'] = self.default_version
         if self.deploy_type is not None:
             result['DeployType'] = self.deploy_type
         if self.publish_time is not None:
             result['PublishTime'] = self.publish_time
         if self.relation_type is not None:
             result['RelationType'] = self.relation_type
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
         if self.service_id is not None:
             result['ServiceId'] = self.service_id
         result['ServiceInfos'] = []
         if self.service_infos is not None:
             for k in self.service_infos:
                 result['ServiceInfos'].append(k.to_map() if k else None)
         if self.service_type is not None:
@@ -3800,14 +3822,16 @@
             self.default_version = m.get('DefaultVersion')
         if m.get('DeployType') is not None:
             self.deploy_type = m.get('DeployType')
         if m.get('PublishTime') is not None:
             self.publish_time = m.get('PublishTime')
         if m.get('RelationType') is not None:
             self.relation_type = m.get('RelationType')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
         if m.get('ServiceId') is not None:
             self.service_id = m.get('ServiceId')
         self.service_infos = []
         if m.get('ServiceInfos') is not None:
             for k in m.get('ServiceInfos'):
                 temp_model = ListServicesResponseBodyServicesServiceInfos()
                 self.service_infos.append(temp_model.from_map(k))
```

### Comparing `alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521.egg-info/PKG-INFO` & `alibabacloud_computenestsupplier20210521-1.2.1/alibabacloud_computenestsupplier20210521.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-computenestsupplier20210521
-Version: 1.2.0
+Version: 1.2.1
 Summary: Alibaba Cloud ComputeNestSupplier (20210521) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521.egg-info/SOURCES.txt` & `alibabacloud_computenestsupplier20210521-1.2.1/alibabacloud_computenestsupplier20210521.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_computenestsupplier20210521-1.2.0/setup.py` & `alibabacloud_computenestsupplier20210521-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_computenestsupplier20210521.
 
-Created on 28/04/2023
+Created on 16/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_computenestsupplier20210521"
 NAME = "alibabacloud_computenestsupplier20210521" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ComputeNestSupplier (20210521) SDK Library for Python"
```

