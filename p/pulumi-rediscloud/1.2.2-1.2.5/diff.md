# Comparing `tmp/pulumi_rediscloud-1.2.2.tar.gz` & `tmp/pulumi_rediscloud-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_rediscloud-1.2.2.tar", last modified: Mon May 15 17:29:49 2023, max compression
+gzip compressed data, was "pulumi_rediscloud-1.2.5.tar", last modified: Mon May 15 18:18:45 2023, max compression
```

## Comparing `pulumi_rediscloud-1.2.2.tar` & `pulumi_rediscloud-1.2.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:29:49.544348 pulumi_rediscloud-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-15 17:29:49.544348 pulumi_rediscloud-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:29:49.544348 pulumi_rediscloud-1.2.2/pulumi_rediscloud/
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40848 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/active_active_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    47125 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/active_active_subscription_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    34935 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/active_active_subscription_peering.py
--rw-r--r--   0 runner    (1001) docker     (123)    16300 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/active_active_subscription_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22528 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/cloud_account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:29:49.544348 pulumi_rediscloud-1.2.2/pulumi_rediscloud/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/get_cloud_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/get_data_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)    14314 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/get_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/get_database_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/get_payment_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/get_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/get_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/get_subscription_peerings.py
--rw-r--r--   0 runner    (1001) docker     (123)    53802 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24388 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    65396 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/subscription_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    31635 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud/subscription_peering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:29:49.544348 pulumi_rediscloud-1.2.2/pulumi_rediscloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/pulumi_rediscloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 17:29:49.544348 pulumi_rediscloud-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-15 17:29:49.000000 pulumi_rediscloud-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:18:45.115424 pulumi_rediscloud-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-15 18:18:45.115424 pulumi_rediscloud-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:18:45.115424 pulumi_rediscloud-1.2.5/pulumi_rediscloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40848 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/active_active_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47125 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/active_active_subscription_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34935 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/active_active_subscription_peering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16300 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/active_active_subscription_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22528 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/cloud_account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:18:45.115424 pulumi_rediscloud-1.2.5/pulumi_rediscloud/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/get_cloud_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/get_data_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14314 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/get_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/get_database_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/get_payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/get_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/get_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/get_subscription_peerings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53802 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24388 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65396 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/subscription_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31635 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud/subscription_peering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:18:45.115424 pulumi_rediscloud-1.2.5/pulumi_rediscloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-15 18:18:45.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-15 18:18:45.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 18:18:45.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 18:18:45.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-15 18:18:45.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 18:18:45.000000 pulumi_rediscloud-1.2.5/pulumi_rediscloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 18:18:45.115424 pulumi_rediscloud-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-15 18:18:44.000000 pulumi_rediscloud-1.2.5/setup.py
```

### Comparing `pulumi_rediscloud-1.2.2/PKG-INFO` & `pulumi_rediscloud-1.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rediscloud
-Version: 1.2.2
+Version: 1.2.5
 Summary: A Pulumi package for creating and managing rediscloud cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/RedisLabs/pulumi-rediscloud
 Keywords: pulumi rediscloud category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_rediscloud-1.2.2/README.md` & `pulumi_rediscloud-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud/__init__.py` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud/_inputs.py` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud/_utilities.py` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud/active_active_subscription.py` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud/active_active_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud/active_active_subscription_database.py` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud/active_active_subscription_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 
 __all__ = ['ActiveActiveSubscriptionDatabaseArgs', 'ActiveActiveSubscriptionDatabase']
 
 @pulumi.input_type
 class ActiveActiveSubscriptionDatabaseArgs:
     def __init__(__self__, *,
                  memory_limit_in_gb: pulumi.Input[float],
-                 subscription_id: pulumi.Input[int],
+                 subscription_id: pulumi.Input[str],
                  client_ssl_certificate: Optional[pulumi.Input[str]] = None,
                  data_eviction: Optional[pulumi.Input[str]] = None,
                  enable_tls: Optional[pulumi.Input[bool]] = None,
                  external_endpoint_for_oss_cluster_api: Optional[pulumi.Input[bool]] = None,
                  global_alerts: Optional[pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionDatabaseGlobalAlertArgs']]]] = None,
                  global_data_persistence: Optional[pulumi.Input[str]] = None,
                  global_password: Optional[pulumi.Input[str]] = None,
                  global_source_ips: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  override_regions: Optional[pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionDatabaseOverrideRegionArgs']]]] = None,
                  support_oss_cluster_api: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a ActiveActiveSubscriptionDatabase resource.
         :param pulumi.Input[float] memory_limit_in_gb: Maximum memory usage for this specific database, including replication and other overhead
-        :param pulumi.Input[int] subscription_id: The ID of the Active-Active subscription to create the database in
+        :param pulumi.Input[str] subscription_id: The ID of the Active-Active subscription to create the database in
         :param pulumi.Input[str] client_ssl_certificate: SSL certificate to authenticate user connections.
         :param pulumi.Input[str] data_eviction: The data items eviction policy (either: 'allkeys-lru', 'allkeys-lfu', 'allkeys-random', 'volatile-lru', 'volatile-lfu', 'volatile-random', 'volatile-ttl' or 'noeviction'. Default: 'volatile-lru')
         :param pulumi.Input[bool] enable_tls: Use TLS for authentication. Default: ‘false’
         :param pulumi.Input[bool] external_endpoint_for_oss_cluster_api: Should use the external endpoint for open-source (OSS) Cluster API.
                Can only be enabled if OSS Cluster API support is enabled. Default: 'false'
         :param pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionDatabaseGlobalAlertArgs']]] global_alerts: A block defining Redis database alert of regions that dont override global settings, documented below, can be specified multiple times
         :param pulumi.Input[str] global_data_persistence: Global rate of database data persistence (in persistent storage) of regions that dont override global settings. Default: 'none'
@@ -81,22 +81,22 @@
 
     @memory_limit_in_gb.setter
     def memory_limit_in_gb(self, value: pulumi.Input[float]):
         pulumi.set(self, "memory_limit_in_gb", value)
 
     @property
     @pulumi.getter(name="subscriptionId")
-    def subscription_id(self) -> pulumi.Input[int]:
+    def subscription_id(self) -> pulumi.Input[str]:
         """
         The ID of the Active-Active subscription to create the database in
         """
         return pulumi.get(self, "subscription_id")
 
     @subscription_id.setter
-    def subscription_id(self, value: pulumi.Input[int]):
+    def subscription_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "subscription_id", value)
 
     @property
     @pulumi.getter(name="clientSslCertificate")
     def client_ssl_certificate(self) -> Optional[pulumi.Input[str]]:
         """
         SSL certificate to authenticate user connections.
@@ -242,15 +242,15 @@
                  global_password: Optional[pulumi.Input[str]] = None,
                  global_source_ips: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  memory_limit_in_gb: Optional[pulumi.Input[float]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  override_regions: Optional[pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionDatabaseOverrideRegionArgs']]]] = None,
                  private_endpoint: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  public_endpoint: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 subscription_id: Optional[pulumi.Input[int]] = None,
+                 subscription_id: Optional[pulumi.Input[str]] = None,
                  support_oss_cluster_api: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering ActiveActiveSubscriptionDatabase resources.
         :param pulumi.Input[str] client_ssl_certificate: SSL certificate to authenticate user connections.
         :param pulumi.Input[str] data_eviction: The data items eviction policy (either: 'allkeys-lru', 'allkeys-lfu', 'allkeys-random', 'volatile-lru', 'volatile-lfu', 'volatile-random', 'volatile-ttl' or 'noeviction'. Default: 'volatile-lru')
         :param pulumi.Input[int] db_id: Identifier of the database created
         :param pulumi.Input[bool] enable_tls: Use TLS for authentication. Default: ‘false’
@@ -261,15 +261,15 @@
         :param pulumi.Input[str] global_password: Password to access the database of regions that dont override global settings. If left empty, the password will be generated automatically
         :param pulumi.Input[Sequence[pulumi.Input[str]]] global_source_ips: List of source IP addresses or subnet masks of regions that dont override global settings. If specified, Redis clients will be able to connect to this database only from within the specified source IP addresses ranges (example: ['192.168.10.0/32', '192.168.12.0/24'])
         :param pulumi.Input[float] memory_limit_in_gb: Maximum memory usage for this specific database, including replication and other overhead
         :param pulumi.Input[str] name: A meaningful name to identify the database
         :param pulumi.Input[Sequence[pulumi.Input['ActiveActiveSubscriptionDatabaseOverrideRegionArgs']]] override_regions: Override region specific configuration, documented below
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] private_endpoint: A map of which private endpoints can to access the database per region, uses region name as key.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] public_endpoint: A map of which public endpoints can to access the database per region, uses region name as key.
-        :param pulumi.Input[int] subscription_id: The ID of the Active-Active subscription to create the database in
+        :param pulumi.Input[str] subscription_id: The ID of the Active-Active subscription to create the database in
         :param pulumi.Input[bool] support_oss_cluster_api: Support Redis open-source (OSS) Cluster API. Default: ‘false’
         """
         if client_ssl_certificate is not None:
             pulumi.set(__self__, "client_ssl_certificate", client_ssl_certificate)
         if data_eviction is not None:
             pulumi.set(__self__, "data_eviction", data_eviction)
         if db_id is not None:
@@ -468,22 +468,22 @@
 
     @public_endpoint.setter
     def public_endpoint(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "public_endpoint", value)
 
     @property
     @pulumi.getter(name="subscriptionId")
-    def subscription_id(self) -> Optional[pulumi.Input[int]]:
+    def subscription_id(self) -> Optional[pulumi.Input[str]]:
         """
         The ID of the Active-Active subscription to create the database in
         """
         return pulumi.get(self, "subscription_id")
 
     @subscription_id.setter
-    def subscription_id(self, value: Optional[pulumi.Input[int]]):
+    def subscription_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "subscription_id", value)
 
     @property
     @pulumi.getter(name="supportOssClusterApi")
     def support_oss_cluster_api(self) -> Optional[pulumi.Input[bool]]:
         """
         Support Redis open-source (OSS) Cluster API. Default: ‘false’
@@ -507,15 +507,15 @@
                  global_alerts: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ActiveActiveSubscriptionDatabaseGlobalAlertArgs']]]]] = None,
                  global_data_persistence: Optional[pulumi.Input[str]] = None,
                  global_password: Optional[pulumi.Input[str]] = None,
                  global_source_ips: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  memory_limit_in_gb: Optional[pulumi.Input[float]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  override_regions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ActiveActiveSubscriptionDatabaseOverrideRegionArgs']]]]] = None,
-                 subscription_id: Optional[pulumi.Input[int]] = None,
+                 subscription_id: Optional[pulumi.Input[str]] = None,
                  support_oss_cluster_api: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         Creates a Database within a specified Active-Active Subscription in your Redis Enterprise Cloud Account.
 
         ## Import
 
@@ -537,15 +537,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ActiveActiveSubscriptionDatabaseGlobalAlertArgs']]]] global_alerts: A block defining Redis database alert of regions that dont override global settings, documented below, can be specified multiple times
         :param pulumi.Input[str] global_data_persistence: Global rate of database data persistence (in persistent storage) of regions that dont override global settings. Default: 'none'
         :param pulumi.Input[str] global_password: Password to access the database of regions that dont override global settings. If left empty, the password will be generated automatically
         :param pulumi.Input[Sequence[pulumi.Input[str]]] global_source_ips: List of source IP addresses or subnet masks of regions that dont override global settings. If specified, Redis clients will be able to connect to this database only from within the specified source IP addresses ranges (example: ['192.168.10.0/32', '192.168.12.0/24'])
         :param pulumi.Input[float] memory_limit_in_gb: Maximum memory usage for this specific database, including replication and other overhead
         :param pulumi.Input[str] name: A meaningful name to identify the database
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ActiveActiveSubscriptionDatabaseOverrideRegionArgs']]]] override_regions: Override region specific configuration, documented below
-        :param pulumi.Input[int] subscription_id: The ID of the Active-Active subscription to create the database in
+        :param pulumi.Input[str] subscription_id: The ID of the Active-Active subscription to create the database in
         :param pulumi.Input[bool] support_oss_cluster_api: Support Redis open-source (OSS) Cluster API. Default: ‘false’
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ActiveActiveSubscriptionDatabaseArgs,
@@ -585,15 +585,15 @@
                  global_alerts: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ActiveActiveSubscriptionDatabaseGlobalAlertArgs']]]]] = None,
                  global_data_persistence: Optional[pulumi.Input[str]] = None,
                  global_password: Optional[pulumi.Input[str]] = None,
                  global_source_ips: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  memory_limit_in_gb: Optional[pulumi.Input[float]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  override_regions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ActiveActiveSubscriptionDatabaseOverrideRegionArgs']]]]] = None,
-                 subscription_id: Optional[pulumi.Input[int]] = None,
+                 subscription_id: Optional[pulumi.Input[str]] = None,
                  support_oss_cluster_api: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
@@ -642,15 +642,15 @@
             global_password: Optional[pulumi.Input[str]] = None,
             global_source_ips: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             memory_limit_in_gb: Optional[pulumi.Input[float]] = None,
             name: Optional[pulumi.Input[str]] = None,
             override_regions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ActiveActiveSubscriptionDatabaseOverrideRegionArgs']]]]] = None,
             private_endpoint: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             public_endpoint: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-            subscription_id: Optional[pulumi.Input[int]] = None,
+            subscription_id: Optional[pulumi.Input[str]] = None,
             support_oss_cluster_api: Optional[pulumi.Input[bool]] = None) -> 'ActiveActiveSubscriptionDatabase':
         """
         Get an existing ActiveActiveSubscriptionDatabase resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
@@ -666,15 +666,15 @@
         :param pulumi.Input[str] global_password: Password to access the database of regions that dont override global settings. If left empty, the password will be generated automatically
         :param pulumi.Input[Sequence[pulumi.Input[str]]] global_source_ips: List of source IP addresses or subnet masks of regions that dont override global settings. If specified, Redis clients will be able to connect to this database only from within the specified source IP addresses ranges (example: ['192.168.10.0/32', '192.168.12.0/24'])
         :param pulumi.Input[float] memory_limit_in_gb: Maximum memory usage for this specific database, including replication and other overhead
         :param pulumi.Input[str] name: A meaningful name to identify the database
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ActiveActiveSubscriptionDatabaseOverrideRegionArgs']]]] override_regions: Override region specific configuration, documented below
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] private_endpoint: A map of which private endpoints can to access the database per region, uses region name as key.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] public_endpoint: A map of which public endpoints can to access the database per region, uses region name as key.
-        :param pulumi.Input[int] subscription_id: The ID of the Active-Active subscription to create the database in
+        :param pulumi.Input[str] subscription_id: The ID of the Active-Active subscription to create the database in
         :param pulumi.Input[bool] support_oss_cluster_api: Support Redis open-source (OSS) Cluster API. Default: ‘false’
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ActiveActiveSubscriptionDatabaseState.__new__(_ActiveActiveSubscriptionDatabaseState)
 
         __props__.__dict__["client_ssl_certificate"] = client_ssl_certificate
@@ -806,15 +806,15 @@
         """
         A map of which public endpoints can to access the database per region, uses region name as key.
         """
         return pulumi.get(self, "public_endpoint")
 
     @property
     @pulumi.getter(name="subscriptionId")
-    def subscription_id(self) -> pulumi.Output[int]:
+    def subscription_id(self) -> pulumi.Output[str]:
         """
         The ID of the Active-Active subscription to create the database in
         """
         return pulumi.get(self, "subscription_id")
 
     @property
     @pulumi.getter(name="supportOssClusterApi")
```

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud/active_active_subscription_peering.py` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud/active_active_subscription_peering.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud/active_active_subscription_regions.py` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud/active_active_subscription_regions.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud/cloud_account.py` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud/cloud_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud/config/vars.py` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud/get_cloud_account.py` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud/get_cloud_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud/get_data_persistence.py` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud/get_data_persistence.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud/get_database.py` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud/get_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud/get_database_modules.py` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud/get_database_modules.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud/get_payment_method.py` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud/get_payment_method.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud/get_regions.py` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud/get_regions.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud/get_subscription.py` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud/get_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud/get_subscription_peerings.py` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud/get_subscription_peerings.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud/outputs.py` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud/provider.py` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud/subscription.py` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud/subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud/subscription_database.py` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud/subscription_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 __all__ = ['SubscriptionDatabaseArgs', 'SubscriptionDatabase']
 
 @pulumi.input_type
 class SubscriptionDatabaseArgs:
     def __init__(__self__, *,
                  memory_limit_in_gb: pulumi.Input[float],
                  protocol: pulumi.Input[str],
-                 subscription_id: pulumi.Input[int],
+                 subscription_id: pulumi.Input[str],
                  throughput_measurement_by: pulumi.Input[str],
                  throughput_measurement_value: pulumi.Input[int],
                  alerts: Optional[pulumi.Input[Sequence[pulumi.Input['SubscriptionDatabaseAlertArgs']]]] = None,
                  average_item_size_in_bytes: Optional[pulumi.Input[int]] = None,
                  client_ssl_certificate: Optional[pulumi.Input[str]] = None,
                  data_eviction: Optional[pulumi.Input[str]] = None,
                  data_persistence: Optional[pulumi.Input[str]] = None,
@@ -37,15 +37,15 @@
                  replication: Optional[pulumi.Input[bool]] = None,
                  source_ips: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  support_oss_cluster_api: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a SubscriptionDatabase resource.
         :param pulumi.Input[float] memory_limit_in_gb: Maximum memory usage for this specific database
         :param pulumi.Input[str] protocol: The protocol that will be used to access the database, (either ‘redis’ or 'memcached’) Default: ‘redis’
-        :param pulumi.Input[int] subscription_id: The ID of the subscription to create the database in
+        :param pulumi.Input[str] subscription_id: The ID of the subscription to create the database in
         :param pulumi.Input[str] throughput_measurement_by: Throughput measurement method, (either ‘number-of-shards’ or ‘operations-per-second’)
         :param pulumi.Input[int] throughput_measurement_value: Throughput value (as applies to selected measurement method)
         :param pulumi.Input[Sequence[pulumi.Input['SubscriptionDatabaseAlertArgs']]] alerts: A block defining Redis database alert, documented below, can be specified multiple times
         :param pulumi.Input[int] average_item_size_in_bytes: Relevant only to ram-and-flash clusters. Estimated average size (measured in bytes)
                of the items stored in the database. Default: 1000
         :param pulumi.Input[str] client_ssl_certificate: SSL certificate to authenticate user connections
         :param pulumi.Input[str] data_eviction: The data items eviction policy (either: 'allkeys-lru', 'allkeys-lfu', 'allkeys-random', 'volatile-lru', 'volatile-lfu', 'volatile-random', 'volatile-ttl' or 'noeviction'). Default: 'volatile-lru'
@@ -127,22 +127,22 @@
 
     @protocol.setter
     def protocol(self, value: pulumi.Input[str]):
         pulumi.set(self, "protocol", value)
 
     @property
     @pulumi.getter(name="subscriptionId")
-    def subscription_id(self) -> pulumi.Input[int]:
+    def subscription_id(self) -> pulumi.Input[str]:
         """
         The ID of the subscription to create the database in
         """
         return pulumi.get(self, "subscription_id")
 
     @subscription_id.setter
-    def subscription_id(self, value: pulumi.Input[int]):
+    def subscription_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "subscription_id", value)
 
     @property
     @pulumi.getter(name="throughputMeasurementBy")
     def throughput_measurement_by(self) -> pulumi.Input[str]:
         """
         Throughput measurement method, (either ‘number-of-shards’ or ‘operations-per-second’)
@@ -383,15 +383,15 @@
                  periodic_backup_path: Optional[pulumi.Input[str]] = None,
                  private_endpoint: Optional[pulumi.Input[str]] = None,
                  protocol: Optional[pulumi.Input[str]] = None,
                  public_endpoint: Optional[pulumi.Input[str]] = None,
                  replica_ofs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  replication: Optional[pulumi.Input[bool]] = None,
                  source_ips: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 subscription_id: Optional[pulumi.Input[int]] = None,
+                 subscription_id: Optional[pulumi.Input[str]] = None,
                  support_oss_cluster_api: Optional[pulumi.Input[bool]] = None,
                  throughput_measurement_by: Optional[pulumi.Input[str]] = None,
                  throughput_measurement_value: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering SubscriptionDatabase resources.
         :param pulumi.Input[Sequence[pulumi.Input['SubscriptionDatabaseAlertArgs']]] alerts: A block defining Redis database alert, documented below, can be specified multiple times
         :param pulumi.Input[int] average_item_size_in_bytes: Relevant only to ram-and-flash clusters. Estimated average size (measured in bytes)
@@ -415,15 +415,15 @@
         :param pulumi.Input[str] protocol: The protocol that will be used to access the database, (either ‘redis’ or 'memcached’) Default: ‘redis’
         :param pulumi.Input[str] public_endpoint: Public endpoint to access the database
         :param pulumi.Input[Sequence[pulumi.Input[str]]] replica_ofs: Set of Redis database URIs, in the format `redis://user:password@host:port`, that this
                database will be a replica of. If the URI provided is Redis Labs Cloud instance, only host and port should be provided.
                Cannot be enabled when `support_oss_cluster_api` is enabled.
         :param pulumi.Input[bool] replication: Databases replication. Default: ‘true’
         :param pulumi.Input[Sequence[pulumi.Input[str]]] source_ips: List of source IP addresses or subnet masks. If specified, Redis clients will be able to connect to this database only from within the specified source IP addresses ranges (example: [‘192.168.10.0/32’, ‘192.168.12.0/24’])
-        :param pulumi.Input[int] subscription_id: The ID of the subscription to create the database in
+        :param pulumi.Input[str] subscription_id: The ID of the subscription to create the database in
         :param pulumi.Input[bool] support_oss_cluster_api: Support Redis open-source (OSS) Cluster API. Default: ‘false’
         :param pulumi.Input[str] throughput_measurement_by: Throughput measurement method, (either ‘number-of-shards’ or ‘operations-per-second’)
         :param pulumi.Input[int] throughput_measurement_value: Throughput value (as applies to selected measurement method)
         """
         if alerts is not None:
             pulumi.set(__self__, "alerts", alerts)
         if average_item_size_in_bytes is not None:
@@ -717,22 +717,22 @@
 
     @source_ips.setter
     def source_ips(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "source_ips", value)
 
     @property
     @pulumi.getter(name="subscriptionId")
-    def subscription_id(self) -> Optional[pulumi.Input[int]]:
+    def subscription_id(self) -> Optional[pulumi.Input[str]]:
         """
         The ID of the subscription to create the database in
         """
         return pulumi.get(self, "subscription_id")
 
     @subscription_id.setter
-    def subscription_id(self, value: Optional[pulumi.Input[int]]):
+    def subscription_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "subscription_id", value)
 
     @property
     @pulumi.getter(name="supportOssClusterApi")
     def support_oss_cluster_api(self) -> Optional[pulumi.Input[bool]]:
         """
         Support Redis open-source (OSS) Cluster API. Default: ‘false’
@@ -786,15 +786,15 @@
                  name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  periodic_backup_path: Optional[pulumi.Input[str]] = None,
                  protocol: Optional[pulumi.Input[str]] = None,
                  replica_ofs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  replication: Optional[pulumi.Input[bool]] = None,
                  source_ips: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 subscription_id: Optional[pulumi.Input[int]] = None,
+                 subscription_id: Optional[pulumi.Input[str]] = None,
                  support_oss_cluster_api: Optional[pulumi.Input[bool]] = None,
                  throughput_measurement_by: Optional[pulumi.Input[str]] = None,
                  throughput_measurement_value: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         Creates a Database within a specified Subscription in your Redis Enterprise Cloud Account.
 
@@ -827,15 +827,15 @@
         :param pulumi.Input[str] periodic_backup_path: Path that will be used to store database backup files
         :param pulumi.Input[str] protocol: The protocol that will be used to access the database, (either ‘redis’ or 'memcached’) Default: ‘redis’
         :param pulumi.Input[Sequence[pulumi.Input[str]]] replica_ofs: Set of Redis database URIs, in the format `redis://user:password@host:port`, that this
                database will be a replica of. If the URI provided is Redis Labs Cloud instance, only host and port should be provided.
                Cannot be enabled when `support_oss_cluster_api` is enabled.
         :param pulumi.Input[bool] replication: Databases replication. Default: ‘true’
         :param pulumi.Input[Sequence[pulumi.Input[str]]] source_ips: List of source IP addresses or subnet masks. If specified, Redis clients will be able to connect to this database only from within the specified source IP addresses ranges (example: [‘192.168.10.0/32’, ‘192.168.12.0/24’])
-        :param pulumi.Input[int] subscription_id: The ID of the subscription to create the database in
+        :param pulumi.Input[str] subscription_id: The ID of the subscription to create the database in
         :param pulumi.Input[bool] support_oss_cluster_api: Support Redis open-source (OSS) Cluster API. Default: ‘false’
         :param pulumi.Input[str] throughput_measurement_by: Throughput measurement method, (either ‘number-of-shards’ or ‘operations-per-second’)
         :param pulumi.Input[int] throughput_measurement_value: Throughput value (as applies to selected measurement method)
         """
         ...
     @overload
     def __init__(__self__,
@@ -881,15 +881,15 @@
                  name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  periodic_backup_path: Optional[pulumi.Input[str]] = None,
                  protocol: Optional[pulumi.Input[str]] = None,
                  replica_ofs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  replication: Optional[pulumi.Input[bool]] = None,
                  source_ips: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 subscription_id: Optional[pulumi.Input[int]] = None,
+                 subscription_id: Optional[pulumi.Input[str]] = None,
                  support_oss_cluster_api: Optional[pulumi.Input[bool]] = None,
                  throughput_measurement_by: Optional[pulumi.Input[str]] = None,
                  throughput_measurement_value: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
@@ -960,15 +960,15 @@
             periodic_backup_path: Optional[pulumi.Input[str]] = None,
             private_endpoint: Optional[pulumi.Input[str]] = None,
             protocol: Optional[pulumi.Input[str]] = None,
             public_endpoint: Optional[pulumi.Input[str]] = None,
             replica_ofs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             replication: Optional[pulumi.Input[bool]] = None,
             source_ips: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            subscription_id: Optional[pulumi.Input[int]] = None,
+            subscription_id: Optional[pulumi.Input[str]] = None,
             support_oss_cluster_api: Optional[pulumi.Input[bool]] = None,
             throughput_measurement_by: Optional[pulumi.Input[str]] = None,
             throughput_measurement_value: Optional[pulumi.Input[int]] = None) -> 'SubscriptionDatabase':
         """
         Get an existing SubscriptionDatabase resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
@@ -997,15 +997,15 @@
         :param pulumi.Input[str] protocol: The protocol that will be used to access the database, (either ‘redis’ or 'memcached’) Default: ‘redis’
         :param pulumi.Input[str] public_endpoint: Public endpoint to access the database
         :param pulumi.Input[Sequence[pulumi.Input[str]]] replica_ofs: Set of Redis database URIs, in the format `redis://user:password@host:port`, that this
                database will be a replica of. If the URI provided is Redis Labs Cloud instance, only host and port should be provided.
                Cannot be enabled when `support_oss_cluster_api` is enabled.
         :param pulumi.Input[bool] replication: Databases replication. Default: ‘true’
         :param pulumi.Input[Sequence[pulumi.Input[str]]] source_ips: List of source IP addresses or subnet masks. If specified, Redis clients will be able to connect to this database only from within the specified source IP addresses ranges (example: [‘192.168.10.0/32’, ‘192.168.12.0/24’])
-        :param pulumi.Input[int] subscription_id: The ID of the subscription to create the database in
+        :param pulumi.Input[str] subscription_id: The ID of the subscription to create the database in
         :param pulumi.Input[bool] support_oss_cluster_api: Support Redis open-source (OSS) Cluster API. Default: ‘false’
         :param pulumi.Input[str] throughput_measurement_by: Throughput measurement method, (either ‘number-of-shards’ or ‘operations-per-second’)
         :param pulumi.Input[int] throughput_measurement_value: Throughput value (as applies to selected measurement method)
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SubscriptionDatabaseState.__new__(_SubscriptionDatabaseState)
@@ -1200,15 +1200,15 @@
         """
         List of source IP addresses or subnet masks. If specified, Redis clients will be able to connect to this database only from within the specified source IP addresses ranges (example: [‘192.168.10.0/32’, ‘192.168.12.0/24’])
         """
         return pulumi.get(self, "source_ips")
 
     @property
     @pulumi.getter(name="subscriptionId")
-    def subscription_id(self) -> pulumi.Output[int]:
+    def subscription_id(self) -> pulumi.Output[str]:
         """
         The ID of the subscription to create the database in
         """
         return pulumi.get(self, "subscription_id")
 
     @property
     @pulumi.getter(name="supportOssClusterApi")
```

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud/subscription_peering.py` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud/subscription_peering.py`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud.egg-info/PKG-INFO` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-rediscloud
-Version: 1.2.2
+Version: 1.2.5
 Summary: A Pulumi package for creating and managing rediscloud cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/RedisLabs/pulumi-rediscloud
 Keywords: pulumi rediscloud category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_rediscloud-1.2.2/pulumi_rediscloud.egg-info/SOURCES.txt` & `pulumi_rediscloud-1.2.5/pulumi_rediscloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_rediscloud-1.2.2/setup.py` & `pulumi_rediscloud-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.2.2"
-PLUGIN_VERSION = "1.2.2"
+VERSION = "1.2.5"
+PLUGIN_VERSION = "1.2.5"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'rediscloud', PLUGIN_VERSION, '--server', 'github://api.github.com/RedisLabs/pulumi-rediscloud'])
         except OSError as error:
```

