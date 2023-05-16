# Comparing `tmp/scintillometry-1.0.1.tar.gz` & `tmp/scintillometry-1.0.4.tar.gz`

## Comparing `scintillometry-1.0.1.tar` & `scintillometry-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/__init__.py
--rw-r--r--   0        0        0    13702 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/backend/__init__.py
--rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/backend/constants.py
--rw-r--r--   0        0        0    25114 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/backend/constructions.py
--rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/backend/derivations.py
--rw-r--r--   0        0        0    15739 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/backend/iterations.py
--rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/backend/transects.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/metrics/__init__.py
--rwxr-xr-x   0        0        0    38541 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/metrics/calculations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/visuals/__init__.py
--rw-r--r--   0        0        0    31290 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/visuals/plotting.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/wrangler/__init__.py
--rw-r--r--   0        0        0    34239 2020-02-02 00:00:00.000000 scintillometry-1.0.1/src/scintillometry/wrangler/data_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0    27735 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/conftest.py
--rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/test_backend_constants.py
--rw-r--r--   0        0        0    28637 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/test_backend_constructions.py
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/test_backend_derivations.py
--rw-r--r--   0        0        0    12604 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/test_backend_iterations.py
--rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/test_backend_transects.py
--rw-r--r--   0        0        0    44917 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/test_metrics_calculations.py
--rw-r--r--   0        0        0    31368 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/test_visuals_plotting.py
--rw-r--r--   0        0        0    48525 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/test_wrangler_data_parser.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/test_data/test_data_v7_empty.mat
--rw-r--r--   0        0        0    12055 2020-02-02 00:00:00.000000 scintillometry-1.0.1/tests/test_data/test_data_v7_results.mat
--rw-r--r--   0        0        0    10813 2020-02-02 00:00:00.000000 scintillometry-1.0.1/LICENSE
--rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 scintillometry-1.0.1/README.md
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 scintillometry-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    22589 2020-02-02 00:00:00.000000 scintillometry-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/__init__.py
+-rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/backend/__init__.py
+-rw-r--r--   0        0        0     8349 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/backend/constants.py
+-rw-r--r--   0        0        0    25114 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/backend/constructions.py
+-rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/backend/derivations.py
+-rw-r--r--   0        0        0    15739 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/backend/iterations.py
+-rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/backend/transects.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/metrics/__init__.py
+-rwxr-xr-x   0        0        0    38541 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/metrics/calculations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/visuals/__init__.py
+-rw-r--r--   0        0        0    31290 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/visuals/plotting.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/wrangler/__init__.py
+-rw-r--r--   0        0        0    34241 2020-02-02 00:00:00.000000 scintillometry-1.0.4/src/scintillometry/wrangler/data_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/__init__.py
+-rw-r--r--   0        0        0    27735 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/conftest.py
+-rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/test_backend_constants.py
+-rw-r--r--   0        0        0    28637 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/test_backend_constructions.py
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/test_backend_derivations.py
+-rw-r--r--   0        0        0    12604 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/test_backend_iterations.py
+-rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/test_backend_transects.py
+-rw-r--r--   0        0        0    44917 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/test_metrics_calculations.py
+-rw-r--r--   0        0        0    31368 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/test_visuals_plotting.py
+-rw-r--r--   0        0        0    48525 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/test_wrangler_data_parser.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/test_data/test_data_v7_empty.mat
+-rw-r--r--   0        0        0    12055 2020-02-02 00:00:00.000000 scintillometry-1.0.4/tests/test_data/test_data_v7_results.mat
+-rw-r--r--   0        0        0    10813 2020-02-02 00:00:00.000000 scintillometry-1.0.4/LICENSE
+-rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 scintillometry-1.0.4/README.md
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 scintillometry-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    22589 2020-02-02 00:00:00.000000 scintillometry-1.0.4/PKG-INFO
```

### Comparing `scintillometry-1.0.1/src/scintillometry/main.py` & `scintillometry-1.0.4/src/scintillometry/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,21 +297,21 @@
         dict: Parsed and labelled datasets for scintillometry
         measurements, weather observations, and topography.
     """
 
     data_parser = DataParser.WranglerParsing()
 
     # Parse BLS, weather, and topographical data
-    datasets = data_parser.stitch.wrangle_data(
+    datasets = data_parser.wrangle_data(
         bls_path=kwargs["input"],
         transect_path=kwargs["transect_path"],
         calibrate=kwargs["calibration"],
         station_id=kwargs["station_id"],
         tzone=kwargs["timezone"],
-        source="zamg",
+        weather_source="zamg",
     )
 
     # Parse vertical measurements
     if kwargs["profile_prefix"]:
         datasets["vertical"] = data_parser.vertical.parse_vertical(
             file_path=kwargs["profile_prefix"],
             source="hatpro",
```

### Comparing `scintillometry-1.0.1/src/scintillometry/backend/constants.py` & `scintillometry-1.0.4/src/scintillometry/backend/constants.py`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.1/src/scintillometry/backend/constructions.py` & `scintillometry-1.0.4/src/scintillometry/backend/constructions.py`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.1/src/scintillometry/backend/derivations.py` & `scintillometry-1.0.4/src/scintillometry/backend/derivations.py`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.1/src/scintillometry/backend/iterations.py` & `scintillometry-1.0.4/src/scintillometry/backend/iterations.py`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.1/src/scintillometry/backend/transects.py` & `scintillometry-1.0.4/src/scintillometry/backend/transects.py`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.1/src/scintillometry/metrics/calculations.py` & `scintillometry-1.0.4/src/scintillometry/metrics/calculations.py`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.1/src/scintillometry/visuals/plotting.py` & `scintillometry-1.0.4/src/scintillometry/visuals/plotting.py`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.1/src/scintillometry/wrangler/data_parser.py` & `scintillometry-1.0.4/src/scintillometry/wrangler/data_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1005,15 +1005,15 @@
         bls_time = bls_data.index[0]
 
         transect_data = self.transect.parse_transect(file_path=transect_path)
 
         weather_data = self.weather.parse_weather(
             timestamp=bls_time,
             source=weather_source,
-            klima_id=station_id,
+            station_id=station_id,
             data_dir=weather_dir,
             timezone=tzone,
         )
         interpolated_data = self.stitch.merge_scintillometry_weather(
             scintillometry=bls_data, weather=weather_data
         )
```

### Comparing `scintillometry-1.0.1/tests/conftest.py` & `scintillometry-1.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.1/tests/test_backend_constants.py` & `scintillometry-1.0.4/tests/test_backend_constants.py`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.1/tests/test_backend_constructions.py` & `scintillometry-1.0.4/tests/test_backend_constructions.py`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.1/tests/test_backend_derivations.py` & `scintillometry-1.0.4/tests/test_backend_derivations.py`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.1/tests/test_backend_iterations.py` & `scintillometry-1.0.4/tests/test_backend_iterations.py`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.1/tests/test_backend_transects.py` & `scintillometry-1.0.4/tests/test_backend_transects.py`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.1/tests/test_metrics_calculations.py` & `scintillometry-1.0.4/tests/test_metrics_calculations.py`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.1/tests/test_visuals_plotting.py` & `scintillometry-1.0.4/tests/test_visuals_plotting.py`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.1/tests/test_wrangler_data_parser.py` & `scintillometry-1.0.4/tests/test_wrangler_data_parser.py`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.1/tests/test_data/test_data_v7_results.mat` & `scintillometry-1.0.4/tests/test_data/test_data_v7_results.mat`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.1/LICENSE` & `scintillometry-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.1/README.md` & `scintillometry-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `scintillometry-1.0.1/pyproject.toml` & `scintillometry-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scintillometry"
-version = "1.0.1"
+version = "1.0.4"
 authors = [
   { name="Scintillometry Contributors", email="" },
 ]
 description = "Analyse data & 2D flux footprints from Scintec's BLS scintillometers."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
```

### Comparing `scintillometry-1.0.1/PKG-INFO` & `scintillometry-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scintillometry
-Version: 1.0.1
+Version: 1.0.4
 Summary: Analyse data & 2D flux footprints from Scintec's BLS scintillometers.
 Project-URL: Homepage, https://github.com/gampnico/scintillometry
 Project-URL: Bug Tracker, https://github.com/gampnico/scintillometry/issues
 Project-URL: Documentation, https://scintillometry.readthedocs.io/en/latest/
 Author: Scintillometry Contributors
 License:                                  Apache License
                                    Version 2.0, January 2004
```

