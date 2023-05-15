# Comparing `tmp/alpineer-0.1.7.tar.gz` & `tmp/alpineer-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpineer-0.1.7.tar", max compression
+gzip compressed data, was "alpineer-0.1.8.tar", max compression
```

## Comparing `alpineer-0.1.7.tar` & `alpineer-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11845 2023-05-05 20:26:14.594905 alpineer-0.1.7/LICENSE
--rw-r--r--   0        0        0     5220 2023-05-05 20:26:14.594905 alpineer-0.1.7/README.md
--rw-r--r--   0        0        0     2758 2023-05-05 20:26:46.391635 alpineer-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-05 20:26:14.598905 alpineer-0.1.7/src/alpineer/__init__.py
--rw-r--r--   0        0        0     1398 2023-05-05 20:26:14.598905 alpineer-0.1.7/src/alpineer/data_utils.py
--rw-r--r--   0        0        0      939 2023-05-05 20:26:14.598905 alpineer-0.1.7/src/alpineer/image_utils.py
--rw-r--r--   0        0        0     7760 2023-05-05 20:26:14.598905 alpineer-0.1.7/src/alpineer/io_utils.py
--rw-r--r--   0        0        0    22804 2023-05-05 20:26:14.598905 alpineer-0.1.7/src/alpineer/load_utils.py
--rw-r--r--   0        0        0     8209 2023-05-05 20:26:14.598905 alpineer-0.1.7/src/alpineer/misc_utils.py
--rw-r--r--   0        0        0        0 2023-05-05 20:26:14.598905 alpineer-0.1.7/src/alpineer/py.typed
--rw-r--r--   0        0        0      223 2023-05-05 20:26:14.598905 alpineer-0.1.7/src/alpineer/settings.py
--rw-r--r--   0        0        0    20206 2023-05-05 20:26:14.598905 alpineer-0.1.7/src/alpineer/test_utils.py
--rw-r--r--   0        0        0     5109 2023-05-05 20:26:14.598905 alpineer-0.1.7/src/alpineer/tiff_utils.py
--rw-r--r--   0        0        0     6298 1970-01-01 00:00:00.000000 alpineer-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11845 2023-05-15 23:49:45.083226 alpineer-0.1.8/LICENSE
+-rw-r--r--   0        0        0     5220 2023-05-15 23:49:45.083226 alpineer-0.1.8/README.md
+-rw-r--r--   0        0        0     2758 2023-05-15 23:50:11.882977 alpineer-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-15 23:49:45.083226 alpineer-0.1.8/src/alpineer/__init__.py
+-rw-r--r--   0        0        0     1398 2023-05-15 23:49:45.083226 alpineer-0.1.8/src/alpineer/data_utils.py
+-rw-r--r--   0        0        0      939 2023-05-15 23:49:45.083226 alpineer-0.1.8/src/alpineer/image_utils.py
+-rw-r--r--   0        0        0     7760 2023-05-15 23:49:45.083226 alpineer-0.1.8/src/alpineer/io_utils.py
+-rw-r--r--   0        0        0    22840 2023-05-15 23:49:45.083226 alpineer-0.1.8/src/alpineer/load_utils.py
+-rw-r--r--   0        0        0     8209 2023-05-15 23:49:45.083226 alpineer-0.1.8/src/alpineer/misc_utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 23:49:45.083226 alpineer-0.1.8/src/alpineer/py.typed
+-rw-r--r--   0        0        0      223 2023-05-15 23:49:45.083226 alpineer-0.1.8/src/alpineer/settings.py
+-rw-r--r--   0        0        0    20206 2023-05-15 23:49:45.087226 alpineer-0.1.8/src/alpineer/test_utils.py
+-rw-r--r--   0        0        0     5109 2023-05-15 23:49:45.087226 alpineer-0.1.8/src/alpineer/tiff_utils.py
+-rw-r--r--   0        0        0     6298 1970-01-01 00:00:00.000000 alpineer-0.1.8/PKG-INFO
```

### Comparing `alpineer-0.1.7/LICENSE` & `alpineer-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.7/README.md` & `alpineer-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.7/pyproject.toml` & `alpineer-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alpineer"
-version = "0.1.7"
+version = "0.1.8"
 description = "Toolbox for Multiplexed Imaging. Contains scripts and little tools which are used throughout ark-analysis, mibi-bin-tools, and toffy."
 authors = [
     "Noah Frey Greenwald <nfgreen@stanford.edu>",
     "Adam Kagel <ackagel@stanford.edu>",
     "Alex Kong <alkong@stanford.edu>",
     "Cami Laura Sowers <csowers@stanford.edu>",
     "Sricharan Reddy Varra <srivarra@stanford.edu>",
```

### Comparing `alpineer-0.1.7/src/alpineer/data_utils.py` & `alpineer-0.1.8/src/alpineer/data_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.7/src/alpineer/image_utils.py` & `alpineer-0.1.8/src/alpineer/image_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.7/src/alpineer/io_utils.py` & `alpineer-0.1.8/src/alpineer/io_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.7/src/alpineer/load_utils.py` & `alpineer-0.1.8/src/alpineer/load_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         misc_utils.verify_same_elements(
             all_channels_in_folder=all_channels_no_delim, all_channels_detected=channels_no_delim
         )
         # reorder back to original
         channels = [chan for _, chan in sorted(zip(channels_indices, all_channels))]
 
     if len(channels) == 0:
-        raise ValueError("No images found in designated folder")
+        raise ValueError(f"No images found in designated folder, {os.path.join(data_dir, fovs[0])}")
 
     test_img = io.imread(os.path.join(data_dir, fovs[0], img_sub_folder, channels[0]))
 
     # The dtype is always the type of the image being loaded in.
     dtype = test_img.dtype
 
     if max_image_size is not None:
```

### Comparing `alpineer-0.1.7/src/alpineer/misc_utils.py` & `alpineer-0.1.8/src/alpineer/misc_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.7/src/alpineer/test_utils.py` & `alpineer-0.1.8/src/alpineer/test_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.7/src/alpineer/tiff_utils.py` & `alpineer-0.1.8/src/alpineer/tiff_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.7/PKG-INFO` & `alpineer-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpineer
-Version: 0.1.7
+Version: 0.1.8
 Summary: Toolbox for Multiplexed Imaging. Contains scripts and little tools which are used throughout ark-analysis, mibi-bin-tools, and toffy.
 Home-page: https://github.com/angelolab/tmi
 License: Modified Apache 2.0
 Author: Noah Frey Greenwald
 Author-email: nfgreen@stanford.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

