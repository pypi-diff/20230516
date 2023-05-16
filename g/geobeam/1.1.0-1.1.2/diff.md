# Comparing `tmp/geobeam-1.1.0.tar.gz` & `tmp/geobeam-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/geobeam-1.1.0.tar", last modified: Mon Mar 27 20:49:50 2023, max compression
+gzip compressed data, was "dist/geobeam-1.1.2.tar", last modified: Tue May 16 14:25:48 2023, max compression
```

## Comparing `geobeam-1.1.0.tar` & `geobeam-1.1.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-x---   0 traviswebb (621083) primarygroup (89939)        0 2023-03-27 20:49:50.331745 geobeam-1.1.0/
--rw-r-----   0 traviswebb (621083) primarygroup (89939)    11122 2023-03-27 20:49:50.327745 geobeam-1.1.0/PKG-INFO
--rw-r-----   0 traviswebb (621083) primarygroup (89939)     8779 2023-03-27 20:38:43.000000 geobeam-1.1.0/README.md
-drwxr-x---   0 traviswebb (621083) primarygroup (89939)        0 2023-03-27 20:49:50.327745 geobeam-1.1.0/geobeam/
--rw-r-----   0 traviswebb (621083) primarygroup (89939)      631 2023-03-24 21:23:39.000000 geobeam-1.1.0/geobeam/__init__.py
-drwxr-x---   0 traviswebb (621083) primarygroup (89939)        0 2023-03-27 20:49:50.327745 geobeam-1.1.0/geobeam/examples/
--rw-r-----   0 traviswebb (621083) primarygroup (89939)      721 2021-01-28 06:06:20.000000 geobeam-1.1.0/geobeam/examples/__init__.py
--rw-r-----   0 traviswebb (621083) primarygroup (89939)     2660 2022-11-18 16:32:32.000000 geobeam-1.1.0/geobeam/examples/crop_geotiff.py
--rw-r-----   0 traviswebb (621083) primarygroup (89939)     2657 2021-02-06 09:18:33.000000 geobeam-1.1.0/geobeam/examples/geodatabase_frd.py
--rw-r-----   0 traviswebb (621083) primarygroup (89939)     2143 2022-04-20 14:15:07.000000 geobeam-1.1.0/geobeam/examples/geojson_stormwater.py
--rw-r-----   0 traviswebb (621083) primarygroup (89939)     2707 2022-11-29 01:32:47.000000 geobeam-1.1.0/geobeam/examples/geotiff_dem.py
--rw-r-----   0 traviswebb (621083) primarygroup (89939)     2241 2022-11-21 23:20:25.000000 geobeam-1.1.0/geobeam/examples/geotiff_soilgrid.py
--rw-r-----   0 traviswebb (621083) primarygroup (89939)     2057 2022-11-17 16:41:17.000000 geobeam-1.1.0/geobeam/examples/rasterblocksource.py
--rw-r-----   0 traviswebb (621083) primarygroup (89939)     2364 2022-03-31 21:55:52.000000 geobeam-1.1.0/geobeam/examples/shapefile_nfhl.py
--rw-r-----   0 traviswebb (621083) primarygroup (89939)     3114 2022-10-01 20:58:28.000000 geobeam-1.1.0/geobeam/examples/shapefile_parcel.py
--rw-r-----   0 traviswebb (621083) primarygroup (89939)     2302 2022-04-20 14:15:07.000000 geobeam-1.1.0/geobeam/examples/streaming_pubsub.py
--rw-r-----   0 traviswebb (621083) primarygroup (89939)     7054 2023-03-24 21:23:39.000000 geobeam-1.1.0/geobeam/fn.py
--rw-r-----   0 traviswebb (621083) primarygroup (89939)    23547 2023-03-24 21:23:39.000000 geobeam-1.1.0/geobeam/io.py
--rw-r-----   0 traviswebb (621083) primarygroup (89939)     5928 2023-03-27 20:39:08.000000 geobeam-1.1.0/geobeam/util.py
-drwxr-x---   0 traviswebb (621083) primarygroup (89939)        0 2023-03-27 20:49:50.327745 geobeam-1.1.0/geobeam.egg-info/
--rw-r-----   0 traviswebb (621083) primarygroup (89939)    11122 2023-03-27 20:49:48.000000 geobeam-1.1.0/geobeam.egg-info/PKG-INFO
--rw-r-----   0 traviswebb (621083) primarygroup (89939)      589 2023-03-27 20:49:48.000000 geobeam-1.1.0/geobeam.egg-info/SOURCES.txt
--rw-r-----   0 traviswebb (621083) primarygroup (89939)        1 2023-03-27 20:49:48.000000 geobeam-1.1.0/geobeam.egg-info/dependency_links.txt
--rw-r-----   0 traviswebb (621083) primarygroup (89939)      115 2023-03-27 20:49:48.000000 geobeam-1.1.0/geobeam.egg-info/requires.txt
--rw-r-----   0 traviswebb (621083) primarygroup (89939)        8 2023-03-27 20:49:48.000000 geobeam-1.1.0/geobeam.egg-info/top_level.txt
--rw-r-----   0 traviswebb (621083) primarygroup (89939)       38 2023-03-27 20:49:50.331745 geobeam-1.1.0/setup.cfg
--rw-r-----   0 traviswebb (621083) primarygroup (89939)     1858 2023-03-27 20:39:01.000000 geobeam-1.1.0/setup.py
+drwxr-x---   0 traviswebb (621083) primarygroup (89939)        0 2023-05-16 14:25:48.775629 geobeam-1.1.2/
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)    11122 2023-05-16 14:25:48.775629 geobeam-1.1.2/PKG-INFO
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)     8779 2023-03-27 20:38:43.000000 geobeam-1.1.2/README.md
+drwxr-x---   0 traviswebb (621083) primarygroup (89939)        0 2023-05-16 14:25:48.519609 geobeam-1.1.2/geobeam/
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)      631 2023-05-16 14:24:58.000000 geobeam-1.1.2/geobeam/__init__.py
+drwxr-x---   0 traviswebb (621083) primarygroup (89939)        0 2023-05-16 14:25:48.751627 geobeam-1.1.2/geobeam/examples/
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)      721 2021-01-28 06:06:20.000000 geobeam-1.1.2/geobeam/examples/__init__.py
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)     3241 2023-05-16 14:24:28.000000 geobeam-1.1.2/geobeam/examples/bigquery_reproject.py
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)     2660 2022-11-18 16:32:32.000000 geobeam-1.1.2/geobeam/examples/crop_geotiff.py
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)     2657 2021-02-06 09:18:33.000000 geobeam-1.1.2/geobeam/examples/geodatabase_frd.py
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)     2143 2022-04-20 14:15:07.000000 geobeam-1.1.2/geobeam/examples/geojson_stormwater.py
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)     2707 2022-11-29 01:32:47.000000 geobeam-1.1.2/geobeam/examples/geotiff_dem.py
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)     2241 2022-11-21 23:20:25.000000 geobeam-1.1.2/geobeam/examples/geotiff_soilgrid.py
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)     2057 2022-11-17 16:41:17.000000 geobeam-1.1.2/geobeam/examples/rasterblocksource.py
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)     2364 2022-03-31 21:55:52.000000 geobeam-1.1.2/geobeam/examples/shapefile_nfhl.py
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)     3114 2022-10-01 20:58:28.000000 geobeam-1.1.2/geobeam/examples/shapefile_parcel.py
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)     2302 2022-04-20 14:15:07.000000 geobeam-1.1.2/geobeam/examples/streaming_pubsub.py
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)     7267 2023-05-15 19:13:36.000000 geobeam-1.1.2/geobeam/fn.py
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)    22815 2023-05-15 19:13:36.000000 geobeam-1.1.2/geobeam/io.py
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)     5928 2023-03-27 20:39:08.000000 geobeam-1.1.2/geobeam/util.py
+drwxr-x---   0 traviswebb (621083) primarygroup (89939)        0 2023-05-16 14:25:48.543610 geobeam-1.1.2/geobeam.egg-info/
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)    11122 2023-05-16 14:25:46.000000 geobeam-1.1.2/geobeam.egg-info/PKG-INFO
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)      628 2023-05-16 14:25:46.000000 geobeam-1.1.2/geobeam.egg-info/SOURCES.txt
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)        1 2023-05-16 14:25:46.000000 geobeam-1.1.2/geobeam.egg-info/dependency_links.txt
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)      114 2023-05-16 14:25:46.000000 geobeam-1.1.2/geobeam.egg-info/requires.txt
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)        8 2023-05-16 14:25:46.000000 geobeam-1.1.2/geobeam.egg-info/top_level.txt
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)       38 2023-05-16 14:25:48.775629 geobeam-1.1.2/setup.cfg
+-rw-r-----   0 traviswebb (621083) primarygroup (89939)     1857 2023-05-16 14:24:28.000000 geobeam-1.1.2/setup.py
```

### Comparing `geobeam-1.1.0/PKG-INFO` & `geobeam-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geobeam
-Version: 1.1.0
+Version: 1.1.2
 Summary: geobeam adds GIS capabilities to your Apache Beam pipelines
 Home-page: UNKNOWN
 Author: Travis Webb
 Author-email: traviswebb@google.com
 License: UNKNOWN
 Description: geobeam adds GIS capabilities to your Apache Beam pipelines.
