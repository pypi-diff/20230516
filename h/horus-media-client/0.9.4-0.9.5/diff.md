# Comparing `tmp/horus-media-client-0.9.4.tar.gz` & `tmp/horus-media-client-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horus-media-client-0.9.4.tar", last modified: Tue Mar 21 11:10:02 2023, max compression
+gzip compressed data, was "horus-media-client-0.9.5.tar", last modified: Tue May 16 08:01:28 2023, max compression
```

## Comparing `horus-media-client-0.9.4.tar` & `horus-media-client-0.9.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 11:10:02.177545 horus-media-client-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-03-21 11:10:02.177545 horus-media-client-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 11:10:02.173545 horus-media-client-0.9.4/horus_analytics/
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_analytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 11:10:02.173545 horus-media-client-0.9.4/horus_camera/
--rw-r--r--   0 runner    (1001) docker     (123)    20770 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_camera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 11:10:02.173545 horus-media-client-0.9.4/horus_db/
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 11:10:02.173545 horus-media-client-0.9.4/horus_geometries/
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_geometries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 11:10:02.173545 horus-media-client-0.9.4/horus_geopandas/
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_geopandas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 11:10:02.173545 horus-media-client-0.9.4/horus_gis/
--rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_gis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 11:10:02.173545 horus-media-client-0.9.4/horus_media/
--rw-r--r--   0 runner    (1001) docker     (123)    15051 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_media/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 11:10:02.173545 horus-media-client-0.9.4/horus_media_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-03-21 11:10:02.000000 horus-media-client-0.9.4/horus_media_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-03-21 11:10:02.000000 horus-media-client-0.9.4/horus_media_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 11:10:02.000000 horus-media-client-0.9.4/horus_media_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-21 11:10:02.000000 horus-media-client-0.9.4/horus_media_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-21 11:10:02.000000 horus-media-client-0.9.4/horus_media_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 11:10:02.177545 horus-media-client-0.9.4/horus_media_examples/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_media_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_media_examples/clustering_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_media_examples/example_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_media_examples/export_orthographic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_media_examples/export_spherical.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_media_examples/export_time_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_media_examples/geosuite_database_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_media_examples/recordings_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_media_examples/single_measurement_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_media_examples/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_media_examples/spherical_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_media_examples/spherical_camera_single_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_media_examples/spherical_camera_single_measurement_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_media_examples/spherical_camera_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_media_examples/test_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_media_examples/triangulate_spherical_camera_single_measurement_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_media_examples/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 11:10:02.177545 horus-media-client-0.9.4/horus_spatialite/
--rw-r--r--   0 runner    (1001) docker     (123)    17425 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/horus_spatialite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 11:10:02.177545 horus-media-client-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 11:10:02.177545 horus-media-client-0.9.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/tests/test_geopandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/tests/test_gis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-03-21 11:09:49.000000 horus-media-client-0.9.4/tests/test_media.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.073034 horus-media-client-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-16 08:01:28.073034 horus-media-client-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.069034 horus-media-client-0.9.5/horus_analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_analytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.069034 horus-media-client-0.9.5/horus_camera/
+-rw-r--r--   0 runner    (1001) docker     (123)    21170 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_camera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.069034 horus-media-client-0.9.5/horus_db/
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.069034 horus-media-client-0.9.5/horus_geometries/
+-rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_geometries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.069034 horus-media-client-0.9.5/horus_geopandas/
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_geopandas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.069034 horus-media-client-0.9.5/horus_gis/
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_gis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.069034 horus-media-client-0.9.5/horus_media/
+-rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.069034 horus-media-client-0.9.5/horus_media_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-16 08:01:28.000000 horus-media-client-0.9.5/horus_media_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-16 08:01:28.000000 horus-media-client-0.9.5/horus_media_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:01:28.000000 horus-media-client-0.9.5/horus_media_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-16 08:01:28.000000 horus-media-client-0.9.5/horus_media_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-16 08:01:28.000000 horus-media-client-0.9.5/horus_media_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.073034 horus-media-client-0.9.5/horus_media_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/clustering_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/example_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/export_orthographic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/export_spherical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/export_time_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/geosuite_database_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/recordings_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/single_measurement_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/spherical_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/spherical_camera_single_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/spherical_camera_single_measurement_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/spherical_camera_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/test_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/triangulate_spherical_camera_single_measurement_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_media_examples/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.073034 horus-media-client-0.9.5/horus_spatialite/
+-rw-r--r--   0 runner    (1001) docker     (123)    18128 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/horus_spatialite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 08:01:28.073034 horus-media-client-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:28.073034 horus-media-client-0.9.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/tests/test_geopandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/tests/test_gis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-16 08:01:11.000000 horus-media-client-0.9.5/tests/test_media.py
```

### Comparing `horus-media-client-0.9.4/LICENSE.txt` & `horus-media-client-0.9.5/LICENSE.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2019, 2020 Horus View and Explore B.V.
+Copyright (c) 2019, 2020, 2021, 2022, 2023 Horus View and Explore B.V.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `horus-media-client-0.9.4/PKG-INFO` & `horus-media-client-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horus-media-client
-Version: 0.9.4
+Version: 0.9.5
 Summary: Horus Media Server Client
 Home-page: https://github.com/horus-view-and-explore/horus-media-client
 Author: Horus View and Explore B.V.
 Author-email: info@horus.nu
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: OS Independent
```

### Comparing `horus-media-client-0.9.4/README.md` & `horus-media-client-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.4/horus_analytics/__init__.py` & `horus-media-client-0.9.5/horus_analytics/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 import pandas as pd
 import geopandas as gpd
 import fiona
 
 from math import radians, cos, sin, asin, sqrt
 
-def haversine(point1, point2 ): #lon1, lat1, lon2, lat2):
+
+def haversine(point1, point2):  # lon1, lat1, lon2, lat2):
     """
     Calculate the great circle distance between two points
     on the earth (specified in decimal degrees)
     """
 
     lon1 = point1.x
     lat1 = point1.y
@@ -20,107 +21,116 @@
     lat2 = point2.y
 
     # convert decimal degrees to radians
     lon1, lat1, lon2, lat2 = map(radians, [lon1, lat1, lon2, lat2])
     # haversine formula
     dlon = lon2 - lon1
     dlat = lat2 - lat1
-    a = sin(dlat/2)**2 + cos(lat1) * cos(lat2) * sin(dlon/2)**2
+    a = sin(dlat / 2) ** 2 + cos(lat1) * cos(lat2) * sin(dlon / 2) ** 2
     c = 2 * asin(sqrt(a))
     m = 6367000 * c
     return m
 
 
-
 class Clustering_analysis:
-
     cluster_layer: HorusGeoDataFrame
     cluster_location_layer: HorusGeoDataFrame
-    schema_provider:SchemaProvider
+    schema_provider: SchemaProvider
 
-    layers:None
+    layers: None
 
     def __init__(self):
         self.schema_provider = SchemaProvider()
-        self.layers ={}
+        self.layers = {}
 
     def cluster_data_layer(self, filename, layer=None):
         schema = self.schema_provider.merge(
-            self.schema_provider.single_measurement(),
-            self.schema_provider.clustering())
+            self.schema_provider.single_measurement(), self.schema_provider.clustering()
+        )
 
         self.cluster_layer = HorusGeoDataFrame(schema)
-        self.cluster_layer.append_file(filename,layer)
+        self.cluster_layer.append_file(filename, layer)
 
     def cluster_location(self, filename, layer=None):
         schema = self.schema_provider.merge(
-            self.schema_provider.geometry_3dpoint(),
-            self.schema_provider.clustering())
+            self.schema_provider.geometry_3dpoint(), self.schema_provider.clustering()
+        )
         self.cluster_location_layer = HorusGeoDataFrame(schema)
-        self.cluster_location_layer.append_file(filename,layer)
+        self.cluster_location_layer.append_file(filename, layer)
 
     def analyse_cluster_entries(self):
         """
         Adds the cluster_entries_analysis layer with:
         distance: meter to triangulation
         """
 
         schema = SchemaProvider.Schema("Analysis cluster entries")
         schema.fields = [
-            SchemaProvider.Field("geometry", "Row idx (observeration) geometry.",
-                                 SchemaProvider.Geometry(SchemaProvider.Geometry.Type.POINT_3D)),
+            SchemaProvider.Field(
+                "geometry",
+                "Row idx (observeration) geometry.",
+                SchemaProvider.Geometry(SchemaProvider.Geometry.Type.POINT_3D),
+            ),
             SchemaProvider.Field("usr_id", "The id", int),
-            SchemaProvider.Field("distance", "Distance between approximation and triangulation.", int),
-            SchemaProvider.Field("angle", "Angle between camera movement and detected object.", float)
+            SchemaProvider.Field(
+                "distance", "Distance between approximation and triangulation.", int
+            ),
+            SchemaProvider.Field(
+                "angle", "Angle between camera movement and detected object.", float
+            ),
         ]
         database = HorusGeoDataFrame(schema)
 
         loc_df = self.cluster_location_layer.dataframe
         data_df = self.cluster_layer.dataframe
         for index, row in loc_df.iterrows():
-            mask = data_df['clstr_id'] == row['clstr_id']
+            mask = data_df["clstr_id"] == row["clstr_id"]
             entries = data_df.loc[mask]
             for point_i, point_r in entries.iterrows():
                 record = database.new_frame()
-                record['geometry'] = point_r['geometry']
-                record['usr_id'] = point_r['usr_id']
-                record['distance'] = haversine(row['geometry'],point_r['geometry'])
-                record['angle'] = (point_r['dt_yaw'] - point_r['azimuth'])
+                record["geometry"] = point_r["geometry"]
+                record["usr_id"] = point_r["usr_id"]
+                record["distance"] = haversine(row["geometry"], point_r["geometry"])
+                record["angle"] = point_r["dt_yaw"] - point_r["azimuth"]
 
                 database.add_frame(record)
 
         self.layers["cluster_entries_analysis"] = database
 
     def analyse_cluster(self):
         """
         Adds the cluster_analysis layer with:
         distance: meter to triangulation
         """
         schema = SchemaProvider.Schema("Analysis clusters")
         schema.fields = [
-            SchemaProvider.Field("geometry", "Cluster geometry.",
-                                 SchemaProvider.Geometry(SchemaProvider.Geometry.Type.POINT_3D)),
-            SchemaProvider.Field("clstr_pts", "Number of points used for clustering.", int)
+            SchemaProvider.Field(
+                "geometry",
+                "Cluster geometry.",
+                SchemaProvider.Geometry(SchemaProvider.Geometry.Type.POINT_3D),
+            ),
+            SchemaProvider.Field(
+                "clstr_pts", "Number of points used for clustering.", int
+            ),
         ]
         database = HorusGeoDataFrame(schema)
 
         loc_df = self.cluster_location_layer.dataframe
         data_df = self.cluster_layer.dataframe
         for index, row in loc_df.iterrows():
-            mask = data_df['clstr_id'] == row['clstr_id']
+            mask = data_df["clstr_id"] == row["clstr_id"]
             entries = data_df.loc[mask]
 
             record = database.new_frame()
             geoms = []
             for point_i, point_r in entries.iterrows():
-                geoms.append(point_r['geometry'])
-            record['clstr_pts'] = len(geoms)
+                geoms.append(point_r["geometry"])
+            record["clstr_pts"] = len(geoms)
             database.add_frame(record)
 
         self.layers["cluster_analysis"] = database
 
     def write_package(self, filename):
         self.layers["cluster_layer"] = self.cluster_layer
         self.layers["cluster_location_layer"] = self.cluster_location_layer
         for k, v in self.layers.items():
             v.write_geopackage(filename, layer=k)
-
```

### Comparing `horus-media-client-0.9.4/horus_camera/__init__.py` & `horus-media-client-0.9.5/horus_camera/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,91 +1,111 @@
 from PIL import Image, ImageDraw
 from io import BytesIO
 import math
 import io
 
 from horus_db import Frame, Recording
-from horus_media import Client, ImageRequestBuilder, ImageRequest, ImageProvider, Size, Direction, \
-    ComputationRequestBuilder, ComputationProvider, Rect
-from horus_gis import GeographicLocation, RelativeLocation, PositionVector, Geographic, CameraModel
+from horus_media import (
+    Client,
+    ImageRequestBuilder,
+    ImageRequest,
+    ImageProvider,
+    Size,
+    Direction,
+    ComputationRequestBuilder,
+    ComputationProvider,
+    Rect,
+)
+from horus_gis import (
+    GeographicLocation,
+    RelativeLocation,
+    PositionVector,
+    Geographic,
+    CameraModel,
+)
 
 horus_geometries_found = False
 
 try:
     from horus_geometries import Geometry_proj
+
     horus_geometries_found = True
 except:
     pass
 
-class FieldOfView():
+
+class FieldOfView:
     value: float
     min: float
     max: float
 
     def __init__(self, value: float, min: float, max: float):
         self.value = value
         self.min = min
         self.max = max
 
-class Pixel():
+
+class Pixel:
     row: int
     col: int
 
-    def __init__(self, row: int,  col: int):
+    def __init__(self, row: int, col: int):
         self.row = row
         self.col = col
 
 
-class ViewParameterizedPixel():
+class ViewParameterizedPixel:
     """Parameters for georeferencing
 
     The ViewParameterizedPixel is a data structure that
     has all the information that is required for geo-referencing
-    pixels. 
+    pixels.
 
-    ViewParameterizedPixels can be obtained from specific 
+    ViewParameterizedPixels can be obtained from specific
     Imagery that have geo-referencing capabilities, such as the SphericalImage.
 
     A set of 3 different ViewParameterizedPixels from 3 different locations
     can than be used for triangulation resulting in a GeographicLocation.
 
     Attributes:
         name                Label to identify the pixel
         pixel_location      The pixel location in pixel coordinates
         viewing_parameters
         recording_id        The id of the source recording
         frame_index         The index of the source frame in the source recording
         user_data           Dictionary to store optional user-defined data about this pixel
     """
+
     name: str
     pixel_location: Pixel
     viewing_parameters: PositionVector
     recording_id: int
     frame_index: int
     user_data: dict
 
     def __init__(self):
         self.user_data = {}
 
 
 class GeoReferencedPixel(ViewParameterizedPixel):
     """Parameters for georeferencing with GeographicLocation.
 
-    The GeoReferencedPixel is the same data structure as the 
+    The GeoReferencedPixel is the same data structure as the
     ViewParameterizedPixel with an additional GeographicLocation.
 
     A single ViewParameterizedPixel can be turned into a GeoReferencedPixel
     when additional constraints/assumptions are added to the Pixel/PositionVector.
 
-    In the case of the SphericalImage, the function project_pixel_on_ground_surface 
+    In the case of the SphericalImage, the function project_pixel_on_ground_surface
     adds constraints on the altitude coordinate, thus allowing for an estimation
     on the GeographicLocation.
 
     The distance is the ground distance from camera to geo_location.
     """
+
     distance: float
     geo_location: GeographicLocation
     relative_loc: RelativeLocation
 
     def __init__(self, vpp: ViewParameterizedPixel):
         super(GeoReferencedPixel, self).__init__()
         self.name = vpp.name
@@ -98,91 +118,90 @@
 """Horus Camera
 
 The camera
 """
 # Copyright(C) 2019, 2020 Horus View and Explore B.V.
 
 
-class Camera():
-    """The base camera class.
+class Camera:
+    """The base camera class."""
 
-    """
-    h_fov: FieldOfView           # horizontal field of view
-    v_fov: FieldOfView           # vertical field of view
-    yaw: float                   # yaw of the camera ?immutable
-    pitch: float                 # pitch of the camera ?immutable
-    frame: Frame                 # current frame
-    recording: Recording         # current recording
-    network_client: Client       # network client
-    height: float                # height in meters
+    h_fov: FieldOfView  # horizontal field of view
+    v_fov: FieldOfView  # vertical field of view
+    yaw: float  # yaw of the camera ?immutable
+    pitch: float  # pitch of the camera ?immutable
+    frame: Frame  # current frame
+    recording: Recording  # current recording
+    network_client: Client  # network client
+    height: float  # height in meters
 
     def __init__(self):
         self.h_fov = None
         self.v_fov = None
 
     def set_horizontal_fov(self, fov: float):
-        """Adjust the camera's horizontal field of view """
+        """Adjust the camera's horizontal field of view"""
 
         if self.h_fov is None:
-            raise Exception(
-                'This camera does not support horizontal field of view.')
+            raise Exception("This camera does not support horizontal field of view.")
         if fov < self.h_fov.min or fov > self.h_fov.max:
-            raise Exception('Horizontal field of view out of bounds.')
+            raise Exception("Horizontal field of view out of bounds.")
 
         self.h_fov.value = fov
 
     def set_vertical_fov(self, fov: float):
-        """Adjust the camera's vertical field of view """
+        """Adjust the camera's vertical field of view"""
 
         if self.v_fov is None:
-            raise Exception(
-                'This camera does not support vertical field of view.')
+            raise Exception("This camera does not support vertical field of view.")
         if fov < self.v_fov.min or fov > self.v_fov.max:
-            raise Exception('Vertical field of view out of bounds.')
+            raise Exception("Vertical field of view out of bounds.")
 
         self.h_fov.value = fov
 
     def set_frame(self, recording: Recording, frame: Frame):
-        """Places the camera at a specific frame """
+        """Places the camera at a specific frame"""
         self.frame = frame
         self.recording = recording
 
         if recording.setup is not None:
             self.set_camera_height(recording.setup.camera_height)
 
     def set_yaw(self, yaw: float):
-        """Changes the yaw of the camera """
+        """Changes the yaw of the camera"""
         self.yaw = yaw
 
     def set_pitch(self, pitch: float):
-        """Changes the pitch of the camera """
+        """Changes the pitch of the camera"""
         self.pitch = pitch
 
     def set_camera_height(self, height: float):
-        """Changes the height (meters) of the camera with respect to the altitude 
-            of the current frame.
+        """Changes the height (meters) of the camera with respect to the altitude
+        of the current frame.
         """
         self.height = height
 
     def set_network_client(self, client: Client):
-        """Add networking capabilities to the camera """
+        """Add networking capabilities to the camera"""
         self.network_client = client
 
+
 ####################################################################
 #               SPHERICAL CAMERA AND IMAGERY                       #
 ####################################################################
 
 
-class SphericalImage():
-    """ Spherical Image
+class SphericalImage:
+    """Spherical Image
 
-        The result of picture taken through a spherical lens, with the 
-        required information for localization.
+    The result of picture taken through a spherical lens, with the
+    required information for localization.
 
     """
+
     nw_client: Client
     image_provider: ImageProvider
     image_request: ImageRequest
     frame: Frame
     recording: Recording
     camera_height: float
     result = None
@@ -194,157 +213,171 @@
     def __init__(self):
         self.camera_model = None
         self.geo_referenced_pixels = {}
         self.view_parameterized_pixels = {}
         pass
 
     def get_geo_location_camera(self) -> GeographicLocation:
-        """ Returns the geographical position of where the image was taken."""
+        """Returns the geographical position of where the image was taken."""
         return GeographicLocation.from_tuple(self.frame.get_location())
 
     def get_geo_location(self) -> GeographicLocation:
-        """ Returns the geographical position on the ground plane."""
+        """Returns the geographical position on the ground plane."""
         geo = GeographicLocation.from_tuple(self.frame.get_location())
         geo.alt -= self.get_camera_height()
 
     def get_camera_height(self):
-        """ Returns the camera height with respect to the altitude of the geographical altitude."""
+        """Returns the camera height with respect to the altitude of the geographical altitude."""
         return self.camera_height
 
     def get_resolution(self) -> Size:
-        """ Returns the image resolution (width,height)"""
+        """Returns the image resolution (width,height)"""
         # appareturn Size(self.result.w,self.result.h)
         return self.image_request.size
 
     def get_field_of_view(self) -> float:
-        """ Returns the image field of view (horizontal,vertical)"""
+        """Returns the image field of view (horizontal,vertical)"""
         return float(self.image_request.fov)
 
-    def set_network_configuration(self, nw_client, provider, computation, request, camera_height, frame, recording):
-        """ Initializes the SphericalImage for network usage.
-
-            Additional computations are available when a SphericalImage has been captured
-            using a SphericalCamera with a connection to the media-server. In almost all cases
-            the SphericalCamera's network configuration is automatically configured by the SphericalCamera.                            
+    def set_network_configuration(
+        self, nw_client, provider, computation, request, camera_height, frame, recording
+    ):
+        """Initializes the SphericalImage for network usage.
+
+        Additional computations are available when a SphericalImage has been captured
+        using a SphericalCamera with a connection to the media-server. In almost all cases
+        the SphericalCamera's network configuration is automatically configured by the SphericalCamera.
         """
         self.nw_client = nw_client
         self.image_provider = provider
         self.computation_provider = computation
         self.image_request = request
         self.camera_height = camera_height
         self.frame = frame
         self.recording = recording
 
     def fetch(self):
-        """ Fetch the internal contents of the image.
+        """Fetch the internal contents of the image.
 
-            The function fetch allows the user to choose when to fetch the actual imagery data
-            from the media-server. By default the SphericalCamera::get_image(..,manual_fetch:bool) function will perform 
-            the fetch automatically, however changing the manual_fetch:bool variable it is possible to control when to 
-            fetch the actual data.
+        The function fetch allows the user to choose when to fetch the actual imagery data
+        from the media-server. By default the SphericalCamera::get_image(..,manual_fetch:bool) function will perform
+        the fetch automatically, however changing the manual_fetch:bool variable it is possible to control when to
+        fetch the actual data.
         """
 
         client_result = self.nw_client.fetch(self.image_request)
         self.result = self.image_provider.fetch(client_result)
 
     def get_image(self) -> io.BytesIO:
         return self.result.image
 
     def get_camera_model(self) -> CameraModel:
-        """ Returns/Creates a camera model from the current position.
+        """Returns/Creates a camera model from the current position.
 
-            The CameraModel(EnuModel) can be used to make inferences as well as generating 
-            points and polygons in carthesian space.
+        The CameraModel(EnuModel) can be used to make inferences as well as generating
+        points and polygons in carthesian space.
         """
         if self.camera_model == None:
             camera_location = self.frame.get_location()
             camera_heading = self.frame.heading
             if self.recording.setup is not None:
-                self.camera_model = CameraModel.with_leverarms(camera_location, camera_heading,
-                                                               self.recording.setup.lever_arm)
+                self.camera_model = CameraModel.with_leverarms(
+                    camera_location, camera_heading, self.recording.setup.lever_arm
+                )
             else:
-                self.camera_model = CameraModel(
-                    camera_location, camera_heading)
+                self.camera_model = CameraModel(camera_location, camera_heading)
 
         return self.camera_model
 
     def get_view_parameterized_pixel(self, pixel: Pixel) -> ViewParameterizedPixel:
-        """ Returns a ViewParameterizedPixel
+        """Returns a ViewParameterizedPixel
 
-            This function transfroms coordinates x,y (col,row)from pixel space to a
-            postition and view direction (ViewParameterizedPixel).
-            A series of labelled GeoReferencedPixels/ViewParameterizedPixels can be used 
-            for triangulation to obtain a GeographicLocation with higher precision.      
+        This function transfroms coordinates x,y (col,row)from pixel space to a
+        postition and view direction (ViewParameterizedPixel).
+        A series of labelled GeoReferencedPixels/ViewParameterizedPixels can be used
+        for triangulation to obtain a GeographicLocation with higher precision.
         """
         vpp = ViewParameterizedPixel()
         vpp.name = None
         vpp.pixel_location = pixel
         vpp.frame_index = self.frame.index
         vpp.recording_id = self.recording.id
 
         request_builder = ComputationRequestBuilder(
-            self.frame.recordingid, self.frame.uuid)
-        request = self.nw_client.fetch(request_builder.build(self.get_resolution(
-        ), self.image_request.direction, self.get_field_of_view(), pixel.col, pixel.row))
+            self.frame.recordingid, self.frame.uuid
+        )
+        request = self.nw_client.fetch(
+            request_builder.build(
+                self.get_resolution(),
+                self.image_request.direction,
+                self.get_field_of_view(),
+                pixel.col,
+                pixel.row,
+            )
+        )
         result = self.computation_provider.fetch(request)
 
         # yaw is with respect to north
         vpp.viewing_parameters = PositionVector(*result.values())
 
         return vpp
 
     def project_pixel_on_ground_surface(self, pixel: Pixel) -> GeoReferencedPixel:
-        """ Returns a GeoReferencedPixel
+        """Returns a GeoReferencedPixel
 
-            This function maps coordinates x,y (col,row)from pixel space into Geographical
-            space, with the corresponding angles and postion with respect to the camera.
-            It does so by assuming that the horizontal plane is uniform over the entire distance,
-            and that the pixel of interest can be mapped on the surface. 
-            This function is typically used to get an estimate of an object in the image that rests 
-            on the ground floor. A series of labelled GeoReferencedPixels/ViewParameterizedPixels can be used 
-            for triangulation to obtain a GeographicLocation with higher precision.  
+        This function maps coordinates x,y (col,row)from pixel space into Geographical
+        space, with the corresponding angles and postion with respect to the camera.
+        It does so by assuming that the horizontal plane is uniform over the entire distance,
+        and that the pixel of interest can be mapped on the surface.
+        This function is typically used to get an estimate of an object in the image that rests
+        on the ground floor. A series of labelled GeoReferencedPixels/ViewParameterizedPixels can be used
+        for triangulation to obtain a GeographicLocation with higher precision.
         """
 
         grp = GeoReferencedPixel(self.get_view_parameterized_pixel(pixel))
 
         if not -90.0 < grp.viewing_parameters.pitch < 0.0:
             raise Exception(
-                'Pitch {p:2f} is out of range [-90.0, 0.0]'.format(p=grp.viewing_parameters.pitch))
+                "Pitch {p:2f} is out of range [-90.0, 0.0]".format(
+                    p=grp.viewing_parameters.pitch
+                )
+            )
 
         angle = 90 + grp.viewing_parameters.pitch
 
-        ground_north_vector = math.tan(
-            math.radians(angle)) * self.get_camera_height()
+        ground_north_vector = math.tan(math.radians(angle)) * self.get_camera_height()
         vector = SphericalImage.rotate(
-            0, ground_north_vector, 0, 0, math.radians(- grp.viewing_parameters.yaw))
+            0, ground_north_vector, 0, 0, math.radians(-grp.viewing_parameters.yaw)
+        )
         camera_model = self.get_camera_model()
         grp.distance = ground_north_vector
         grp.relative_loc = RelativeLocation(*vector, -self.get_camera_height())
         grp.geo_location = GeographicLocation(
-            *camera_model.to_geodetic(grp.relative_loc.location()))
+            *camera_model.to_geodetic(grp.relative_loc.location())
+        )
 
         return grp
 
     def store_geo_referenced_pixel(self, grp: GeoReferencedPixel):
-        """ Store the GeoReferencedPixel"""
+        """Store the GeoReferencedPixel"""
         self.geo_referenced_pixels[grp.name] = grp
 
     def store_view_parameterized_pixel(self, vvp: ViewParameterizedPixel):
-        """ Store the ViewParameterizedPixel"""
+        """Store the ViewParameterizedPixel"""
         self.view_parameterized_pixels[vvp.name] = vvp
 
     def rotate(x, y, xo, yo, theta):  # rotate x,y around xo,yo by theta (rad)
-        xr = math.cos(theta)*(x-xo)-math.sin(theta)*(y-yo) + xo
-        yr = math.sin(theta)*(x-xo)+math.cos(theta)*(y-yo) + yo
+        xr = math.cos(theta) * (x - xo) - math.sin(theta) * (y - yo) + xo
+        yr = math.sin(theta) * (x - xo) + math.cos(theta) * (y - yo) + yo
         return [xr, yr]
 
     @staticmethod
     def triangulate(label, list_of_images) -> GeographicLocation:
-        """ Triangulate using the stored labelled 
-            ViewParameterizedPixels and GeoReferencedPixels.
+        """Triangulate using the stored labelled
+        ViewParameterizedPixels and GeoReferencedPixels.
         """
         viewing_params_with_label = []
 
         for img in list_of_images:
             for name in img.geo_referenced_pixels:
                 grp: GeoReferencedPixel = img.geo_referenced_pixels[name]
                 if grp.name == label:
