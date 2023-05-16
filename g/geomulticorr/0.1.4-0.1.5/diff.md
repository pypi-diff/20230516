# Comparing `tmp/geomulticorr-0.1.4.tar.gz` & `tmp/geomulticorr-0.1.5.tar.gz`

## Comparing `geomulticorr-0.1.4.tar` & `geomulticorr-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/src/geomulticorr/__init__.py
--rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/src/geomulticorr/geomorph.py
--rw-r--r--   0        0        0    14736 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/src/geomulticorr/pair.py
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/src/geomulticorr/pzone.py
--rw-r--r--   0        0        0    20383 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/src/geomulticorr/session.py
--rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/src/geomulticorr/spine.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/src/geomulticorr/thumb.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/src/geomulticorr/xzone.py
--rwxr-xr-x   0        0        0    12941 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/src/geomulticorr/resources/map_styles/vector-field_style_1.qml
--rw-r--r--   0        0        0 19431424 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/src/geomulticorr/resources/project_template/map_template-project.qgz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/tests/test_geomorph.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/tests/test_pair.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/tests/test_pzone.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/tests/test_session.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/tests/test_thumb.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/tests/test_xzone.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/LICENSE.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/README.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/src/geomulticorr/__init__.py
+-rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/src/geomulticorr/geomorph.py
+-rw-r--r--   0        0        0    15000 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/src/geomulticorr/pair.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/src/geomulticorr/pzone.py
+-rw-r--r--   0        0        0    20383 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/src/geomulticorr/session.py
+-rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/src/geomulticorr/spine.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/src/geomulticorr/thumb.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/src/geomulticorr/xzone.py
+-rwxr-xr-x   0        0        0    12941 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/src/geomulticorr/resources/map_styles/vector-field_style_1.qml
+-rw-r--r--   0        0        0 19431424 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/src/geomulticorr/resources/project_template/map_template-project.qgz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/tests/test_geomorph.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/tests/test_pair.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/tests/test_pzone.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/tests/test_session.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/tests/test_thumb.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/tests/test_xzone.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/LICENSE.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/README.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 geomulticorr-0.1.5/PKG-INFO
```

### Comparing `geomulticorr-0.1.4/src/geomulticorr/geomorph.py` & `geomulticorr-0.1.5/src/geomulticorr/geomorph.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.4/src/geomulticorr/pair.py` & `geomulticorr-0.1.5/src/geomulticorr/pair.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,29 +7,33 @@
 from telenvi import raster_tools as rt
 
 try:
     import geomulticorr.thumb as gmc_thumb
 except ModuleNotFoundError:
     import src.geomulticorr.thumb as gmc_thumb
 
+# ASP cannot write his outputs everywhere
+# In the temp (for temporary) directory, we know it will be ok
+# Then, we move the data (def save_corr_data)
 ROOT_OUTPUTS  = Path(__file__).with_name('temp')
+if not ROOT_OUTPUTS.exists():
+    ROOT_OUTPUTS.mkdir()
 
 class Pair:
 
     def __init__(self, session=None, target_path=None, left=None, right=None):
 
         """
         soit session et target_path sont definis
         soit left et right
         """
 
         # Construction from a pair path
         if type(target_path) in (str, Path):
             target_path = Path(target_path)
-            print(target_path)
             assert Path(target_path).parent.exists() and Path(target_path).parent.name.lower() == 'displacements', 'this path is not leading to a well-formed pair'
 
             # Get metadata about the thumbs component of the pair
             left_year, left_month, left_day, left_sensor = target_path.name.split('_')[1].split('-')
             right_year, right_month, right_day, right_sensor = target_path.name.split('_')[2].split('-')
             left_date = f"{left_year}-{left_month}-{left_day}"
             right_date = f"{right_year}-{right_month}-{right_day}"
@@ -236,14 +240,16 @@
         departure = Path(ROOT_OUTPUTS, self.pa_key)
 
         # get the displacements folder path in the current session
         destination = self.pa_asp_path
 
         # send the command to bring back the temporal data in the current session
         os.system(f"mv {departure} {destination} {verbose_mode[verbose]}")
+
+        # If the transfer have worked, we delete the data in the temp dir
         if self.pa_asp_path.exists():
             os.system(f"rm -rf {departure}")
             return True
 
         return False
 
     def del_useless_data(self):
@@ -352,15 +358,15 @@
 
         # Write vector layer in geopackage
         if write == True:
             current_vector_layer_name = f"{output_pixel_size}_{self.pa_key}"
             vectors.to_file(self.pa_vect_path, layer=current_vector_layer_name)
 
             # Copy .qml file
-            template_style = 'styles/vector-field_style_1.qml'
+            template_style = 'resources/map_styles/vector-field_style_1.qml'
             target_style = str(self.pa_vect_path)[:-5]
             cp_command = f"cp {template_style} {target_style}.qml"
             os.system(cp_command)
 
         return vectors
 
     def pa_full(self, corr_algorithm=2, corr_kernel_size=7, corr_xthreshold=10, vector_res=20, method='average'):
