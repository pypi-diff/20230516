# Comparing `tmp/cognite_power_ops-0.4.2.tar.gz` & `tmp/cognite_power_ops-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_power_ops-0.4.2.tar", max compression
+gzip compressed data, was "cognite_power_ops-0.5.0.tar", max compression
```

## Comparing `cognite_power_ops-0.4.2.tar` & `cognite_power_ops-0.5.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0    10758 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/LICENSE
--rw-r--r--   0        0        0      250 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/README.md
--rw-r--r--   0        0        0       76 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/__init__.py
--rw-r--r--   0        0        0    10260 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/bootstrap.py
--rw-r--r--   0        0        0       65 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/client/__init__.py
--rw-r--r--   0        0        0     6203 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/client/asset_apis.py
--rw-r--r--   0        0        0      601 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/client/config_client.py
--rw-r--r--   0        0        0        0 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/client/dm/__init__.py
--rw-r--r--   0        0        0     1750 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/client/dm/client.py
--rw-r--r--   0        0        0      895 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/client/dm/schema.graphql
--rw-r--r--   0        0        0     2037 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/client/dm/schema.py
--rw-r--r--   0        0        0     1883 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/client/dm_apis.py
--rw-r--r--   0        0        0     2294 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/client/powerops_client.py
--rw-r--r--   0        0        0     2990 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/client/shop_api.py
--rw-r--r--   0        0        0    26552 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/config.py
--rw-r--r--   0        0        0        0 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/data_classes/__init__.py
--rw-r--r--   0        0        0     1221 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/data_classes/asset_lists.py
--rw-r--r--   0        0        0     3057 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/data_classes/benchmarking_config.py
--rw-r--r--   0        0        0     2984 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/data_classes/bid_matrix_generator_config.py
--rw-r--r--   0        0        0    13238 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/data_classes/cdf_resource_collection.py
--rw-r--r--   0        0        0     2513 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/data_classes/common.py
--rw-r--r--   0        0        0      129 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/data_classes/config_model.py
--rw-r--r--   0        0        0     3630 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/data_classes/core.py
--rw-r--r--   0        0        0      128 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/data_classes/generators.py
--rw-r--r--   0        0        0     1482 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/data_classes/market_config.py
--rw-r--r--   0        0        0    16796 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/data_classes/plant.py
--rw-r--r--   0        0        0       99 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/data_classes/price_area.py
--rw-r--r--   0        0        0     5114 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/data_classes/reserve_scenario.py
--rw-r--r--   0        0        0      180 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/data_classes/reservoirs.py
--rw-r--r--   0        0        0     1609 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/data_classes/rkom_bid_combination_config.py
--rw-r--r--   0        0        0      994 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/data_classes/rkom_market_config.py
--rw-r--r--   0        0        0      163 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/data_classes/shared.py
--rw-r--r--   0        0        0     2171 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/data_classes/shop_file_config.py
--rw-r--r--   0        0        0     2815 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/data_classes/shop_output_definition.py
--rw-r--r--   0        0        0     9189 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/data_classes/time_series_mapping.py
--rw-r--r--   0        0        0     1144 2023-05-15 14:13:34.153111 cognite_power_ops-0.4.2/cognite/powerops/data_classes/transformation.py
--rw-r--r--   0        0        0     1042 2023-05-15 14:13:34.157111 cognite_power_ops-0.4.2/cognite/powerops/logger.py
--rw-r--r--   0        0        0     2070 2023-05-15 14:13:34.157111 cognite_power_ops-0.4.2/cognite/powerops/main.py
--rw-r--r--   0        0        0        0 2023-05-15 14:13:34.157111 cognite_power_ops-0.4.2/cognite/powerops/utils/__init__.py
--rw-r--r--   0        0        0     1936 2023-05-15 14:13:34.157111 cognite_power_ops-0.4.2/cognite/powerops/utils/asset_types.py
--rw-r--r--   0        0        0     1424 2023-05-15 14:13:34.157111 cognite_power_ops-0.4.2/cognite/powerops/utils/cdf_auth.py
--rw-r--r--   0        0        0     2724 2023-05-15 14:13:34.157111 cognite_power_ops-0.4.2/cognite/powerops/utils/cdf_utils.py
--rw-r--r--   0        0        0      744 2023-05-15 14:13:34.157111 cognite_power_ops-0.4.2/cognite/powerops/utils/common.py
--rw-r--r--   0        0        0      324 2023-05-15 14:13:34.157111 cognite_power_ops-0.4.2/cognite/powerops/utils/constants.py
--rw-r--r--   0        0        0     3271 2023-05-15 14:13:34.157111 cognite_power_ops-0.4.2/cognite/powerops/utils/files.py
--rw-r--r--   0        0        0     4979 2023-05-15 14:13:34.157111 cognite_power_ops-0.4.2/cognite/powerops/utils/labels.py
--rw-r--r--   0        0        0     1766 2023-05-15 14:13:34.157111 cognite_power_ops-0.4.2/cognite/powerops/utils/mapping/mapping.py
--rw-r--r--   0        0        0     2609 2023-05-15 14:13:34.157111 cognite_power_ops-0.4.2/cognite/powerops/utils/mapping/static_mapping.py
--rw-r--r--   0        0        0     3165 2023-05-15 14:13:34.157111 cognite_power_ops-0.4.2/cognite/powerops/utils/powerops_asset_hierarchy.py
--rw-r--r--   0        0        0      718 2023-05-15 14:13:34.157111 cognite_power_ops-0.4.2/cognite/powerops/utils/powerops_status_events.py
--rw-r--r--   0        0        0     4495 2023-05-15 14:13:34.157111 cognite_power_ops-0.4.2/cognite/powerops/utils/relationship_types.py
--rw-r--r--   0        0        0    11602 2023-05-15 14:13:34.157111 cognite_power_ops-0.4.2/cognite/powerops/utils/resource_generation.py
--rw-r--r--   0        0        0     1495 2023-05-15 14:13:34.157111 cognite_power_ops-0.4.2/cognite/powerops/utils/serializer.py
--rw-r--r--   0        0        0       22 2023-05-15 14:13:34.157111 cognite_power_ops-0.4.2/cognite/powerops/version.py
--rw-r--r--   0        0        0     1434 2023-05-15 14:13:34.157111 cognite_power_ops-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 cognite_power_ops-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    10758 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/LICENSE
+-rw-r--r--   0        0        0      250 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/README.md
+-rw-r--r--   0        0        0       76 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/__init__.py
+-rw-r--r--   0        0        0    10260 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/bootstrap.py
+-rw-r--r--   0        0        0       65 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/client/__init__.py
+-rw-r--r--   0        0        0     6203 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/client/asset_apis.py
+-rw-r--r--   0        0        0      601 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/client/config_client.py
+-rw-r--r--   0        0        0        0 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/client/dm/__init__.py
+-rw-r--r--   0        0        0     1750 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/client/dm/client.py
+-rw-r--r--   0        0        0      895 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/client/dm/schema.graphql
+-rw-r--r--   0        0        0     2037 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/client/dm/schema.py
+-rw-r--r--   0        0        0     1883 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/client/dm_apis.py
+-rw-r--r--   0        0        0     2294 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/client/powerops_client.py
+-rw-r--r--   0        0        0     2990 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/client/shop_api.py
+-rw-r--r--   0        0        0    26552 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/config.py
+-rw-r--r--   0        0        0        0 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/__init__.py
+-rw-r--r--   0        0        0     1221 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/asset_lists.py
+-rw-r--r--   0        0        0     3057 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/benchmarking_config.py
+-rw-r--r--   0        0        0     2984 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/bid_matrix_generator_config.py
+-rw-r--r--   0        0        0    13238 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/cdf_resource_collection.py
+-rw-r--r--   0        0        0     2513 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/common.py
+-rw-r--r--   0        0        0      129 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/config_model.py
+-rw-r--r--   0        0        0     3630 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/core.py
+-rw-r--r--   0        0        0      128 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/generators.py
+-rw-r--r--   0        0        0     1482 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/market_config.py
+-rw-r--r--   0        0        0    16698 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/plant.py
+-rw-r--r--   0        0        0       99 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/price_area.py
+-rw-r--r--   0        0        0     5114 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/reserve_scenario.py
+-rw-r--r--   0        0        0      180 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/reservoirs.py
+-rw-r--r--   0        0        0     1609 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/rkom_bid_combination_config.py
+-rw-r--r--   0        0        0      994 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/rkom_market_config.py
+-rw-r--r--   0        0        0      163 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/shared.py
+-rw-r--r--   0        0        0     2171 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/shop_file_config.py
+-rw-r--r--   0        0        0     2815 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/shop_output_definition.py
+-rw-r--r--   0        0        0     9189 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/time_series_mapping.py
+-rw-r--r--   0        0        0     1144 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/data_classes/transformation.py
+-rw-r--r--   0        0        0     1042 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/logger.py
+-rw-r--r--   0        0        0     2070 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/main.py
+-rw-r--r--   0        0        0        0 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/__init__.py
+-rw-r--r--   0        0        0     1936 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/asset_types.py
+-rw-r--r--   0        0        0     1424 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/cdf_auth.py
+-rw-r--r--   0        0        0     2724 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/cdf_utils.py
+-rw-r--r--   0        0        0      744 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/common.py
+-rw-r--r--   0        0        0      324 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/constants.py
+-rw-r--r--   0        0        0     3271 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/files.py
+-rw-r--r--   0        0        0     5039 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/labels.py
+-rw-r--r--   0        0        0     1766 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/mapping/mapping.py
+-rw-r--r--   0        0        0     2609 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/mapping/static_mapping.py
+-rw-r--r--   0        0        0     3165 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/powerops_asset_hierarchy.py
+-rw-r--r--   0        0        0      718 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/powerops_status_events.py
+-rw-r--r--   0        0        0     4495 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/relationship_types.py
+-rw-r--r--   0        0        0    11602 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/resource_generation.py
+-rw-r--r--   0        0        0     1495 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/utils/serializer.py
+-rw-r--r--   0        0        0       22 2023-05-16 11:32:00.030569 cognite_power_ops-0.5.0/cognite/powerops/version.py
+-rw-r--r--   0        0        0     1434 2023-05-16 11:32:00.034569 cognite_power_ops-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 cognite_power_ops-0.5.0/PKG-INFO
```

### Comparing `cognite_power_ops-0.4.2/LICENSE` & `cognite_power_ops-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/bootstrap.py` & `cognite_power_ops-0.5.0/cognite/powerops/bootstrap.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/client/asset_apis.py` & `cognite_power_ops-0.5.0/cognite/powerops/client/asset_apis.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/client/config_client.py` & `cognite_power_ops-0.5.0/cognite/powerops/client/config_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/client/dm/client.py` & `cognite_power_ops-0.5.0/cognite/powerops/client/dm/client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/client/dm/schema.graphql` & `cognite_power_ops-0.5.0/cognite/powerops/client/dm/schema.graphql`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/client/dm/schema.py` & `cognite_power_ops-0.5.0/cognite/powerops/client/dm/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/client/dm_apis.py` & `cognite_power_ops-0.5.0/cognite/powerops/client/dm_apis.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/client/powerops_client.py` & `cognite_power_ops-0.5.0/cognite/powerops/client/powerops_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/client/shop_api.py` & `cognite_power_ops-0.5.0/cognite/powerops/client/shop_api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/config.py` & `cognite_power_ops-0.5.0/cognite/powerops/config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/data_classes/asset_lists.py` & `cognite_power_ops-0.5.0/cognite/powerops/data_classes/asset_lists.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/data_classes/benchmarking_config.py` & `cognite_power_ops-0.5.0/cognite/powerops/data_classes/benchmarking_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/data_classes/bid_matrix_generator_config.py` & `cognite_power_ops-0.5.0/cognite/powerops/data_classes/bid_matrix_generator_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/data_classes/cdf_resource_collection.py` & `cognite_power_ops-0.5.0/cognite/powerops/data_classes/cdf_resource_collection.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/data_classes/common.py` & `cognite_power_ops-0.5.0/cognite/powerops/data_classes/common.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/data_classes/core.py` & `cognite_power_ops-0.5.0/cognite/powerops/data_classes/core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/data_classes/market_config.py` & `cognite_power_ops-0.5.0/cognite/powerops/data_classes/market_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/data_classes/plant.py` & `cognite_power_ops-0.5.0/cognite/powerops/data_classes/plant.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     # TODO: Consider splitting this into a separate class/subclass
     inlet_level_time_series: Optional[ExternalId] = None  # external ID of time series with values in m.a.s.l.
     outlet_level_time_series: Optional[ExternalId] = None  # external ID of time series with values in m.a.s.l.
     water_value_time_series: Optional[ExternalId] = None  # external ID of time series with values in €/MWh
     feeding_fee_time_series: Optional[ExternalId] = None  # external ID of time series with values in percent
     p_min_time_series: Optional[ExternalId] = None  # external ID of time series with values in MW
     p_max_time_series: Optional[ExternalId] = None  # external ID of time series with values in MW
-    startcost_split_hours_time_series: Optional[ExternalId] = None  # external ID of time series with values in h
+    head_direct: Optional[ExternalId] = None  # external ID of time series with values in m
 
     @validator("penstock_head_loss_factors", pre=True)
     def parse_dict(cls, value):
         if isinstance(value, str):
             value = json.loads(value)
         return value
 
@@ -137,16 +137,16 @@
                 plant.water_value_time_series = ts_ext_id
             elif rl.FEEDING_FEE_TIME_SERIES in labels:
                 plant.feeding_fee_time_series = ts_ext_id
             elif rl.P_MIN_TIME_SERIES in labels:
                 plant.p_min_time_series = ts_ext_id
             elif rl.P_MAX_TIME_SERIES in labels:
                 plant.p_max_time_series = ts_ext_id
-            elif rl.STARTCOST_SPLIT_HOURS_TIME_SERIES in labels:
-                plant.startcost_split_hours_time_series = ts_ext_id
+            elif rl.HEAD_DIRECT in labels:
+                plant.head_direct = ts_ext_id
 
         # Find generators based on relationships
         plant.generator_ext_ids = [
             rel.target_external_id for rel in relationships if label_in_labels(rl.GENERATOR, rel.labels)
         ]
 
         # Find inlet reservoir based on relationships
@@ -228,15 +228,15 @@
             # insert the time series given in the csv file, or None if no time series is specified
             plants[plant].water_value_time_series = time_series.get("Water_value")
             plants[plant].inlet_level_time_series = time_series.get("Inlet_reservoir_level")
             plants[plant].outlet_level_time_series = time_series.get("Outlet_reservoir_level")
             plants[plant].feeding_fee_time_series = time_series.get("Feeding_fee")
             plants[plant].p_min_time_series = time_series.get("P_min")
             plants[plant].p_max_time_series = time_series.get("P_max")
-            plants[plant].startcost_split_hours_time_series = time_series.get("Startcost_split_hours")
+            plants[plant].head_direct = time_series.get("Head_direct")
 
 
 def label_in_labels(label_external_id: str, labels: list[Label]) -> bool:
     """Check if a label with a given external id is in a list of labels."""
     return label_external_id in [label.external_id for label in labels]
```

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/data_classes/reserve_scenario.py` & `cognite_power_ops-0.5.0/cognite/powerops/data_classes/reserve_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/data_classes/rkom_bid_combination_config.py` & `cognite_power_ops-0.5.0/cognite/powerops/data_classes/rkom_bid_combination_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/data_classes/rkom_market_config.py` & `cognite_power_ops-0.5.0/cognite/powerops/data_classes/rkom_market_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/data_classes/shop_file_config.py` & `cognite_power_ops-0.5.0/cognite/powerops/data_classes/shop_file_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/data_classes/shop_output_definition.py` & `cognite_power_ops-0.5.0/cognite/powerops/data_classes/shop_output_definition.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/data_classes/time_series_mapping.py` & `cognite_power_ops-0.5.0/cognite/powerops/data_classes/time_series_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/data_classes/transformation.py` & `cognite_power_ops-0.5.0/cognite/powerops/data_classes/transformation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/logger.py` & `cognite_power_ops-0.5.0/cognite/powerops/logger.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/main.py` & `cognite_power_ops-0.5.0/cognite/powerops/main.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/utils/asset_types.py` & `cognite_power_ops-0.5.0/cognite/powerops/utils/asset_types.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/utils/cdf_auth.py` & `cognite_power_ops-0.5.0/cognite/powerops/utils/cdf_auth.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/utils/cdf_utils.py` & `cognite_power_ops-0.5.0/cognite/powerops/utils/cdf_utils.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/utils/common.py` & `cognite_power_ops-0.5.0/cognite/powerops/utils/common.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/utils/files.py` & `cognite_power_ops-0.5.0/cognite/powerops/utils/files.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/utils/labels.py` & `cognite_power_ops-0.5.0/cognite/powerops/utils/labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     TURBINE_EFFICIENCY_CURVE = "relationship_to.turbine_efficiency_curve"
     P_MIN_TIME_SERIES = "relationship_to.p_min_time_series"
     P_MAX_TIME_SERIES = "relationship_to.p_max_time_series"
     WATER_VALUE_TIME_SERIES = "relationship_to.water_value_time_series"
     FEEDING_FEE_TIME_SERIES = "relationship_to.feeding_fee_time_series"
     INLET_LEVEL_TIME_SERIES = "relationship_to.inlet_level_time_series"
     OUTLET_LEVEL_TIME_SERIES = "relationship_to.outlet_level_time_series"