@@ -358,95 +391,101 @@
         loc = Geographic.triangulate(viewing_params_with_label)
         return GeographicLocation(loc[1], loc[0], loc[2])
 
 
 class SphericalCamera(Camera):
     """Camera with a spherical lens.
 
-    This class describes a camera with a spherical lens based on the gnomonic projection 
-    https://en.wikipedia.org/wiki/Gnomonic_projection. 
+    This class describes a camera with a spherical lens based on the gnomonic projection
+    https://en.wikipedia.org/wiki/Gnomonic_projection.
 
     The lens has the following properties:
-        horizontal field of view [0,90]  <--- @todo marten
-        vertical field of view [0,90]    <--- @todo marten
+        horizontal field of view [1,180]
+        vertical field of view [1,160]
 
     """
+
     yaw: float
     pitch: float
 
     def __init__(self):
-        """Construct a Spherical camera. """
+        """Construct a Spherical camera."""
         super().__init__()
-        self.h_fov = FieldOfView(90.0, 1.0, 160.0)
+        self.h_fov = FieldOfView(90.0, 1.0, 180.0)
+        self.v_fov = FieldOfView(90.0, 1.0, 160.0)
         self.set_pitch(0)
         self.set_yaw(0)
 
     def set_pitch(self, pitch: float):
         """Adjust the camera's pitch
 
-            The pitch range: 
-            looking down:   -90 deg
-            looking up  :    90 deg
+        The pitch range:
+        looking down:   -90 deg
+        looking up  :    90 deg
 
         """
         self.pitch = pitch
 
     def set_yaw(self, yaw: float):
         """Adjust the camera's yaw
 
-            The yaw range: 
-            max left :  -180 deg
-            max right:   180 deg
+        The yaw range:
+        max left :  -180 deg
+        max right:   180 deg
 
         """
         self.yaw = yaw
 
     def set_horizontal_fov(self, fov: float):
-        """Adjust the camera's horizontal field of view """
+        """Adjust the camera's horizontal field of view"""
         super().set_horizontal_fov(fov)
 
     def set_frame(self, recording: Recording, frame: Frame):
-        """Places the camera at a specific frame """
+        """Places the camera at a specific frame"""
         super().set_frame(recording, frame)
 
     def set_camera_height(self, height: float):
-        """Changes the height (meters) of the camera with respect to the altitude 
-            of the current frame.
+        """Changes the height (meters) of the camera with respect to the altitude
+        of the current frame.
         """
         super().set_camera_height(height)
 
     def set_network_client(self, client: Client):
-        """Add networking capabilities to the camera """
+        """Add networking capabilities to the camera"""
         super().set_network_client(client)
 
     def look_at(self, geo_location: GeographicLocation):
         """Set the view direction yaw/pitch of the current frame to a geographic location"""
         if self.recording.setup is not None:
-            camera_model = CameraModel.with_leverarms(self.frame.get_location(), self.frame.heading,
-                                                      self.recording.setup.lever_arm)
+            camera_model = CameraModel.with_leverarms(
+                self.frame.get_location(),
+                self.frame.heading,
+                self.recording.setup.lever_arm,
+            )
         else:
-            camera_model = CameraModel(
-                self.frame.get_location(), self.frame.heading)
+            camera_model = CameraModel(self.frame.get_location(), self.frame.heading)
 
         yaw, pitch = camera_model.look_at(
-            [geo_location.lon, geo_location.lat, geo_location.alt])
+            [geo_location.lon, geo_location.lat, geo_location.alt]
+        )
         self.set_yaw(yaw - self.frame.heading)
         self.set_pitch(pitch)
 
     def look_at_all(self, geo_locations: [GeographicLocation], width: int):
-
         if not horus_geometries_found:
-            raise Exception('Function not supported, requires horus_geometries.')
+            raise Exception("Function not supported, requires horus_geometries.")
 
         if self.recording.setup is not None:
-            camera_model = CameraModel.with_leverarms(self.frame.get_location(), self.frame.heading,
-                                                      self.recording.setup.lever_arm)
+            camera_model = CameraModel.with_leverarms(
+                self.frame.get_location(),
+                self.frame.heading,
+                self.recording.setup.lever_arm,
+            )
         else:
-            camera_model = CameraModel(
-                self.frame.get_location(), self.frame.heading)
+            camera_model = CameraModel(self.frame.get_location(), self.frame.heading)
 
         gp = Geometry_proj()
         proj = gp.Projection(camera_model, False)
 
         geom = gp.to_enu(gp.geographic_to_polygon(geo_locations), proj).geometry
         c = geom.centroid
         bearing = math.degrees(math.atan2(c.x, c.y))
@@ -456,83 +495,121 @@
         br, tl = [gp.to_point(p) for p in bb.exterior.coords[:-1:2]]
         z = geom.exterior.coords[0][2]
         c = bb.centroid
         ct = gp.to_point([c.x, tl.y, z])
         cb = gp.to_point([c.x, br.y, z])
 
         vfov = camera_model.angle_between(*ct.coords, *cb.coords)
-        hfov = camera_model.angle_between([0, cb.y, cb.z], [max(abs(tl.x), br.x), cb.y, z]) * 2
+        hfov = (
+            camera_model.angle_between([0, cb.y, cb.z], [max(abs(tl.x), br.x), cb.y, z])
+            * 2
+        )
         pitch = camera_model.angle_between(*ct.coords, [0, 0, 1]) + vfov / 2
-        height = int(math.tan(math.radians(vfov) / 2) * width / math.tan(math.radians(hfov) / 2))
+        height = int(
+            math.tan(math.radians(vfov) / 2) * width / math.tan(math.radians(hfov) / 2)
+        )
 
         self.set_yaw(360 - self.frame.heading + bearing)
         self.set_pitch(90 - pitch)
         self.set_horizontal_fov(hfov)
 
         return Size(width, height)
 
-    def crop_to_geometry(self, image:SphericalImage, geo_locations: [GeographicLocation], draw_geometry: bool = False) -> SphericalImage:
-        
+    def crop_to_geometry(
+        self,
+        image: SphericalImage,
+        geo_locations: [GeographicLocation],
+        draw_geometry: bool = False,
+    ) -> SphericalImage:
         if not horus_geometries_found:
-            raise Exception('Function not supported, requires horus_geometries.')
+            raise Exception("Function not supported, requires horus_geometries.")
 
         if self.recording.setup is not None:
-            camera_model = CameraModel.with_leverarms(self.frame.get_location(), self.frame.heading,
-                                            self.recording.setup.lever_arm)
+            camera_model = CameraModel.with_leverarms(
+                self.frame.get_location(),
+                self.frame.heading,
+                self.recording.setup.lever_arm,
+            )
         else:
-            camera_model = CameraModel(
-                self.frame.get_location(), self.frame.heading)
+            camera_model = CameraModel(self.frame.get_location(), self.frame.heading)
 
         size = image.image_request.size
-        computation_request_builder = ComputationRequestBuilder('project')
-        
+        computation_request_builder = ComputationRequestBuilder("project")
+
         points = []
         for p in [*geo_locations, geo_locations[0]]:
             y, p = camera_model.look_at([p.lon, p.lat, p.alt])
-            computation_request = image.nw_client.fetch(computation_request_builder.build(size, Direction(y - self.frame.heading, p), 
-                                        self.h_fov.value, direction0 = Direction(self.yaw, self.pitch)))
+            computation_request = image.nw_client.fetch(
+                computation_request_builder.build(
+                    size,
+                    Direction(y - self.frame.heading, p),
+                    self.h_fov.value,
+                    direction0=Direction(self.yaw, self.pitch),
+                )
+            )
             result = image.computation_provider.fetch(computation_request)
-            if 'error' in result:
-                print(result['error'])
+            if "error" in result:
+                print(result["error"])
             else:
                 x, y = result.values()
                 points.append((x, y))
 
         if len(points) > 0:
             with Image.open(image.get_image()) as im:
                 if draw_geometry:
                     draw = ImageDraw.Draw(im)
                     for i in range(len(points) - 1):
                         draw.line((points[i], points[i + 1]), fill=(12, 255, 36))
 
                 out = BytesIO()
-                im.crop(Geometry_proj().to_polygon(points).bounds).save(out, format="JPEG", quality=95)
-                image.result = ImageProvider.Result(out, [0, 0, size.width, size.height], size.width, size.height)
+                im.crop(Geometry_proj().to_polygon(points).bounds).save(
+                    out, format="JPEG", quality=95
+                )
+                image.result = ImageProvider.Result(
+                    out, [0, 0, size.width, size.height], size.width, size.height
+                )
 
         return image
-    
+
     def acquire(self, size: Size, manual_fetch: bool = False) -> SphericalImage:
         """Acquire a Spherical image from the current position/configuration of the camera"""
 
-        ver_fov = 2 * math.degrees(math.atan(size.height * math.tan(
-            (math.radians(self.h_fov.value)) / 2) / size.width))
+        ver_fov = 2 * math.degrees(
+            math.atan(
+                size.height
+                * math.tan((math.radians(self.h_fov.value)) / 2)
+                / size.width
+            )
+        )
 
-        if not self.h_fov.min < ver_fov < self.h_fov.max:
-            raise Exception('Vertical fov {ver_fov:2f} is out of range [{min:1f}, [{max:1f}]]'.format(
-                ver_fov=ver_fov, min=self.h_fov.min, max=self.h_fov.max))
+        if not self.v_fov.min < ver_fov < self.v_fov.max:
+            raise Exception(
+                "Vertical field of view {ver_fov:2f} is out of range [{min:1f}, {max:1f}]".format(
+                    ver_fov=ver_fov, min=self.v_fov.min, max=self.v_fov.max
+                )
+            )
 
         if self.network_client != None:
             request_builder = ImageRequestBuilder(
-                self.frame.recordingid, self.frame.uuid)
+                self.frame.recordingid, self.frame.uuid
+            )
             request = request_builder.build_spherical(
-                size, Direction(self.yaw, self.pitch), self.h_fov.value)
+                size, Direction(self.yaw, self.pitch), self.h_fov.value
+            )
 
             image = SphericalImage()
-            image.set_network_configuration(self.network_client, ImageProvider(
-            ), ComputationProvider(), request, self.height, self.frame, self.recording)
+            image.set_network_configuration(
+                self.network_client,
+                ImageProvider(),
+                ComputationProvider(),
+                request,
+                self.height,
+                self.frame,
+                self.recording,
+            )
 
             if not manual_fetch:
                 image.fetch()
 
             return image
 
         return None
```

### Comparing `horus-media-client-0.9.4/horus_db/__init__.py` & `horus-media-client-0.9.5/horus_db/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Horus database"""
 # Copyright(C) 2019, 2020, 2021 Horus View and Explore B.V.
 
 import logging
 from typing import NamedTuple
 
+
 class Table:
     attributes = {}
     repr_attributes = ["id"]
 
     def __new__(cls, cursor):
         self = cls._instance = object.__new__(cls)
         self.__result = cursor.fetchone()
@@ -33,16 +34,18 @@
         item = cls(cursor)
         while item:
             yield item
             item = cls(cursor)
 
     def __repr__(self):
         cls = type(self)
-        attrs = ', '.join('{}={}'.format(attr, getattr(self, attr))
-                          for attr in type(self).repr_attributes)
+        attrs = ", ".join(
+            "{}={}".format(attr, getattr(self, attr))
+            for attr in type(self).repr_attributes
+        )
         return f"{cls.__name__}({attrs})"
 
 
 class LeverArm(NamedTuple):
     x: float
     y: float
     z: float
@@ -56,80 +59,82 @@
         "lever_arm_z": "leverArmZ",
         "id": "recording_id",
     }
     repr_attributes = ["id", "camera_height", "lever_arm"]
 
     @property
     def lever_arm(self):
-        return LeverArm(self.leverArmX,
-                        self.leverArmY,
-                        self.leverArmZ)
+        return LeverArm(self.leverArmX, self.leverArmY, self.leverArmZ)
 
 
 class Recording(Table):
     attributes = {
         "directory": "recordingdirectory",
         "bounding_box": "boundingbox",
         "file_format": "fileformat",
     }
     repr_attributes = ["id", "boundingbox"]
     setup: RecordingSetup = None
 
 
 class Frame(Table):
-    attributes = {
-        "heading": "azimuth",
-        "timestamp": "stamp",
-        "uuid": "guid"
-    }
+    attributes = {"heading": "azimuth", "timestamp": "stamp", "uuid": "guid"}
     repr_attributes = ["id", "recordingid", "index"]
 
     def get_location(self):
-        return (
-            self.longitude,
-            self.latitude,
-            self.altitude)
+        return (self.longitude, self.latitude, self.altitude)
 
 
 class RecordingSetups:
     def __init__(self, connection):
         self.__connection = connection
 
     def all(self):
         cursor = self.__connection.cursor()
         cursor.execute('SELECT * FROM "MoviePlayer_recordingsetup"')
         return cursor
 
     def get(self, id):
         cursor = self.__connection.cursor()
-        cursor.execute("""SELECT "cameraHeight", "leverArmX", "leverArmY", "leverArmZ", "recording_id"
-FROM "MoviePlayer_recordingsetup" WHERE recording_id = %s;""", (id,))
+        cursor.execute(
+            """SELECT "cameraHeight", "leverArmX", "leverArmY", "leverArmZ", "recording_id"
+FROM "MoviePlayer_recordingsetup" WHERE recording_id = %s;""",
+            (id,),
+        )
         return cursor
 
 
 class Recordings:
     def __init__(self, connection):
         self.__connection = connection
 
     def get(self, id):
         cursor = self.__connection.cursor()
-        cursor.execute("""SELECT id, recordingdirectory, boundingbox, fileformat
-FROM recordings WHERE id = %s;""", (id,))
+        cursor.execute(
+            """SELECT id, recordingdirectory, boundingbox, fileformat
+FROM recordings WHERE id = %s;""",
+            (id,),
+        )
         return cursor
 
     def get_setup(self, recording):
         cursor = self.__connection.cursor()
-        cursor.execute("""SELECT "cameraHeight", "leverArmX", "leverArmY", "leverArmZ", "recording_id"
-FROM "MoviePlayer_recordingsetup" WHERE recording_id = %s;""", (recording.id,))
+        cursor.execute(
+            """SELECT "cameraHeight", "leverArmX", "leverArmY", "leverArmZ", "recording_id"
+FROM "MoviePlayer_recordingsetup" WHERE recording_id = %s;""",
+            (recording.id,),
+        )
         recording.setup = RecordingSetup(cursor)
 
     def all(self):
         cursor = self.__connection.cursor()
-        cursor.execute("""SELECT id, recordingdirectory, boundingbox, fileformat
-FROM recordings""")
+        cursor.execute(
+            """SELECT id, recordingdirectory, boundingbox, fileformat
+FROM recordings"""
+        )
         return cursor
 
     def query(self, **kwargs):
         select_clause = {
             "id",
             "recordingdirectory",
             "boundingbox",
@@ -164,16 +169,15 @@
                 continue
             if arg == "order_by":
                 if type(value) != tuple:
                     value = (value,)
                 orderby_clause += value
                 continue
 
-            logging.warning(
-                f'Recordings query unknown argument "{arg}" skipped')
+            logging.warning(f'Recordings query unknown argument "{arg}" skipped')
 
         sql = "SELECT " + ", ".join(select_clause) + " FROM recordings"
 
         if len(where_clause) > 0:
             sql += " WHERE " + " AND ".join(where_clause)
 
         if len(orderby_clause) > 0:
@@ -200,38 +204,41 @@
             "latitude",
             "longitude",
             "altitude",
             "roll",
             "pitch",
             "azimuth",
             "stamp",
-            "index"
+            "index",
         }
         where_clause = []
         orderby_clause = []
         params = []
         tail = []
 
         for arg, value in kwargs.items():
             if value == None:
                 continue
             if arg == "within":
                 point, distance = value
                 st_point = f"ST_SetSRID(ST_Point({point[0]}, {point[1]}), 4326)"
                 select_clause.add(
-                    f"ST_Distance(geom::geography, {st_point}::geography) as distance")
+                    f"ST_Distance(geom::geography, {st_point}::geography) as distance"
+                )
                 orderby_clause.append("distance")
                 where_clause.append(
-                    f"ST_DWithin(geom::geography, {st_point}::geography, {distance})")
+                    f"ST_DWithin(geom::geography, {st_point}::geography, {distance})"
+                )
                 continue
             if arg == "distance":
                 point, operator, distance = value
                 st_point = f"ST_SetSRID(ST_Point({point[0]}, {point[1]}), 4326)"
                 where_clause.append(
-                    f"ST_Distance(geom::geography, {st_point}::geography) {operator}")
+                    f"ST_Distance(geom::geography, {st_point}::geography) {operator}"
+                )
                 params.append(distance)
                 continue
             if arg == "time_interval":
                 start, end = value
                 orderby_clause.append("stamp")
                 where_clause.append(f"stamp BETWEEN '{start}' AND '{end}'")
                 continue
```

### Comparing `horus-media-client-0.9.4/horus_geometries/__init__.py` & `horus-media-client-0.9.5/horus_geometries/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,208 +5,215 @@
 try:
     import shapely as SP
     from shapely import geometry
     import pyproj as PP
 except ModuleNotFoundError as e:
     print(f"Install module '{e.name}' to use this module.")
     raise e
-    
-class Geometry_proj:
 
+
+class Geometry_proj:
     class Projection:
-        def __init__(self, model=None,is_enu=None,geometry=None,geod=None) -> None:
-            self.model:HG.EnuModel = model
-            self.is_enu:bool = is_enu
+        def __init__(self, model=None, is_enu=None, geometry=None, geod=None) -> None:
+            self.model: HG.EnuModel = model
+            self.is_enu: bool = is_enu
             self.geometry = geometry
             self.geod: PP.Geod = geod
 
-    def create_projection(self,geom):                
-        
+    def create_projection(self, geom):
         proj = Geometry_proj.Projection()
         proj.geod = PP.Geod(ellps="WGS84")
-        proj.is_enu = False       
+        proj.is_enu = False
 
-        if geom.type == "Polygon":
+        if geom.geom_type == "Polygon":
             proj.model = HG.EnuModel(geom.exterior.coords[0])
-        elif geom.type == "LineString" or geom.type == "Point":
+        elif geom.geom_type == "LineString" or geom.geom_type == "Point":
             proj.model = HG.EnuModel(geom.coords[0])
         else:
             raise Exception("Geometry_proj not supported geometry.")
-                
+
         return proj
 
     def to_polygon(self, values):
         return SP.geometry.Polygon(values)
 
     def to_linestring(self, values):
         return SP.geometry.LineString(values)
 
     def to_point(self, value):
         return SP.geometry.Point(value)
 
-    def geographic_to_polygon(self,geoms:[HG.GeographicLocation]):
-        return self.to_polygon([[x.lon,x.lat,x.alt] for x in geoms])
+    def geographic_to_polygon(self, geoms: [HG.GeographicLocation]):
+        return self.to_polygon([[x.lon, x.lat, x.alt] for x in geoms])
 
-    def geographic_to_linestring(self,geoms:[HG.GeographicLocation]):
-        return self.to_linestring([[x.lon,x.lat,x.alt] for x in geoms])
+    def geographic_to_linestring(self, geoms: [HG.GeographicLocation]):
+        return self.to_linestring([[x.lon, x.lat, x.alt] for x in geoms])
 
-    def geographic_to_point(self,geom:HG.GeographicLocation):
-        return self.to_point([geom.lon,geom.lat,geom.alt])
+    def geographic_to_point(self, geom: HG.GeographicLocation):
+        return self.to_point([geom.lon, geom.lat, geom.alt])
 
     def to_geographic(self, geometry):
-        if geometry.type == "Polygon":
-            return [HG.GeographicLocation(*x) for x in geometry.exterior.coords] 
+        if geometry.geom_type == "Polygon":
+            return [HG.GeographicLocation(*x) for x in geometry.exterior.coords]
         return [HG.GeographicLocation(*x) for x in geometry.coords]
 
     def bounding_box(self, geometry):
         return SP.geometry.box(*geometry.bounds)
 
     def rotate(self, geometry, projection, angle):
-        return SP.geometry.Polygon([projection.model.rotate(p, math.radians(angle)) for p in geometry.exterior.coords])
+        return SP.geometry.Polygon(
+            [
+                projection.model.rotate(p, math.radians(angle))
+                for p in geometry.exterior.coords
+            ]
+        )
 
-    def to_enu(self,geom, projection:Projection = None):
-                
-        if projection is None:        
+    def to_enu(self, geom, projection: Projection = None):
+        if projection is None:
             projection = self.create_projection(geom)
-            
+
         projection.is_enu = True
 
-        if geom.type == "Polygon":
+        if geom.geom_type == "Polygon":
             enu_list = [projection.model.to_enu(e) for e in geom.exterior.coords]
             projection.geometry = SP.geometry.Polygon(enu_list)
-        
-        elif geom.type == "LineString":
+
+        elif geom.geom_type == "LineString":
             enu_list = [projection.model.to_enu(e) for e in geom.coords]
             projection.geometry = SP.geometry.LineString(enu_list)
-        
-        elif geom.type == "Point":
+
+        elif geom.geom_type == "Point":
             enu_point = projection.model.to_enu(*geom.coords)
-            projection.geometry = SP.geometry.Point(enu_point)   
+            projection.geometry = SP.geometry.Point(enu_point)
         else:
             raise Exception("Geometry_proj not supported geometry.")
-        
+
         return projection
-    
-    def to_geodetic(self,geom, projection:Projection):
-                
-        if projection is None:        
+
+    def to_geodetic(self, geom, projection: Projection):
+        if projection is None:
             raise Exception("Geometry_proj::to_wgs requires a projection.")
-        
+
         if not projection.is_enu:
             raise Exception("Geometry_proj::to_wgs projection should be in enu.")
-        
+
         p = Geometry_proj.Projection()
         p.model = projection.model
         p.geod = projection.geod
 
-        if geom.type == "Polygon":
+        if geom.geom_type == "Polygon":
             geo_list = [projection.model.to_geodetic(e) for e in geom.exterior.coords]
             p.geometry = SP.geometry.Polygon(geo_list)
             p.is_enu = False
-        
-        elif geom.type == "LineString":
+
+        elif geom.geom_type == "LineString":
             geo_list = [projection.model.to_geodetic(e) for e in geom.coords]
             p.geometry = SP.geometry.LineString(geo_list)
             p.is_enu = False
-                    
-        elif geom.type == "Point":
+
+        elif geom.geom_type == "Point":
             geo_point = projection.model.to_geodetic(*geom.coords)
             p.geometry = SP.geometry.Point(geo_point)
-            p.is_enu = False     
+            p.is_enu = False
         else:
             raise Exception("Geometry_proj not supported geometry.")
-        
+
         return p
 
-    def split_linestring(self,geometry,max_length:float):
+    def split_linestring(self, geometry, max_length: float):
         projection = self.create_projection(geometry)
-        projection.geometry = geometry        
-        
-        return [ x.geometry for x in self.split_linestring_proj(projection,max_length)]
+        projection.geometry = geometry
 
-    def split_linestring_proj(self,projection:Projection,max_length:float):
+        return [x.geometry for x in self.split_linestring_proj(projection, max_length)]
 
+    def split_linestring_proj(self, projection: Projection, max_length: float):
         proj = projection
         incomming_is_enu = proj.is_enu
-        
+
         if not incomming_is_enu:
             proj = self.to_enu(proj.geometry)
-        
+
         length = proj.geometry.length
         equal_distance = length / math.ceil(length / max_length)
 
         linestrings = []
         points = []
 
-        geoms  = list(proj.geometry.coords)
+        geoms = list(proj.geometry.coords)
         while len(geoms) > 0:
             cp = geoms.pop(0)
 
             if len(points) >= 1:
-                linestring = SP.geometry.LineString([*points,cp])
-                
+                linestring = SP.geometry.LineString([*points, cp])
+
                 if linestring.length <= equal_distance:
                     points.append(cp)
                 else:
                     split_point = linestring.interpolate(equal_distance)
-                    linestring = SP.geometry.LineString([*points,split_point])
+                    linestring = SP.geometry.LineString([*points, split_point])
                     linestrings.append(linestring)
-                    geoms.insert(0,cp)
-                    geoms.insert(0,split_point)
+                    geoms.insert(0, cp)
+                    geoms.insert(0, split_point)
                     points = []
             else:
                 points.append(cp)
 
         if len(points) > 1:
             linestring = SP.geometry.LineString(points)
             if linestring.length > 0.01:
                 linestrings.append(linestring)
-    
+
         projections = []
         for l in linestrings:
-             p = Geometry_proj.Projection()
-             p.geometry = l
-             p.is_enu = proj.is_enu
-             p.geod = proj.geod
-             p.model = proj.model
-             projections.append(p)
-    
+            p = Geometry_proj.Projection()
+            p.geometry = l
+            p.is_enu = proj.is_enu
+            p.geod = proj.geod
+            p.model = proj.model
+            projections.append(p)
+
         if not incomming_is_enu:
-            projections = [self.to_geodetic(proj.geometry,proj) for proj in projections]
-                
+            projections = [
+                self.to_geodetic(proj.geometry, proj) for proj in projections
+            ]
+
         return projections
 
-    def point_to_square(self,geometry,width:float):        
+    def point_to_square(self, geometry, width: float):
         projection = self.create_projection(geometry)
-        projection.geometry = geometry        
+        projection.geometry = geometry
 
-        return self.point_square_proj(projection,width).geometry
+        return self.point_square_proj(projection, width).geometry
 
-    def point_square_proj(self,projection:Projection,width):
+    def point_square_proj(self, projection: Projection, width):
         s = width / 2.0