```

### Comparing `geomulticorr-0.1.4/src/geomulticorr/pzone.py` & `geomulticorr-0.1.5/src/geomulticorr/pzone.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 except ModuleNotFoundError:
     import src.geomulticorr.thumb as gmc_thumb
 
 class Pzone:
 
     def __init__(self, target_pz_name, session):
         
-        # Vérification de la validité du nom de pzone par rapport au projet
+        # Vérification de la validité du nom de pzone par rapport à la session
         assert target_pz_name in session.pz_names, f'{target_pz_name} not existing in the Pzones layer'
         assert Path(session.p_root, session.p_raster_data, target_pz_name).exists(), f'no raster data folder for {target_pz_name}'
 
         # Ecriture attributs
-        self.proj = session
+        self.session = session
         self.pz_name = target_pz_name
 
     def get_thumbs_overview(self, criterias=''):
         criterias = [criterias] + [self.pz_name]
-        return self.proj.get_thumbs_overview(criterias)
+        return self.session.get_thumbs_overview(criterias)
 
     def get_thumbs(self, criterias=''):
         criterias = [criterias] + [self.pz_name]
-        return self.proj.get_thumbs(criterias)
+        return self.session.get_thumbs(criterias)
 
     def get_pairs_overview(self, criterias=''):
         pairs = gpd.GeoDataFrame([pa.to_pdserie() for pa in self.get_pairs()])
         return pairs
 
     def get_pairs(self):
         """
@@ -47,15 +47,15 @@
                     continue
         return pairs
 
     def get_valid_thumbs(self):
         """
         Renvoie les vignettes selectionnées par l'user dans qgis, en modifiant la valeur attributaire "th_valid" dans la table Thumbs
         """
-        ths = self.proj.get_thumbs_overview(self.pz_name)
+        ths = self.session.get_thumbs_overview(self.pz_name)
         ths_valid = ths[ths.th_valid=='1']
         gmc_ths_valid = [gmc_thumb.Thumb(th.th_path) for th in ths_valid.iloc]
         return gmc_ths_valid
 
     def get_valid_pairs(self):
         ps = []
         for left in self.get_valid_thumbs():
@@ -63,15 +63,15 @@
                 try:
                     ps.append(left+right)
                 except AssertionError:
                     continue
         return ps
     
     def get_complete_pairs(self):
-        proj = proj.update_pairs()
+        session = session.update_pairs()
         return [p for p in self.get_pairs() if p.get_status() == 'complete']
 
     def pz_full(self, corr_algorithm=2, corr_kernel_size=7, corr_xthreshold=10, vector_res=20, method='average'):
         logs = {}
         logs['COMPLETE'] = []
         logs['ABORT'] = []
         for p in self.get_valid_pairs():
```

### Comparing `geomulticorr-0.1.4/src/geomulticorr/session.py` & `geomulticorr-0.1.5/src/geomulticorr/session.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.4/src/geomulticorr/spine.py` & `geomulticorr-0.1.5/src/geomulticorr/spine.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.4/src/geomulticorr/thumb.py` & `geomulticorr-0.1.5/src/geomulticorr/thumb.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.4/src/geomulticorr/xzone.py` & `geomulticorr-0.1.5/src/geomulticorr/xzone.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.4/src/geomulticorr/resources/map_styles/vector-field_style_1.qml` & `geomulticorr-0.1.5/src/geomulticorr/resources/map_styles/vector-field_style_1.qml`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.4/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg` & `geomulticorr-0.1.5/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.4/src/geomulticorr/resources/project_template/map_template-project.qgz` & `geomulticorr-0.1.5/src/geomulticorr/resources/project_template/map_template-project.qgz`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.4/tests/test_geomorph.py` & `geomulticorr-0.1.5/tests/test_geomorph.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.4/tests/test_pair.py` & `geomulticorr-0.1.5/tests/test_pair.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.4/tests/test_pzone.py` & `geomulticorr-0.1.5/tests/test_pzone.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
     def test_get_valid_thumbs(self):
         self.assertIsInstance(self.test_pzone.get_valid_thumbs(), list)
     
     def test_get_valid_pairs(self):
         self.assertIsInstance(self.test_pzone.get_valid_pairs(), list)
     
     # def test_pz_full(self):
-    #     self.assertIsInstance(self.test_pzone.pz_full(), dict)
+    #     self.assertIsInstance(self.test_pzone.pz_full(), dict)
```

### Comparing `geomulticorr-0.1.4/tests/test_session.py` & `geomulticorr-0.1.5/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.4/tests/test_thumb.py` & `geomulticorr-0.1.5/tests/test_thumb.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.4/LICENSE.md` & `geomulticorr-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.4/pyproject.toml` & `geomulticorr-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "geomulticorr"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Thibaut Duvanel", email="thibaut.duvanel@univ-smb.fr" },
 ]
 description = "A python lib to study earth-surface displacements from optical images with Ames Stereo Pipeline"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `geomulticorr-0.1.4/PKG-INFO` & `geomulticorr-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomulticorr
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python lib to study earth-surface displacements from optical images with Ames Stereo Pipeline
 Author-email: Thibaut Duvanel <thibaut.duvanel@univ-smb.fr>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