```

### Comparing `geobeam-1.1.0/README.md` & `geobeam-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `geobeam-1.1.0/geobeam/__init__.py` & `geobeam-1.1.2/geobeam/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 geobeam root namespace.
 """
 
-__version__ = '1.1.0'
+__version__ = '1.1.2'
```

### Comparing `geobeam-1.1.0/geobeam/examples/__init__.py` & `geobeam-1.1.2/geobeam/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `geobeam-1.1.0/geobeam/examples/crop_geotiff.py` & `geobeam-1.1.2/geobeam/examples/crop_geotiff.py`

 * *Files identical despite different names*

### Comparing `geobeam-1.1.0/geobeam/examples/geodatabase_frd.py` & `geobeam-1.1.2/geobeam/examples/geodatabase_frd.py`

 * *Files identical despite different names*

### Comparing `geobeam-1.1.0/geobeam/examples/geojson_stormwater.py` & `geobeam-1.1.2/geobeam/examples/geojson_stormwater.py`

 * *Files identical despite different names*

### Comparing `geobeam-1.1.0/geobeam/examples/geotiff_dem.py` & `geobeam-1.1.2/geobeam/examples/geotiff_dem.py`

 * *Files identical despite different names*

### Comparing `geobeam-1.1.0/geobeam/examples/geotiff_soilgrid.py` & `geobeam-1.1.2/geobeam/examples/geotiff_soilgrid.py`

 * *Files identical despite different names*