-        square =  SP.geometry.Polygon([(s, s, 0), (-s, s, 0), (-s, -s, 0), (s, -s, 0)])
+        square = SP.geometry.Polygon([(s, s, 0), (-s, s, 0), (-s, -s, 0), (s, -s, 0)])
         projection.is_enu = True
-        return self.to_geodetic(square,projection)
+        return self.to_geodetic(square, projection)
 
     def buffer(self, geometry, value):
         projection = self.create_projection(geometry)
-        projection.geometry = geometry        
+        projection.geometry = geometry
 
         return self.buffer_proj(projection, value).geometry
 
     def buffer_proj(self, projection, value):
         proj = projection
         incomming_is_enu = proj.is_enu
-        
+
         if not incomming_is_enu:
             proj = self.to_enu(proj.geometry)
 
-        if proj.geometry.type == "Polygon":
+        if proj.geometry.geom_type == "Polygon":
             z = proj.geometry.exterior.coords[0][2]
-        elif proj.geometry.type == "LineString" or proj.geometry.type == "Point":
+        elif (
+            proj.geometry.geom_type == "LineString"
+            or proj.geometry.geom_type == "Point"
+        ):
             z = proj.geometry.coords[0][2]
         else:
             raise Exception("Geometry_proj not supported geometry.")
 
-        geom = SP.geometry.Polygon([(*p, z) for p in proj.geometry.buffer(value).exterior.coords])        
-        return self.to_geodetic(geom,proj)          
-
+        geom = SP.geometry.Polygon(
+            [(*p, z) for p in proj.geometry.buffer(value).exterior.coords]
+        )
+        return self.to_geodetic(geom, proj)
```

### Comparing `horus-media-client-0.9.4/horus_geopandas/__init__.py` & `horus-media-client-0.9.5/horus_geopandas/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,82 +13,95 @@
     import fiona as fi
     from fiona.crs import from_epsg
     import geopandas as gpd
 except ModuleNotFoundError as e:
     print(f"Install module '{e.name}' to use this module.")
     raise e
 
-class HorusGeoDataFrame:
 
+class HorusGeoDataFrame:
     schema: SchemaProvider.Schema
     dataframe: gpd.GeoDataFrame
     non_geom_schema: pa.DataFrameSchema
-    fiona_schema:dict
-    crs:str
+    fiona_schema: dict
+    crs: str
 
-    fields:None
-    def __init__(self,schema:SchemaProvider.Schema):
+    fields: None
 
+    def __init__(self, schema: SchemaProvider.Schema):
         self.crs = "EPSG:4326"
         self.schema = schema
 
         # Convert schema's
         # https://pandera.readthedocs.io/en/latest/dataframe_schemas.html
         the_geom_field = False
 
         pan_schema = {}
-        self.fiona_schema = {'geometry':None, 'properties':{}}
-        self.fields=[]
+        self.fiona_schema = {"geometry": None, "properties": {}}
+        self.fields = []
         for field in self.schema.fields:
-            is_geom:bool = type(field.type) is hg.SchemaProvider.Geometry
+            is_geom: bool = type(field.type) is hg.SchemaProvider.Geometry
 
             if is_geom:
                 pan_schema[field.name] = pa.Column(pa.engines.pandas_engine.Geometry)
                 self.fiona_schema[field.name] = str(field.type)
             else:
                 pan_schema[field.name] = pa.Column(field.type)
-                self.fiona_schema['properties'][field.name] = \
-                    list(fi.FIELD_TYPES_MAP.keys())[list(fi.FIELD_TYPES_MAP.values()).index(field.type)]
+                self.fiona_schema["properties"][field.name] = list(
+                    fi.FIELD_TYPES_MAP.keys()
+                )[list(fi.FIELD_TYPES_MAP.values()).index(field.type)]
 
             self.fields.append(field.name)
-        
-        self.non_geom_schema = pa.DataFrameSchema(pan_schema,
+
+        self.non_geom_schema = pa.DataFrameSchema(
+            pan_schema,
             index=pa.Index(int),
             strict=True,
-            coerce=True,)
+            coerce=True,
+        )
 
-        self.dataframe = gpd.GeoDataFrame(columns = self.fields)
+        self.dataframe = gpd.GeoDataFrame(columns=self.fields)
         self.at = self.dataframe.at
 
     def new_frame(self, geom=None):
         if geom is None:
-            geom = gpd.points_from_xy([0], [0],[0])
-        return gpd.GeoDataFrame(columns = self.fields, geometry=geom,crs=self.crs)
+            geom = gpd.points_from_xy([0], [0], [0])
+        return gpd.GeoDataFrame(columns=self.fields, geometry=geom, crs=self.crs)
 
     def add_frame(self, dataframe, validate=True):
         if validate:
             self.non_geom_schema.validate(dataframe)
         self.dataframe = pd.concat([self.dataframe, dataframe])
 
-    def append_file(self,filename, layer=None,default_values={}):
-        dataframe = gpd.read_file(filename,layer=layer, schema=self.fiona_schema)
+    def append_file(self, filename, layer=None, default_values={}):
+        dataframe = gpd.read_file(filename, layer=layer, schema=self.fiona_schema)
 
         for dv in default_values.keys():
             dataframe[dv] = default_values[dv]
 
         self.non_geom_schema.validate(dataframe)
 
         self.dataframe = pd.concat([self.dataframe, dataframe])
 
     def write_shapefile(self, filename):
-        self.dataframe.to_file(filename, crs=from_epsg(int(self.crs.split(':')[1])), 
-        schema=self.fiona_schema)
+        self.dataframe.to_file(
+            filename,
+            crs=from_epsg(int(self.crs.split(":")[1])),
+            schema=self.fiona_schema,
+        )
 
     def write_geojson(self, filename):
-        self.dataframe.to_file(filename, driver='GeoJSON', crs=from_epsg(int(self.crs.split(':')[1])), 
-        schema=self.fiona_schema)
-        
-    def write_geopackage(self,filename,layer):
-        self.dataframe.to_file(filename, layer=layer, driver="GPKG", crs=from_epsg(int(self.crs.split(':')[1])), 
-        schema=self.fiona_schema)
-
-
+        self.dataframe.to_file(
+            filename,
+            driver="GeoJSON",
+            crs=from_epsg(int(self.crs.split(":")[1])),
+            schema=self.fiona_schema,
+        )
+
+    def write_geopackage(self, filename, layer):
+        self.dataframe.to_file(
+            filename,
+            layer=layer,
+            driver="GPKG",
+            crs=from_epsg(int(self.crs.split(":")[1])),
+            schema=self.fiona_schema,
+        )
```

### Comparing `horus-media-client-0.9.4/horus_gis/__init__.py` & `horus-media-client-0.9.5/horus_gis/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,22 +9,26 @@
 import math
 import argparse
 from typing import NamedTuple
 from ast import literal_eval
 from scipy.spatial.transform import Rotation
 from enum import Enum
 
+
 def angle_between(v1, v2, up=numpy.array((0, 0, 1))):
-    """ Returns the angle in radians between vectors 'v1' and 'v2'
+    """Returns the angle in radians between vectors 'v1' and 'v2'
 
     The angle is oriented according to the up vector.
     """
 
-    angle = numpy.arccos(numpy.clip(numpy.dot(v1 / numpy.linalg.norm(v1), \
-                v2 / numpy.linalg.norm(v2)), -1.0, 1.0))
+    angle = numpy.arccos(
+        numpy.clip(
+            numpy.dot(v1 / numpy.linalg.norm(v1), v2 / numpy.linalg.norm(v2)), -1.0, 1.0
+        )
+    )
     if numpy.dot(numpy.cross(v1, v2), up) < 0:
         return -angle
     return angle
 
 
 def xyz_to_yxz(p):
     """Swaps x and y iterating over a 3D vector"""
@@ -37,16 +41,15 @@
     try:
         value = literal_eval(f"({string})")
         value = tuple(map(lambda x: float(x), value))
         if len(value) == 3:
             return value
     except:
         pass
-    raise argparse.ArgumentTypeError(
-        "'{string}' is not a valid location")
+    raise argparse.ArgumentTypeError("'{string}' is not a valid location")
 
 
 class EnuModel:
     """East North Up spatial of reference
 
     Conversions between ENU and Geodetic."""
 
@@ -54,16 +57,19 @@
     north = numpy.array((0, 1, 0))
     up = numpy.array((0, 0, 1))
 
     def __init__(self, geodeticPoint):
         self.geodeticPoint = geodeticPoint
 
     def to_enu(self, geodeticPoint):
-        return numpy.array(pymap3d.geodetic2enu(
-            *xyz_to_yxz(geodeticPoint), *xyz_to_yxz(self.geodeticPoint)))
+        return numpy.array(
+            pymap3d.geodetic2enu(
+                *xyz_to_yxz(geodeticPoint), *xyz_to_yxz(self.geodeticPoint)
+            )
+        )
 
     def to_geodetic(self, point):
         """
         ENU to Azimuth, Elevation, Range
 
         Parameters
         ----------
@@ -71,259 +77,328 @@
         point : collection
             ENU point (meters, meters, meters)
 
         Results
         -------
             WGS84 point (lon, lat, alt)
         """
-        return numpy.array([x for x in xyz_to_yxz(
-            pymap3d.enu2geodetic(*point, *xyz_to_yxz(self.geodeticPoint)))])
+        return numpy.array(
+            [
+                x
+                for x in xyz_to_yxz(
+                    pymap3d.enu2geodetic(*point, *xyz_to_yxz(self.geodeticPoint))
+                )
+            ]
+        )
 
     def rotate(self, point, angle):
-        r = Rotation.from_euler('z', angle, degrees=True)
+        r = Rotation.from_euler("z", angle, degrees=True)
         return r.apply(point)
 
     def to_orientation(self, angle):
         # should use altitude ?
         return self.rotate(EnuModel.north, angle)
 
     def angle_between(self, v1, v2):
         return math.degrees(angle_between(v1, v2, [0, 0, 0]))
 
     def get_heading(self, point):
         return math.degrees(angle_between(EnuModel.north, point))
-    
+
     def get_direction(self, point):
         yaw = (math.degrees(math.atan2(*point[:2])) + 360) % 360
-        r = Rotation.from_euler('z', yaw, degrees=True)
+        r = Rotation.from_euler("z", yaw, degrees=True)
         pitch = 90 - math.degrees(math.atan2(*(r.apply(point)[1:3])))
         return [yaw, pitch]
 
 
 class CameraModel(EnuModel):
     def __init__(self, origin, heading):
         super(CameraModel, self).__init__(origin)
         self.orientation = self.to_orientation(-heading)
 
     @staticmethod
     def with_leverarms(origin, heading, leverarms):
         enu = EnuModel(origin)
-        r = Rotation.from_euler('z', -heading + 90.0, degrees=True)
+        r = Rotation.from_euler("z", -heading + 90.0, degrees=True)
         return CameraModel(enu.to_geodetic(r.apply(leverarms)), heading)
 
     def look_at(self, location):
         return self.get_direction(self.to_enu(location))
 
     def look_at_angle(self, location):
         enu_location = self.to_enu(location)
         return math.degrees(angle_between(self.orientation, enu_location))
 
 
-class GeographicLocation():
+class GeographicLocation:
     """GeographicLocation longitude,latitude,altitude
 
-    Geographic location refers to a position on the Earth. 
+    Geographic location refers to a position on the Earth.
     Your absolute geographic location is defined by two coordinates,
     longitude and latitude. In the case of imagery, the altitude is added/required
     to be able to georeference pixels from this imagery.
 
     The reference system is that in which the recording has been stored in the database,
-    which is usually EPSG Projection 4326 - WGS 84. 
+    which is usually EPSG Projection 4326 - WGS 84.
     """
+
     lat: float
     lon: float
     alt: float
 
     def __init__(self, lon: float, lat: float, alt: float):
         self.lon = lon
         self.lat = lat
         self.alt = alt
 
     @staticmethod
     def from_tuple(tuple_lon_lat_alt):
         return GeographicLocation(
-            tuple_lon_lat_alt[0],
-            tuple_lon_lat_alt[1],
-            tuple_lon_lat_alt[2])
+            tuple_lon_lat_alt[0], tuple_lon_lat_alt[1], tuple_lon_lat_alt[2]
+        )
 
 
-class RelativeLocation():
+class RelativeLocation:
     """RelativeLocation, east, north, up
 
-        The relative location in meters using the ENU coordinate system.
+    The relative location in meters using the ENU coordinate system.
     """
+
     east: float
     north: float
     up: float
 
     def __init__(self, east: float, north: float, up: float):
         self.east = east
         self.north = north
         self.up = up
 
     def location(self):
         return [self.east, self.north, self.up]
 
+
 class PositionVector(NamedTuple):
     lat: float
     lon: float
     alt: float
     yaw: float
     pitch: float
 
+
 class Geographic:
     @staticmethod
     def __normalize(v):
         norm = numpy.linalg.norm(v)
-        if norm == 0: 
+        if norm == 0:
             return v
         return v / norm
 
     @staticmethod
     def __get_line(lat, lon, alt, bearing, pitch):
         p = pymap3d.geodetic2ecef(lat, lon, alt)
 
-        d = numpy.array([math.cos(math.radians(pitch)) * math.sin(math.radians(bearing)),
-                        math.cos(math.radians(pitch)) * math.cos(math.radians(bearing)),
-                        math.sin(math.radians(pitch))])
-
-        m = numpy.array([[-1 * math.sin(math.radians(lon)), 
-                        -1 * math.sin(math.radians(lat)) * math.cos(math.radians(lon)), 
-                        math.cos(math.radians(lat)) * math.cos(math.radians(lon))], 
-                        [math.cos(math.radians(lon)), 
-                        -1 * math.sin(math.radians(lat)) * math.sin(math.radians(lon)), 
-                        math.cos(math.radians(lat)) * math.sin(math.radians(lon))],
-                        [0, math.cos(math.radians(lat)), math.sin(math.radians(lat))]])
+        d = numpy.array(
+            [
+                math.cos(math.radians(pitch)) * math.sin(math.radians(bearing)),
+                math.cos(math.radians(pitch)) * math.cos(math.radians(bearing)),
+                math.sin(math.radians(pitch)),
+            ]
+        )
+
+        m = numpy.array(
+            [
+                [
+                    -1 * math.sin(math.radians(lon)),
+                    -1 * math.sin(math.radians(lat)) * math.cos(math.radians(lon)),
+                    math.cos(math.radians(lat)) * math.cos(math.radians(lon)),
+                ],
+                [
+                    math.cos(math.radians(lon)),
+                    -1 * math.sin(math.radians(lat)) * math.sin(math.radians(lon)),
+                    math.cos(math.radians(lat)) * math.sin(math.radians(lon)),
+                ],
+                [0, math.cos(math.radians(lat)), math.sin(math.radians(lat))],
+            ]
+        )
 
         d = m.dot(d)
         d = Geographic.__normalize(d)
 
         return p, d
 
     @staticmethod
     def __get_point(lines):
-        m = numpy.zeros([3,3])
-        left = numpy.zeros([3,3])
+        m = numpy.zeros([3, 3])
+        left = numpy.zeros([3, 3])
         right = numpy.zeros([3])
 
         for origin, direction in lines:
-            m = numpy.identity(3) - \
-                numpy.column_stack([numpy.array([direction * direction[0]]).T, 
-                numpy.array([direction * direction[1]]).T, 
-                numpy.array([direction * direction[2]]).T])
+            m = numpy.identity(3) - numpy.column_stack(
+                [
+                    numpy.array([direction * direction[0]]).T,
+                    numpy.array([direction * direction[1]]).T,
+                    numpy.array([direction * direction[2]]).T,
+                ]
+            )
             left += m
             right += m.dot(origin)
 
         output = numpy.linalg.inv(left).dot(right)
 
         return numpy.array(pymap3d.ecef2geodetic(*output))
-    
+
     @staticmethod
     def triangulate(pos_vectors):
-        """ Triangulate position based on at least 3 position vectors """
+        """Triangulate position based on at least 3 position vectors"""
         lines = []
         for i in pos_vectors:
             lines.append(Geographic.__get_line(*i))
         return Geographic.__get_point(lines)
 
 
-
 class SchemaProvider:
     ### Provides database schemas ###
     class Geometry:
         class Type(Enum):
             POINT_2D = 1
             POINT_3D = 2
+
         ### placeholder geometry class ###
-        type:Type
-        def __init__(self,type:Type):
+        type: Type
+
+        def __init__(self, type: Type):
             self.type = type
 
         def __repr__(self):
             if self.type == self.Type.POINT_2D:
-                return 'Point'
+                return "Point"
             if self.type == self.Type.POINT_3D:
-                return '3D Point'
-                
+                return "3D Point"
+
     class AutoIncrement:
         def __init__(self):
             pass
 
     class Field:
-        name:str
-        description:str
+        name: str
+        description: str
         type
 
-        def __init__(self, name:str, description,type):
+        def __init__(self, name: str, description, type):
             self.name = name
             self.description = description
             self.type = type
 
         def __repr__(self):
             cls = type(self)
             return f"{cls.__name__}({self.name}, {getattr(self.type, '__name__', self.type)})"
 
     class Schema:
-        fields=[]
-        name:str
+        fields = []
+        name: str
 
         def __init__(self, name: str):
             self.name = name
 
     @staticmethod
     def merge(schema_a, schema_b):
         schema = SchemaProvider.Schema(schema_a.name + " / " + schema_b.name)
         schema.fields = schema_a.fields + schema_b.fields
         return schema
 
     @staticmethod
     def single_measurement():
         schema = SchemaProvider.Schema("Single measurement schema")
-        schema.fields =  [
-            SchemaProvider.Field("geometry","Center of the detection projected on the surface.",
-                                 SchemaProvider.Geometry(SchemaProvider.Geometry.Type.POINT_3D)),
-
-            #Frame fields (viewpoint information)
+        schema.fields = [
+            SchemaProvider.Field(
+                "geometry",
+                "Center of the detection projected on the surface.",
+                SchemaProvider.Geometry(SchemaProvider.Geometry.Type.POINT_3D),
+            ),
+            # Frame fields (viewpoint information)
             SchemaProvider.Field("rec_id", "The id of the recording.", int),
             SchemaProvider.Field("frame_idx", "The index of the frame.", int),
-            SchemaProvider.Field("azimuth", "Heading/Azimuth (true north) of movement of the camera.", float),
+            SchemaProvider.Field(
+                "azimuth",
+                "Heading/Azimuth (true north) of movement of the camera.",
+                float,
+            ),
             SchemaProvider.Field("usr_id", "An unique id for this record.", int),
-
-
-            #SchemaProvider.Field("camera_geom", "Position of the camera.",
+            # SchemaProvider.Field("camera_geom", "Position of the camera.",
             #                     SchemaProvider.Geometry(SchemaProvider.Geometry.Type.POINT_3D)),
-            #Camera fields (rendering parameters)
+            # Camera fields (rendering parameters)
             SchemaProvider.Field("cam_lat", "The latitude of the camera.", float),
             SchemaProvider.Field("cam_lon", "The longitude of the camera.", float),
             SchemaProvider.Field("cam_alt", "The altitude of the camera.", float),
-            SchemaProvider.Field("cam_fov", "The field of view of the spherical camera.",float),
-            SchemaProvider.Field("cam_yaw", "The yaw of the spherical camera.",float),
-            SchemaProvider.Field("cam_pitch", "The pitch of the spherical camera.",float),
-            SchemaProvider.Field("cam_width", "The width of the spherical camera.",int),
-            SchemaProvider.Field("cam_height", "The height of the spherical camera.",int),
-
+            SchemaProvider.Field(
+                "cam_fov", "The field of view of the spherical camera.", float
+            ),
+            SchemaProvider.Field("cam_yaw", "The yaw of the spherical camera.", float),
+            SchemaProvider.Field(
+                "cam_pitch", "The pitch of the spherical camera.", float
+            ),
+            SchemaProvider.Field(
+                "cam_width", "The width of the spherical camera.", int
+            ),
+            SchemaProvider.Field(
+                "cam_height", "The height of the spherical camera.", int
+            ),
             # Detection fields
-            SchemaProvider.Field("dt_class", "The detection class/type ID.",int),
-            SchemaProvider.Field("dt_name", "The detection name.",str),
-            SchemaProvider.Field("dt_x", "The highest left pixel of the detection.",int),
-            SchemaProvider.Field("dt_y", "The highest top pixel of the detection.",int),
-            SchemaProvider.Field("dt_width", "The width of the detection.",int),
-            SchemaProvider.Field("dt_height", "The height of the detection.",int),
-            SchemaProvider.Field("dt_conf", "The confidence.",float),
-            SchemaProvider.Field("dt_dist", "The surface distance in meters to the detection.",float),
-            SchemaProvider.Field("dt_px_x", "The pixel x coordinate of the detection(could be centroid x).", int),
-            SchemaProvider.Field("dt_px_y", "The pixel y coordinate of the detection (could be centroid y).", int),
-            SchemaProvider.Field("dt_yaw", "The geographical yaw of the camera wrt the detection.", float),
-            SchemaProvider.Field("dt_pitch", "The geographical pitch of the camera wrt the detection.", float),
-            # 
-            SchemaProvider.Field("surf_px_x","The pixel x coordinate of the surface(could be centroid x).",int),
-            SchemaProvider.Field("surf_px_y","The pixel y coordinate of the surface (could be centroid y).",int),
-            SchemaProvider.Field("surf_yaw","The geographical yaw of the camera wrt the surface.",float),
-            SchemaProvider.Field("surf_pitch","The geographical pitch of the camera wrt the surface.",float)
-
+            SchemaProvider.Field("dt_class", "The detection class/type ID.", int),
+            SchemaProvider.Field("dt_name", "The detection name.", str),
+            SchemaProvider.Field(
+                "dt_x", "The highest left pixel of the detection.", int
+            ),
+            SchemaProvider.Field(
+                "dt_y", "The highest top pixel of the detection.", int
+            ),
+            SchemaProvider.Field("dt_width", "The width of the detection.", int),
+            SchemaProvider.Field("dt_height", "The height of the detection.", int),
+            SchemaProvider.Field("dt_conf", "The confidence.", float),
+            SchemaProvider.Field(
+                "dt_dist", "The surface distance in meters to the detection.", float
+            ),
+            SchemaProvider.Field(
+                "dt_px_x",
+                "The pixel x coordinate of the detection(could be centroid x).",
+                int,
+            ),
+            SchemaProvider.Field(
+                "dt_px_y",
+                "The pixel y coordinate of the detection (could be centroid y).",
+                int,
+            ),
+            SchemaProvider.Field(
+                "dt_yaw", "The geographical yaw of the camera wrt the detection.", float
+            ),
+            SchemaProvider.Field(
+                "dt_pitch",
+                "The geographical pitch of the camera wrt the detection.",
+                float,
+            ),
+            #
+            SchemaProvider.Field(
+                "surf_px_x",
+                "The pixel x coordinate of the surface(could be centroid x).",
+                int,
+            ),
+            SchemaProvider.Field(
+                "surf_px_y",
+                "The pixel y coordinate of the surface (could be centroid y).",
+                int,
+            ),
+            SchemaProvider.Field(
+                "surf_yaw", "The geographical yaw of the camera wrt the surface.", float
+            ),
+            SchemaProvider.Field(
+                "surf_pitch",
+                "The geographical pitch of the camera wrt the surface.",
+                float,
+            ),
         ]
 
         return schema
 
     @staticmethod
     def clustering():
         schema = SchemaProvider.Schema("Clustering schema")
@@ -333,12 +408,15 @@
         ]
 
         return schema
 
     def geometry_3dpoint(self):
         schema = SchemaProvider.Schema("Geometry 3dPoint")
         schema.fields = [
-            SchemaProvider.Field("geometry", "Basic 3D Point geometry.",
-                                 SchemaProvider.Geometry(SchemaProvider.Geometry.Type.POINT_3D))
+            SchemaProvider.Field(
+                "geometry",
+                "Basic 3D Point geometry.",
+                SchemaProvider.Geometry(SchemaProvider.Geometry.Type.POINT_3D),
+            )
         ]
 
-        return schema
+        return schema
```

### Comparing `horus-media-client-0.9.4/horus_media/__init__.py` & `horus-media-client-0.9.5/horus_media/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,48 +47,51 @@
     min: Point
     max: Point
 
     @classmethod
     def create(cls, center, width=0, height=0):
         if not isinstance(center, Point):
             center = Point(*center)
-        x_interval = (center.x + width/2, center.x - width/2)
-        y_interval = (center.y + height/2, center.y - height/2)
-        return Box(Point(min(x_interval), min(y_interval)), Point(max(x_interval), max(y_interval)))
+        x_interval = (center.x + width / 2, center.x - width / 2)
+        y_interval = (center.y + height / 2, center.y - height / 2)
+        return Box(
+            Point(min(x_interval), min(y_interval)),
+            Point(max(x_interval), max(y_interval)),
+        )
 
 
 @dataclass(frozen=True)
 class Section:
     x: int
     y: int
     ax: float
     ay: float
     index: int
 
 
 class Grid:
-    """ Grid  8x4 (c x r) """
+    """Grid  8x4 (c x r)"""
 
     def __init__(self, w_min=-180, w_max=180, h_min=-90, h_max=90, r=4, c=8):
         assert w_min < w_max
         assert h_min < h_max
         self.rows = r
         self.cols = c
-        self.section_height = (h_max - h_min)/r
-        self.section_width = (w_max - w_min)/c
+        self.section_height = (h_max - h_min) / r
+        self.section_width = (w_max - w_min) / c
         self.__map = {}
         for index in range(r * c):
             x = index % c
-            y = (r-1) - index // c
-            ax = x*self.section_width - w_max
-            ay = y*self.section_height - h_max
+            y = (r - 1) - index // c
+            ax = x * self.section_width - w_max
+            ay = y * self.section_height - h_max
             self.__map[index] = Section(x, y, ax, ay, index)
 
     def __iter__(self):
-        """ Returns the Iterator object """
+        """Returns the Iterator object"""
         return (section for section in self.__map.values())
 
     def __str__(self):
         return str(self.__map)
 
     def __getitem__(self, ii):
         """Get a list item"""
@@ -130,26 +133,25 @@
         if w_min_wrapped < -180:
             w_min_wrapped = 360 + w_min_wrapped
 
         w_max_wrapped = (w_max % 360) - (360 if w_max < 0 else 0)
         if w_max_wrapped > 180:
             w_max_wrapped = -360 + w_max_wrapped
 
-        h = self.Comparator(h_min,  h_max, self.section_height)
+        h = self.Comparator(h_min, h_max, self.section_height)
         if w_min_wrapped < w_max_wrapped:
-            w = self.Comparator(
-                w_min_wrapped,  w_max_wrapped, self.section_width)
+            w = self.Comparator(w_min_wrapped, w_max_wrapped, self.section_width)
             for section in self.__map.values():
                 if section.ay in h and section.ax in w:
                     yield section
         elif w_min_wrapped > w_max_wrapped:
             assert w_max_wrapped >= -180
             assert w_min_wrapped <= 180
-            w_left = self.Comparator(-180,  w_max_wrapped, self.section_width)
-            w_right = self.Comparator(w_min_wrapped,  180, self.section_width)
+            w_left = self.Comparator(-180, w_max_wrapped, self.section_width)
+            w_right = self.Comparator(w_min_wrapped, 180, self.section_width)
             for section in self.__map.values():
                 if section.ay in h and (section.ax in w_left or section.ax in w_right):
                     yield section
 
 
 @dataclass(frozen=True)
 class Scale:
@@ -171,75 +173,80 @@
         Px_1024,
         Px_2048,
         Px_4096,
     )
 
     @classmethod
     def from_size(cls, size):
-        """ Returns the closest round-up scale that contains the requested size.
+        """Returns the closest round-up scale that contains the requested size.
         Returns None if no applicable scale is found.
         """
         result = cls.__SCALES[-1]
         for scale in reversed(cls.__SCALES):
             if scale.size < size:
                 return result
             result = scale
         return result
 
