# Comparing `tmp/zensvi-0.1.7.tar.gz` & `tmp/zensvi-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zensvi-0.1.7.tar", max compression
+gzip compressed data, was "zensvi-0.1.8.tar", max compression
```

## Comparing `zensvi-0.1.7.tar` & `zensvi-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.1.7/LICENSE
--rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.1.7/README.md
--rwxr-xr-x   0        0        0      694 2023-05-16 03:25:18.705375 zensvi-0.1.7/pyproject.toml
--rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.1.7/src/zensvi/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.1.7/src/zensvi/cv/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.1.7/src/zensvi/cv/segmentation/__init__.py
--rwxr-xr-x   0        0        0    39332 2023-05-16 03:24:41.275521 zensvi-0.1.7/src/zensvi/cv/segmentation/segmentation.py
--rwxr-xr-x   0        0        0       55 2023-05-14 01:59:06.771355 zensvi-0.1.7/src/zensvi/download/__init__.py
--rwxr-xr-x   0        0        0    20153 2023-05-16 03:24:41.276347 zensvi-0.1.7/src/zensvi/download/streetview_downloader.py
--rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.1.7/src/zensvi/download/utils/UserAgent.csv
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.1.7/src/zensvi/download/utils/__init__.py
--rwxr-xr-x   0        0        0     8291 2023-05-14 13:25:54.052907 zensvi-0.1.7/src/zensvi/download/utils/geoprocess.py
--rwxr-xr-x   0        0        0     2000 2023-05-14 12:56:31.947491 zensvi-0.1.7/src/zensvi/download/utils/get_pids.py
--rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.1.7/src/zensvi/download/utils/helpers.py
--rwxr-xr-x   0        0        0     8165 2023-05-15 13:48:37.487829 zensvi-0.1.7/src/zensvi/download/utils/imtool.py
--rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.1.7/src/zensvi/download/utils/proxies.csv
--rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.1.7/src/zensvi/transform/__init__.py
--rwxr-xr-x   0        0        0     6500 2023-05-14 01:59:06.778828 zensvi-0.1.7/src/zensvi/transform/transform_image.py
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.1.7/src/zensvi/zensvi.py
--rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 zensvi-0.1.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.1.8/LICENSE
+-rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.1.8/README.md
+-rwxr-xr-x   0        0        0      694 2023-05-16 12:55:59.338096 zensvi-0.1.8/pyproject.toml
+-rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.1.8/src/zensvi/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.1.8/src/zensvi/cv/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.1.8/src/zensvi/cv/segmentation/__init__.py
+-rwxr-xr-x   0        0        0    39320 2023-05-16 12:53:24.202232 zensvi-0.1.8/src/zensvi/cv/segmentation/segmentation.py
+-rwxr-xr-x   0        0        0       55 2023-05-14 01:59:06.771355 zensvi-0.1.8/src/zensvi/download/__init__.py
+-rwxr-xr-x   0        0        0    21150 2023-05-16 12:53:24.204133 zensvi-0.1.8/src/zensvi/download/streetview_downloader.py
+-rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.1.8/src/zensvi/download/utils/UserAgent.csv
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.1.8/src/zensvi/download/utils/__init__.py
+-rwxr-xr-x   0        0        0     8291 2023-05-14 13:25:54.052907 zensvi-0.1.8/src/zensvi/download/utils/geoprocess.py
+-rwxr-xr-x   0        0        0     2000 2023-05-14 12:56:31.947491 zensvi-0.1.8/src/zensvi/download/utils/get_pids.py
+-rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.1.8/src/zensvi/download/utils/helpers.py
+-rwxr-xr-x   0        0        0     8165 2023-05-15 13:48:37.487829 zensvi-0.1.8/src/zensvi/download/utils/imtool.py
+-rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.1.8/src/zensvi/download/utils/proxies.csv
+-rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.1.8/src/zensvi/transform/__init__.py
+-rwxr-xr-x   0        0        0     6500 2023-05-14 01:59:06.778828 zensvi-0.1.8/src/zensvi/transform/transform_image.py
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.1.8/src/zensvi/zensvi.py
+-rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 zensvi-0.1.8/PKG-INFO
```

### Comparing `zensvi-0.1.7/LICENSE` & `zensvi-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.7/README.md` & `zensvi-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.7/pyproject.toml` & `zensvi-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zensvi"
-version = "0.1.7"
+version = "0.1.8"
 description = "This package handles downloading, cleaning, analyzing street view imagery in one-stop and zen manner."
 authors = ["koito19960406"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `zensvi-0.1.7/src/zensvi/cv/segmentation/segmentation.py` & `zensvi-0.1.8/src/zensvi/cv/segmentation/segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,15 +380,15 @@
 
         Args:
             pixel_ratio_dict (dict): Dictionary with class names as keys and pixel ratios as values.
             dir_output (pathlib.Path): Output directory path.
         """
         pixel_ratios_df = pd.DataFrame(pixel_ratio_dict).transpose()
         pixel_ratios_df.fillna(0, inplace=True)
-        pixel_ratios_df.index.names = ["filename_key"]
+        pixel_ratios_df.index.names = ["panoid"]
         pixel_ratios_df.to_csv(dir_output / "pixel_ratios.csv")
 
     def _panoptic_segmentation(self, images, original_img_shape):
         """
         Perform panoptic segmentation on the given images.
 
         Args:
@@ -667,15 +667,15 @@
             pixel_ratio_dict = {}
 
             for image_file_key, label_ratios in results:
                 pixel_ratio_dict[str(image_file_key)] = label_ratios
 
             pixel_ratios_df = pd.DataFrame(pixel_ratio_dict).transpose()
             pixel_ratios_df.fillna(0, inplace=True)
-            pixel_ratios_df.index.names = ["filename_key"]
+            pixel_ratios_df.index.names = ["panoid"]
 
             return pixel_ratios_df
         
         def results_to_nested_dict(results):
             """
             Converts the results obtained from processing each image file into a nested dictionary.
```

### Comparing `zensvi-0.1.7/src/zensvi/download/streetview_downloader.py` & `zensvi-0.1.8/src/zensvi/download/streetview_downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from shapely.geometry import Point
 import warnings
 from shapely.errors import ShapelyDeprecationWarning
 warnings.filterwarnings("ignore", category=ShapelyDeprecationWarning)
 import csv
 import glob
 import shutil
+import numpy as np
 
 from zensvi.download.utils.imtool import ImageTool
 from zensvi.download.utils.get_pids import panoids
 from zensvi.download.utils.geoprocess import GeoProcessor
 from zensvi.download.utils.helpers import standardize_column_names, create_buffer_gdf
 
 class StreetViewDownloader:
@@ -214,101 +215,120 @@
         dir_cache_pids = self.dir_cache / 'raw_pids'
         dir_cache_pids.mkdir(parents=True, exist_ok=True)
 
         # 2. Load all the checkpoint csv files
         checkpoints = glob.glob(str(dir_cache_pids / '*.csv'))
         checkpoint_start_index = len(checkpoints)
         if checkpoint_start_index > 0:
-            completed_rows = pd.concat([pd.read_csv(checkpoint) for checkpoint in checkpoints], ignore_index=True)
+            dataframes = []
+            for checkpoint in checkpoints:
+                try:
+                    df_checkpoint = pd.read_csv(checkpoint)
+                    dataframes.append(df_checkpoint)
+                except pd.errors.EmptyDataError:
+                    print(f"Warning: {checkpoint} is empty and has been skipped.")
+                    continue
+            completed_rows = pd.concat(dataframes, ignore_index=True)
 
-            if id_columns is None:
-                # Use 'longitude' and 'latitude' columns to filter rows if id_columns is None
-                id_columns = ['longitude', 'latitude']
+            completed_ids = completed_rows['lat_lon_id'].drop_duplicates()
 
-            completed_ids = completed_rows[id_columns].drop_duplicates()
+            # Merge on the ID column, keeping track of where each row originates
+            merged = df.merge(completed_ids, on='lat_lon_id', how='outer', indicator=True)
 
-            # Filter df to get remaining lat lon to get pids for
-            df = df[~df[id_columns].isin(completed_ids).all(axis=1)]
+            # Filter out rows that come from the 'completed_ids' DataFrame
+            df = merged[merged['_merge'] == 'left_only'].drop(columns='_merge')
 
         def get_street_view_info(longitude, latitude, proxies):
             results = panoids(latitude, longitude, proxies, closest=closest, disp=disp)
             return results
 
         def worker(row):
             input_longitude = row.longitude
             input_latitude = row.latitude
-            return {column: getattr(row, column) for column in id_columns}, (input_longitude, input_latitude), get_street_view_info(input_longitude, input_latitude, self.proxies)
+            lat_lon_id = row.lat_lon_id
+            id_dict = {column: getattr(row, column) for column in id_columns} if id_columns else {}
+            return lat_lon_id, (input_longitude, input_latitude), get_street_view_info(input_longitude, input_latitude, self.proxies), id_dict
 
         results = []
         batch_size = 1000  # Modify this to a suitable value
         num_batches = (len(df) + batch_size - 1) // batch_size
         failed_rows = []
-
+        
+        # if there's no rows to process, return completed_ids
+        if len(df) == 0:
+            return completed_ids
+        
+        # if not, process the rows
         for i in tqdm(range(num_batches), desc=f"Getting pids by batch size {min(batch_size, len(df))}"):
             with ThreadPoolExecutor() as executor:
                 batch_futures = {executor.submit(worker, row): row for row in df.iloc[i*batch_size : (i+1)*batch_size].itertuples()}
                 for future in tqdm(as_completed(batch_futures), total=len(batch_futures), desc=f"Getting pids for batch #{i+1}"):
                     try:
-                        id_dict, (input_longitude, input_latitude), row_results = future.result()
+                        lat_lon_id, (input_longitude, input_latitude), row_results, id_dict = future.result()
                         for result in row_results:
                             result['input_longitude'] = input_longitude
                             result['input_latitude'] = input_latitude
+                            result['lat_lon_id'] = lat_lon_id
                             result.update(id_dict)
                             results.append(result)
                     except Exception as e:
                         print(f"Error: {e}")
                         failed_rows.append(batch_futures[future])  # Store the failed row
 
                 # Save checkpoint for each batch
-                pd.DataFrame(results).to_csv(f'{dir_cache_pids}/checkpoint_batch_{checkpoint_start_index+i+1}.csv', index=False)
+                if len(results) > 0:
+                    pd.DataFrame(results).to_csv(f'{dir_cache_pids}/checkpoint_batch_{checkpoint_start_index+i+1}.csv', index=False)
                 results = []  # Clear the results list for the next batch
 
         # Merge all checkpoints into a single dataframe
         results_df = pd.concat([pd.read_csv(checkpoint) for checkpoint in glob.glob(str(dir_cache_pids / '*.csv'))], ignore_index=True)
 
         # Retry failed rows
         if failed_rows:
             print("Retrying failed rows...")
             with ThreadPoolExecutor() as executor:
                 retry_futures = {executor.submit(worker, row): row for row in failed_rows}
                 for future in tqdm(as_completed(retry_futures), total=len(retry_futures), desc="Retrying failed rows"):
                     try:
-                        id_dict, (input_longitude, input_latitude), row_results = future.result()
+                        lat_lon_id, (input_longitude, input_latitude), row_results, id_dict = future.result()
                         for result in row_results:
                             result['input_longitude'] = input_longitude
                             result['input_latitude'] = input_latitude
+                            result['lat_lon_id'] = lat_lon_id
                             result.update(id_dict)
                             results.append(result)
                     except Exception as e:
                         print(f"Failed again: {e}")
 
             # Save the results of retried rows as another checkpoint
-            pd.DataFrame(results).to_csv(f'{dir_cache_pids}/checkpoint_retry.csv', index=False)
-
-            # Merge the retry checkpoint into the final dataframe
-            retry_df = pd.read_csv(f'{dir_cache_pids}/checkpoint_retry.csv')
-            results_df = pd.concat([results_df, retry_df], ignore_index=True)
+            if len(results) > 0:
+                pd.DataFrame(results).to_csv(f'{dir_cache_pids}/checkpoint_retry.csv', index=False)
+                # Merge the retry checkpoint into the final dataframe
+                retry_df = pd.read_csv(f'{dir_cache_pids}/checkpoint_retry.csv')
+                results_df = pd.concat([results_df, retry_df], ignore_index=True)
 
-        # now save results_df as a new cache
+        # now save results_df as a new cache afte dropping lat_lon_id
+        results_df = results_df.drop(columns='lat_lon_id')
         results_df.to_csv(self.cache_pids_raw, index=False)
-        
+
         # delete the cache directory
         if dir_cache_pids.exists():
             shutil.rmtree(dir_cache_pids)
         return results_df
 
 
     def _get_pids_from_gdf(self, gdf, id_columns, closest=False, disp=False):  
         if self.cache_lat_lon.exists():
             df = pd.read_csv(self.cache_lat_lon)
             print("The lat and lon have been read from the cache")
         else:
             # read shapefile
             gp = GeoProcessor(gdf, distance=self.distance, grid=self.grid, grid_size=self.grid_size, id_columns = id_columns)
             df = gp.get_lat_lon()
+            df['lat_lon_id'] = np.arange(1, len(df) + 1)
             # save df to cache
             df.to_csv(self.cache_lat_lon, index=False)
 
         if self.cache_pids_raw.exists():
             results_df = pd.read_csv(self.cache_pids_raw)
         else:
             # Use _get_pids_from_csv to get pids from df
```

### Comparing `zensvi-0.1.7/src/zensvi/download/utils/UserAgent.csv` & `zensvi-0.1.8/src/zensvi/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.7/src/zensvi/download/utils/geoprocess.py` & `zensvi-0.1.8/src/zensvi/download/utils/geoprocess.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.7/src/zensvi/download/utils/get_pids.py` & `zensvi-0.1.8/src/zensvi/download/utils/get_pids.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.7/src/zensvi/download/utils/helpers.py` & `zensvi-0.1.8/src/zensvi/download/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.7/src/zensvi/download/utils/imtool.py` & `zensvi-0.1.8/src/zensvi/download/utils/imtool.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.7/src/zensvi/download/utils/proxies.csv` & `zensvi-0.1.8/src/zensvi/download/utils/proxies.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.7/src/zensvi/transform/transform_image.py` & `zensvi-0.1.8/src/zensvi/transform/transform_image.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.7/PKG-INFO` & `zensvi-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zensvi
-Version: 0.1.7
+Version: 0.1.8
 Summary: This package handles downloading, cleaning, analyzing street view imagery in one-stop and zen manner.
 License: MIT
 Author: koito19960406
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