### Comparing `geobeam-1.1.0/geobeam/examples/rasterblocksource.py` & `geobeam-1.1.2/geobeam/examples/rasterblocksource.py`

 * *Files identical despite different names*

### Comparing `geobeam-1.1.0/geobeam/examples/shapefile_nfhl.py` & `geobeam-1.1.2/geobeam/examples/shapefile_nfhl.py`

 * *Files identical despite different names*

### Comparing `geobeam-1.1.0/geobeam/examples/shapefile_parcel.py` & `geobeam-1.1.2/geobeam/examples/shapefile_parcel.py`

 * *Files identical despite different names*

### Comparing `geobeam-1.1.0/geobeam/examples/streaming_pubsub.py` & `geobeam-1.1.2/geobeam/examples/streaming_pubsub.py`

 * *Files identical despite different names*

### Comparing `geobeam-1.1.0/geobeam/fn.py` & `geobeam-1.1.2/geobeam/fn.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """
 Beam functions, transforms, and filters that can be used to process
 geometries in your pipeline
 """
 
 import apache_beam as beam
 
+
 def make_valid(element, drop_z=True):
     """
     Attempt to make a geometry valid. Returns `None` if the geometry cannot
     be made valid.
 
     Example:
     .. code-block:: python
@@ -30,18 +31,22 @@
         p | beam.Map(geobeam.fn.make_valid)
           | beam.Map(geobeam.fn.filter_invalid)
     """
     from shapely.geometry import shape
     from shapely import validation, wkb
 
     props, geom = element
-    shape_geom = shape(geom)
+    try:
+        shape_geom = shape(geom)
+    except Exception:
+        return None
 
     if not shape_geom.is_valid:
         shape_geom = validation.make_valid(shape_geom)
+        #shape_geom = force_2d(shape_geom)
 
     if drop_z and shape_geom.has_z:
         shape_geom = wkb.loads(wkb.dumps(shape_geom, output_dimension=2))
 
     if shape_geom is not None:
         return (props, shape_geom.__geo_interface__)
     else:
@@ -103,20 +108,20 @@
     shape_geom = shape(geom)
 
     if shape_geom.type not in ['Polygon', 'MultiPolygon']:
         return (props, geom)
 
     return (
         props,
-        shape_geom
+        (shape_geom
             .buffer(-d)
             .buffer(d * cf)
             .intersection(shape_geom)
             .simplify(d)
-            .__geo_interface__
+            .__geo_interface__)
     )
 
 
 def format_rasterblock_record(element, band_mapping=None):
     """
     Format the tuple received from a RasterBlockSource into a
     record that can be inserted into BigQuery or another database.