+
 class Mode(Enum):
     panoramic = 0
     spherical = 1
     orthographic = 2
     geographic = 3
 
     def __str__(self):
         return self.name
 
+
 @dataclass(frozen=True)
 class Size:
     width: int
     height: int
 
+
 @dataclass(frozen=True)
 class Direction:
     yaw: float
     pitch: float
 
+
 @dataclass(frozen=True)
 class Geometry:
     scale: int
     width: float
     height: float
     distance: float
     shift: float
     altitude: float
 
+
 class Client:
     def __init__(self, url="http://localhost:5050/web/", timeout=4):
         self.url = url
         self.__parsed_url = urllib.parse.urlparse(url)
         self.__connection = http.client.HTTPConnection(
-            self.__parsed_url.hostname, self.__parsed_url.port, timeout=timeout)
+            self.__parsed_url.hostname, self.__parsed_url.port, timeout=timeout
+        )
         self.__connection.connect()
         self.attempts = 5
-        self.attempts_interval = 3 #seconds
+        self.attempts_interval = 3  # seconds
 
     def fetch(self, request):
-        request.url = urllib.parse.urljoin(
-            self.__parsed_url.path, request.resource)
+        request.url = urllib.parse.urljoin(self.__parsed_url.path, request.resource)
         self.__connection.request("GET", request.url)
         attempts = self.attempts
         while attempts > 0:
             attempts -= 1
             try:
                 response = self.__connection.getresponse()
                 attempts = 0
             except Exception as exception:
                 logging.error(f'{exception}. Requesting "{request.url}".')
-                logging.error(f'New attempt in {self.attempts_interval}s .')
+                logging.error(f"New attempt in {self.attempts_interval}s .")
                 time.sleep(self.attempts_interval)
 
         request.response = response
         result = response.read()
         if type(request.local_file) == str:
             with open(request.local_file, "wb") as file:
                 file.write(result)
@@ -252,15 +259,27 @@
             self.fetch(request)
             jobs.append(request)
 
         return jobs
 
 
 class ImageRequest:
-    def __init__(self, builder, resource, mode=None, scale=None, section=None, size=None, direction=None, fov=None, cams = None, geometry=None):
+    def __init__(
+        self,
+        builder,
+        resource,
+        mode=None,
+        scale=None,
+        section=None,
+        size=None,
+        direction=None,
+        fov=None,
+        cams=None,
+        geometry=None,
+    ):
         self.local_file = None
         self.builder = builder
         self.resource = resource
         self.mode = mode
         self.scale = scale
         self.section = section
         self.size = size
@@ -273,14 +292,15 @@
         self.__result = None
 
     def set_result(self, value):
         self.__result = value
 
     def result(self):
         return self.__result
+
     def __repr__(self):
         cls = type(self)
         return f"{cls.__name__}({self.url})"
 
 
 class ImageRequestBuilder:
     def __init__(self, recording, frame):
@@ -293,33 +313,47 @@
         cls = type(self)
         return f"{cls.__name__}({self.__resource})"
 
     def build_spherical(self, size=None, direction=None, vof=None, cams=None):
         return self.build(Mode.spherical, None, None, size, direction, vof, cams, None)
 
     def build_orthographic(self, size, geometry):
-        return self.build(Mode.orthographic, None, None, size, None, None, None, geometry)
+        return self.build(
+            Mode.orthographic, None, None, size, None, None, None, geometry
+        )
 
     def build_geographic(self, size, direction=None, vof=None, x=None, y=None):
         if x and y:
             geometry = Geometry(0, x, y, 0, 0, 0)
         else:
             geometry = None
-        return self.build(Mode.geographic, None, None, size, direction, vof, None, geometry)
-
-    def build(self, mode=None, scale=None, section=None, size=None, direction=None, fov=None, cams=None, geometry=None):
+        return self.build(
+            Mode.geographic, None, None, size, direction, vof, None, geometry
+        )
+
+    def build(
+        self,
+        mode=None,
+        scale=None,
+        section=None,
+        size=None,
+        direction=None,
+        fov=None,
+        cams=None,
+        geometry=None,
+    ):
         data = {}
         if mode is not None:
             data["mode"] = mode
         if scale is not None:
             data["scale"] = scale.id
         if section is not None:
             data["section"] = section.index
         if size is not None:
-            data["size"] = str(size.width) + 'x' + str(size.height)
+            data["size"] = str(size.width) + "x" + str(size.height)
         if direction is not None:
             data["yaw"] = direction.yaw
             data["pitch"] = direction.pitch
         if fov is not None:
             data["hor_fov"] = fov
         if cams is not None:
             data["cams"] = cams
@@ -329,81 +363,98 @@
             data["geom_height"] = geometry.height
             data["geom_dist"] = geometry.distance
             data["geom_shift"] = geometry.shift
             if geometry.altitude is not None:
                 data["alti_next"] = geometry.altitude
         url_values = urllib.parse.urlencode(data)
         url = urllib.parse.urljoin(self.__resource, "?" + url_values)
-        request = ImageRequest(self, url, mode, scale, section, size, direction, fov, cams, geometry)
+        request = ImageRequest(
+            self, url, mode, scale, section, size, direction, fov, cams, geometry
+        )
         if self.path_template:
             request.local_file = self.path_template.format(
-                recording=self.recording, frame=self.frame, mode=mode if mode else "", 
-                scale=scale.id if scale else "", section=section.index if section else "")
+                recording=self.recording,
+                frame=self.frame,
+                mode=mode if mode else "",
+                scale=scale.id if scale else "",
+                section=section.index if section else "",
+            )
         return request
 
+
 class ImageProvider:
     @dataclass(frozen=True)
     class Result:
         image: io.BytesIO
         fov: Rect
         w: int
         h: int
 
         def to_pixel_coordinates(self, point):
             """
             the components of thepoint represent two angles (in Grid space)
             """
             px, py = point
-            py = (py/py*(py % 90) if py != 0 else 0) + 90
-            dy = 180 - (self.fov.y/self.fov.y*(self.fov.y % 90) if self.fov.y != 0 else 0)
-            y = (1 + (py - dy)/self.fov.height)*self.h
-
-            px = (px/px*(px % 180) if px != 0 else 0) + 180
-            dx = (self.fov.x/self.fov.x*(self.fov.x % 180) if self.fov.x != 0 else 0) + 180
-            x = (px - dx)/self.fov.width*self.w
+            py = (py / py * (py % 90) if py != 0 else 0) + 90
+            dy = 180 - (
+                self.fov.y / self.fov.y * (self.fov.y % 90) if self.fov.y != 0 else 0
+            )
+            y = (1 + (py - dy) / self.fov.height) * self.h
+
+            px = (px / px * (px % 180) if px != 0 else 0) + 180
+            dx = (
+                self.fov.x / self.fov.x * (self.fov.x % 180) if self.fov.x != 0 else 0
+            ) + 180
+            x = (px - dx) / self.fov.width * self.w
 
-            return Point(math.floor(x),math.floor(y))
+            return Point(math.floor(x), math.floor(y))
 
     def __init__(self, grid=Grid()):
         self.grid = grid
 
-    def fetch(self, image_request, w = None, h = None):
-        return self.Result(io.BytesIO(image_request.result()), 
-            Rect(0, 0, w, h) if w and h else Rect(0, 0, 1, 1), w if w else 0, h if h else 0)
+    def fetch(self, image_request, w=None, h=None):
+        return self.Result(
+            io.BytesIO(image_request.result()),
+            Rect(0, 0, w, h) if w and h else Rect(0, 0, 1, 1),
+            w if w else 0,
+            h if h else 0,
+        )
 
     def combine(self, image_requests, w, h):
         rows = set()
         cols = set()
         for req in image_requests:
             if req.section in self.grid:
                 rows.add(req.section.y)
                 cols.add(req.section.x)
 
         row_map = self.set_to_map(sorted(rows))
         col_map = self.set_to_map(self.wrap(sorted(cols)))
         row_index_shift = len(rows) - 1
 
-        stitched = Image.new('RGB', (w * len(col_map), h * len(row_map)))
+        stitched = Image.new("RGB", (w * len(col_map), h * len(row_map)))
         fov = Rect(math.inf, math.inf, 0, 0)
         fov.width = len(col_map) * self.grid.section_width
         fov.height = len(row_map) * self.grid.section_height
 
         for req in image_requests:
             r = row_map[req.section.y]
             c = col_map[req.section.x]
             fov.y = min(req.section.ay, fov.y)
             fov.x = min(req.section.ax, fov.x)
 
             try:
                 image = Image.open(io.BytesIO(req.result()))
                 stitched.paste(image, (c * w, (row_index_shift - r) * h))
             except Exception as exception:
-                logging.error(f"{exception}. Stitching section {req.section} from {req.url}")
-        image = io.BytesIO();
-        stitched.save(image, format='jpeg', quality=95)
+                logging.error(
+                    f"{exception}. Stitching section {req.section} from {req.url}"
+                )
+        image = io.BytesIO()
+        stitched.save(image, format="jpeg", quality=95)
         return self.Result(image, fov, stitched.width, stitched.height)
 
     @classmethod
     def wrap(cls, cols):
         if len(cols) > 0:
             prev = cols[0]
             list_1 = []
@@ -418,20 +469,31 @@
         return cols
 
     @classmethod
     def set_to_map(cls, my_set):
         size = len(my_set)
         if size > 0:
             mx = min(my_set)
-            mp = range(size+1)
+            mp = range(size + 1)
             return dict(zip(my_set, mp))
         return {}
 
+
 class ComputationRequest:
-    def __init__(self, builder, resource, size=None, direction=None, fov=None, x=None, y=None, direction0=None):
+    def __init__(
+        self,
+        builder,
+        resource,
+        size=None,
+        direction=None,
+        fov=None,
+        x=None,
+        y=None,
+        direction0=None,
+    ):
         self.local_file = None
         self.builder = builder
         self.resource = resource
         self.size = size
         self.direction = direction
         self.fov = fov
         self.x = x
@@ -443,27 +505,30 @@
 
     def set_result(self, value):
         self.__result = value
 
     def result(self):
         return self.__result
 
+
 class ComputationRequestBuilder:
-    def __init__(self, method, frame = None):
+    def __init__(self, method, frame=None):
         self.path_template = None
         self.method = method
         self.frame = frame
         self.__resource = f"./computation/{method}"
         if frame != None:
             self.__resource += f"/{frame}"
 
-    def build(self, size=None, direction=None, fov=None, x=None, y=None, direction0=None):
+    def build(
+        self, size=None, direction=None, fov=None, x=None, y=None, direction0=None
+    ):
         data = {}
         if size is not None:
-            data["size"] = str(size.width) + 'x' + str(size.height)
+            data["size"] = str(size.width) + "x" + str(size.height)
         if direction is not None:
             data["yaw"] = direction.yaw
             data["pitch"] = direction.pitch
         else:
             data["yaw"] = 0
             data["pitch"] = 0
         if fov is not None:
@@ -475,19 +540,21 @@
         if direction0 is not None:
             data["yaw0"] = direction0.yaw
             data["pitch0"] = direction0.pitch
         url_values = urllib.parse.urlencode(data)
         url = urllib.parse.urljoin(self.__resource, "?" + url_values)
         return ComputationRequest(self, url, size, direction, fov, x, y, direction0)
 
+
 class ComputationProvider:
     @dataclass(frozen=True)
     class Result:
         data: io.BytesIO
 
     def fetch(self, computation_request):
         try:
-            result = self.Result(io.BytesIO(
-                computation_request.result())).data.getvalue()
+            result = self.Result(
+                io.BytesIO(computation_request.result())
+            ).data.getvalue()
             return json.loads(result)
         except json.decoder.JSONDecodeError as error:
             return {"error": error}
