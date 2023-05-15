# Comparing `tmp/geolibs-0.0.6.tar.gz` & `tmp/geolibs-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geolibs-0.0.6.tar", max compression
+gzip compressed data, was "geolibs-0.0.7.tar", max compression
```

## Comparing `geolibs-0.0.6.tar` & `geolibs-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0      566 2023-05-06 21:58:44.569227 geolibs-0.0.6/README.rst
--rwxr-xr-x   0        0        0      512 2023-05-15 21:43:43.069320 geolibs-0.0.6/geolibs/__init__.py
--rwxr-xr-x   0        0        0    12279 2023-05-15 21:42:07.360993 geolibs-0.0.6/geolibs/engine_cocoext.py
--rwxr-xr-x   0        0        0     2469 2023-05-03 11:53:56.288065 geolibs-0.0.6/geolibs/engine_cocometric.py
--rwxr-xr-x   0        0        0     4167 2023-05-06 21:58:44.616807 geolibs-0.0.6/geolibs/engine_csv.py
--rwxr-xr-x   0        0        0     5015 2023-05-03 11:53:56.299297 geolibs-0.0.6/geolibs/enginelogger_hook.py
--rwxr-xr-x   0        0        0    12170 2023-05-15 18:42:52.457794 geolibs-0.0.6/geolibs/loading.py
--rwxr-xr-x   0        0        0     1122 2023-05-03 11:53:56.323004 geolibs-0.0.6/geolibs/misc.py
--rwxr-xr-x   0        0        0     1066 2023-05-15 21:43:43.059319 geolibs-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 geolibs-0.0.6/PKG-INFO
+-rwxr-xr-x   0        0        0      566 2023-05-06 21:58:44.569227 geolibs-0.0.7/README.rst
+-rwxr-xr-x   0        0        0      512 2023-05-15 23:28:10.304224 geolibs-0.0.7/geolibs/__init__.py
+-rwxr-xr-x   0        0        0    12311 2023-05-15 23:27:54.339092 geolibs-0.0.7/geolibs/engine_cocoext.py
+-rwxr-xr-x   0        0        0     2469 2023-05-03 11:53:56.288065 geolibs-0.0.7/geolibs/engine_cocometric.py
+-rwxr-xr-x   0        0        0     4167 2023-05-06 21:58:44.616807 geolibs-0.0.7/geolibs/engine_csv.py
+-rwxr-xr-x   0        0        0     5015 2023-05-03 11:53:56.299297 geolibs-0.0.7/geolibs/enginelogger_hook.py
+-rwxr-xr-x   0        0        0    12195 2023-05-15 22:23:50.825583 geolibs-0.0.7/geolibs/loading.py
+-rwxr-xr-x   0        0        0     1122 2023-05-03 11:53:56.323004 geolibs-0.0.7/geolibs/misc.py
+-rwxr-xr-x   0        0        0     1066 2023-05-15 23:28:10.298099 geolibs-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 geolibs-0.0.7/PKG-INFO
```

### Comparing `geolibs-0.0.6/README.rst` & `geolibs-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.6/geolibs/__init__.py` & `geolibs-0.0.7/geolibs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 from .engine_cocoext import EngineCocoExt
 from .engine_csv import EngineCSV
 from .loading import LoadBandsFromFile, LoadVariableSizedBandsFromFile, LoadMasks
 from .engine_cocometric import EngineCocoMetric
 
 __author__ = """Sagar Verma"""
 __email__ = 'sagar@granular.ai'
-__version__ = 'v0.0.6'
+__version__ = 'v0.0.7'
 
 __all__ = ["EngineLoggerHook", "EngineCocoExt", "EngineCocoMetric",
            "EngineCSV", "LoadBandsFromFile", "LoadVariableSizedBandsFromFile",
            "LoadMasks"]
```

### Comparing `geolibs-0.0.6/geolibs/engine_cocoext.py` & `geolibs-0.0.7/geolibs/engine_cocoext.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,47 +93,47 @@
                 for slice_x in range(0, img_width, self.stride[1]):
                     if (slice_x + self.window[1]) < img_width:
                         new_info = deepcopy(img_map)
                         new_info["slice_x"] = slice_x
                         new_info["slice_y"] = slice_y
                         new_info["slice_w"] = self.window[1]
                         new_info["slice_h"] = self.window[0]