@@ -183,53 +188,59 @@
 
     return {
         band_column: cast(props),
         'geom': json.dumps(shape(geom).__geo_interface__)
     }
 
 
-def format_record(element):
+def format_record(element, geom_format='geojson'):
     """Format the tuple received from the geobeam file source into a record
     that can be inserted into BigQuery or another database.
 
     Example:
     .. code-block:: python
 
         # vector
         p | beam.Map(geobeam.fn.format_record)
     """
     import json
     from shapely.geometry import shape
 
     props, geom = element
 
+    if geom is None:
+        return {**props}
+
+    if geom_format == 'wkt':
+        geom_value = shape(geom).wkt
+    else:
+        geom_value = json.dumps(shape(geom).__geo_interface__)
+
     return {
         **props,
-        'geom': json.dumps(shape(geom).__geo_interface__)
+        'geom': geom_value
     }
 
 
 class DoBlockToPixelExterior(beam.DoFn):
     def process(self, element):
         """Decompose a raster block into individual pixels in order to store one
         pixel per row"""
 
-        #import json
-        #from shapely.geometry import shape
         from fiona.transform import transform_geom
 
         block_data, geom, xfrm, width, height, src_crs = element
 
         for j in range(0, height):
             for i in range(0, width):
                 exterior_ring = pixel_to_ring(i, j, xfrm)
 
                 geom_obj = {
                     'type': 'Polygon',
-                    'coordinates': [ exterior_ring ]
+                    'coordinates': [exterior_ring]
                 }
                 geom = transform_geom(src_crs, 'epsg:4326', geom_obj)
                 pixel_data = []
 
                 for bidx in range(0, len(block_data)):
                     pixel_data.append(block_data[bidx][j][i])
```

### Comparing `geobeam-1.1.0/geobeam/io.py` & `geobeam-1.1.2/geobeam/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,19 +69,14 @@
         from fiona.transform import transform_geom
         import json
 
         total_bytes = self.estimate_size()
 
         next_pos = range_tracker.start_position()
 
-        #def split_points_unclaimed(stop_pos):
-            #return 0 if stop_pos <= next_pos else iobase.RangeTracker.SPLIT_POINTS_UNKNOWN
-
-        #range_tracker.set_split_points_unclaimed_callback(split_points_unclaimed)
-
         with rasterio.open(file_name) as src:
             is_wgs84, src_crs = _GeoSourceUtils.validate_crs(src.crs, self.in_epsg, self.in_proj)
 
             block_windows = list([win for ji, win in src.block_windows()])
             num_windows = len(block_windows)
             window_bytes = math.floor(total_bytes / num_windows)
             i = 0
@@ -119,15 +114,15 @@
                     xfrm * (0, -win.height),
                     xfrm * (win.width, -win.height),
                     xfrm * (win.width, 0),
                     xfrm * (0, 0)
                 ]
                 geom_obj = {
                     'type': 'Polygon',
-                    'coordinates': [ exterior_ring ]
+                    'coordinates': [exterior_ring]
                 }
 
                 if self.skip_reproject:
                     geom = geom_obj
                 else:
                     geom = transform_geom(src_crs, 'epsg:4326', geom_obj)
 
@@ -150,14 +145,15 @@
         self.in_proj = in_proj
         self.bidx = bidx
         self.skip_reproject = skip_reproject
         self.return_block_transform = return_block_transform
 
         super(RasterBlockSource, self).__init__(file_pattern, splittable=False)
 