```

### Comparing `horus-media-client-0.9.4/horus_media_client.egg-info/PKG-INFO` & `horus-media-client-0.9.5/horus_media_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horus-media-client
-Version: 0.9.4
+Version: 0.9.5
 Summary: Horus Media Server Client
 Home-page: https://github.com/horus-view-and-explore/horus-media-client
 Author: Horus View and Explore B.V.
 Author-email: info@horus.nu
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: OS Independent
```

### Comparing `horus-media-client-0.9.4/horus_media_client.egg-info/SOURCES.txt` & `horus-media-client-0.9.5/horus_media_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.4/horus_media_examples/example_strategy.py` & `horus-media-client-0.9.5/horus_media_examples/example_strategy.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,87 +14,174 @@
 In addition it exemplifies geo-query based acquisition of georeferenced orthographic projection images (geotiff)
 """
 
 import psycopg2
 
 from horus_gis import CameraModel, geoPointParser
 from horus_db import Frames, Recordings, Recording, Frame, Iterator
-from horus_media import Client, ImageRequestBuilder, ImageProvider, Grid, Scales, Point, Box, Mode, Size, Direction, Geometry
+from horus_media import (
+    Client,
+    ImageRequestBuilder,
+    ImageProvider,
+    Grid,
+    Scales,
+    Point,
+    Box,
+    Mode,
+    Size,
+    Direction,
+    Geometry,
+)
 
 import argparse
 import logging
 
 
-parser = argparse.ArgumentParser(
-    formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 
-parser.add_argument("target", nargs='+', metavar="lon,lat,alt",
-                    type=geoPointParser, help="target GPS location in decimal degrees")
-parser.add_argument("-r", "--recording", metavar="ID",
-                    nargs='*', type=int, help="recording id")
-parser.add_argument("-s", "--server",  metavar="URL", type=str, default="http://localhost:5050/web/",
-                    help="Horus Media Server endpoint")
-parser.add_argument("-f", "--fov",  metavar=("HORIZONTAL", "VERTICAL"), nargs=2, type=float, default=(25, 90),
-                    help="field of view size in degrees")
-parser.add_argument("-m", "--mode",  type=str, default="panoramic", choices=[x.name for x in list(Mode)],
-                    help="rendering mode")
-parser.add_argument("-si", "--size",  metavar=("WIDTH", "HEIGHT"), nargs=2, type=int, default=(1024, 1024),
-                    help="size of the image (spherical), size of the back-buffer (orthographic)")
-parser.add_argument("-ci", "--clipping",  metavar=("MIN", "MAX"), type=float, nargs=2, default=(15, 100),
-                    help="clipping interval in degrees")
-parser.add_argument("-d", "--distance", type=float, default=10,
-                    help="maximum distance from the target in meters")
+parser.add_argument(
+    "target",
+    nargs="+",
+    metavar="lon,lat,alt",
+    type=geoPointParser,
+    help="target GPS location in decimal degrees",
+)
+parser.add_argument(
+    "-r", "--recording", metavar="ID", nargs="*", type=int, help="recording id"
+)
+parser.add_argument(
+    "-s",
+    "--server",
+    metavar="URL",
+    type=str,
+    default="http://localhost:5050/web/",
+    help="Horus Media Server endpoint",
+)
+parser.add_argument(
+    "-f",
+    "--fov",
+    metavar=("HORIZONTAL", "VERTICAL"),
+    nargs=2,
+    type=float,
+    default=(25, 90),
+    help="field of view size in degrees",
+)
+parser.add_argument(
+    "-m",
+    "--mode",
+    type=str,
+    default="panoramic",
+    choices=[x.name for x in list(Mode)],
+    help="rendering mode",
+)
+parser.add_argument(
+    "-si",
+    "--size",
+    metavar=("WIDTH", "HEIGHT"),
+    nargs=2,
+    type=int,
+    default=(1024, 1024),
+    help="size of the image (spherical), size of the back-buffer (orthographic)",
+)
+parser.add_argument(
+    "-ci",
+    "--clipping",
+    metavar=("MIN", "MAX"),
+    type=float,
+    nargs=2,
+    default=(15, 100),
+    help="clipping interval in degrees",
+)
+parser.add_argument(
+    "-d",
+    "--distance",
+    type=float,
+    default=10,
+    help="maximum distance from the target in meters",
+)
 parser.add_argument("--path", type=str, help="output location")
-parser.add_argument("--attempts", metavar=("NUMBER"), type=int, help="maximum number of attempts", default=100)
+parser.add_argument(
+    "--attempts",
+    metavar=("NUMBER"),
+    type=int,
+    help="maximum number of attempts",
+    default=100,
+)
 
 # geom
-parser.add_argument("-gsc", "--geom-scale", type=int, default=400,
-                    help="output scale in px/m (orthographic)")
-parser.add_argument("-gw", "--geom-width", type=float, default=6,
-                    help="geometry width (orthographic)")
-parser.add_argument("-gh", "--geom-height", type=float, default=2,
-                    help="geometry height (orthographic)")
-parser.add_argument("-gd", "--geom-dist", type=float, default=4,
-                    help="geometry distance (orthographic)")
-parser.add_argument("-gs", "--geom-shift", type=float, default=0,
-                    help="geometry shift (orthographic)")
+parser.add_argument(
+    "-gsc",
+    "--geom-scale",
+    type=int,
+    default=400,
+    help="output scale in px/m (orthographic)",
+)
+parser.add_argument(
+    "-gw", "--geom-width", type=float, default=6, help="geometry width (orthographic)"
+)
+parser.add_argument(
+    "-gh", "--geom-height", type=float, default=2, help="geometry height (orthographic)"
+)
+parser.add_argument(
+    "-gd", "--geom-dist", type=float, default=4, help="geometry distance (orthographic)"
+)
+parser.add_argument(
+    "-gs", "--geom-shift", type=float, default=0, help="geometry shift (orthographic)"
+)
 
 # db
-parser.add_argument("--db-name", type=str,
-                    default="HorusWebMoviePlayer", help="the database name")
-parser.add_argument("--db-user", type=str, default="postgres",
-                    help="database user name used to authenticate")
-parser.add_argument("--db-password", type=str,
-                    help="database password used to authenticate")
-parser.add_argument("--db-host", type=str, default="localhost",
-                    help="database database host address")
-parser.add_argument("--db-port", type=int, default=5432,
-                    help="database connection port number")
+parser.add_argument(
+    "--db-name", type=str, default="HorusWebMoviePlayer", help="the database name"
+)
+parser.add_argument(
+    "--db-user",
+    type=str,
+    default="postgres",
+    help="database user name used to authenticate",
+)
+parser.add_argument(
+    "--db-password", type=str, help="database password used to authenticate"
+)
+parser.add_argument(
+    "--db-host", type=str, default="localhost", help="database database host address"
+)
+parser.add_argument(
+    "--db-port", type=int, default=5432, help="database connection port number"
+)
 
 args = parser.parse_args()
 
 temp_path = args.path
 recording_id = tuple(args.recording) if args.recording != None else None
 distance = args.distance
 horizontal_fov = args.fov[0]
 vertical_fov = args.fov[1]
 mode = args.mode
 size = Size(args.size[0], args.size[1])
 clipping_interval = tuple(args.clipping)
-geometry = Geometry(args.geom_scale, args.geom_width, args.geom_height, args.geom_dist, args.geom_shift, None)
-
-db_params = [("host", args.db_host),
-             ("port", str(args.db_port)),
-             ("dbname", args.db_name),
-             ("user", args.db_user),
-             ("password", args.db_password),
-             ]
+geometry = Geometry(
+    args.geom_scale,
+    args.geom_width,
+    args.geom_height,
+    args.geom_dist,
+    args.geom_shift,
+    None,
+)
+
+db_params = [
+    ("host", args.db_host),
+    ("port", str(args.db_port)),
+    ("dbname", args.db_name),
+    ("user", args.db_user),
+    ("password", args.db_password),
+]
 try:
     connection_string = " ".join(
-        map("=".join, filter(lambda x: x[1] != None, db_params)))
+        map("=".join, filter(lambda x: x[1] != None, db_params))
+    )
     connection = psycopg2.connect(connection_string)
 except psycopg2.OperationalError as exception:
     logging.error(f"{exception} Connecting to database")
     exit()
 try:
     client = Client(args.server)
 except OSError as exception:
@@ -104,102 +191,122 @@
 frames = Frames(connection)
 grid = Grid()
 image_provider = ImageProvider(grid)
 
 
 def compute_angle(frame, sign_location):
     camera_model = CameraModel(frame.get_location(), frame.heading)
-    return - camera_model.look_at_angle(sign_location)
+    return -camera_model.look_at_angle(sign_location)
 
 
 for location in args.target:
     print(f"Looking for {location}")
     results = []
-    cursor = frames.query(within=(location, distance),
-                          recordingid=recording_id, limit=1)
+    cursor = frames.query(
+        within=(location, distance), recordingid=recording_id, limit=1
+    )
     frame = Frame(cursor)
     if not frame:
-        logging.warning(
-            f"Location {location} not found within {distance} meters")
+        logging.warning(f"Location {location} not found within {distance} meters")
         continue
 
     if recording_id:
         assert frame.recordingid in recording_id
     angle = compute_angle(frame, location)
     attempts = args.attempts
     while True:
-        if (clipping_interval[0] <= angle <= clipping_interval[1]):
+        if clipping_interval[0] <= angle <= clipping_interval[1]:
             requestBuilder = ImageRequestBuilder(frame.recordingid, frame.uuid)
 
             filename = None
 
             if mode == Mode.panoramic.name:
-                fov = Box.create(center=(angle, 0),
-                                width=horizontal_fov, height=vertical_fov)
+                fov = Box.create(
+                    center=(angle, 0), width=horizontal_fov, height=vertical_fov
+                )
                 sections = grid.filter(fov=fov)
-                requests = client.fetch_all(requestBuilder.build(
-                    mode, Scales.Px_1024, section) for section in sections)
+                requests = client.fetch_all(
+                    requestBuilder.build(mode, Scales.Px_1024, section)
+                    for section in sections
+                )
                 result = image_provider.combine(
-                    requests, Scales.Px_1024.size, Scales.Px_1024.size)
+                    requests, Scales.Px_1024.size, Scales.Px_1024.size
+                )
                 if temp_path:
-                    filename = temp_path + \
-                        "stitched_{}_{}.jpg".format(
-                            frame.recordingid,  frame.index)
-                results.append({
-                    "frame": frame,
-                    "angle": angle,
-                    "pixel_coordinate": result.to_pixel_coordinates((angle, 0)),
-                    "stitch": result})
+                    filename = temp_path + "stitched_{}_{}.jpg".format(
+                        frame.recordingid, frame.index
+                    )
+                results.append(
+                    {
+                        "frame": frame,
+                        "angle": angle,
+                        "pixel_coordinate": result.to_pixel_coordinates((angle, 0)),
+                        "stitch": result,
+                    }
+                )
 
             if mode == Mode.spherical.name:
-                request = client.fetch(requestBuilder.build_spherical(
-                    size, Direction(angle, 0), horizontal_fov))
+                request = client.fetch(
+                    requestBuilder.build_spherical(
+                        size, Direction(angle, 0), horizontal_fov
+                    )
+                )
                 result = image_provider.fetch(request, size.width, size.height)
                 if temp_path:
                     filename = temp_path + "spherical_{}_{}.jpg".format(
-                        frame.recordingid,  frame.index)
-                results.append({
-                    "frame": frame,
-                    "angle": angle,
-                    "pixel_coordinate": Point(size.width / 2, 0),
-                    "stitch": result})
+                        frame.recordingid, frame.index
+                    )
+                results.append(
+                    {
+                        "frame": frame,
+                        "angle": angle,
+                        "pixel_coordinate": Point(size.width / 2, 0),
+                        "stitch": result,
+                    }
+                )
 
             if mode == Mode.orthographic.name:
-                request = client.fetch(requestBuilder.build_orthographic(size, geometry))
-                                                            
+                request = client.fetch(
+                    requestBuilder.build_orthographic(size, geometry)
+                )
+
                 result = image_provider.fetch(request)
                 if temp_path:
                     filename = temp_path + "orthographic_{}_{}.tif".format(
-                        frame.recordingid,  frame.index)
-                results.append({
-                    "frame": frame,
-                    "angle": angle,
-                    "pixel_coordinate": Point(0, 0),
-                    "stitch": result})
+                        frame.recordingid, frame.index
+                    )
+                results.append(
+                    {
+                        "frame": frame,
+                        "angle": angle,
+                        "pixel_coordinate": Point(0, 0),
+                        "stitch": result,
+                    }
+                )
 
             if filename:
-                with open(filename, 'wb') as f:
+                with open(filename, "wb") as f:
                     f.write(result.image.getvalue())
                 result.image.close()
         elif len(results) > 0:
             break
         elif attempts < 0:
             print("Exceeded maximum number of attempts.")
             break
         else:
             attempts = attempts - 1
 
-
         next_index = frame.index
         frame = Frame(cursor)
         if not frame:
             # request in batches of 40 frames using decreasing indexes
             indexes = tuple(range(next_index - 40, next_index))
             cursor = frames.query(
-                index=indexes, order_by="index DESC", recordingid=recording_id)
+                index=indexes, order_by="index DESC", recordingid=recording_id
+            )
             frame = Frame(cursor)
             if not frame:
                 break
         angle = compute_angle(frame, location)
 
     for result in results:
         print()
```

### Comparing `horus-media-client-0.9.4/horus_media_examples/export_orthographic.py` & `horus-media-client-0.9.5/horus_media_examples/export_orthographic.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,18 +16,20 @@
 parser = util.create_argument_parser()
 util.add_database_arguments(parser)
 util.add_server_arguments(parser)
 util.add_size_argument(parser, (4096, 2048))
 util.add_geometry_arguments(parser)
 
 parser.add_argument("--path", type=str, help="path to output location")
-parser.add_argument("--limit", metavar=("NUMBER"), type=int,
-                    help="maximum number of frames")
-parser.add_argument("-r", "--recording", metavar="ID",
-                    nargs='*', type=int, help="recording id")
+parser.add_argument(
+    "--limit", metavar=("NUMBER"), type=int, help="maximum number of frames"
+)
+parser.add_argument(
+    "-r", "--recording", metavar="ID", nargs="*", type=int, help="recording id"
+)
 
 args = parser.parse_args()
 
 # This example shows how to request orthographic images
 output_path = args.path
 
 if output_path is None:
@@ -44,15 +46,19 @@
 
 # Output parameters
 size = Size(args.size[0], args.size[1])  # defaults to (4096px, 2048px)
 recording_id = tuple(args.recording) if args.recording != None else None
 
 
 # Get frames
-results = Frame.query(frames, recordingid=recording_id, order_by="index",)
+results = Frame.query(
+    frames,
+    recordingid=recording_id,
+    order_by="index",
+)
 if args.limit:
     results = itertools.islice(results, args.limit)
 for frame in results:
     if frame is None:
         print("No frames!")
         exit()
 
@@ -65,16 +71,15 @@
     cursor = frames.query(recordingid=frame.recordingid, index=frame.index + 1)
     next_frame = Frame(cursor)
     if next_frame is not None:
         geometry = util.get_geometry(args, next_frame.altitude)
     else:
         geometry = util.get_geometry(args)
 
-    request = client.fetch(
-        request_builder.build_orthographic(size, geometry))
+    request = client.fetch(request_builder.build_orthographic(size, geometry))
 
     result = image_provider.fetch(request)
     # Save the file
     filename = "orthographic_{}.tif".format(frame.index)
-    with open(os.path.join(output_path, filename), 'wb') as image_file:
+    with open(os.path.join(output_path, filename), "wb") as image_file:
         image_file.write(result.image.getvalue())
         result.image.close()
```

### Comparing `horus-media-client-0.9.4/horus_media_examples/export_spherical.py` & `horus-media-client-0.9.5/horus_media_examples/export_spherical.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,35 +4,50 @@
 import os
 import sys
 import csv
 import logging
 import itertools
 
 from horus_db import Frames, Frame
-from horus_media import Client, ImageRequestBuilder, ImageProvider, Size, Direction, \
-    ComputationRequestBuilder, ComputationProvider
+from horus_media import (
+    Client,
+    ImageRequestBuilder,
+    ImageProvider,
+    Size,
+    Direction,
+    ComputationRequestBuilder,
+    ComputationProvider,
+)
 from horus_gis import PositionVector, Geographic
 
 from . import util
 
 
 # Command line input handling
 parser = util.create_argument_parser()
 util.add_database_arguments(parser)
 util.add_server_arguments(parser)
 util.add_size_argument(parser, (1024, 1024))
-parser.add_argument("-hf", "--horizontal-fov", type=float, default=(90),
-                    help="horizontal field of view size in degrees")
-parser.add_argument("-o", "--overlap", type=float, default=(20),
-                    help="horizontal overlap in degrees")
+parser.add_argument(
+    "-hf",
+    "--horizontal-fov",
+    type=float,
+    default=(90),
+    help="horizontal field of view size in degrees",
+)
+parser.add_argument(
+    "-o", "--overlap", type=float, default=(20), help="horizontal overlap in degrees"
+)
 parser.add_argument("--path", type=str, help="path to output location")
-parser.add_argument("--limit", metavar=("NUMBER"), type=int,
-                    help="maximum number of frames")
-parser.add_argument("-r", "--recording", metavar="ID",
-                    nargs='*', type=int, help="recording id")
+parser.add_argument(
+    "--limit", metavar=("NUMBER"), type=int, help="maximum number of frames"
+)
+parser.add_argument(
+    "-r", "--recording", metavar="ID", nargs="*", type=int, help="recording id"
+)
 
 
 args = parser.parse_args()
 
 # This example shows how to request a spherical image
 output_path = args.path
 
@@ -76,56 +91,63 @@
     "Index",
     "Altitude",
     "Azimuth",
     "Latitude",
     "Longitude",
     "Pitch",
     "Roll",
-    "Stamp"
+    "Stamp",
 ]
 
 
 # Open output csv file
-with open(os.path.join(output_path, 'output.csv'), 'w', newline='') as csvfile:
+with open(os.path.join(output_path, "output.csv"), "w", newline="") as csvfile:
     writer = csv.writer(csvfile, quoting=csv.QUOTE_MINIMAL)
     writer.writerow(csv_header)
 
     # Get frames
-    results = Frame.query(frames, recordingid=recording_id, order_by="index",)
+    results = Frame.query(
+        frames,
+        recordingid=recording_id,
+        order_by="index",
+    )
     if args.limit:
         results = itertools.islice(results, args.limit)
     for frame in results:
         if frame is None:
             print("No frames!")
             exit()
 
         print(frame)
 
         # Get the image
         # Set parameters
         request_builder = ImageRequestBuilder(frame.recordingid, frame.uuid)
         for direction_id, direction in directions.items():
-            request = client.fetch(request_builder.build_spherical(
-                size, direction, horizontal_fov))
+            request = client.fetch(
+                request_builder.build_spherical(size, direction, horizontal_fov)
+            )
             result = image_provider.fetch(request)
 
             # Save the file
             filename = "{}_{}.jpg".format(frame.index, direction_id)
 
-            with open(os.path.join(output_path, filename), 'wb') as image_file:
+            with open(os.path.join(output_path, filename), "wb") as image_file:
                 image_file.write(result.image.getvalue())
                 result.image.close()
 
             # Compute accurate position with lever arm.
-            position = get_position_vector(
-                frame, size, direction, horizontal_fov)
+            position = get_position_vector(frame, size, direction, horizontal_fov)
 
-            writer.writerow([
-                filename,
-                frame.index,
-                position.alt,
-                frame.azimuth,
-                position.lat,
-                position.lon,
-                frame.pitch,
-                frame.roll,
-                frame.stamp.isoformat()])
+            writer.writerow(
+                [
+                    filename,
+                    frame.index,
+                    position.alt,
+                    frame.azimuth,
+                    position.lat,
+                    position.lon,
+                    frame.pitch,
+                    frame.roll,
+                    frame.stamp.isoformat(),
+                ]
+            )
```

### Comparing `horus-media-client-0.9.4/horus_media_examples/export_time_interval.py` & `horus-media-client-0.9.5/horus_media_examples/export_time_interval.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,21 +9,33 @@
 
 from . import util
 
 # Command line input handling
 parser = util.create_argument_parser()
 util.add_database_arguments(parser)
 util.add_server_arguments(parser)
-parser.add_argument("-t", "--time",  metavar=("START", "END"), nargs=2, type=str,
-                    help="time interval to query. E.g. '2022-02-13T14:30:00' '2022-02-13T15:00:00'")
+parser.add_argument(
+    "-t",
+    "--time",
+    metavar=("START", "END"),
+    nargs=2,
+    type=str,
+    help="time interval to query. E.g. '2022-02-13T14:30:00' '2022-02-13T15:00:00'",
+)
 parser.add_argument("--path", type=str, help="path to output location")
-parser.add_argument("--limit", metavar=("NUMBER"), type=int, default=100,
-                    help="maximum number of frames")
-parser.add_argument("-r", "--recording", metavar="ID",
-                    nargs='*', type=int, help="recording id")
+parser.add_argument(
+    "--limit",
+    metavar=("NUMBER"),
+    type=int,
+    default=100,
+    help="maximum number of frames",
+)
+parser.add_argument(
+    "-r", "--recording", metavar="ID", nargs="*", type=int, help="recording id"
+)
 
 
 args = parser.parse_args()
 
 # This example shows how to request a spherical image
 output_path = args.path
 
@@ -42,36 +54,35 @@
 image_provider = ImageProvider()
 
 # Input parameters
 recording_id = tuple(args.recording) if args.recording != None else None
 
 
 # Get frames
-results = Frame.query(frames,
-                      # tuple of timestamp strings (begin, end)in ISO format
-                      time_interval=args.time,
-                      # recording id (optional)
-                      recordingid=recording_id,
-                      order_by="index",
-                      limit=args.limit,
-                      )
+results = Frame.query(
+    frames,
+    # tuple of timestamp strings (begin, end)in ISO format
+    time_interval=args.time,
+    # recording id (optional)
+    recordingid=recording_id,
+    order_by="index",
+    limit=args.limit,
+)
 
 for frame in results:
     if frame is None:
         print("No frames!")
         exit()
 
     print(frame, "at", frame.stamp)
 
     # Get the image
     request_builder = ImageRequestBuilder(frame.recordingid, frame.uuid)
-    request = client.fetch(request_builder.build(
-        Mode.panoramic, Scales.Px_1024))
+    request = client.fetch(request_builder.build(Mode.panoramic, Scales.Px_1024))
     result = image_provider.fetch(request)
 
     # Save the file
-    filename = "{}_{}_{}.jpg".format(
-        frame.recordingid, frame.index, frame.stamp)
+    filename = "{}_{}_{}.jpg".format(frame.recordingid, frame.index, frame.stamp)
 
-    with open(os.path.join(output_path, filename), 'wb') as image_file:
+    with open(os.path.join(output_path, filename), "wb") as image_file:
         image_file.write(result.image.getvalue())
         result.image.close()
```

### Comparing `horus-media-client-0.9.4/horus_media_examples/geosuite_database_info.py` & `horus-media-client-0.9.5/horus_media_examples/geosuite_database_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 if not path.exists(sqlite_file):
     print("Database file: [", sqlite_file, "] could not be found.")
     exit()
 
 db = horus_spatialite.Spatialite(sqlite_file)
 
 for arg in sys.argv[2:]:
-    db.blob_contains_geometry(arg) 
+    db.blob_contains_geometry(arg)
 
 db.open()
 db.resolve()
 db.show_info()
 
 # Iterate over data
 for row in db.query():
```

### Comparing `horus-media-client-0.9.4/horus_media_examples/recordings_tool.py` & `horus-media-client-0.9.5/horus_media_examples/recordings_tool.py`

 * *Files identical despite different names*

### Comparing `horus-media-client-0.9.4/horus_media_examples/single_measurement_clustering.py` & `horus-media-client-0.9.5/horus_media_examples/single_measurement_clustering.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,98 +9,100 @@
 
 try:
     from sklearn.neighbors import BallTree
 except ModuleNotFoundError:
     print("Install module 'sklearn' to run this example.")
     exit(1)
 
-def dt_class_filter(database,index,indices):
-    dt_class = database.at[index,'dt_class']
-    return [idx for idx in indices if database.at[idx,'dt_class'] == dt_class]
 
+def dt_class_filter(database, index, indices):
+    dt_class = database.at[index, "dt_class"]
+    return [idx for idx in indices if database.at[idx, "dt_class"] == dt_class]
 
-# Algorithm
-def cluster(radius,tree, row_idx,database, datapoints, filter):
 
+# Algorithm
+def cluster(radius, tree, row_idx, database, datapoints, filter):
     # we have seen this point before
-    if database.at[row_idx,'clstr_id'] != 0:
+    if database.at[row_idx, "clstr_id"] != 0:
         return
 
     # Get the rows that fall within
-    query  = np.array([datapoints[row_idx]])
+    query = np.array([datapoints[row_idx]])
     ind = tree.query_radius(query, r=radius)
-    ind = filter(database,row_idx,ind[0])
+    ind = filter(database, row_idx, ind[0])
 
-    relation = {idx:database.iloc[idx]['clstr_id'] for idx in ind}
+    relation = {idx: database.iloc[idx]["clstr_id"] for idx in ind}
     cids = {relation[k] for k in relation.keys()}
 
     cids.remove(0)
 
     length = len(cids)
 
     # all elements will receive the row_idx as clstr_id
     if length == 0:
         for k in relation:
-            database.at[k,'clstr_id'] = row_idx
-            database.at[k, 'clstr_conf'] = 1.0
+            database.at[k, "clstr_id"] = row_idx
+            database.at[k, "clstr_conf"] = 1.0
 
     # add instace to the found cluster
     if len(cids) == 1:
-        new_id  = next(iter(cids))
+        new_id = next(iter(cids))
         for k in relation.keys():
-            if database.at[k,'clstr_id'] != new_id:
-                database.at[k,'clstr_id'] = new_id
-                database.at[k, 'clstr_conf'] = 1.0
+            if database.at[k, "clstr_id"] != new_id:
+                database.at[k, "clstr_id"] = new_id
+                database.at[k, "clstr_conf"] = 1.0
 
     if len(cids) > 2:
         print("Edge case")
         exit(1)
 
 
 ### Read Data ####
 sp = SchemaProvider()
-schema = sp.merge(sp.single_measurement(),sp.clustering())
+schema = sp.merge(sp.single_measurement(), sp.clustering())
 database = HorusGeoDataFrame(schema)
 
 # provide a map of the new 'fields' with their default value
 # missing fields will cause a schema exception
 single_measurement_path = "output/single_measurement.shp"
 if not os.path.exists(single_measurement_path):
-    print(f"File '{single_measurement_path}' not found.\nRun 'horus_media_examples.spherical_camera_single_measurement' first.")
+    print(
+        f"File '{single_measurement_path}' not found.\nRun 'horus_media_examples.spherical_camera_single_measurement' first."
+    )
     exit(1)
 
-database.append_file(single_measurement_path, default_values={'clstr_id':0,'clstr_conf':0.0})
+database.append_file(
+    single_measurement_path, default_values={"clstr_id": 0, "clstr_conf": 0.0}
+)
 
 # database has performed schema checks, and we will only update the cluster fields
 # hence we can use the Geopandas dataframe directly
 dataframe = database.dataframe
 
 
-
 # Convert datapoints
 datapoints = []
 
-for index, row in dataframe.iterrows(): # Looping over all points
-    datapoints.append(np.deg2rad([row['geometry'].y,row['geometry'].x]))
+for index, row in dataframe.iterrows():  # Looping over all points
+    datapoints.append(np.deg2rad([row["geometry"].y, row["geometry"].x]))
 
 
 # Setup the Search tree
-tree = BallTree(datapoints, metric='haversine')
+tree = BallTree(datapoints, metric="haversine")
 
 # Adjust parameters
 r_meter = 6371000.0
-radius = 3.0 * (1.0/ r_meter)
+radius = 3.0 * (1.0 / r_meter)
 
 
 # go fish
 for index, row in dataframe.iterrows():
-    cluster(radius,tree,index,dataframe,datapoints,dt_class_filter)
+    cluster(radius, tree, index, dataframe, datapoints, dt_class_filter)
 
 
 # Create output directory
-output_dir = os.path.join(os.getcwd(), 'output')
+output_dir = os.path.join(os.getcwd(), "output")
 
 if not os.path.exists(output_dir):
     os.makedirs(output_dir)
 
 database.write_shapefile(os.path.join(output_dir, "single_measurement_clusters.shp"))
-
```

### Comparing `horus-media-client-0.9.4/horus_media_examples/snapshots.py` & `horus-media-client-0.9.5/horus_media_examples/snapshots.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,38 +5,45 @@
 from pyproj import Geod
 from horus_geometries import Geometry_proj
 import geopandas as gpd
 import pandas as pd
 import sys
 from os import path
 import traceback
+import math
 
 from . import util
 
 parser = util.create_argument_parser()
 
-parser.add_argument("--sqlite-db", type=str,
-                    help="the geosuite_database name")
+parser.add_argument("--sqlite-db", type=str, help="the geosuite_database name")
 
-parser.add_argument("--sqlite-framenr", type=str,
-                    help="the field specifying the framenr")
-
-parser.add_argument("--sqlite-recording", type=str,
-                    help="the field specifying the recordingname")
-
-parser.add_argument("--sqlite-geometry", type=str,
-                    help="the field specifying an alternative geometry blob")
+parser.add_argument(
+    "--sqlite-framenr", type=str, help="the field specifying the framenr"
+)
+
+parser.add_argument(
+    "--sqlite-recording", type=str, help="the field specifying the recordingname"
+)
+
+parser.add_argument(
+    "--sqlite-geometry",
+    type=str,
+    help="the field specifying an alternative geometry blob",
+)
 
 # Not tested
-parser.add_argument("--recordings-on-disk", type=str,
-                    help="Optionally provide a recording folder")
+parser.add_argument(
+    "--recordings-on-disk", type=str, help="Optionally provide a recording folder"
+)
 
 # Not tested
-parser.add_argument("--recording-id", type=int,
-                    help="Optionally provide a the static recording id.")
+parser.add_argument(
+    "--recording-id", type=int, help="Optionally provide a the static recording id."
+)
 
 
 util.add_database_arguments(parser)
 util.add_server_arguments(parser)
 
 
 args = parser.parse_args()
@@ -49,159 +56,225 @@
     exit()
 
 # sqlite_frame_idx_field = "Frame_numb"
 output_database = None
 geod = Geod(ellps="WGS84")
 
 
+def compute_heading(long_0, lat_0, long_1, lat_1):
+    long_0 = math.radians(long_0)
+    lat_0 = math.radians(lat_0)
+    long_1 = math.radians(long_1)
+    lat_1 = math.radians(lat_1)
+    heading = math.atan2(
+        math.sin(long_1 - long_0) * math.cos(lat_1),
+        math.cos(lat_0) * math.sin(lat_1)
+        - math.sin(lat_0) * math.cos(lat_1) * math.cos(long_1 - long_0),
+    )
+    heading = math.degrees(heading)
+    heading = (heading + 360) % 360
+    return heading
+
+
+def compute_rel_geom_heading(frame, geom_centroid):
+    geom_heading = compute_heading(frame.longitude, frame.latitude, *geom_centroid)
+    return (360 + geom_heading - frame.heading) % 360
+
+
+class GeomHeadingFrameSelector:
+    """
+    Select frame based on the direction of the geometry.
+    """
+
+    def __init__(self, rel_geom_heading_min, rel_geom_heading_max):
+        self.rel_geom_heading_min = rel_geom_heading_min
+        self.rel_geom_heading_max = rel_geom_heading_max
+
+    def __call__(self, geom, cursor):
+        """
+        Return the first frame for which the relative geometry heading is within range.
+        Return the first frame if no such frame is found.
+        """
+        geom_centroid = geom.centroid.coords[0]
+        first_frame = Frame(cursor)
+        frame = first_frame
+        while frame is not None:
+            rel_geom_heading = compute_rel_geom_heading(frame, geom_centroid)
+            if self.rel_geom_heading_min < rel_geom_heading < self.rel_geom_heading_max:
+                return frame
+            frame = Frame(cursor)
+        return first_frame
+
+
+DISTANCE_MIN = 10
+DISTANCE_MAX = 20
+FRAME_LIMIT = 10
+GEOM_HEADING_FRAME_SELECTOR = GeomHeadingFrameSelector(90, 270)
+
+
 class Look_at:
     """
-        Simple class that describes what geometry the virtual camera
-        should look at and from which frame.        
+    Simple class that describes what geometry the virtual camera
+    should look at and from which frame.
     """
+
     frame: Frame = None
     geometry = None
 
     def __init__(self, frame, geometry):
         self.frame = frame
         self.geometry = geometry
         self.gp = Geometry_proj()
 
     def to_geographic_loc_list(self):
-        return self.gp.to_geographic(self.geometry) 
+        return self.gp.to_geographic(self.geometry)
 
 
 def add_to_output(frame, geometry, filename, nr, matched_frame):
     """
-       Add the current geometry and attributes to the output database
+    Add the current geometry and attributes to the output database
     """
     global output_database
 
     record = {}
     record["geometry"] = gpd.GeoSeries(geometry)
     record["snapshot"] = filename
     record["sub_id"] = nr
     record["frame_index"] = frame.index
     record["recording_id"] = frame.recordingid
-    record["distance"] = geod.line_length(*zip(*[frame.get_location()[:2], geometry.centroid.coords[0]]))
+    record["distance"] = geod.line_length(
+        *zip(*[frame.get_location()[:2], geometry.centroid.coords[0]])
+    )
 
     for k, v in matched_frame.metadata.items():
         record[k] = v
 
     gdf = gpd.GeoDataFrame(record)
 
     if output_database is None:
         output_database = gdf
     else:
         output_database = pd.concat([output_database, gdf])
 
 
-def try_find_frame_within(geometry, mf: FrameMatchedIterator.MatchedFrame, distance_min, distance_max):
+def try_find_frame(geometry, mf: FrameMatchedIterator.MatchedFrame):
     """
-       Try to find a frame from the same recording that is within (distance_min,distance_max)
+    Try to find a frame from the same recording that is within (DISTANCE_MIN, DISTANCE_MAX)
     """
     frames = Frames(connection)
-    cursor = frames.query(within=(*geometry.centroid.coords, distance_max),
-                          recordingid=mf.recording.id,
-                          distance=(*geometry.centroid.coords, "> %s",
-                                    distance_min), limit=1)
-
-    if (cursor != None):
-        return Frame(cursor)
-    return None
+    cursor = frames.query(
+        within=(*geometry.centroid.coords, DISTANCE_MAX),
+        recordingid=mf.recording.id,
+        distance=(*geometry.centroid.coords, "> %s", DISTANCE_MIN),
+        limit=FRAME_LIMIT,
+    )
+    return GEOM_HEADING_FRAME_SELECTOR(geometry, cursor)
 
 
 def look_at_point(point, mf: FrameMatchedIterator.MatchedFrame, side):
     """
-        Transforms a 'Point' geometry into a square of sides 'side'x'side'
-        in meters
+    Transforms a 'Point' geometry into a square of sides 'side'x'side'
+    in meters
     """
     gp = Geometry_proj()
-    square = gp.point_to_square(point, 0.5)
+    square = gp.point_to_square(point, side)
     return [Look_at(mf.frame, square)]
 
 
-def look_at_linestring(linestring, mf: FrameMatchedIterator.MatchedFrame, max_length, distance_min, distance_max, offset):
+def look_at_linestring(
+    linestring,
+    mf: FrameMatchedIterator.MatchedFrame,
+    max_length,
+    offset,
+):
     """
-        Transforms a 'LineString' geometry into sub LineStrings of maximum length
-        of 'max_length' in meters.
+    Transforms a 'LineString' geometry into sub LineStrings of maximum length
+    of 'max_length' in meters.
     """
     gp = Geometry_proj()
-    
+
     if geod.geometry_length(linestring) > max_length:
-        
-        linestrings = gp.split_linestring(linestring,max_length)
-                
+        linestrings = gp.split_linestring(linestring, max_length)
+
         look_at_all_sub_string = []
         for w in linestrings:
-
-            frame = try_find_frame_within(w, mf, distance_min, distance_max)
+            frame = try_find_frame(w, mf)
 
             if not frame is None:
                 mf.frame = frame
 
-            look_at_all_sub_string.append(look_at_linestring(
-                w, mf, max_length, distance_min, distance_max, offset)[0])
+            look_at_all_sub_string.append(
+                look_at_linestring(w, mf, max_length, offset)[0]
+            )
 
         return look_at_all_sub_string
 
-    return [Look_at(mf.frame,gp.buffer(linestring, offset))]    
+    return [Look_at(mf.frame, gp.buffer(linestring, offset))]
 
 
 def look_at_polygon(polygon, mf: FrameMatchedIterator.MatchedFrame):
     """