-                        box_poly = box(slice_x, slice_y, slice_x + self.window[1], slice_y + self.window[0])
+                        box_poly = box(slice_x, slice_y, slice_x + self.window[1] - 1, slice_y + self.window[0] - 1)
                         new_info["instances"] = self._slice_annotations(vec_map["annotations"], box_poly)
                         data_infos.append(new_info)
                     elif slice_x < img_width:
                         new_info = deepcopy(img_map)
                         new_info["slice_y"] = slice_y
                         slice_x = img_width - self.window[1] - 1
                         new_info["slice_x"] = slice_x
                         new_info["slice_w"] = self.window[1]
                         new_info["slice_h"] = self.window[0]
-                        box_poly = box(slice_x, slice_y, slice_x + self.window[1], slice_y + self.window[0])
+                        box_poly = box(slice_x, slice_y, slice_x + self.window[1] - 1, slice_y + self.window[0] - 1)
                         new_info["instances"] = self._slice_annotations(vec_map["annotations"], box_poly)
                         data_infos.append(new_info)
             elif slice_y < img_height:
                 slice_y = img_height - self.window[0] - 1
                 for slice_x in range(0, img_width, self.stride[1]):
                     if (slice_x + self.window[1]) < img_width:
                         new_info = deepcopy(img_map)
                         new_info["slice_x"] = slice_x
                         new_info["slice_y"] = slice_y
                         new_info["slice_w"] = self.window[1]
                         new_info["slice_h"] = self.window[0]
-                        box_poly = box(slice_x, slice_y, slice_x + self.window[1], slice_y + self.window[0])
+                        box_poly = box(slice_x, slice_y, slice_x + self.window[1] - 1, slice_y + self.window[0] - 1)
                         new_info["instances"] = self._slice_annotations(vec_map["annotations"], box_poly)
                         data_infos.append(new_info)
                     elif slice_x < img_width:
                         new_info = deepcopy(img_map)
                         new_info["slice_y"] = slice_y
                         slice_x = img_width - self.window[1] - 1
                         new_info["slice_x"] = slice_x
                         new_info["slice_w"] = self.window[1]
                         new_info["slice_h"] = self.window[0]
-                        box_poly = box(slice_x, slice_y, slice_x + self.window[1], slice_y + self.window[0])
+                        box_poly = box(slice_x, slice_y, slice_x + self.window[1] - 1, slice_y + self.window[0] - 1)
                         new_info["instances"] = self._slice_annotations(vec_map["annotations"], box_poly)
                         data_infos.append(new_info)
 
         return data_infos
 
     def _load_vector_file(self, vec_path):
         vec_map = json.load(open(vec_path))
```

### Comparing `geolibs-0.0.6/geolibs/engine_cocometric.py` & `geolibs-0.0.7/geolibs/engine_cocometric.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.6/geolibs/engine_csv.py` & `geolibs-0.0.7/geolibs/engine_csv.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.6/geolibs/enginelogger_hook.py` & `geolibs-0.0.7/geolibs/enginelogger_hook.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.6/geolibs/loading.py` & `geolibs-0.0.7/geolibs/loading.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,16 +112,16 @@
                 self.file_client_args, filename)
             band_bytes = file_client.get(filename)
         else:
             band_bytes = fileio.get(
                 filename, backend_args=self.backend_args)
         
         bands, metadata = bandsfrombytes(band_bytes, band_ids=self.band_ids)
-        if self.gray2rgb:
-            assert bands.shape[0] == 1, "gray2rgb is only for grayscale images"
+        if self.gray2rgb or bands.shape[0] == 1:
+            # assert bands.shape[0] == 1, "gray2rgb is only for grayscale images"
             bands = np.asarray([bands[0], bands[0], bands[0]])
         bands = bands.transpose(1, 2, 0)
 
         bands = self._make_patch(bands, results)
         if self.to_float32:
             bands = bands.astype(np.float32)
```

### Comparing `geolibs-0.0.6/geolibs/misc.py` & `geolibs-0.0.7/geolibs/misc.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.6/pyproject.toml` & `geolibs-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geolibs"
-version = "v0.0.6"
+version = "v0.0.7"
 description = "A wrapper library that integrates GeoEngine and MMLab libraries for GeoSpatial ML development."
 authors = ["Sagar Verma <sagar@granular.ai>"]
 license = "MIT"
 readme = "README.rst"
 packages = [{include = "geolibs"}]
 classifiers = [
     'Intended Audience :: Developers',
```

### Comparing `geolibs-0.0.6/PKG-INFO` & `geolibs-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geolibs
-Version: 0.0.6
+Version: 0.0.7
 Summary: A wrapper library that integrates GeoEngine and MMLab libraries for GeoSpatial ML development.
 Home-page: https://github.com/granularai/geolibs
 License: MIT
 Author: Sagar Verma
 Author-email: sagar@granular.ai
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Intended Audience :: Developers
```

