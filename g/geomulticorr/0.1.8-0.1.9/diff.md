# Comparing `tmp/geomulticorr-0.1.8.tar.gz` & `tmp/geomulticorr-0.1.9.tar.gz`

## Comparing `geomulticorr-0.1.8.tar` & `geomulticorr-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/src/geomulticorr/__init__.py
--rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/src/geomulticorr/geomorph.py
--rw-r--r--   0        0        0    15559 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/src/geomulticorr/pair.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/src/geomulticorr/pzone.py
--rw-r--r--   0        0        0    20383 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/src/geomulticorr/session.py
--rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/src/geomulticorr/spine.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/src/geomulticorr/thumb.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/src/geomulticorr/xzone.py
--rwxr-xr-x   0        0        0    12941 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/src/geomulticorr/resources/map_styles/vector-field_style_1.qml
--rw-r--r--   0        0        0 19431424 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/src/geomulticorr/resources/project_template/map_template-project.qgz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/tests/test_geomorph.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/tests/test_pair.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/tests/test_pzone.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/tests/test_session.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/tests/test_thumb.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/tests/test_xzone.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/LICENSE.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/README.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 geomulticorr-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/src/geomulticorr/__init__.py
+-rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/src/geomulticorr/geomorph.py
+-rw-r--r--   0        0        0    15568 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/src/geomulticorr/pair.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/src/geomulticorr/pzone.py
+-rw-r--r--   0        0        0    20383 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/src/geomulticorr/session.py
+-rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/src/geomulticorr/spine.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/src/geomulticorr/thumb.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/src/geomulticorr/xzone.py
+-rwxr-xr-x   0        0        0    12941 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/src/geomulticorr/resources/map_styles/vector-field_style_1.qml
+-rw-r--r--   0        0        0 19431424 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/src/geomulticorr/resources/project_template/map_template-project.qgz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/tests/test_geomorph.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/tests/test_pair.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/tests/test_pzone.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/tests/test_session.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/tests/test_thumb.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/tests/test_xzone.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/LICENSE.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/README.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 geomulticorr-0.1.9/PKG-INFO
```

### Comparing `geomulticorr-0.1.8/src/geomulticorr/geomorph.py` & `geomulticorr-0.1.9/src/geomulticorr/geomorph.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.8/src/geomulticorr/pair.py` & `geomulticorr-0.1.9/src/geomulticorr/pair.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         # Write vector layer in geopackage
         if write == True:
             current_vector_layer_name = f"{output_pixel_size}_{self.pa_key}"
             vectors.to_file(self.pa_vect_path, layer=current_vector_layer_name)
 
             # Copy .qml file
-            template_style = Path(__file__).with_name('resources/map_styles/vector-field_style_1.qml')
+            template_style = Path(Path(__file__).parent, 'resources', 'map_styles', 'vector-field_style_1.qml')
             target_style = str(self.pa_vect_path)[:-5]
             cp_command = f"cp {template_style} {target_style}.qml"
             os.system(cp_command)
 
         return vectors
 
     def pa_full(self, corr_algorithm=2, corr_kernel_size=7, corr_xthreshold=10, vector_res=20, method='average'):
```

### Comparing `geomulticorr-0.1.8/src/geomulticorr/pzone.py` & `geomulticorr-0.1.9/src/geomulticorr/pzone.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.8/src/geomulticorr/session.py` & `geomulticorr-0.1.9/src/geomulticorr/session.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.8/src/geomulticorr/spine.py` & `geomulticorr-0.1.9/src/geomulticorr/spine.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.8/src/geomulticorr/thumb.py` & `geomulticorr-0.1.9/src/geomulticorr/thumb.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.8/src/geomulticorr/xzone.py` & `geomulticorr-0.1.9/src/geomulticorr/xzone.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.8/src/geomulticorr/resources/map_styles/vector-field_style_1.qml` & `geomulticorr-0.1.9/src/geomulticorr/resources/map_styles/vector-field_style_1.qml`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.8/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg` & `geomulticorr-0.1.9/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.8/src/geomulticorr/resources/project_template/map_template-project.qgz` & `geomulticorr-0.1.9/src/geomulticorr/resources/project_template/map_template-project.qgz`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.8/tests/test_geomorph.py` & `geomulticorr-0.1.9/tests/test_geomorph.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.8/tests/test_pair.py` & `geomulticorr-0.1.9/tests/test_pair.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.8/tests/test_pzone.py` & `geomulticorr-0.1.9/tests/test_pzone.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.8/tests/test_session.py` & `geomulticorr-0.1.9/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.8/tests/test_thumb.py` & `geomulticorr-0.1.9/tests/test_thumb.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.8/LICENSE.md` & `geomulticorr-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.8/pyproject.toml` & `geomulticorr-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "geomulticorr"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Thibaut Duvanel", email="thibaut.duvanel@univ-smb.fr" },
 ]
 description = "A python lib to study earth-surface displacements from optical images with Ames Stereo Pipeline"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `geomulticorr-0.1.8/PKG-INFO` & `geomulticorr-0.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomulticorr
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python lib to study earth-surface displacements from optical images with Ames Stereo Pipeline
 Author-email: Thibaut Duvanel <thibaut.duvanel@univ-smb.fr>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