-        Transforms a 'Polygon' geometry into a collection of Polygons..
+    Transforms a 'Polygon' geometry into a collection of Polygons..
     """
     return [Look_at(mf.frame, polygon)]
 
 
-def take_shaphost(db, mf: FrameMatchedIterator.MatchedFrame, geod):
-
+def take_snapshot(db, mf: FrameMatchedIterator.MatchedFrame, geod):
     geometries = []
     geo = db.get_geometry(mf.spatialite_cursor)[db.geometry_field_name]
-    
-    if geo.type.startswith('Multi'):
+
+    if geo.geom_type.startswith("Multi"):
         for g in geo.geoms:
             geometries.append(g)
     else:
         geometries.append(geo)
 
     width = 800
     look_at_all: [Look_at] = []
 
     for geom in geometries:
-        if geom.type == "Polygon":
+        if geom.geom_type == "Polygon":
             look_at_all = [*look_at_all, *look_at_polygon(geom, mf)]
-        elif geom.type == "LineString":
-            look_at_all = [*look_at_all, *look_at_linestring(geom, mf, 5, 10, 20, 0.1)]       
-        elif geom.type == "Point":
-            look_at_all = [*look_at_all, *look_at_point(geom,mf, 0.3) ]       
+        elif geom.geom_type == "LineString":
+            look_at_all = [*look_at_all, *look_at_linestring(geom, mf, 5, 0.1)]
+        elif geom.geom_type == "Point":
+            look_at_all = [*look_at_all, *look_at_point(geom, mf, 0.5)]
         else:
-            print("Not supported", geom.type)
+            print("Not supported", geom.geom_type)
 
-    nr_shaphosts = len(look_at_all)
+    nr_snapshots = len(look_at_all)
 
     for x, look_at in enumerate(look_at_all):
         look_at_geometry = look_at.to_geographic_loc_list()
 
         sp_camera.set_frame(mf.recording, look_at.frame)
         size = sp_camera.look_at_all(look_at_geometry, width)
-        spherical_image = sp_camera.crop_to_geometry(sp_camera.acquire(size), look_at_geometry)
+        spherical_image = sp_camera.crop_to_geometry(
+            sp_camera.acquire(size), look_at_geometry
+        )
 
         # Write output
         db_id = mf.spatialite_cursor[db.field_info_map["rowid"].idx]
-        print("Snapshot:", "db id", db_id, "nr",
-              x+1, "/", nr_shaphosts, geom.type)
-
-        filename = 'output/snapshot_db_id:' + \
-            str(db_id) + '_' + str(x+1) + '_' + geom.type + '.jpeg'
+        print(
+            "Snapshot:", "db id", db_id, "nr", x + 1, "/", nr_snapshots, geom.geom_type
+        )
+
+        filename = (
+            "output/snapshot_db_id:"
+            + str(db_id)
+            + "_"
+            + str(x + 1)
+            + "_"
+            + geom.geom_type
+            + ".jpeg"
+        )
 
-        add_to_output(look_at.frame, look_at.geometry, filename, x+1, mf)
+        add_to_output(look_at.frame, look_at.geometry, filename, x + 1, mf)
 
-        with open(filename, 'wb') as image_file:
+        with open(filename, "wb") as image_file:
             image_file.write(spherical_image.get_image().getvalue())
             spherical_image.get_image().close()
 
 
 db = Spatialite(args.sqlite_db)
 
 
@@ -224,38 +297,39 @@
 db.resolve()
 db.show_info()
 
 sp_camera = SphericalCamera()
 sp_camera.set_network_client(client)
 
 fmi: FrameMatchedIterator = db.get_matched_frames_iterator()
-fmi.set_distance_limits(10, 20)
+fmi.set_distance_limits(DISTANCE_MIN, DISTANCE_MAX)
+fmi.set_frame_limit(FRAME_LIMIT)
+fmi.set_frame_selector(GEOM_HEADING_FRAME_SELECTOR)
 
-if (not args.recording_id is None):
+if not args.recording_id is None:
     fmi.set_static_recording_by_id(args.recording_id)
 
 
 mf: FrameMatchedIterator.MatchedFrame = next(fmi, None)
 
 while mf != None:
-
     try:
         if mf.oke():
-            take_shaphost(db, mf, geod)
+            take_snapshot(db, mf, geod)
         else:
             print("\nIncomplete match")
             print(mf.dump())
     except Exception as e:
         if str(e) == "Request-sent":
             # reset network connection
             client = util.get_client(args)
             sp_camera.set_network_client(client)
-        print("Exception", e)
-        print("Properties: ", mf.properties)
-        print("Metadata: ", mf.metadata)
+        print("Exception:", e)
+        print("Properties:", mf.properties)
+        print("Metadata:", mf.metadata)
         pass
     mf = next(fmi, None)
 
 db.close()
 
 if not output_database is None:
-    output_database.to_file("output/snapshots.geojson", driver='GeoJSON')
+    output_database.to_file("output/snapshots.geojson", driver="GeoJSON")
```

### Comparing `horus-media-client-0.9.4/horus_media_examples/spherical_camera.py` & `horus-media-client-0.9.5/horus_media_examples/spherical_camera.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,32 +8,39 @@
 from horus_camera import SphericalCamera, Pixel, SphericalImage, GeoReferencedPixel
 from horus_db import Frames, Recordings, Frame, Recording
 from horus_gis import SchemaProvider, GeographicLocation
 
 from . import util
 
 
-#------- If geopandas & pandora are installed
+# ------- If geopandas & pandora are installed
 database = None
 try:
     from horus_geopandas import HorusGeoDataFrame
     import geopandas as gpd
 
     sp = SchemaProvider()
     database = HorusGeoDataFrame(sp.single_measurement())
 
 except ModuleNotFoundError:
     pass
 
-def fill_record(record,grp: GeoReferencedPixel, camera:SphericalCamera, image:SphericalImage):
-    print("TEST--->", )
-    print("TEST--->",  image.get_geo_location_camera().lat)
+
+def fill_record(
+    record, grp: GeoReferencedPixel, camera: SphericalCamera, image: SphericalImage
+):
+    print(
+        "TEST--->",
+    )
+    print("TEST--->", image.get_geo_location_camera().lat)
 
     # update geometry
-    record["geometry"] = geopandas.points_from_xy(x=[grp.geo_location.lon], y=[grp.geo_location.lat])
+    record["geometry"] = geopandas.points_from_xy(
+        x=[grp.geo_location.lon], y=[grp.geo_location.lat]
+    )
     # Record
     record["rec_id"] = grp.recording_id
     record["frame_idx"] = grp.frame_index
     #
     record["cam_fov"] = camera.h_fov.value
     record["cam_yaw"] = camera.yaw
     record["cam_pitch"] = camera.pitch
@@ -56,15 +63,14 @@
     #
     record["vp_px_x"] = grp.pixel_location.col
     record["vp_px_y"] = grp.pixel_location.row
     record["vp_yaw"] = grp.viewing_parameters.yaw
     record["vp_pitch"] = grp.viewing_parameters.pitch
 
 
-
 # ----------    Overview  --------------
 #
 # This example shows how a series --minimum of 3-- of geo referenced pixels (GeoReferencedPixel)
 # obtained from a spherical image are used to calculate an accurate GeographicLocation for a specific label.
 #
 # This is done in several steps:
 #
@@ -86,36 +92,42 @@
 args = parser.parse_args()
 
 connection = util.get_connection(args)
 client = util.get_client(args)
 recordings = Recordings(connection)
 
 # Select the demo city of Rotterdam
-recording = next(Recording.query(
-    recordings, directory_like="Rotterdam360\\\\Ladybug5plus"))
+recording = next(
+    Recording.query(recordings, directory_like="Rotterdam360\\\\Ladybug5plus")
+)
 recordings.get_setup(recording)
 print(recording, " -> ", recording.directory)
 print(recording.setup)
 
 # Step 1. create and configure spherical camera
 sp_camera = SphericalCamera()
 sp_camera.set_network_client(client)
 
 # Step 2. Get a recorded frame and place the camera onto that 'frame'
 frames = Frames(connection)
-results = Frame.query(frames, recordingid=recording.id,
-                      index=210, order_by="index",)
+results = Frame.query(
+    frames,
+    recordingid=recording.id,
+    index=210,
+    order_by="index",
+)
 
 # step 3. do some sight seeing..
 # This sections hardcodes looking at points of interest, which
 # normally would come from image processing or AI tooling.
 
 
-class Poi():
-    """Describes and labels a point of interest within the image """
+class Poi:
+    """Describes and labels a point of interest within the image"""
+
     pixel: Pixel
     name: str
     yaw: float
     pitch: float
 
     def __init__(self, pixel, name, yaw, pitch) -> None:
         self.name = name
@@ -123,81 +135,94 @@
         self.yaw = yaw
         self.pixel = pixel
 
 
 # The list that describes:
 # [ frame index -> [Points of interests] ]
 frames_of_interest = [
-    [210, [
-        Poi(Pixel(287, 353), "p1", 20, -30),
-        Poi(Pixel(209, 284), "p2", 20, -30),
-        Poi(Pixel(213, 595), "p3", -40, -30)
-    ]],
-    [212, [
-        Poi(Pixel(465, 590), "p1", 20, -30),
-        Poi(Pixel(215, 343), "p2", 20, -30),
-        Poi(Pixel(225, 604), "p3", -40, -30)
+    [
+        210,
+        [
+            Poi(Pixel(287, 353), "p1", 20, -30),
+            Poi(Pixel(209, 284), "p2", 20, -30),
+            Poi(Pixel(213, 595), "p3", -40, -30),
+        ],
     ],
+    [
+        212,
+        [
+            Poi(Pixel(465, 590), "p1", 20, -30),
+            Poi(Pixel(215, 343), "p2", 20, -30),
+            Poi(Pixel(225, 604), "p3", -40, -30),
+        ],
+    ],
+    [
+        214,
+        [
+            Poi(Pixel(379, 613), "p1", 120, -30),
+            Poi(Pixel(234, 303), "p2", 30, -30),
+            Poi(Pixel(244, 542), "p3", -40, -30),
+        ],
     ],
-    [214, [
-        Poi(Pixel(379, 613), "p1", 120, -30),
-        Poi(Pixel(234, 303), "p2", 30, -30),
-        Poi(Pixel(244, 542), "p3", -40, -30)
-    ]
-    ]
 ]
 
 # Step 4,
 # That actual processing of the provided data
 # Creating a set of labelled geo referenced pixels [GeoReferencedPixel]
 # which we will use to triangulate in step 6 for a more accurate location
 list_of_images = []
 
 for foi in frames_of_interest:
-    results = Frame.query(frames, recordingid=recording.id,
-                          index=foi[0], order_by="index",)
+    results = Frame.query(
+        frames,
+        recordingid=recording.id,
+        index=foi[0],
+        order_by="index",
+    )
     frame = next(results)
     if frame is None:
         print("No frames!")
         exit()
 
     print("Got frame:", frame, frame.get_location())
     sp_camera.set_frame(recording, frame)
     print("camera_height", sp_camera.height)
 
     for poi in foi[1]:
-
         # -- obtain database
         record = None
         if database is not None:
             record = database.new_frame()
 
         sp_camera.set_horizontal_fov(90)
         sp_camera.set_yaw(poi.yaw)
         sp_camera.set_pitch(poi.pitch)
 
         spherical_image = sp_camera.acquire(Size(800, 800))
 
-        with open('frame' + str(frame.index) + '_' + poi.name + '.jpeg', 'wb') as image_file:
+        with open(
+            "frame" + str(frame.index) + "_" + poi.name + ".jpeg", "wb"
+        ) as image_file:
             image_file.write(spherical_image.get_image().getvalue())
             spherical_image.get_image().close()
 
         # Step 5
         # obtain a GeoReferencedPixel
         grp: GeoReferencedPixel = spherical_image.project_pixel_on_ground_surface(
-            poi.pixel)
+            poi.pixel
+        )
         grp.name = poi.name
 
         # you can store multiple GeoReferencedPixels with a different label
         spherical_image.store_geo_referenced_pixel(grp)
 
         list_of_images.append(spherical_image)
 
         if record is not None:
-            fill_record(record,grp,sp_camera,spherical_image)
+            fill_record(record, grp, sp_camera, spherical_image)
             database.add_frame(record)
 
     if database:
         record = database.new_frame()
 
 # Step 6
 # Triangulate the labels
@@ -210,13 +235,21 @@
 print("")
 print("latitude longitude altitude name frame recording row col")
 
 # print  GeoReferencedPixel's
 for img in list_of_images:
     for name in img.geo_referenced_pixels:
         grp: GeoReferencedPixel = img.geo_referenced_pixels[name]
-        print(grp.geo_location.lat, grp.geo_location.lon, grp.geo_location.alt, grp.name,
-              grp.frame_index, grp.recording_id, grp.pixel_location.row, grp.pixel_location.col)
+        print(
+            grp.geo_location.lat,
+            grp.geo_location.lon,
+            grp.geo_location.alt,
+            grp.name,
+            grp.frame_index,
+            grp.recording_id,
+            grp.pixel_location.row,
+            grp.pixel_location.col,
+        )
 
 print(p1_tri.lat, p1_tri.lon, p1_tri.alt, "p1_tr", -1, -1, -1, -1)
 print(p2_tri.lat, p2_tri.lon, p2_tri.alt, "p2_tr", -1, -1, -1, -1)
 print(p3_tri.lat, p3_tri.lon, p3_tri.alt, "p3_tr", -1, -1, -1, -1)
```

### Comparing `horus-media-client-0.9.4/horus_media_examples/spherical_camera_single_measurement.py` & `horus-media-client-0.9.5/horus_media_examples/spherical_camera_single_measurement.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,25 +2,41 @@
 import copy
 import os
 from pprint import pprint
 
 
 import json
 from horus_media import Size
-from horus_camera import SphericalCamera, Pixel, SphericalImage, GeoReferencedPixel, ViewParameterizedPixel
+from horus_camera import (
+    SphericalCamera,
+    Pixel,
+    SphericalImage,
+    GeoReferencedPixel,
+    ViewParameterizedPixel,
+)
 from horus_db import Frames, Recordings, Frame, Recording
 from horus_gis import SchemaProvider
 from . import util
 from horus_geopandas import HorusGeoDataFrame
 import geopandas as gpd
 
-def fill_record(record,frame,grp: GeoReferencedPixel, det_vp: ViewParameterizedPixel,camera:SphericalCamera, image:SphericalImage, detection):
 
+def fill_record(
+    record,
+    frame,
+    grp: GeoReferencedPixel,
+    det_vp: ViewParameterizedPixel,
+    camera: SphericalCamera,
+    image: SphericalImage,
+    detection,
+):
     # update geometry
-    record["geometry"] = gpd.points_from_xy(x=[grp.geo_location.lon], y=[grp.geo_location.lat])
+    record["geometry"] = gpd.points_from_xy(
+        x=[grp.geo_location.lon], y=[grp.geo_location.lat]
+    )
     # Record
     record["rec_id"] = grp.recording_id
     record["frame_idx"] = grp.frame_index
     record["azimuth"] = frame.azimuth
     #
     record["cam_fov"] = camera.h_fov.value
     record["cam_yaw"] = camera.yaw
@@ -28,15 +44,15 @@
     record["cam_width"] = image.get_resolution().width
     record["cam_height"] = image.get_resolution().height
     record["cam_lat"] = image.get_geo_location_camera().lat
     record["cam_lon"] = image.get_geo_location_camera().lon
     record["cam_alt"] = image.get_geo_location_camera().alt
     #
     record["dt_class"] = detection.classification
-    record["dt_name"] =  detection.name
+    record["dt_name"] = detection.name
     record["dt_x"] = detection.detection_pixel.col
     record["dt_y"] = detection.detection_pixel.row
     record["dt_width"] = detection.detection_size.width
     record["dt_height"] = detection.detection_size.height
     record["dt_conf"] = detection.confidence
     record["dt_dist"] = grp.distance
 
@@ -49,15 +65,14 @@
     # viewing parameters of the surface projection
     record["surf_px_x"] = grp.pixel_location.col
     record["surf_px_y"] = grp.pixel_location.row
     record["surf_yaw"] = grp.viewing_parameters.yaw
     record["surf_pitch"] = grp.viewing_parameters.pitch
 
 
-
 # ----------    Overview  --------------
 #
 # This example shows how a series --minimum of 3-- of geo referenced pixels (GeoReferencedPixel)
 # obtained from a spherical image are used to calculate an accurate GeographicLocation for a specific label.
 #
 # This is done in several steps:
 #
@@ -80,136 +95,141 @@
 
 connection = util.get_connection(args)
 client = util.get_client(args)
 recordings = Recordings(connection)
 
 
 # Opening JSON file
-f = open('input/spherical_camera_single_measurement.json')
+f = open("input/spherical_camera_single_measurement.json")
 data = json.load(f)
 
 # Select the demo city of Rotterdam
-recording = next(Recording.query(
-    recordings, directory_like=data["recording_name"]))
+recording = next(Recording.query(recordings, directory_like=data["recording_name"]))
 recordings.get_setup(recording)
 print(recording, " -> ", recording.directory)
 print(recording.setup)
 
 
-
-
 # Step 1. create and configure spherical camera
 sp_camera = SphericalCamera()
 sp_camera.set_network_client(client)
 
 # Step 2. Get a recorded frame and place the camera onto that 'frame'
 frames = Frames(connection)
-results = Frame.query(frames, recordingid=recording.id,
-                      index=210, order_by="index",)
+results = Frame.query(
+    frames,
+    recordingid=recording.id,
+    index=210,
+    order_by="index",
+)
 
 # step 3. do some sight seeing..
 # This sections hardcodes looking at points of interest, which
 # normally would come from image processing or AI tooling.
 
 sp = SchemaProvider()
 database = HorusGeoDataFrame(sp.single_measurement())
 
 
 class Camera:
     yaw: float
     pitch: float
     cam_size: Size
-    cam_hor_fov:float
+    cam_hor_fov: float
 
     def __init__(self):
         self.yaw = 0
         self.pitch = -10
-        self.cam_size = Size(800,800)
+        self.cam_size = Size(800, 800)
         self.cam_hor_fov = 90
 
-    def load(self,data):
+    def load(self, data):
         if "width" in data:
-            self.cam_size = Size(int(data["width"]),self.cam_size.height)
+            self.cam_size = Size(int(data["width"]), self.cam_size.height)
         if "height" in data:
-            self.cam_size = Size(self.cam_size.width,int(data["height"]))
+            self.cam_size = Size(self.cam_size.width, int(data["height"]))
         if "yaw" in data:
             self.yaw = float(data["yaw"])
         if "pitch" in data:
             self.pitch = float(data["pitch"])
         if "horizontal_fov" in data:
             self.cam_hor_fov = float(data["horizontal_fov"])
 
-
     def clone(self):
         return copy.deepcopy(self)
 
+
 class Detection:
-    """Describes and a Detection / Point of interest within the image """
+    """Describes and a Detection / Point of interest within the image"""
+
     surface_pixel: Pixel
     detection_pixel: Pixel
     detection_size: Size
-    classification :int
-    name:str
-    confidence : float
+    classification: int
+    name: str
+    confidence: float
     camera: Camera
 
-    def __init__(self,camera) -> None:
+    def __init__(self, camera) -> None:
         self.camera = camera
 
-    def load(self,dt):
-        self.surface_pixel = Pixel(int(dt["surface_pixel"]["r"]),int(dt["surface_pixel"]["c"]))
-        self.detection_pixel = Pixel(int(dt["detection_pixel"]["r"]), int(dt["detection_pixel"]["c"]))
-        self.detection_size = Size(int(dt["detection_size"]["width"]), int(dt["detection_size"]["height"]))
+    def load(self, dt):
+        self.surface_pixel = Pixel(
+            int(dt["surface_pixel"]["r"]), int(dt["surface_pixel"]["c"])
+        )
+        self.detection_pixel = Pixel(
+            int(dt["detection_pixel"]["r"]), int(dt["detection_pixel"]["c"])
+        )
+        self.detection_size = Size(
+            int(dt["detection_size"]["width"]), int(dt["detection_size"]["height"])
+        )
 
         self.name = dt["name"]
         self.confidence = float(dt["confidence"])
         self.classification = int(dt["classification"])
 
         if "camera" in dt:
             self.camera.load(dt["camera"])
 
 
-
-
-
-
-
 # Step 4,
 # That actual processing of the provided data
 # Creating a set of labelled geo referenced pixels [GeoReferencedPixel]
 # which we will use to triangulate in step 6 for a more accurate location
 list_of_images = []
 
 camera = Camera()
 camera.load(data["camera"])
 
 detections_per_frame = data["detections_per_frame"]
 
 # Create output directory
-output_dir = os.path.join(os.getcwd(), 'output')
+output_dir = os.path.join(os.getcwd(), "output")
 
 if not os.path.exists(output_dir):
     os.makedirs(output_dir)
 
 
 for frame_id in detections_per_frame:
-    results = Frame.query(frames, recordingid=recording.id,
-                          index=frame_id, order_by="index",)
+    results = Frame.query(
+        frames,
+        recordingid=recording.id,
+        index=frame_id,
+        order_by="index",
+    )
     frame = next(results)
     if frame is None:
         print("No frames!")
         exit()
 
     print("Got frame:", frame, frame.get_location())
     sp_camera.set_frame(recording, frame)
     print("camera_height", sp_camera.height)
 
-
     for detection_id in detections_per_frame[frame_id]:
-
         detection = Detection(camera.clone())
         detection.load(detections_per_frame[frame_id][detection_id])
 
         # -- obtain database frame
         record = database.new_frame()
 
         # -- set the camera
@@ -223,22 +243,25 @@
         # with open(output_dir + '/frame' + str(frame.index) + '_' + detection.name + '.jpeg', 'wb') as image_file:
         #    image_file.write(spherical_image.get_image().getvalue())
         #    spherical_image.get_image().close()
 
         # Step 5
         # obtain a GeoReferencedPixel on the surface
         grp: GeoReferencedPixel = spherical_image.project_pixel_on_ground_surface(
-            detection.surface_pixel)
+            detection.surface_pixel
+        )
         grp.name = detection.name
 
         # step 6
         # obtain the ViewParameterizedPixel of the actual detection
-        detection_parms = spherical_image.get_view_parameterized_pixel(detection.detection_pixel);
-
-        fill_record(record,frame,grp,detection_parms,sp_camera,spherical_image, detection)
+        detection_parms = spherical_image.get_view_parameterized_pixel(
+            detection.detection_pixel
+        )
+
+        fill_record(
+            record, frame, grp, detection_parms, sp_camera, spherical_image, detection
+        )
         record["usr_id"] = database.dataframe.shape[0]
         database.add_frame(record)
 
 
-
 database.write_shapefile(os.path.join(output_dir, "single_measurement.shp"))
-
```

### Comparing `horus-media-client-0.9.4/horus_media_examples/spherical_camera_single_measurement_reconstruction.py` & `horus-media-client-0.9.5/horus_media_examples/spherical_camera_single_measurement_reconstruction.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,144 +3,161 @@
 import geopandas as gpd
 import pandas as pd
 import sys
 from PIL import Image, ImageDraw
 import io
 
 
-
-
 from horus_gis import SchemaProvider
 from horus_geopandas import HorusGeoDataFrame
 from horus_camera import SphericalCamera
 from horus_db import Frames, Recordings, Frame, Recording
 from horus_media import Size
 from . import util
 
 
 # Step 0
 # Configuration part
 parser = util.create_argument_parser()
 util.add_database_arguments(parser)
 util.add_server_arguments(parser)
-parser.add_argument("-f", "--frame", type=int,nargs=1)
-parser.add_argument("-i", "--input", type=str,nargs=1)
+parser.add_argument("-f", "--frame", type=int, nargs=1)
+parser.add_argument("-i", "--input", type=str, nargs=1)
 
 
 args = parser.parse_args()
 
 
-
-
 ### Read Data ####
 sp = SchemaProvider()
 database = HorusGeoDataFrame(sp.single_measurement())
 
 # provide a map of the new 'fields' with their default value
 # missing fields will cause a schema exception
 single_measurement_path = "output/single_measurement.shp"
 if not os.path.exists(single_measurement_path):
     print(f"File '{single_measurement_path}' not found.")
     exit(1)
 
 database.append_file(single_measurement_path)
 
+
 ## Prepare Work,
 class Work:
     info = None
-    indices:[]
+    indices: []
+
 
 worklist = {}
 
-for index, row in database.dataframe.iterrows(): # Looping over all points
-    if row['frame_idx'] == args.frame[0]:
-        id = str(row['frame_idx']) + ":" + str(row['cam_width']) + "x" + str(row['cam_height'])
-        id += "_[" + str(row['cam_fov']) + "][" + str(row['cam_yaw']) + "][" + str(row['cam_pitch'])+"]"
+for index, row in database.dataframe.iterrows():  # Looping over all points
+    if row["frame_idx"] == args.frame[0]:
+        id = (
+            str(row["frame_idx"])
+            + ":"
+            + str(row["cam_width"])
+            + "x"
+            + str(row["cam_height"])
+        )
+        id += (
+            "_["
+            + str(row["cam_fov"])
+            + "]["
+            + str(row["cam_yaw"])
+            + "]["
+            + str(row["cam_pitch"])
+            + "]"
+        )
 
         if id not in worklist:
             worklist[id] = Work()
             worklist[id].info = row
             worklist[id].indices = [index]
         else:
             worklist[id].indices.append(index)
 
 ## Perform Work,
 
 
-
 connection = util.get_connection(args)
 client = util.get_client(args)
 recordings = Recordings(connection)
 
 # Step 1. create and configure spherical camera
 sp_camera = SphericalCamera()
 sp_camera.set_network_client(client)
 
 # Step 2. Get a recorded frame and place the camera onto that 'frame'
 frames = Frames(connection)
 
 df = database.dataframe
 cnt = 0
 for workid in worklist:
-   cnt+=1
-   print(cnt,"/", len(worklist),workid)
-   job = worklist[workid]
-
-   recording = next(Recording.query(
-      recordings, id=job.info["rec_id"]))
-   recordings.get_setup(recording)
-
-   results = Frame.query(frames,
-       recordingid=job.info["rec_id"],
-       index=job.info["frame_idx"], order_by="index",)
-
-   frame = next(results)
-   # -- set the camera
-   sp_camera.set_frame(recording, frame)
-   sp_camera.set_horizontal_fov(job.info['cam_fov'])
-   sp_camera.set_yaw(job.info['cam_yaw'])
-   sp_camera.set_pitch(job.info['cam_pitch'])
-
-   # -- acquire
-   spherical_image = sp_camera.acquire(Size(job.info["cam_width"],job.info["cam_height"]))
-
-
-   # -- draw our findings
-
-   data = spherical_image.get_image().getvalue()
-   stream = io.BytesIO(data)
-   img = Image.open(stream)
-
-
-   draw = ImageDraw.Draw(img)
-   spherical_image.get_image().close()
-
-   for row in job.indices:
-      #print(row,"/",len(job))
-      record = df.loc[[row]]
-
-      if record.iloc[0]['dt_class'] != -1:
-         # pil upper left 0,0
-         x0 = record.iloc[0]['dt_x']
-         y0 = record.iloc[0]['dt_y']
-         w = record.iloc[0]['dt_width']
-         h = record.iloc[0]['dt_height']
-
-         shape = [ x0, y0, x0 + w , y0 + h]
-         draw.rectangle(shape, outline ="red")
-
-
-         surf_x =  record.iloc[0]['surf_px_x']
-         surf_y =  record.iloc[0]['surf_px_y']
-         #print(surf_x,surf_y)
-         draw.ellipse([surf_x-2, surf_y-2, surf_x+2, surf_y+2], fill = 'blue', outline ='blue')
-
-      draw.text((surf_x + 4, surf_y), record.iloc[0]['dt_name'], fill=None, font=None, anchor=None, spacing=0, align="left")
-
-
-
-      img.save('output/' + workid+'.jpeg')
-
-
-
-
+    cnt += 1
+    print(cnt, "/", len(worklist), workid)
+    job = worklist[workid]
+
+    recording = next(Recording.query(recordings, id=job.info["rec_id"]))
+    recordings.get_setup(recording)
+
+    results = Frame.query(
+        frames,
+        recordingid=job.info["rec_id"],
+        index=job.info["frame_idx"],
+        order_by="index",
+    )
+
+    frame = next(results)
+    # -- set the camera
+    sp_camera.set_frame(recording, frame)
+    sp_camera.set_horizontal_fov(job.info["cam_fov"])
+    sp_camera.set_yaw(job.info["cam_yaw"])
+    sp_camera.set_pitch(job.info["cam_pitch"])
+
+    # -- acquire
+    spherical_image = sp_camera.acquire(
+        Size(job.info["cam_width"], job.info["cam_height"])
+    )
+
+    # -- draw our findings
+
+    data = spherical_image.get_image().getvalue()
+    stream = io.BytesIO(data)
+    img = Image.open(stream)
+
+    draw = ImageDraw.Draw(img)
+    spherical_image.get_image().close()
+
+    for row in job.indices:
+        # print(row,"/",len(job))
+        record = df.loc[[row]]
+
+        if record.iloc[0]["dt_class"] != -1:
+            # pil upper left 0,0
+            x0 = record.iloc[0]["dt_x"]
+            y0 = record.iloc[0]["dt_y"]
+            w = record.iloc[0]["dt_width"]
+            h = record.iloc[0]["dt_height"]
+
+            shape = [x0, y0, x0 + w, y0 + h]
+            draw.rectangle(shape, outline="red")
+
+            surf_x = record.iloc[0]["surf_px_x"]
+            surf_y = record.iloc[0]["surf_px_y"]
+            # print(surf_x,surf_y)
+            draw.ellipse(
+                [surf_x - 2, surf_y - 2, surf_x + 2, surf_y + 2],
+                fill="blue",
+                outline="blue",
+            )
+
+        draw.text(
+            (surf_x + 4, surf_y),
+            record.iloc[0]["dt_name"],
+            fill=None,
+            font=None,
+            anchor=None,
+            spacing=0,
+            align="left",
+        )
 
+        img.save("output/" + workid + ".jpeg")
```

### Comparing `horus-media-client-0.9.4/horus_media_examples/spherical_camera_snapshot.py` & `horus-media-client-0.9.5/horus_media_examples/spherical_camera_snapshot.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,29 @@
-# Copyright(C) 2020 Horus View and Explore B.V.
+# Copyright(C) 2020, 2023 Horus View and Explore B.V.
 
 import psycopg2
 import os
 
 from horus_db import Frames, Frame, Recordings, Recording
-from horus_media import Client, ImageRequestBuilder, ImageProvider, Mode, Direction, Size
+from horus_media import (
+    Client,
+    ImageRequestBuilder,
+    ImageProvider,
+    Mode,
+    Direction,
+    Size,
+)
 from horus_camera import SphericalCamera
 from horus_gis import GeographicLocation
 
 from . import util
 
 
 # Create output directory
-output_dir = os.path.join(os.getcwd(), 'output')
+output_dir = os.path.join(os.getcwd(), "output")
 
 if not os.path.exists(output_dir):
     os.makedirs(output_dir)
 
 # This example shows how to create snapshots based on geometry
 
 
@@ -39,69 +46,81 @@
 
 
 # Step 1. create and configure spherical camera
 sp_camera = SphericalCamera()
 sp_camera.set_network_client(client)
 
 
-
-
-def take_shaphost(nr,recording:Recording, frame:Frame, positions):
+def take_snapshot(nr, recording: Recording, frame: Frame, positions):
     sp_camera.set_frame(recording, frame)
-    size = sp_camera.look_at_all(positions,1024)
+    size = sp_camera.look_at_all(positions, 1024)
 
-    spherical_image = sp_camera.crop_to_geometry(sp_camera.acquire(size), positions, True)
+    spherical_image = sp_camera.crop_to_geometry(
+        sp_camera.acquire(size), positions, True
+    )
 
-    with open(output_dir + '/snapshot'+ str(nr) + '.jpeg', 'wb') as image_file:
+    with open(output_dir + "/snapshot" + str(nr) + ".jpeg", "wb") as image_file:
         image_file.write(spherical_image.get_image().getvalue())
         spherical_image.get_image().close()
 
 
+snapshot_1 = [
+    "DemoData\Rotterdam360\Ladybug5plus",
+    16,
+    [
+        GeographicLocation(4.4883159319642543, 51.908492027690912, 53.361715),
+        GeographicLocation(4.4884184967537415, 51.908456244872745, 53.361715),
+        GeographicLocation(4.48847610048205, 51.908519406825874, 53.361715),
+        GeographicLocation(4.4883735356838885, 51.90855518966265, 53.361715),
+    ],
+]
+
+
+snapshot_2 = [
+    "DemoData\Rotterdam360\Ladybug5plus",
+    981,
+    [
+        GeographicLocation(4.4643636161038245, 51.910632575408812, 47.090053),
+        GeographicLocation(4.4644063962677194, 51.910582531617663, 47.090053),
+        GeographicLocation(4.46443096611172, 51.910590565679584, 47.090053),
+        GeographicLocation(4.464388185974328, 51.9106406094716, 47.090053),
+    ],
+]
+
+
+snapshot_3 = [
+    "DemoData\Rotterdam360\Ladybug5plus",
+    981,
+    [
+        GeographicLocation(4.4644173663344944, 51.910644188474507, 47.090053),
+        GeographicLocation(4.464431966331305, 51.910622670221294, 47.090053),
+        GeographicLocation(4.4644493531869944, 51.910627182612672, 47.090053),
+        GeographicLocation(4.4644347531983941, 51.910648700866034, 47.090053),
+    ],
+]
 
-
-snapshot_1 = ["DemoData\Rotterdam360\Ladybug5plus" , 16, [
-    GeographicLocation (4.4883159319642543,51.908492027690912, 53.361715),
-    GeographicLocation (4.4884184967537415,51.908456244872745, 53.361715),
-    GeographicLocation (4.48847610048205,51.908519406825874, 53.361715),
-    GeographicLocation (4.4883735356838885,51.90855518966265, 53.361715)
-    ]]
-
-
-snapshot_2 = ["DemoData\Rotterdam360\Ladybug5plus" , 981, [
-    GeographicLocation (4.4643636161038245,51.910632575408812,47.090053),
-    GeographicLocation (4.4644063962677194,51.910582531617663,47.090053),
-    GeographicLocation ( 4.46443096611172,51.910590565679584,47.090053),
-    GeographicLocation (4.464388185974328,51.9106406094716,47.090053)
-    ]]
-
-
-snapshot_3 = ["DemoData\Rotterdam360\Ladybug5plus" , 981, [
-    GeographicLocation (4.4644173663344944,51.910644188474507,47.090053),
-    GeographicLocation (4.464431966331305,51.910622670221294,47.090053),
-    GeographicLocation (4.4644493531869944,51.910627182612672,47.090053),
-    GeographicLocation (4.4644347531983941,51.910648700866034,47.090053)
-]]
-
-snapshots = [snapshot_1,snapshot_2,snapshot_3]
-
+snapshots = [snapshot_1, snapshot_2, snapshot_3]
 
 
 recordings = Recordings(connection)
 cursor = recordings.all()
 recording = Recording(cursor)
 while recording is not None:
     if snapshot_1[0] in recording.directory:
         recordings.get_setup(recording)
 
         nr = 0
         for snapshot in snapshots:
-            results = Frame.query(frames, recordingid=recording.id,
-                              index=snapshot[1],)
+            results = Frame.query(
+                frames,
+                recordingid=recording.id,
+                index=snapshot[1],
+            )
             frame = next(results)
-            take_shaphost(nr,recording,frame,snapshot[2])
+            take_snapshot(nr, recording, frame, snapshot[2])
             nr += 1
 
     # next recording
     recording = Recording(cursor)
 
 
-print("done")
+print("done")
```

### Comparing `horus-media-client-0.9.4/horus_media_examples/test_tool.py` & `horus-media-client-0.9.5/horus_media_examples/test_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 image_provider = ImageProvider()
 
 recordings = list(Recording.iter(Recordings(connection).all()))
 frames = Frames(connection)
 grid = Grid()
 
 streamHandler = logging.StreamHandler(sys.stdout)
-formatter = logging.Formatter('%(asctime)s %(levelname)s %(message)s')
+formatter = logging.Formatter("%(asctime)s %(levelname)s %(message)s")
 streamHandler.setFormatter(formatter)
 
 logger = logging.getLogger()
 logger.addHandler(streamHandler)
 logger.info("Started")
 logger.setLevel(logging.INFO)
 
@@ -36,13 +36,13 @@
     recording = sample(recordings, 1)[0]
     cursor = frames.query(recordingid=recording.id)
 
     frame = Frame(cursor)
 
     while frame is not None:
         request_builder = ImageRequestBuilder(frame.recordingid, frame.uuid)
-        requests = client.fetch_all(request_builder.build(
-            Mode.panoramic, Scales.Px_2048, section) for section in grid)
+        requests = client.fetch_all(
+            request_builder.build(Mode.panoramic, Scales.Px_2048, section)
+            for section in grid
+        )
         logging.info(f"{frame} {request_builder}")
         frame = Frame(cursor)
-
-
```

### Comparing `horus-media-client-0.9.4/horus_media_examples/triangulate_spherical_camera_single_measurement_clusters.py` & `horus-media-client-0.9.5/horus_media_examples/triangulate_spherical_camera_single_measurement_clusters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 from horus_gis import SchemaProvider, PositionVector, Geographic
 from horus_geopandas import HorusGeoDataFrame
 import geopandas as gpd
 import os
 
 ### Read Data ####
 sp = SchemaProvider()
-schema = sp.merge(sp.single_measurement(),sp.clustering())
+schema = sp.merge(sp.single_measurement(), sp.clustering())
 database = HorusGeoDataFrame(schema)
 
 single_measurement_path = "output/single_measurement.shp"
 if not os.path.exists(single_measurement_path):
-    print(f"File '{single_measurement_path}' not found.\nRun 'horus_media_examples.spherical_camera_single_measurement' first.")
+    print(
+        f"File '{single_measurement_path}' not found.\nRun 'horus_media_examples.spherical_camera_single_measurement' first."
+    )
     exit(1)
 database.append_file("output/single_measurement_clusters.shp")
 
 dataframe = database.dataframe
 
 ### Reconstruct PositionVector
-surf_vpp_per_cluster =  {k: [] for k in dataframe['clstr_id'].unique()}
+surf_vpp_per_cluster = {k: [] for k in dataframe["clstr_id"].unique()}
 geolocation_per_cluster = {}
-confidence_per_cluster ={}
+confidence_per_cluster = {}
 
 
-for index, row in dataframe.iterrows(): # Looping over all points
+for index, row in dataframe.iterrows():  # Looping over all points
     ### Surface info =  ViewParameterizedPixel
     pos_vector = PositionVector(
         dataframe.at[index, "cam_lat"],
         dataframe.at[index, "cam_lon"],
         dataframe.at[index, "cam_alt"],
         dataframe.at[index, "surf_yaw"],
-        dataframe.at[index, "surf_pitch"])
-    id =  dataframe.at[index, "clstr_id"]
+        dataframe.at[index, "surf_pitch"],
+    )
+    id = dataframe.at[index, "clstr_id"]
     surf_vpp_per_cluster[id].append(pos_vector)
 
 
 ### Triangulate
 for vpp in surf_vpp_per_cluster:
     pos_vectors = surf_vpp_per_cluster[vpp]
     geolocation_per_cluster[vpp] = Geographic.triangulate(pos_vectors)
-    confidence_per_cluster[vpp] = 0.7 # some metric
+    confidence_per_cluster[vpp] = 0.7  # some metric
 
 ### Write Data
 schema = sp.merge(sp.geometry_3dpoint(), sp.clustering())
 database = HorusGeoDataFrame(schema)
 
 for vpp in surf_vpp_per_cluster:
     lat = geolocation_per_cluster[vpp][0]
@@ -52,10 +55,8 @@
     record = database.new_frame()
     record["geometry"] = gpd.points_from_xy(x=[lon], y=[lat], z=[alt])
     record["clstr_id"] = vpp
     record["clstr_conf"] = confidence_per_cluster[vpp]
     database.add_frame(record)
 
 
-
-
-database.write_shapefile("output/cluster_locations.shp")
+database.write_shapefile("output/cluster_locations.shp")
```

### Comparing `horus-media-client-0.9.4/horus_media_examples/util.py` & `horus-media-client-0.9.5/horus_media_examples/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,95 +20,181 @@
         if option_string == "--s-file":
             file_name = namespace.s_file
 
         if file_name != None:
             f = open(file_name, "r")
             parser.parse_args(f.read().split(), namespace)
 
+
 def create_argument_parser():
     return argparse.ArgumentParser(
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter
+    )
+
 
 def add_database_arguments(parser):
     # db
-    parser.add_argument("--db-name", type=str,
-                        default="HorusWebMoviePlayer", help="the database name")
-    parser.add_argument("--db-user", type=str, default="postgres",
-                        help="database user name used to authenticate")
-    parser.add_argument("--db-password", type=str,
-                        help="database password used to authenticate")
-    parser.add_argument("--db-host", type=str, default="localhost",
-                        help="database database host address")
-    parser.add_argument("--db-port", type=int, default=5432,
-                        help="database connection port number")
-
-    parser.add_argument('--db-file', help="database configuration file", type=str,default="input/db.conf",action=read_arguments_from_file,nargs=0)
+    parser.add_argument(
+        "--db-name", type=str, default="HorusWebMoviePlayer", help="the database name"
+    )
+    parser.add_argument(
+        "--db-user",
+        type=str,
+        default="postgres",
+        help="database user name used to authenticate",
+    )
+    parser.add_argument(
+        "--db-password", type=str, help="database password used to authenticate"
+    )
+    parser.add_argument(
+        "--db-host",
+        type=str,
+        default="localhost",
+        help="database database host address",
+    )
+    parser.add_argument(
+        "--db-port", type=int, default=5432, help="database connection port number"
+    )
+
+    parser.add_argument(
+        "--db-file",
+        help="database configuration file",
+        type=str,
+        default="input/db.conf",
+        action=read_arguments_from_file,
+        nargs=0,
+    )
 
 
 def add_server_arguments(parser):
-    parser.add_argument("-s", "--server",  metavar="URL", type=str, default="http://localhost:5050/web/",
-                        help="Horus Media Server endpoint")
-    parser.add_argument("-st", "--server-timeout",  metavar="SECONDS", type=int, default=4,
-                        help="Horus Media Server timeout in seconds")
-    parser.add_argument("-sa", "--server-attempts",  metavar="ATTEMPTS", type=int, default=5,
-                        help="Horus Media Server number of attempts on connection failure")
-
-    parser.add_argument('--s-file', help="server configuration file",type=str, default="input/server.conf", action=read_arguments_from_file, nargs=0)
+    parser.add_argument(
+        "-s",
+        "--server",
+        metavar="URL",
+        type=str,
+        default="http://localhost:5050/web/",
+        help="Horus Media Server endpoint",
+    )
+    parser.add_argument(
+        "-st",
+        "--server-timeout",
+        metavar="SECONDS",
+        type=int,
+        default=4,
+        help="Horus Media Server timeout in seconds",
+    )
+    parser.add_argument(
+        "-sa",
+        "--server-attempts",
+        metavar="ATTEMPTS",
+        type=int,
+        default=5,
+        help="Horus Media Server number of attempts on connection failure",
+    )
+
+    parser.add_argument(
+        "--s-file",
+        help="server configuration file",
+        type=str,
+        default="input/server.conf",
+        action=read_arguments_from_file,
+        nargs=0,
+    )
 
 
 def add_size_argument(parser, default=(1024, 1024)):
-    parser.add_argument("-S", "--size",  metavar=("WIDTH", "HEIGHT"), nargs=2, type=int, default=default,
-                        help="size of the image")
+    parser.add_argument(
+        "-S",
+        "--size",
+        metavar=("WIDTH", "HEIGHT"),
+        nargs=2,
+        type=int,
+        default=default,
+        help="size of the image",
+    )
 
 
 def add_geometry_arguments(parser):
-    parser.add_argument("-gsc", "--geom-scale", type=int, default=400,
-                        help="output scale in px/m (orthographic)")
-    parser.add_argument("-gw", "--geom-width", type=float, default=6,
-                        help="geometry width (orthographic)")
-    parser.add_argument("-gh", "--geom-height", type=float, default=2,
-                        help="geometry height (orthographic)")
-    parser.add_argument("-gd", "--geom-dist", type=float, default=4,
-                        help="geometry distance (orthographic)")
-    parser.add_argument("-gs", "--geom-shift", type=float, default=0,
-                        help="geometry shift (orthographic)")
+    parser.add_argument(
+        "-gsc",
+        "--geom-scale",
+        type=int,
+        default=400,
+        help="output scale in px/m (orthographic)",
+    )
+    parser.add_argument(
+        "-gw",
+        "--geom-width",
+        type=float,
+        default=6,
+        help="geometry width (orthographic)",
+    )
+    parser.add_argument(
+        "-gh",
+        "--geom-height",
+        type=float,
+        default=2,
+        help="geometry height (orthographic)",
+    )
+    parser.add_argument(
+        "-gd",
+        "--geom-dist",
+        type=float,
+        default=4,
+        help="geometry distance (orthographic)",
+    )
+    parser.add_argument(
+        "-gs",
+        "--geom-shift",
+        type=float,
+        default=0,
+        help="geometry shift (orthographic)",
+    )
 
 
 def get_database_connection_string(args):
-    db_params = [("host", args.db_host),
-                 ("port", str(args.db_port)),
-                 ("dbname", args.db_name),
-                 ("user", args.db_user),
-                 ("password", args.db_password),
-                 ]
+    db_params = [
+        ("host", args.db_host),
+        ("port", str(args.db_port)),
+        ("dbname", args.db_name),
+        ("user", args.db_user),
+        ("password", args.db_password),
+    ]
 
-    return " ".join(
-        map("=".join, filter(lambda x: x[1] != None, db_params)))
+    return " ".join(map("=".join, filter(lambda x: x[1] != None, db_params)))
 
 
 def get_connection(args):
     try:
         return psycopg2.connect(get_database_connection_string(args))
     except psycopg2.OperationalError as exception:
         logging.error(f"{exception} Connecting to database")
         exit()
 
 
 def get_geometry(args, altitude_next=None):
-    return Geometry(args.geom_scale, args.geom_width,
-                    args.geom_height, args.geom_dist, args.geom_shift, altitude_next)
+    return Geometry(
+        args.geom_scale,
+        args.geom_width,
+        args.geom_height,
+        args.geom_dist,
+        args.geom_shift,
+        altitude_next,
+    )
 
 
 def get_client(args):
     try:
         client = Client(args.server, args.server_timeout)
         client.attempts = args.server_attempts
         return client
     except OSError as exception:
         logging.error(f"{exception}. Connecting to server {args.server}")
         exit(1)
 
 
 def sample_script_header(name):
     if name == "__main__":
-        print(f"This module is a sample script. It cannot run as an interactive example.")
+        print(
+            f"This module is a sample script. It cannot run as an interactive example."
+        )
         exit(1)
```

### Comparing `horus-media-client-0.9.4/horus_spatialite/__init__.py` & `horus-media-client-0.9.5/horus_spatialite/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Horus database"""
-# Copyright(C) 2022 Horus View and Explore B.V.
+# Copyright(C) 2022, 2023 Horus View and Explore B.V.
 
 import os
 import pathlib
 import glob
 from xml.etree import ElementTree
 from horus_db import Recording, Recordings, Frame, Frames
 
