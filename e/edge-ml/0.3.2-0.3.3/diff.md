# Comparing `tmp/edge-ml-0.3.2.tar.gz` & `tmp/edge-ml-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge-ml-0.3.2.tar", last modified: Tue May 16 11:49:39 2023, max compression
+gzip compressed data, was "edge-ml-0.3.3.tar", last modified: Tue May 16 12:07:15 2023, max compression
```

## Comparing `edge-ml-0.3.2.tar` & `edge-ml-0.3.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:49:39.911188 edge-ml-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-16 11:49:18.000000 edge-ml-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-16 11:49:39.911188 edge-ml-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-05-16 11:49:18.000000 edge-ml-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-16 11:49:18.000000 edge-ml-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-16 11:49:39.911188 edge-ml-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:49:39.907188 edge-ml-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:49:39.907188 edge-ml-0.3.2/src/edge_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-16 11:49:39.000000 edge-ml-0.3.2/src/edge_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-16 11:49:39.000000 edge-ml-0.3.2/src/edge_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 11:49:39.000000 edge-ml-0.3.2/src/edge_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 11:49:39.000000 edge-ml-0.3.2/src/edge_ml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:49:39.911188 edge-ml-0.3.2/src/edgeml/
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-16 11:49:18.000000 edge-ml-0.3.2/src/edgeml/Dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-16 11:49:18.000000 edge-ml-0.3.2/src/edgeml/Labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-16 11:49:18.000000 edge-ml-0.3.2/src/edgeml/TimeSeries.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 11:49:18.000000 edge-ml-0.3.2/src/edgeml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-16 11:49:18.000000 edge-ml-0.3.2/src/edgeml/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-16 11:49:18.000000 edge-ml-0.3.2/src/edgeml/edgeml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:49:39.911188 edge-ml-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-16 11:49:18.000000 edge-ml-0.3.2/tests/test_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:07:15.577928 edge-ml-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-16 12:06:52.000000 edge-ml-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-16 12:07:15.577928 edge-ml-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-05-16 12:06:52.000000 edge-ml-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-16 12:06:52.000000 edge-ml-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-16 12:07:15.581928 edge-ml-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:07:15.573928 edge-ml-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:07:15.577928 edge-ml-0.3.3/src/edge_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-16 12:07:15.000000 edge-ml-0.3.3/src/edge_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-16 12:07:15.000000 edge-ml-0.3.3/src/edge_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:07:15.000000 edge-ml-0.3.3/src/edge_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 12:07:15.000000 edge-ml-0.3.3/src/edge_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:07:15.577928 edge-ml-0.3.3/src/edgeml/
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-16 12:06:52.000000 edge-ml-0.3.3/src/edgeml/Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-16 12:06:52.000000 edge-ml-0.3.3/src/edgeml/Labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-16 12:06:52.000000 edge-ml-0.3.3/src/edgeml/TimeSeries.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 12:06:52.000000 edge-ml-0.3.3/src/edgeml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-16 12:06:52.000000 edge-ml-0.3.3/src/edgeml/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-16 12:06:52.000000 edge-ml-0.3.3/src/edgeml/edgeml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:07:15.577928 edge-ml-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-16 12:06:52.000000 edge-ml-0.3.3/tests/test_predictor.py
```

### Comparing `edge-ml-0.3.2/LICENSE` & `edge-ml-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `edge-ml-0.3.2/PKG-INFO` & `edge-ml-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-ml
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python library of edge-ml.org: end-to-end machine learning for embedded devices
 Home-page: https://github.com/edge-ml/python
 Author: KIT/TECO
 Author-email: KIT/TECO <info@edge-ml.org>
 Project-URL: Home, https://edge-ml.org
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `edge-ml-0.3.2/README.md` & `edge-ml-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `edge-ml-0.3.2/setup.cfg` & `edge-ml-0.3.3/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = edge-ml
-version = 0.3.2
+version = 0.3.3
 author = KIT/TECO
 autor_email = info@edge-ml.org
 description = Python library of edge-ml.org: end-to-end machine learning for embedded devices
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/edge-ml/python
 project_urls =
```

### Comparing `edge-ml-0.3.2/src/edge_ml.egg-info/PKG-INFO` & `edge-ml-0.3.3/src/edge_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-ml
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python library of edge-ml.org: end-to-end machine learning for embedded devices
 Home-page: https://github.com/edge-ml/python
 Author: KIT/TECO
 Author-email: KIT/TECO <info@edge-ml.org>
 Project-URL: Home, https://edge-ml.org
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `edge-ml-0.3.2/src/edgeml/Dataset.py` & `edge-ml-0.3.3/src/edgeml/Dataset.py`

 * *Files identical despite different names*

### Comparing `edge-ml-0.3.2/src/edgeml/Labeling.py` & `edge-ml-0.3.3/src/edgeml/Labeling.py`

 * *Files identical despite different names*

### Comparing `edge-ml-0.3.2/src/edgeml/TimeSeries.py` & `edge-ml-0.3.3/src/edgeml/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `edge-ml-0.3.2/src/edgeml/edgeml.py` & `edge-ml-0.3.3/src/edgeml/edgeml.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,33 +99,31 @@
             raise ValueError("invalid time-series name")
 
         if not isinstance(value, (int, float)):
             raise ValueError("Datapoint is not a number")
 
         if not isinstance(timestamp, (int)):
             raise ValueError("Provide a valid timestamp")
-
         self.dataStore[name].append([timestamp, value])
 
         if time.time() * 1000 - self.lastChecked > UPLOAD_INTERVAL:
             self.upload(self.labeling)
             self.lastChecked = time.time() * 1000
-            self.dataStore = {"data": []}
 
 
     async def upload(self, uploadLabel):
         tmp_dataStore = self.dataStore.copy()
         tmp_dataStore = [{"name": k, "data": tmp_dataStore[k]} for k in tmp_dataStore.keys()]
         response = req.post(
             self.url
             + addDatasetIncrement
             + self.apiKey
             + "/"
             + self.datasetKey,
-            json={"data": tmp_dataStore, "labeling": uploadLabel},
+            json={"data": tmp_dataStore, "labeling": None},
         )
         self.dataStore = {x: [] for x in self.timeSeries}
         if response.status_code != 200:
             raise RuntimeError("Upload failed")
 
     # Synchronizes the server with the data when you have added all data
     def onComplete(self):
```

### Comparing `edge-ml-0.3.2/tests/test_predictor.py` & `edge-ml-0.3.3/tests/test_predictor.py`

 * *Files identical despite different names*