+    HEAD_DIRECT = "relationship_to.head_direct_time_series"
     STARTCOST_SPLIT_HOURS_TIME_SERIES = "relationship_to.startcost_split_hours_time_series"
 
 
 def label_external_ids(labels_class: Callable) -> list:
     return [v for k, v in labels_class.__dict__.items() if not k.startswith("__")]
```

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/utils/mapping/mapping.py` & `cognite_power_ops-0.5.0/cognite/powerops/utils/mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/utils/mapping/static_mapping.py` & `cognite_power_ops-0.5.0/cognite/powerops/utils/mapping/static_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/utils/powerops_asset_hierarchy.py` & `cognite_power_ops-0.5.0/cognite/powerops/utils/powerops_asset_hierarchy.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/utils/powerops_status_events.py` & `cognite_power_ops-0.5.0/cognite/powerops/utils/powerops_status_events.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/utils/relationship_types.py` & `cognite_power_ops-0.5.0/cognite/powerops/utils/relationship_types.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/utils/resource_generation.py` & `cognite_power_ops-0.5.0/cognite/powerops/utils/resource_generation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/cognite/powerops/utils/serializer.py` & `cognite_power_ops-0.5.0/cognite/powerops/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.4.2/pyproject.toml` & `cognite_power_ops-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-power-ops"
-version = "0.4.2"
+version = "0.5.0"
 description = "SDK for power markets operations on Cognite Data Fusion"
 readme = "README.md"
 authors = ["Cognite <support@cognite.com>"]
 license = "Apache 2.0"
 packages = [{include = "cognite", from = "."}]
 
 [tool.black]
```

### Comparing `cognite_power_ops-0.4.2/PKG-INFO` & `cognite_power_ops-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-power-ops
-Version: 0.4.2
+Version: 0.5.0
 Summary: SDK for power markets operations on Cognite Data Fusion
 License: Apache 2.0
 Author: Cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