@@ -18,14 +18,15 @@
     raise e
 
 
 class Spatialite:
     """
     Database used for making annotations using the Horus Geo Suite
     """
+
     class Field_info(NamedTuple):
         idx: int
         name: str
         type: str
 
     recordings = {}
     blob_containing_geometry = {}
@@ -78,53 +79,66 @@
     def check_cursor(self, cursor):
         if cursor is None:
             cursor = self.get_cursor()
             return True, cursor
         return False, cursor
 
     def version(self):
-        return self.conn.execute('SELECT spatialite_version()').fetchone()[0]
+        return self.conn.execute("SELECT spatialite_version()").fetchone()[0]
 
     def get_table_name(self):
         return self.table_name
 
     def set_table_name(self, name):
         self.table_name = name
 
     def get_field_query(self, cursor):
-        cursor.execute("SELECT sql FROM sqlite_master WHERE tbl_name = '" +
-                       self.table_name + "' AND type = 'table'")
+        cursor.execute(
+            "SELECT sql FROM sqlite_master WHERE tbl_name = '"
+            + self.table_name
+            + "' AND type = 'table'"
+        )
 
     def get_table_info_query(self, cursor):
-        cursor.execute("PRAGMA table_info(\""+self.table_name+"\")")
+        cursor.execute('PRAGMA table_info("' + self.table_name + '")')
 
     def get_table_names(self, cursor):
         cursor.execute("SELECT name FROM sqlite_master WHERE type='table';")
 
     def get_recordings(self, cursor):
-        cursor.execute("SELECT DISTINCT	" + self.recording_field_name +
-                       " FROM \"" + self.table_name + "\";")
-    
+        cursor.execute(
+            "SELECT DISTINCT	"
+            + self.recording_field_name
+            + ' FROM "'
+            + self.table_name
+            + '";'
+        )
+
     def set_geometry_field_name(self, field_name):
-        self.geometry_field_name = field_name;
+        self.geometry_field_name = field_name
 
-    def blob_contains_geometry(self,field_name):
+    def blob_contains_geometry(self, field_name):
         self.blob_containing_geometry[field_name] = True
 
     def get_field_names_map(self, cursor=None) -> {str: Field_info}:
         if not self.field_info_map is None:
             return self.field_info_map
 
         cleanup, cursor = self.check_cursor(cursor)
         self.get_table_info_query(cursor)
         records = cursor.fetchall()
 
-        data = {row[self.FIELD_INFO_NAME]: Spatialite.Field_info(row[self.FIELD_INFO_IDX],
-                                                                 row[self.FIELD_INFO_NAME],
-                                                                 row[self.FIELD_INFO_TYPE]) for row in records}
+        data = {
+            row[self.FIELD_INFO_NAME]: Spatialite.Field_info(
+                row[self.FIELD_INFO_IDX],
+                row[self.FIELD_INFO_NAME],
+                row[self.FIELD_INFO_TYPE],
+            )
+            for row in records
+        }
         row_idx = len(data)
         data["rowid"] = Spatialite.Field_info(row_idx, "rowid", "INTEGER")
 
         if cleanup:
             cursor.close()
 
         return data
@@ -141,17 +155,17 @@
         fields = []
         for k, field in field_names_map.items():
             if field.type == self.FIELD_NAME_GEOM:
                 fields.append("AsText(" + k + ")")
             else:
                 fields.append(k)
 
-        myselect = ','.join(fields)
+        myselect = ",".join(fields)
 
-        query_ = "SELECT " + myselect + " FROM \""+self.table_name+"\""
+        query_ = "SELECT " + myselect + ' FROM "' + self.table_name + '"'
 
         add = " "
         for x in order_by_list:
             query_ += add + "ORDER BY " + x + " ASC"
             add = ","
 
         query_ += ";"
@@ -162,18 +176,18 @@
         if field_names_map == None:
             field_names_map = self.field_info_map
         geoms = {}
         for k, field in field_names_map.items():
             if field.type == self.FIELD_NAME_GEOM:
                 if cursor[field.idx] != None:
                     geoms[k] = wkt.loads(cursor[field.idx])
-            elif field.type == self.FIELD_NAME_BLOB:                
-                if field.name in self.blob_containing_geometry:                    
-                    if cursor[field.idx] != None:                        
-                        geoms[k] = wkb.loads(cursor[field.idx])                            
+            elif field.type == self.FIELD_NAME_BLOB:
+                if field.name in self.blob_containing_geometry:
+                    if cursor[field.idx] != None:
+                        geoms[k] = wkb.loads(cursor[field.idx])
         return geoms
 
     def get_matched_frames_iterator(self):
         cursor = self.get_cursor()
         orderby = []
         if self.recording_field_name in self.field_info_map:
             orderby.append(self.recording_field_name)
@@ -181,37 +195,41 @@
         return FrameMatchedIterator(cursor, self.RD_connection, self)
 
     def resolve(self):
         # obtain the fields with the table appended with rowid
         cursor = self.get_cursor()
         self.field_info_map = self.get_field_names_map(cursor)
 
-        if self.recording_field_name != None and self.recording_field_name in self.field_info_map:
+        if (
+            self.recording_field_name != None
+            and self.recording_field_name in self.field_info_map
+        ):
             # Get all the unique recordings in spatialite
             self.get_recordings(cursor)
             data = [x[0] for x in cursor.fetchall() if x[0] != None]
             for path in data:
                 __FIX_ME__ = path.replace("\\", "/")  # windows unix hell
                 p = pathlib.PurePath(__FIX_ME__)
                 if p.suffix.strip() == ".idx":
                     p = p.parent
                 self.recordings[path] = p.name
 
         # Resolve relation local recording(field) => remote
         if self.recording_field_name != None and self.RD_connection != None:
             self.spatialite_RD_recording_map = self.resolve_remote_recording(
-                self.recording_field_name, self.RD_connection, cursor)
+                self.recording_field_name, self.RD_connection, cursor
+            )
 
         # Resolve relation local recording(field => disk)
         if self.ROD_recordings_root_folder != None:
             self.resolve_on_disk_recording(self.ROD_recordings_root_folder)
 
     def match_paths(self, r, p, candidates):
-        r1 = r.split('\\')
-        c1 = [c.split('/') for c in candidates]
+        r1 = r.split("\\")
+        c1 = [c.split("/") for c in candidates]
 
         while r1[-1] != p:
             r1.pop()
 
         try:
             while True:
                 r1.pop()
@@ -228,64 +246,62 @@
                 if matched == 1:
                     return candidates[index]
         except:
             return None
 
     def resolve_on_disk_recording(self, recording_folder: str):
         for k, v in self.recordings.items():
-            folder = recording_folder+"**/"+v
+            folder = recording_folder + "**/" + v
 
             candidates = glob.glob(folder, recursive=True)
             matched = self.match_paths(k, v, candidates)
             if matched != None:
                 self.spatialite_ROD_recording_map[k] = matched
 
     def resolve_remote_recording(self, recording_field_name: str, connection, cursor):
         cleanup, cursor = self.check_cursor(cursor)
         resolved = {}
 
         for k, v in self.recordings.items():
             recordings = Recordings(connection)
-            cursor2 = Recording.query(
-                recordings, directory_like=v, order_by="id")
+            cursor2 = Recording.query(recordings, directory_like=v, order_by="id")
 
             rec = next(cursor2, None)
             recordings.get_setup(rec)
 
             recs = []
             while (rec) != None:
                 recs.append(rec)
                 rec = next(cursor2, None)
 
             while len(recs) != 1:
-                raise Exception(
-                    "Spatialite::resolve_recording Implement duplicate!")
+                raise Exception("Spatialite::resolve_recording Implement duplicate!")
 
             resolved[k] = recs[0]
 
         if cleanup:
             cursor.close()
 
         return resolved
 
     def resolve_frames(self, recording_name):
         for k, v in self.spatialite_ROD_recording_map.items():
             if k == recording_name:
-                tree = ElementTree.parse(v+"/frames.xml")
+                tree = ElementTree.parse(v + "/frames.xml")
                 root = tree.getroot()
                 a = tree.findall(
-                    "./{http://tempuri.org/FramesDataSet.xsd}Location/{http://tempuri.org/FramesDataSet.xsd}GUID")
+                    "./{http://tempuri.org/FramesDataSet.xsd}Location/{http://tempuri.org/FramesDataSet.xsd}GUID"
+                )
                 frame_location_guids = [x.text for x in a]
                 return frame_location_guids
 
     def __table_name_from_file__(self):
         return os.path.splitext(os.path.basename(self.filename))[0]
 
     def show_info(self):
-
         print("\n------- Spatialite --------")
         print("Version: ", self.version())
         print("Table: ", self.get_table_name())
         print("\n")
 
         print("\n------- Field Info --------")
         for k, field_info in self.field_info_map.items():
@@ -297,19 +313,19 @@
         print("\n------- Browse Data --------")
         self.query(cursor, self.field_info_map)
 
         entries = 4
         for row in cursor:
             if entries > 0:
                 entries -= 1
-                geoms = self.get_geometry(row, self.field_info_map)                
+                geoms = self.get_geometry(row, self.field_info_map)
                 print("--------------------")
                 for k, field_info in self.field_info_map.items():
                     if k in geoms:
-                        print(field_info.idx, ":", geoms[k]) 
+                        print(field_info.idx, ":", geoms[k])
                     else:
                         print(field_info.idx, ":", row[field_info.idx])
 
         print("\n-------  Recordings / Spatialite --------")
         for k, v in self.recordings.items():
             print(k, " -> ", v)
 
@@ -319,34 +335,38 @@
 
         print("\n-------  Recording / On Disk relation --------")
         for k, v in self.spatialite_ROD_recording_map.items():
             print(k, " -> ", v)
 
 
 class FrameMatchedIterator:
-
     class MatchedFrame:
         spatialite_cursor = None
         frame: Frame = None
         recording: Recording = None
         properties = {}
         metadata = {}
 
         def dump(self):
             print("spatialite_cursor", self.spatialite_cursor)
             print("Frame", self.frame)
             print("Recording", self.recording)
             print("Properties", self.properties)
 
         def oke(self):
-            return self.spatialite_cursor != None and self.frame != None and self.recording != None
+            return (
+                self.spatialite_cursor != None
+                and self.frame != None
+                and self.recording != None
+            )
 
     spatialite_db: Spatialite
     d_min: int = 5
     d_max: int = 10
+    frame_limit: int = 10
     current_recording: str = None
     static_recording: Recording = None
     recordings_list: [str, Recording] = {}
 
     guids: [str] = None
 
     use_recording_field = False
@@ -358,33 +378,48 @@
 
     def __init__(self, cursor, connection, spatialite_db: Spatialite):
         self.cursor = cursor
         self.connection = connection
         self.spatialite_db = spatialite_db
         self.frames = Frames(connection)
         self.recordings = Recordings(connection)
