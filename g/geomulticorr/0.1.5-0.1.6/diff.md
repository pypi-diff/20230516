# Comparing `tmp/geomulticorr-0.1.5.tar.gz` & `tmp/geomulticorr-0.1.6.tar.gz`

## Comparing `geomulticorr-0.1.5.tar` & `geomulticorr-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/src/geomulticorr/__init__.py
--rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/src/geomulticorr/geomorph.py
--rw-r--r--   0        0        0    15000 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/src/geomulticorr/pair.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/src/geomulticorr/pzone.py
--rw-r--r--   0        0        0    20383 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/src/geomulticorr/session.py
--rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/src/geomulticorr/spine.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/src/geomulticorr/thumb.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/src/geomulticorr/xzone.py
--rwxr-xr-x   0        0        0    12941 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/src/geomulticorr/resources/map_styles/vector-field_style_1.qml
--rw-r--r--   0        0        0 19431424 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/src/geomulticorr/resources/project_template/map_template-project.qgz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/tests/test_geomorph.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/tests/test_pair.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/tests/test_pzone.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/tests/test_session.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/tests/test_thumb.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/tests/test_xzone.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/LICENSE.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/README.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/src/geomulticorr/__init__.py
+-rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/src/geomulticorr/geomorph.py
+-rw-r--r--   0        0        0    15205 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/src/geomulticorr/pair.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/src/geomulticorr/pzone.py
+-rw-r--r--   0        0        0    20383 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/src/geomulticorr/session.py
+-rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/src/geomulticorr/spine.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/src/geomulticorr/thumb.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/src/geomulticorr/xzone.py
+-rwxr-xr-x   0        0        0    12941 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/src/geomulticorr/resources/map_styles/vector-field_style_1.qml
+-rw-r--r--   0        0        0 19431424 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/src/geomulticorr/resources/project_template/map_template-project.qgz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/tests/test_geomorph.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/tests/test_pair.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/tests/test_pzone.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/tests/test_session.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/tests/test_thumb.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/tests/test_xzone.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/LICENSE.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/README.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 geomulticorr-0.1.6/PKG-INFO
```

### Comparing `geomulticorr-0.1.5/src/geomulticorr/geomorph.py` & `geomulticorr-0.1.6/src/geomulticorr/geomorph.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.5/src/geomulticorr/pair.py` & `geomulticorr-0.1.6/src/geomulticorr/pair.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,33 +292,33 @@
         output_pixel_size : space between each point. By default, it is the pixel size of the pair disparity map
         method  : algorithm to use to resample the data (is a output_pixel_size value is given)
         """
 
         # Get vector components - unit = pixels and referential = matrix (Y top is Y min)
         initial_dx = self.get_dispX_geoim()
         initial_dy = self.get_dispY_geoim()
-        initial_pixel_size = initial_dx.getPixelSize()[0]
+        initial_pixel_size_x, initial_pixel_size_y = initial_dx.getPixelSize()
 
         # Modify the original displacement rasters by resampling them with output resolution asked
         if output_pixel_size != None:
             dx_in_pixels = initial_dx.resize(output_pixel_size, method=method)
             dy_in_pixels = initial_dy.resize(output_pixel_size, method=method)
 
         # Elsewhere, we will work on a copy of the original displacement rasters
         else:
             dx_in_pixels = initial_dx.copy()
             dy_in_pixels = initial_dy.copy()
-            output_pixel_size = initial_pixel_size
+            output_pixel_size = initial_pixel_size_x
 
         # Get metadata
         _, nRows, nCols = dx_in_pixels.getShape()
 
         # Convert displacements in meters
-        dx_in_meters = dx_in_pixels * initial_pixel_size
-        dy_in_meters = dy_in_pixels * initial_pixel_size
+        dx_in_meters = dx_in_pixels * initial_pixel_size_x
+        dy_in_meters = dy_in_pixels * initial_pixel_size_y
 
         # Switch from matrixian to geographic spatial referential
         dy_in_meters_switched = dy_in_meters * -1
 
         # Compute vector norm (magnitude) in meters
         d_in_meters = (dx_in_meters ** 2 + dy_in_meters_switched ** 2) **0.5
 
@@ -345,17 +345,19 @@
             dy_in_meters,
             d_in_meters,
             dx_in_meters_per_year,
             dy_in_meters_per_year,
             d_in_meters_per_year,
             direction
         ])
-        
-        vectors = rt.vectorize(to_vectorize).set_crs(epsg=2154)
 
+        # Use the vectorize raster_tools function to make a vector point on each pixel
+        # with an attribute column with the pixel value for each band (here we got 9 band)
+        vectors = rt.vectorize(to_vectorize).set_crs(epsg=2154)
+        
         """
         changer le nom des colonnes attributaires
         """
 
         # Write vector layer in geopackage
         if write == True:
             current_vector_layer_name = f"{output_pixel_size}_{self.pa_key}"
```

### Comparing `geomulticorr-0.1.5/src/geomulticorr/pzone.py` & `geomulticorr-0.1.6/src/geomulticorr/pzone.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.5/src/geomulticorr/session.py` & `geomulticorr-0.1.6/src/geomulticorr/session.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.5/src/geomulticorr/spine.py` & `geomulticorr-0.1.6/src/geomulticorr/spine.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.5/src/geomulticorr/thumb.py` & `geomulticorr-0.1.6/src/geomulticorr/thumb.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.5/src/geomulticorr/xzone.py` & `geomulticorr-0.1.6/src/geomulticorr/xzone.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.5/src/geomulticorr/resources/map_styles/vector-field_style_1.qml` & `geomulticorr-0.1.6/src/geomulticorr/resources/map_styles/vector-field_style_1.qml`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.5/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg` & `geomulticorr-0.1.6/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.5/src/geomulticorr/resources/project_template/map_template-project.qgz` & `geomulticorr-0.1.6/src/geomulticorr/resources/project_template/map_template-project.qgz`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.5/tests/test_geomorph.py` & `geomulticorr-0.1.6/tests/test_geomorph.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.5/tests/test_pair.py` & `geomulticorr-0.1.6/tests/test_pair.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.5/tests/test_pzone.py` & `geomulticorr-0.1.6/tests/test_pzone.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.5/tests/test_session.py` & `geomulticorr-0.1.6/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.5/tests/test_thumb.py` & `geomulticorr-0.1.6/tests/test_thumb.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.5/LICENSE.md` & `geomulticorr-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.5/pyproject.toml` & `geomulticorr-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "geomulticorr"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Thibaut Duvanel", email="thibaut.duvanel@univ-smb.fr" },
 ]
 description = "A python lib to study earth-surface displacements from optical images with Ames Stereo Pipeline"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `geomulticorr-0.1.5/PKG-INFO` & `geomulticorr-0.1.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomulticorr
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python lib to study earth-surface displacements from optical images with Ames Stereo Pipeline
 Author-email: Thibaut Duvanel <thibaut.duvanel@univ-smb.fr>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

