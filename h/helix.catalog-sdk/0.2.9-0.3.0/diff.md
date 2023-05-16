# Comparing `tmp/helix.catalog-sdk-0.2.9.tar.gz` & `tmp/helix.catalog-sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/helix.catalog-sdk-0.2.9.tar", last modified: Tue Jun 28 19:23:47 2022, max compression
+gzip compressed data, was "dist/helix.catalog-sdk-0.3.0.tar", last modified: Mon May 15 23:59:27 2023, max compression
```

## Comparing `helix.catalog-sdk-0.2.9.tar` & `helix.catalog-sdk-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2226 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-06-28 19:23:46.000000 helix.catalog-sdk-0.2.9/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/helix.catalog_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/helix.catalog_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/helix.catalog_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/helix.catalog_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/helix.catalog_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/helix.catalog_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/helix.catalog_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/helix_catalog_sdk/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/helix_catalog_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16614 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/helix_catalog_sdk/catalog.py
--rw-r--r--   0 runner    (1001) docker     (121)     7105 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/helix_catalog_sdk/data_source.py
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/helix_catalog_sdk/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/helix_catalog_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     5756 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/helix_catalog_sdk/repo.py
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2076 2022-06-28 19:23:45.000000 helix.catalog-sdk-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 19:23:47.000000 helix.catalog-sdk-0.2.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17163 2022-06-28 19:22:42.000000 helix.catalog-sdk-0.2.9/tests/test_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-15 23:59:26.000000 helix.catalog-sdk-0.3.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/helix.catalog_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/helix.catalog_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/helix.catalog_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/helix.catalog_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/helix.catalog_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/helix.catalog_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/helix.catalog_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/helix_catalog_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/helix_catalog_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16614 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/helix_catalog_sdk/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/helix_catalog_sdk/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/helix_catalog_sdk/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/helix_catalog_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/helix_catalog_sdk/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-15 23:59:26.000000 helix.catalog-sdk-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:59:27.000000 helix.catalog-sdk-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17530 2023-05-15 23:58:31.000000 helix.catalog-sdk-0.3.0/tests/test_catalog.py
```

### Comparing `helix.catalog-sdk-0.2.9/LICENSE` & `helix.catalog-sdk-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `helix.catalog-sdk-0.2.9/Makefile` & `helix.catalog-sdk-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `helix.catalog-sdk-0.2.9/PKG-INFO` & `helix.catalog-sdk-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helix.catalog-sdk
-Version: 0.2.9
+Version: 0.3.0
 Summary: SDK for interacting with the Helix Data and Connection Catalog
 Home-page: https://github.com/icanbwell/helix.catalog-sdk
 Author: Michael Vidal
 Author-email: michael.vidal@icanbwell.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `helix.catalog-sdk-0.2.9/helix.catalog_sdk.egg-info/PKG-INFO` & `helix.catalog-sdk-0.3.0/helix.catalog_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helix.catalog-sdk
-Version: 0.2.9
+Version: 0.3.0
 Summary: SDK for interacting with the Helix Data and Connection Catalog
 Home-page: https://github.com/icanbwell/helix.catalog-sdk
 Author: Michael Vidal
 Author-email: michael.vidal@icanbwell.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `helix.catalog-sdk-0.2.9/helix.catalog_sdk.egg-info/SOURCES.txt` & `helix.catalog-sdk-0.3.0/helix.catalog_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helix.catalog-sdk-0.2.9/helix_catalog_sdk/catalog.py` & `helix.catalog-sdk-0.3.0/helix_catalog_sdk/catalog.py`

 * *Files identical despite different names*

### Comparing `helix.catalog-sdk-0.2.9/helix_catalog_sdk/data_source.py` & `helix.catalog-sdk-0.3.0/helix_catalog_sdk/data_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,15 @@
         self.name = data_source_name
         self.base_connection = content.base_connection
         self.base_connection_formatted = self.get_connection(content, environment)
         self.production = getattr(content, "production", None)
         self.staging = getattr(content, "staging", None)
         self.qa = getattr(content, "qa", None)
         self.dev = getattr(content, "dev", None)
+        self.client_sandbox = getattr(content, "client_sandbox", None)
         self.connection_type = content.connection_type
         self.resources: List[ResourceItem] = []
         for resource_item in content.resources:
             self.resources.append(
                 ResourceItem(resource_item, self.base_connection_formatted, environment)
             )
         self.pipeline_subscriptions: List[PipelineSubscription] = []
@@ -112,14 +113,18 @@
             base_connection_formatted = content.base_connection.format(
                 env=content.staging
             )
         elif environment == HelixEnvironment.QA:
             base_connection_formatted = content.base_connection.format(env=content.qa)
         elif environment == HelixEnvironment.DEV:
             base_connection_formatted = content.base_connection.format(env=content.dev)