+        self.select_frame = lambda geom, cursor: Frame(cursor)
 
         # Can we use the Recording field
         if spatialite_db.recording_field_name != None:
-            if self.spatialite_db.recording_field_name in self.spatialite_db.field_info_map:
+            if (
+                self.spatialite_db.recording_field_name
+                in self.spatialite_db.field_info_map
+            ):
                 self.use_recording_field = True
                 self.recording_field_idx = self.spatialite_db.field_info_map[
-                    self.spatialite_db.recording_field_name].idx
+                    self.spatialite_db.recording_field_name
+                ].idx
 
         # Can we use Frame index field
         if spatialite_db.frame_index_field_name != None:
-            if self.spatialite_db.frame_index_field_name in self.spatialite_db.field_info_map:
+            if (
+                self.spatialite_db.frame_index_field_name
+                in self.spatialite_db.field_info_map
+            ):
                 self.use_frame_index_field = True
                 self.frame_index_field_idx = self.spatialite_db.field_info_map[
-                    self.spatialite_db.frame_index_field_name].idx
+                    self.spatialite_db.frame_index_field_name
+                ].idx
 
     def set_distance_limits(self, distance_min, distance_max):
         self.d_min = distance_min
         self.d_max = distance_max
 
+    def set_frame_limit(self, frame_limit):
+        self.frame_limit = frame_limit
+
+    def set_frame_selector(self, select_frame):
+        self.select_frame = select_frame
+
     def set_static_recording_by_id(self, id):
         recordings = Recordings(self.connection)
         cursor = Recording.query(recordings, id=id)
         recording = next(cursor, None)
         if recording != None:
             recordings.get_setup(recording)
             self.use_static_recording = True
@@ -393,100 +428,113 @@
     def __iter__(self):
         return self
 
     def __next__(self):
         frame = next(self.cursor, None)
 
         while frame != None:
-
             # Build up the matched frame
             f = self.MatchedFrame()
 
+            f.spatialite_cursor = frame
+
             use_recording_field = self.use_recording_field
             use_frame_index_field = self.use_frame_index_field
             frame_guid = None
             frame_index = None
 
             if use_recording_field:
                 if frame[self.recording_field_idx] == None:
                     use_recording_field = False
                 else:
                     if frame[self.recording_field_idx] != self.current_recording:
                         self.current_recording = frame[self.recording_field_idx]
                         self.guids = self.spatialite_db.resolve_frames(
-                            self.current_recording)
+                            self.current_recording
+                        )
 
             if use_frame_index_field:
                 if frame[self.frame_index_field_idx] == None:
                     use_frame_index_field = False
                 else:
                     frame_index = int(frame[self.frame_index_field_idx])
                     # Try to be more precise with GUID
                     if self.guids != None and len(self.guids) >= frame_index:
-                        frame_guid = self.guids[int(
-                            frame[self.frame_index_field_idx])]
+                        frame_guid = self.guids[int(frame[self.frame_index_field_idx])]
 
             if frame_guid != None:
                 f.properties["guid"] = frame_guid
 
             if frame_index != None:
                 f.properties["index"] = frame_index
 
             # Allow static recordings set_static_recording_by_id(..)
             if self.use_static_recording:
                 f.properties["recordingid"] = self.static_recording.id
 
             elif not self.current_recording is None:
                 if not self.spatialite_db.spatialite_RD_recording_map is None:
-                    if self.current_recording in self.spatialite_db.spatialite_RD_recording_map:
-                        f.properties["recordingid"] = self.spatialite_db.spatialite_RD_recording_map[self.current_recording].id
+                    if (
+                        self.current_recording
+                        in self.spatialite_db.spatialite_RD_recording_map
+                    ):
+                        f.properties[
+                            "recordingid"
+                        ] = self.spatialite_db.spatialite_RD_recording_map[
+                            self.current_recording
+                        ].id
 
             has_guid = "guid" in f.properties
             has_frame_index = "index" in f.properties
             has_recording_id = "recordingid" in f.properties
 
             if (has_recording_id and has_frame_index) or has_guid:
                 cursor = self.frames.query(**f.properties)
+                f.frame = Frame(cursor)
             else:
-                geom = self.spatialite_db.get_geometry(
-                    frame)[self.spatialite_db.geometry_field_name]
-
-                cursor = self.frames.query(within=(*geom.centroid.coords, self.d_max),
-                                           **f.properties,
-                                           distance=(*geom.centroid.coords, "> %s",
-                                                     self.d_min), limit=1)
-
-            f.spatialite_cursor = frame
-            f.frame = Frame(cursor)
+                geom = self.spatialite_db.get_geometry(frame)[
+                    self.spatialite_db.geometry_field_name
+                ]
+                cursor = self.frames.query(
+                    within=(*geom.centroid.coords, self.d_max),
+                    **f.properties,
+                    distance=(*geom.centroid.coords, "> %s", self.d_min),
+                    limit=self.frame_limit,
+                )
+                f.frame = self.select_frame(geom, cursor)
 
-            if (f.frame == None):
+            if f.frame == None:
                 return f
 
             if not f.frame.recordingid in self.recordings_list:
-                temp_rec = next(Recording.query(
-                    self.recordings, id=f.frame.recordingid))
+                temp_rec = next(
+                    Recording.query(self.recordings, id=f.frame.recordingid)
+                )
                 self.recordings.get_setup(temp_rec)
                 self.recordings_list[f.frame.recordingid] = temp_rec
 
             f.recording = self.recordings_list[f.frame.recordingid]
 
             self.add_metadata_from_remote_db(f, {"file", "path"})
 
             return f
         else:
             raise StopIteration
 
     def add_metadata_from_remote_db(self, f, keys):
-        iie_query = "select * from frames,image_index_entries where image_index_entries.frame_id = " + \
-            str(f.frame.id) + " and frames.recordingid = " + \
-            str(f.recording.id)
+        iie_query = (
+            "select * from frames,image_index_entries where image_index_entries.frame_id = "
+            + str(f.frame.id)
+            + " and frames.recordingid = "
+            + str(f.recording.id)
+        )
 
         __cursor__ = self.connection.cursor()
         __cursor__.execute(iie_query)
 
         values = __cursor__.fetchone()
         field_names = [field[0] for field in __cursor__.description]
         row = dict(zip(field_names, values))
 
         for k in keys:
             if k in row:
-                f.metadata["image_index_entries."+k] = row[k]
+                f.metadata["image_index_entries." + k] = row[k]
```

### Comparing `horus-media-client-0.9.4/tests/test_db.py` & `horus-media-client-0.9.5/tests/test_db.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-
 # Copyright(C) 2019, 2020 Horus View and Explore B.V.
 
 import unittest
 import datetime
 
 import psycopg2
 
 from horus_db import Frames, Recordings, Frame, Recording, RecordingSetups
 from horus_db import Iterator
 
 
 def get_connection():
     return psycopg2.connect(
-        "dbname=HorusWebMoviePlayer user=postgres password=horusweb")
+        "dbname=HorusWebMoviePlayer user=postgres password=horusweb"
+    )
 
 
 class TestRecordings(unittest.TestCase):
-
     def test_get(self):
         connection = get_connection()
         recording_id = 5
         recordings = Recordings(connection)
         recording = Recording(recordings.get(recording_id))
         self.assertEqual(recording.id, 5)
         self.assertEqual(
-            recording.directory, "D:\\Recordings\\DemoData\\Rotterdam360\\Ladybug5plus\\Recording_18-12-2019_12-03-08")
-        self.assertEqual(recording.bounding_box,
-                         "BOX(4.461778927 51.892380339,4.497248851 51.930770724)")
+            recording.directory,
+            "D:\\Recordings\\DemoData\\Rotterdam360\\Ladybug5plus\\Recording_18-12-2019_12-03-08",
+        )
+        self.assertEqual(
+            recording.bounding_box,
+            "BOX(4.461778927 51.892380339,4.497248851 51.930770724)",
+        )
         self.assertEqual(recording.file_format, 1)
 
         self.assertEqual(recording.setup, None)
         recordings.get_setup(recording)
         setup = recording.setup
         self.assertEqual(setup.camera_height, 2.49)
         self.assertEqual(setup.lever_arm_x, 0)
@@ -41,35 +44,43 @@
         self.assertEqual(lever_arm.x, 0)
         self.assertEqual(lever_arm.y, 0)
         self.assertEqual(lever_arm.z, 0)
 
     def test_get_with_directory(self):
         connection = get_connection()
         recordings = Recordings(connection)
-        results = list(Recording.query(
-            recordings, directory_like="Rotterdam360", order_by="id"))
+        results = list(
+            Recording.query(recordings, directory_like="Rotterdam360", order_by="id")
+        )
 
         self.assertEqual(len(results), 2)
         self.assertEqual(results[0].id, 4)
         self.assertEqual(
-            results[0].directory, "D:\\Recordings\\DemoData\\Rotterdam360\\GoProMax\\Recording2019-12-18_12-53-06")
+            results[0].directory,
+            "D:\\Recordings\\DemoData\\Rotterdam360\\GoProMax\\Recording2019-12-18_12-53-06",
+        )
 
         self.assertEqual(results[1].id, 5)
         self.assertEqual(
-            results[1].directory, "D:\\Recordings\\DemoData\\Rotterdam360\\Ladybug5plus\\Recording_18-12-2019_12-03-08")
+            results[1].directory,
+            "D:\\Recordings\\DemoData\\Rotterdam360\\Ladybug5plus\\Recording_18-12-2019_12-03-08",
+        )
 
     def test_get_with_directory_single(self):
         connection = get_connection()
         recordings = Recordings(connection)
-        recording = next(Recording.query(
-            recordings, directory_like="Rotterdam360\\\\Ladybug5plus"))
+        recording = next(
+            Recording.query(recordings, directory_like="Rotterdam360\\\\Ladybug5plus")
+        )
 
         self.assertEqual(recording.id, 5)
         self.assertEqual(
-            recording.directory, "D:\\Recordings\\DemoData\\Rotterdam360\\Ladybug5plus\\Recording_18-12-2019_12-03-08")
+            recording.directory,
+            "D:\\Recordings\\DemoData\\Rotterdam360\\Ladybug5plus\\Recording_18-12-2019_12-03-08",
+        )
 
     def test_query(self):
         connection = get_connection()
         recordings = Recordings(connection)
         cursor = recordings.all()
         self.assertIsNotNone(cursor)
 
@@ -99,25 +110,23 @@
             self.assertEqual(len(result), description_len)
 
         self.assertGreater(cursor.rowcount, 3)
         self.assertEqual(iterator_count, cursor.rowcount)
 
 
 class TestFrames(unittest.TestCase):
-
     def test_query(self):
         connection = get_connection()
 
         recordings = (973, 972)
         point = (5.7058276, 50.8510157)  # EPSG:4326 (lon, lat)
         distance = 2  # in meters
 
         frames = Frames(connection)
-        cursor = frames.query(within=(point, distance),
-                              recordingid=recordings, limit=1)
+        cursor = frames.query(within=(point, distance), recordingid=recordings, limit=1)
         self.assertIsNotNone(cursor)
 
         frame = Frame(cursor)
 
         timestamp = datetime.datetime(2016, 5, 11, 8, 6, 24, 90000)
         self.assertEqual(frame.id, 727692)
         self.assertEqual(frame.recordingid, 972)
@@ -142,35 +151,36 @@
         point = (5.7058276, 50.8510157)  # EPSG:4326 (lon, lat)
         distance_max = 2  # in meters
         distance_min = 5  # in meters
 
         frames = Frames(connection)
         cursor = frames.query(
             within=(point, distance_max),
-            distance=(point,  "> %s", distance_min),
+            distance=(point, "> %s", distance_min),
             recordingid=recordings,
-            limit=1
+            limit=1,
         )
         self.assertIsNotNone(cursor)
 
     def test_query_recordingid(self):
         connection = get_connection()
 
         recordings = 972
         point = (5.7058276, 50.8510157)  # EPSG:4326 (lon, lat)
         distance = 2  # in meters
 
         frames = Frames(connection)
-        cursor = frames.query(within=(point, distance),
-                              recordingid=recordings, limit=3, offset=1)
+        cursor = frames.query(
+            within=(point, distance), recordingid=recordings, limit=3, offset=1
+        )
         self.assertIsNotNone(cursor)
 
         frame = Frame(cursor)
 
         timestamp = datetime.datetime(2016, 5, 11, 8, 6, 24, 90000)
         self.assertEqual(frame.id, 727953)
         self.assertEqual(frame.recordingid, 972)
         self.assertEqual(frame.uuid, "9089f29d-9437-4a3c-bd88-ed9e27445289")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `horus-media-client-0.9.4/tests/test_geopandas.py` & `horus-media-client-0.9.5/tests/test_geopandas.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,32 +11,47 @@
 # Create output directory
 output_dir = "./tests/data/"
 try:
     os.mkdir(output_dir)
 except OSError:
     pass
 
+
 class TestTriangulation(unittest.TestCase):
     def test_triangulation_examples(self):
         # import horus_media_examples.spherical_camera_single_measurement
         try:
             import horus_media_examples.single_measurement_clustering
         except Exception as e:
-            self.fail("{} failed ({}: {})".format("horus_media_examples.single_measurement_clustering", type(e), e))
+            self.fail(
+                "{} failed ({}: {})".format(
+                    "horus_media_examples.single_measurement_clustering", type(e), e
+                )
+            )
         try:
             import horus_media_examples.triangulate_spherical_camera_single_measurement_clusters
         except Exception as e:
-            self.fail("{} failed ({}: {})".format("horus_media_examples.triangulate_spherical_camera_single_measurement_clusters", type(e), e))
+            self.fail(
+                "{} failed ({}: {})".format(
+                    "horus_media_examples.triangulate_spherical_camera_single_measurement_clusters",
+                    type(e),
+                    e,
+                )
+            )
         try:
             import horus_media_examples.clustering_analytics
         except Exception as e:
-            self.fail("{} failed ({}: {})".format("horus_media_examples.clustering_analytics", type(e), e))
+            self.fail(
+                "{} failed ({}: {})".format(
+                    "horus_media_examples.clustering_analytics", type(e), e
+                )
+            )
 
-class TestHorusGeoDataFrame(unittest.TestCase):
 
+class TestHorusGeoDataFrame(unittest.TestCase):
     def __init__(self, *args, **kwargs):
         super(TestHorusGeoDataFrame, self).__init__(*args, **kwargs)
         # Obtain schema
         self.schema = SchemaProvider()
         self.database = HorusGeoDataFrame(self.schema.single_measurement())
 
     def test_create_record(self):
@@ -44,16 +59,16 @@
         record = self.database.new_frame(geom)
 
         # update geometry
         record["geometry"] = geom
         # Record
         record["rec_id"] = 1
         record["frame_idx"] = 2
-        record['azimuth'] = 3
-        record['usr_id'] = 4
+        record["azimuth"] = 3
+        record["usr_id"] = 4
         #
         record["cam_fov"] = 90.0
         record["cam_yaw"] = 20.0
         record["cam_pitch"] = -30
         record["cam_width"] = 800
         record["cam_height"] = 800
         record["cam_lat"] = 51.912414163999998
@@ -79,15 +94,19 @@
         record["surf_px_x"] = 15
         record["surf_px_y"] = 15
         record["surf_yaw"] = 15.6
         record["surf_pitch"] = 15.6
 
         self.database.add_frame(record)
 
-        self.database.write_shapefile(os.path.join(
-            output_dir, "single_measurement.shp"))
-
-        self.database.write_geojson(os.path.join(
-            output_dir, "single_measurement.geojson"))
-
-        self.database.write_geopackage(os.path.join(
-            output_dir, "single_measurement.gpkg"), layer='singlemeasurement')
+        self.database.write_shapefile(
+            os.path.join(output_dir, "single_measurement.shp")
+        )
+
+        self.database.write_geojson(
+            os.path.join(output_dir, "single_measurement.geojson")
+        )
+
+        self.database.write_geopackage(
+            os.path.join(output_dir, "single_measurement.gpkg"),
+            layer="singlemeasurement",
+        )
```

### Comparing `horus-media-client-0.9.4/tests/test_gis.py` & `horus-media-client-0.9.5/tests/test_gis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,65 +1,64 @@
-
 # Copyright(C) 2019, 2020 Horus View and Explore B.V.
 
 import unittest
 
 import numpy
 from horus_gis import EnuModel, CameraModel, SchemaProvider
 
 
 class TestEnuModel(unittest.TestCase):
-
     def __init__(self, *args, **kwargs):
         super(TestEnuModel, self).__init__(*args, **kwargs)
 
         # lon, lat, altitude # origin of ENU, (altitude is height above ellipsoid)
         self.camera_location = numpy.array((48.0, 5.0, 10.0))
         self.look_at_target_location = numpy.array((48.001, 5.01, 10.0))
-        self.look_at_vector_result = (110.897, 1105.829, - 0.097)
+        self.look_at_vector_result = (110.897, 1105.829, -0.097)
 
     def test_to_enu_reference(self):
         camera_enu_reference = EnuModel(self.camera_location)
         origin = camera_enu_reference.to_geodetic((0, 0, 0))
         self.assertTrue(numpy.allclose(origin, self.camera_location))
 
     def test_to_enu(self):
         camera_enu_reference = EnuModel(self.camera_location)
-        look_at_vector = camera_enu_reference.to_enu(
-            self.look_at_target_location)
-
-        self.assertTrue(numpy.allclose(
-            numpy.around(look_at_vector, 3),
-            self.look_at_vector_result), "look_at_target_location to ENU")
+        look_at_vector = camera_enu_reference.to_enu(self.look_at_target_location)
 
-        self.assertEqual(numpy.around(numpy.linalg.norm(
-            look_at_vector), 3), 1111.376, "look_at_vector_result magnitude")
+        self.assertTrue(
+            numpy.allclose(numpy.around(look_at_vector, 3), self.look_at_vector_result),
+            "look_at_target_location to ENU",
+        )
+
+        self.assertEqual(
+            numpy.around(numpy.linalg.norm(look_at_vector), 3),
+            1111.376,
+            "look_at_vector_result magnitude",
+        )
 
         heading = camera_enu_reference.get_heading(look_at_vector)
         self.assertEqual(numpy.around(heading, 3), -5.727, "Heading")
 
 
 class TestCameraModel(unittest.TestCase):
-
     def test_look_at(self):
         camera_location = (4.486625622, 51.895778197, 49.305309)
         camera_heading = 65.734584
         look_at_location = (4.486649, 51.89575, 47.28)
 
         camera_model = CameraModel(camera_location, camera_heading)
         look_at_angle = camera_model.look_at_angle(look_at_location)
 
         diff = look_at_angle - 87.49439415551622
 
         self.assertTrue(diff < 0.001, "look_at_angle")
 
 
 class TestSchemaProvider(unittest.TestCase):
-
     def single_measurement_schema(self):
         sp = SchemaProvider()
         schema = sp.single_measurement()
         self.assertEqual(23, len(schema))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `horus-media-client-0.9.4/tests/test_media.py` & `horus-media-client-0.9.5/tests/test_media.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,30 @@
-
 # Copyright(C) 2019, 2020 Horus View and Explore B.V.
 
 import unittest
 import os
 
-from horus_media import Client, ImageRequestBuilder, ImageProvider, Grid, Scales, Rect, Mode
+from horus_media import (
+    Client,
+    ImageRequestBuilder,
+    ImageProvider,
+    Grid,
+    Scales,
+    Rect,
+    Mode,
+)
 
 path = "./tests/data/"
 try:
     os.mkdir(path)
 except OSError:
     pass
 
 
 class TestScales(unittest.TestCase):
-
     def test_to_size(self):
         self.assertEqual(Scales.Px_256.size, 256)
         self.assertEqual(Scales.Px_512.size, 512)
         self.assertEqual(Scales.Px_1024.size, 1024)
         self.assertEqual(Scales.Px_2048.size, 2048)
         self.assertEqual(Scales.Px_4096.size, 4096)
 
@@ -26,15 +32,14 @@
         self.assertEqual(Scales.Px_256, Scales.from_size(100))
         self.assertEqual(Scales.Px_256, Scales.from_size(256))
         self.assertEqual(Scales.Px_1024, Scales.from_size(570))
         self.assertEqual(Scales.Px_2048, Scales.from_size(2000))
 
 
 class TestGrid(unittest.TestCase):
-
     def __init__(self, *args, **kwargs):
         super(TestGrid, self).__init__(*args, **kwargs)
 
     def test_default_constructor(self):
         grid = Grid()
         count = 0
         result = set(range(32))
@@ -44,124 +49,142 @@
         self.assertEqual(count, 32)
         self.assertEqual(len(result), 0)
 
     def test_filter(self):
         grid = Grid()
         sections = grid.filter(h_min=-44, h_max=44, w_min=-170, w_max=-1)
         count = 0
-        result = {
-            8, 9, 10, 11,
-            16, 17, 18, 19
-        }
+        result = {8, 9, 10, 11, 16, 17, 18, 19}
         for section in sections:
             count += 1
             result.remove(section.index)
 
         self.assertEqual(count, 8)
         self.assertEqual(len(result), 0)
 
     def test_filter_wrap_right(self):
         grid = Grid()
         sections = grid.filter(w_min=36, w_max=250)
         count = 0
         result = {
-            4, 5, 6, 7, 0, 1,
-            12, 13, 14, 15, 8, 9,
-            20, 21, 22, 23, 16, 17,
-            28, 29, 30, 31, 24, 25,
+            4,
+            5,
+            6,
+            7,
+            0,
+            1,
+            12,
+            13,
+            14,
+            15,
+            8,
+            9,
+            20,
+            21,
+            22,
+            23,
+            16,
+            17,
+            28,
+            29,
+            30,
+            31,
+            24,
+            25,
         }
         for section in sections:
             result.remove(section.index)
             count += 1
         self.assertEqual(count, 24)
         self.assertEqual(len(result), 0)
 
     def test_filter_wrap_left(self):
         grid = Grid()
         sections = grid.filter(h_min=-44, h_max=44, w_min=-200, w_max=-36)
-        result = {
-            15, 8, 9, 10, 11,
-            23, 16, 17, 18, 19
-        }
+        result = {15, 8, 9, 10, 11, 23, 16, 17, 18, 19}
         count = 0
         for section in sections:
             result.remove(section.index)
             count += 1
         self.assertEqual(count, 10)
         self.assertEqual(len(result), 0)
 
 
 class TestClient(unittest.TestCase):
-
     def __init__(self, *args, **kwargs):
         super(TestClient, self).__init__(*args, **kwargs)
 
         recording_id = 5
         frame_uuid = "1708a7fb-af45-41b2-a0c1-1b9962f58ac0"
         host_url = "http://pocms.horus.nu:5050/web/"
 
         self.grid = Grid()
         self.request_builder = ImageRequestBuilder(recording_id, frame_uuid)
         self.stitcher = ImageProvider()
         self.client = Client(host_url)
 
     def request_stitched_sections(self, sections, scale, path=None):
         requests = self.client.fetch_all(
-            self.request_builder.build(Mode.panoramic, scale, section) for section in sections)
+            self.request_builder.build(Mode.panoramic, scale, section)
+            for section in sections
+        )
 
         result = self.stitcher.combine(requests, scale.size, scale.size)
         if path:
-            with open(path, 'wb') as f:
+            with open(path, "wb") as f:
                 f.write(result.image.getvalue())
             result.image.close()
         return result
 
     def test_client_request_pano(self):
-        request = self.client.fetch(self.request_builder.build(Mode.panoramic, Scales.Px_1024))
-        with open('./tests/data/pano.jpg', "wb") as file:
+        request = self.client.fetch(
+            self.request_builder.build(Mode.panoramic, Scales.Px_1024)
+        )
+        with open("./tests/data/pano.jpg", "wb") as file:
             file.write(request.result())
 
     def test_client_request(self):
         sections = self.grid.filter(h_min=-44, h_max=44, w_min=-170, w_max=-1)
         self.request_stitched_sections(
-            sections, Scales.Px_1024, './tests/data/stitched.jpg')
+            sections, Scales.Px_1024, "./tests/data/stitched.jpg"
+        )
 
     def test_client_request_pano_stitched(self):
         result = self.request_stitched_sections(
-            self.grid, Scales.Px_1024, './tests/data/pano_stitched.jpg')
+            self.grid, Scales.Px_1024, "./tests/data/pano_stitched.jpg"
+        )
         self.assertEqual(result.to_pixel_coordinates((0, 0)).x, 0)
-        self.assertEqual(result.fov, Rect(
-            x=-180.0, y=-90.0, width=360.0, height=180.0))
-
+        self.assertEqual(result.fov, Rect(x=-180.0, y=-90.0, width=360.0, height=180.0))
 
     def test_client_request_single_section_stitched(self):
         result = self.request_stitched_sections(
-            (self.grid[3],), Scales.Px_1024, './tests/data/single_section_stitched.jpg')
+            (self.grid[3],), Scales.Px_1024, "./tests/data/single_section_stitched.jpg"
+        )
         self.assertEqual(result.to_pixel_coordinates((170.0, 0)).x, 796)
-        self.assertEqual(result.fov, Rect(
-            x=-45.0, y=45.0, width=45.0, height=45.0))
+        self.assertEqual(result.fov, Rect(x=-45.0, y=45.0, width=45.0, height=45.0))
 
     def test_client_request_left_wrapped(self):
         sections = self.grid.filter(h_min=-46, h_max=1, w_min=-270, w_max=-46)
         result = self.request_stitched_sections(
-            sections, Scales.Px_1024, './tests/data/stitched_lw.jpg')
+            sections, Scales.Px_1024, "./tests/data/stitched_lw.jpg"
+        )
         self.assertEqual(result.to_pixel_coordinates((0, 0)).x, 0)
 
     def test_client_request_right_wrapped(self):
         sections = self.grid.filter(h_min=0, w_min=70, w_max=246)
         result = self.request_stitched_sections(
-            sections, Scales.Px_1024, './tests/data/stitched_rw.jpg')
+            sections, Scales.Px_1024, "./tests/data/stitched_rw.jpg"
+        )
         self.assertEqual(result.to_pixel_coordinates((70.0, 0)).x, 1592)
-        self.assertEqual(result.fov, Rect(
-            x=-180.0, y=0.0, width=225.0, height=90.0))
+        self.assertEqual(result.fov, Rect(x=-180.0, y=0.0, width=225.0, height=90.0))
 
     def test_client_request_left_right_wrapped(self):
         sections = self.grid.filter(w_min=-240, w_max=246)
         result = self.request_stitched_sections(
-            sections, Scales.Px_1024, './tests/data/stitched_lrw.jpg')
+            sections, Scales.Px_1024, "./tests/data/stitched_lrw.jpg"
+        )
         self.assertEqual(result.to_pixel_coordinates((-240.0, 0)).x, 2730)
-        self.assertEqual(result.fov, Rect(
-            x=-180.0, y=-90.0, width=180.0, height=180.0))
+        self.assertEqual(result.fov, Rect(x=-180.0, y=-90.0, width=180.0, height=180.0))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