+
 class RasterPolygonSource(filebasedsource.FileBasedSource):
     """A Beam FileBasedSource for reading pixels grouped by value from raster
     files.
 
     The raster file is read in blocks and each block is polygonized. Each
     polygon is returned as a (`value`, `geom`) tuple, where `value` is the band
     value of the polygonized pixels, and `geom` is the Polygon geometry that
@@ -197,19 +193,14 @@
         from fiona.transform import transform_geom
         import json
 
         total_bytes = self.estimate_size()
 
         next_pos = range_tracker.start_position()
 
-        #def split_points_unclaimed(stop_pos):
-        #    return 0 if stop_pos <= next_pos else iobase.RangeTracker.SPLIT_POINTS_UNKNOWN
-
-        #range_tracker.set_split_points_unclaimed_callback(split_points_unclaimed)
-
         with rasterio.open(file_name) as src:
             is_wgs84, src_crs = _GeoSourceUtils.validate_crs(src.crs, self.in_epsg, self.in_proj)
 
             block_windows = list([win for ji, win in src.block_windows()])
             num_windows = len(block_windows)
             window_bytes = math.floor(total_bytes / num_windows)
             i = 0
@@ -284,30 +275,24 @@
         from fiona import BytesCollection
         from fiona.transform import transform_geom
         import json
 
         total_bytes = self.estimate_size()
         next_pos = range_tracker.start_position()
 
-        def split_points_unclaimed(stop_pos):
-            return 0 if stop_pos <= next_pos else iobase.RangeTracker.SPLIT_POINTS_UNKNOWN
-
-        range_tracker.set_split_points_unclaimed_callback(split_points_unclaimed)
-
         with self.open_file(file_name) as f:
             if self.layer_name:
                 collection = BytesCollection(f.read(), layer=self.layer_name)
             else:
                 collection = BytesCollection(f.read())
 
             is_wgs84, src_crs = _GeoSourceUtils.validate_crs(collection.crs, self.in_epsg, self.in_proj)
 
             num_features = len(collection)
             feature_bytes = math.floor(total_bytes / num_features)
-            i = 0
 
             logging.info(json.dumps({
                 'msg': 'read_records',
                 'next_pos': next_pos,
                 'file_name': file_name,
                 'profile': collection.profile,
                 'num_features': num_features,
@@ -326,23 +311,24 @@
                 if not self.skip_reproject:
                     geom = transform_geom(src_crs, 'epsg:4326', geom)
 
                 yield (props, geom)
 
                 next_pos = next_pos + feature_bytes
 
+
     def __init__(self, file_pattern, layer_name=None, skip_reproject=False,
-                 in_epsg=None, in_proj=None,**kwargs):
+                 in_epsg=None, in_proj=None, **kwargs):
 
         self.layer_name = layer_name
         self.skip_reproject = skip_reproject
         self.in_epsg = in_epsg
         self.in_proj = in_proj
 
-        super(ShapefileSource, self).__init__(file_pattern)
+        super(ShapefileSource, self).__init__(file_pattern, splittable=False)
 
 
 class GeodatabaseSource(filebasedsource.FileBasedSource):
     """A Beam FileBasedSource for reading geodatabases.
 
     The given file(s) should be a zip archive containing .gdb geodatabase
     directory.
@@ -373,19 +359,14 @@
         import json
 
         fiona_path = 'zip+{}/{}'.format(file_name, self.gdb_name)
 
         total_bytes = self.estimate_size()
         next_pos = range_tracker.start_position()
 