+        elif environment == HelixEnvironment.CLIENT_SANDBOX:
+            base_connection_formatted = content.base_connection.format(
+                env=content.client_sandbox
+            )
 
         return base_connection_formatted
 
     @property
     def json_dict(self) -> Dict[str, Any]:
         json_obj = dict(
             (key, value)
@@ -158,31 +163,35 @@
 
 
 class PipelineSubscription:
     def __init__(self, content: SimpleNamespace):
         if isinstance(content, str):
             self.flow_name: str = content
             self.flow_parameters: List[str] = []
+            self.deployment_name: Optional[str] = None
         else:
             self.flow_name = content.flow_name
             self.flow_parameters = []
             if hasattr(content, "flow_parameters"):
                 self.flow_parameters = content.flow_parameters
+            if hasattr(content, "deployment_name"):
+                self.deployment_name = content.deployment_name
 
     @property
     def json_dict(self) -> Dict[str, Any]:
         return self.__dict__
 
 
 class LastProcessed:
     def __init__(self, content: SimpleNamespace, environment: HelixEnvironment):
         self.dev = content.dev
         self.production = content.production
         self.staging = content.staging
         self.qa = content.qa
+        self.client_sandbox = content.client_sandbox
 
     @property
     def json_dict(self) -> Dict[str, Any]:
         return self.__dict__
 
     def set_last_processed(
         self, last_processed_value: str, environment: HelixEnvironment
@@ -193,8 +202,10 @@
         last_processed_item: str = self.dev
         if environment == HelixEnvironment.PRODUCTION:
             last_processed_item = self.production
         elif environment == HelixEnvironment.STAGING:
             last_processed_item = self.staging
         elif environment == HelixEnvironment.QA:
             last_processed_item = self.qa
+        elif environment == HelixEnvironment.CLIENT_SANDBOX:
+            last_processed_item = self.client_sandbox
         return last_processed_item
```

### Comparing `helix.catalog-sdk-0.2.9/helix_catalog_sdk/repo.py` & `helix.catalog-sdk-0.3.0/helix_catalog_sdk/repo.py`

 * *Files identical despite different names*

### Comparing `helix.catalog-sdk-0.2.9/setup.py` & `helix.catalog-sdk-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `helix.catalog-sdk-0.2.9/tests/test_catalog.py` & `helix.catalog-sdk-0.3.0/tests/test_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,28 +80,33 @@
     things_resource = data_source.resources[2]
     assert things_resource.name == "things"
     assert (
         things_resource.full_path
         == "s3://prod-ingestion/raw/gencon/icd/Things/ThingFeed_06092021.json"
     )
 
-    assert len(data_source.pipeline_subscriptions) == 3
+    assert len(data_source.pipeline_subscriptions) == 4
     pipeline_subscription = data_source.pipeline_subscriptions[0]
     assert pipeline_subscription.flow_name == "Simple subscription"
     assert pipeline_subscription.flow_parameters == []
 
     pipeline_subscription = data_source.pipeline_subscriptions[1]
     assert pipeline_subscription.flow_name == "INGEN Data Ingestion"
     assert pipeline_subscription.flow_parameters == ["people", "places"]
 
     pipeline_subscription = data_source.pipeline_subscriptions[2]
     assert pipeline_subscription.flow_name == "Test Flow"
     assert len(pipeline_subscription.flow_parameters) == 0
     assert pipeline_subscription.flow_parameters == []
 
+    pipeline_subscription = data_source.pipeline_subscriptions[3]
+    assert pipeline_subscription.flow_name == "Prefect Flow"
+    assert pipeline_subscription.flow_parameters == ["places"]
+    assert pipeline_subscription.deployment_name == "Deployment Name"
+
     assert data_source.connection_type == "file"
 
 
 def test_catalog_update_data_source_resource() -> None:
     clean_test_folder()
     repo = DirectoryRepo(location="")
     catalog = Catalog(repo=repo)
@@ -136,15 +141,15 @@
     things_resource = updated_data_source.resources[2]
     assert things_resource.name == "things"
     assert (
         things_resource.full_path
         == "s3://prod-ingestion/raw/gencon/icd/Things/ThingFeed_06092021.json"
     )
 
-    assert len(updated_data_source.pipeline_subscriptions) == 3
+    assert len(updated_data_source.pipeline_subscriptions) == 4
     pipeline_subscription = updated_data_source.pipeline_subscriptions[0]
     assert pipeline_subscription.flow_name == "Simple subscription"
     assert pipeline_subscription.flow_parameters == []
 
     pipeline_subscription = updated_data_source.pipeline_subscriptions[1]
     assert pipeline_subscription.flow_name == "INGEN Data Ingestion"
     assert pipeline_subscription.flow_parameters == ["people", "places"]
@@ -164,14 +169,15 @@
         {
             "load_folders": False,
             "last_processed": {
                 "dev": "s3://dev-ingestion/raw/gencon/icd/People/PeopleFeed_06092021.json",
                 "production": "s3://prod-ingestion/raw/gencon/icd/People/PeopleFeed_06092021.json",
                 "qa": "",
                 "staging": "s3://staging-ingestion/raw/gencon/icd/People/PeopleFeed_06092021.json",
+                "client_sandbox": "s3://prod-ingestion/raw/gencon/icd/People/PeopleFeed_06092021.json",
             },
             "name": "people",
             "path": "People/PeopleFeed_06142021.json",
             "path_slug": "People/PeopleFeed_",
             "date_segment": None,
             "date_format": None,
         },
@@ -441,15 +447,15 @@
     ] = catalog.get_last_processed_dates_for_resources(
         data_source=data_source, environment=HelixEnvironment.PRODUCTION
     )
     assert result[people_resource.name] == datetime.datetime(2021, 11, 11)
 
 
 def test_catalog_get_resource_last_processed_date_for_folders() -> None:
-    clean_test_folder()
+    # clean_test_folder()
     repo = DirectoryRepo(location="")
     catalog = Catalog(repo=repo)
     data_source = catalog.get_data_source(
         "catalog/events/mixpanel/events_parquet.json", HelixEnvironment.PRODUCTION
     )
     assert data_source is not None
     assert data_source is not None
```