-        def split_points_unclaimed(stop_pos):
-            return 0 if stop_pos <= next_pos else iobase.RangeTracker.SPLIT_POINTS_UNKNOWN
-
-        range_tracker.set_split_points_unclaimed_callback(split_points_unclaimed)
-
         gdb_layers = fiona.listlayers(fiona_path)
         if self.layer_name and self.layer_name not in gdb_layers:
             logging.warning(json.dumps({
                 'msg': 'gdb_layer_not_found',
                 'layer_name': self.layer_name,
                 'gdb_name': self.gdb_name,
                 'gdb_layers': gdb_layers
@@ -401,15 +382,15 @@
             i = 0
 
             logging.info(json.dumps({
                 'msg': 'read_records',
                 'next_pos': next_pos,
                 'file_name': file_name,
                 'layer_name': self.layer_name,
-                'profile': collection.profile,
+                #'profile': collection.profile,
                 'num_features': num_features,
                 'total_bytes': total_bytes
             }))
 
             while range_tracker.try_claim(next_pos):
                 i = math.ceil(next_pos / feature_bytes)
                 if i >= num_features:
@@ -419,14 +400,17 @@
 
                 cur_feature = collection[i]
                 if cur_feature is None:
                     continue
 
                 geom = cur_feature['geometry']
 
+                if src_crs is None:
+                    yield (cur_feature['properties'], None)
+
                 if geom is None:
                     logging.info('Skipping null geometry: {}'.format(cur_feature))
                     continue
 
                 if not geom['coordinates']:
                     logging.info('Skipping empty geometry: {}'.format(cur_feature))
                     continue
@@ -442,15 +426,15 @@
 
         self.gdb_name = gdb_name
         self.layer_name = layer_name
         self.skip_reproject = skip_reproject
         self.in_epsg = in_epsg
         self.in_proj = in_proj
 
-        super(GeodatabaseSource, self).__init__(file_pattern)
+        super(GeodatabaseSource, self).__init__(file_pattern, splittable=False)
 
 
 class GeoJSONSource(filebasedsource.FileBasedSource):
     """A Beam FileBasedSource for reading GeoJSON Files.
 
     The given file(s) should be a .geojson file.
 
@@ -561,16 +545,17 @@
             return 0 if stop_pos <= next_pos else iobase.RangeTracker.SPLIT_POINTS_UNKNOWN
 
         range_tracker.set_split_points_unclaimed_callback(split_points_unclaimed)
 
         esri_dump = EsriDumper(file_name)
 
         geojson = {
-        "type": "FeatureCollection",
-        "features": list(esri_dump) }
+            "type": "FeatureCollection",
+            "features": list(esri_dump)
+        }
 
         collection = BytesCollection(json.dumps(geojson, indent=2).encode('utf-8'))
         is_wgs84, src_crs = _GeoSourceUtils.validate_crs(collection.crs, self.in_epsg, self.in_proj)
 
         num_features = len(collection)
         feature_bytes = math.floor(total_bytes / num_features)
         i = 0
@@ -642,11 +627,12 @@
             if bool(src_crs) is True:
                 logging.warning('manually specified CRS {} is being used instead of raster CRS {}.'.format(
                     in_crs, src_crs))
 
             return in_crs
 
         if bool(src_crs) is False:
-            logging.error('--in_epsg must be specified because raster CRS is empty.')
-            raise Exception()
+            logging.error('--in_epsg must be specified because CRS is empty.')
+            return False, None
+            #raise Exception()
 
         return is_wgs84, src_crs
```

### Comparing `geobeam-1.1.0/geobeam/util.py` & `geobeam-1.1.2/geobeam/util.py`

 * *Files identical despite different names*

### Comparing `geobeam-1.1.0/geobeam.egg-info/PKG-INFO` & `geobeam-1.1.2/geobeam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geobeam
-Version: 1.1.0
+Version: 1.1.2
 Summary: geobeam adds GIS capabilities to your Apache Beam pipelines
 Home-page: UNKNOWN
 Author: Travis Webb
 Author-email: traviswebb@google.com
 License: UNKNOWN
 Description: geobeam adds GIS capabilities to your Apache Beam pipelines.
```

### Comparing `geobeam-1.1.0/geobeam.egg-info/SOURCES.txt` & `geobeam-1.1.2/geobeam.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 geobeam/util.py
 geobeam.egg-info/PKG-INFO
 geobeam.egg-info/SOURCES.txt
 geobeam.egg-info/dependency_links.txt
 geobeam.egg-info/requires.txt
 geobeam.egg-info/top_level.txt
 geobeam/examples/__init__.py
+geobeam/examples/bigquery_reproject.py
 geobeam/examples/crop_geotiff.py
 geobeam/examples/geodatabase_frd.py
 geobeam/examples/geojson_stormwater.py
 geobeam/examples/geotiff_dem.py
 geobeam/examples/geotiff_soilgrid.py
 geobeam/examples/rasterblocksource.py
 geobeam/examples/shapefile_nfhl.py
```

### Comparing `geobeam-1.1.0/setup.py` & `geobeam-1.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 
 import setuptools
 from distutils.command.build import build as _build
 from distutils.core import setup
 import geobeam
 
 REQUIRED_PACKAGES = [
-    'apache_beam[gcp]==2.41.0',
-    'fiona==1.8.21',
-    'shapely==1.8.4',
-    'rasterio==1.3.2',
+    'apache_beam[gcp]==2.46.0',
+    'fiona==1.9.3',
+    'shapely==1.8.5',
+    'rasterio==1.3.6',
     'google-cloud-storage==2.5.0',
     'esridump==1.11.0'
 ]
 
 
 class build(_build):
     sub_commands = _build.sub_commands + [('GeobeamCommands', None)]
```

