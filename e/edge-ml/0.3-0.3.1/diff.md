# Comparing `tmp/edge-ml-0.3.tar.gz` & `tmp/edge-ml-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge-ml-0.3.tar", last modified: Tue May 16 10:58:14 2023, max compression
+gzip compressed data, was "edge-ml-0.3.1.tar", last modified: Tue May 16 11:03:45 2023, max compression
```

## Comparing `edge-ml-0.3.tar` & `edge-ml-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:58:14.467615 edge-ml-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-16 10:57:53.000000 edge-ml-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-16 10:58:14.467615 edge-ml-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-05-16 10:57:53.000000 edge-ml-0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-16 10:57:53.000000 edge-ml-0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-16 10:58:14.467615 edge-ml-0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:58:14.463616 edge-ml-0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:58:14.463616 edge-ml-0.3/src/edge_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-16 10:58:14.000000 edge-ml-0.3/src/edge_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-16 10:58:14.000000 edge-ml-0.3/src/edge_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 10:58:14.000000 edge-ml-0.3/src/edge_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 10:58:14.000000 edge-ml-0.3/src/edge_ml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:58:14.463616 edge-ml-0.3/src/edgeml/
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-16 10:57:53.000000 edge-ml-0.3/src/edgeml/Dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-16 10:57:53.000000 edge-ml-0.3/src/edgeml/Labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-16 10:57:53.000000 edge-ml-0.3/src/edgeml/TimeSeries.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 10:57:53.000000 edge-ml-0.3/src/edgeml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-16 10:57:53.000000 edge-ml-0.3/src/edgeml/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-05-16 10:57:53.000000 edge-ml-0.3/src/edgeml/edgeml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:58:14.463616 edge-ml-0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-16 10:57:53.000000 edge-ml-0.3/tests/test_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:03:45.328443 edge-ml-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-16 11:03:22.000000 edge-ml-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-16 11:03:45.328443 edge-ml-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-05-16 11:03:22.000000 edge-ml-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-16 11:03:22.000000 edge-ml-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-16 11:03:45.332443 edge-ml-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:03:45.328443 edge-ml-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:03:45.328443 edge-ml-0.3.1/src/edge_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-16 11:03:45.000000 edge-ml-0.3.1/src/edge_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-16 11:03:45.000000 edge-ml-0.3.1/src/edge_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 11:03:45.000000 edge-ml-0.3.1/src/edge_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 11:03:45.000000 edge-ml-0.3.1/src/edge_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:03:45.328443 edge-ml-0.3.1/src/edgeml/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-16 11:03:22.000000 edge-ml-0.3.1/src/edgeml/Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-16 11:03:22.000000 edge-ml-0.3.1/src/edgeml/Labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-16 11:03:22.000000 edge-ml-0.3.1/src/edgeml/TimeSeries.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 11:03:22.000000 edge-ml-0.3.1/src/edgeml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-16 11:03:22.000000 edge-ml-0.3.1/src/edgeml/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-16 11:03:22.000000 edge-ml-0.3.1/src/edgeml/edgeml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:03:45.328443 edge-ml-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-16 11:03:22.000000 edge-ml-0.3.1/tests/test_predictor.py
```

### Comparing `edge-ml-0.3/LICENSE` & `edge-ml-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edge-ml-0.3/PKG-INFO` & `edge-ml-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-ml
-Version: 0.3
+Version: 0.3.1
 Summary: Python library of edge-ml.org: end-to-end machine learning for embedded devices
 Home-page: https://github.com/edge-ml/python
 Author: KIT/TECO
 Author-email: KIT/TECO <info@edge-ml.org>
 Project-URL: Home, https://edge-ml.org
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `edge-ml-0.3/README.md` & `edge-ml-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `edge-ml-0.3/setup.cfg` & `edge-ml-0.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = edge-ml
-version = 0.3
+version = 0.3.1
 author = KIT/TECO
 autor_email = info@edge-ml.org
 description = Python library of edge-ml.org: end-to-end machine learning for embedded devices
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/edge-ml/python
 project_urls =
```

### Comparing `edge-ml-0.3/src/edge_ml.egg-info/PKG-INFO` & `edge-ml-0.3.1/src/edge_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-ml
-Version: 0.3
+Version: 0.3.1
 Summary: Python library of edge-ml.org: end-to-end machine learning for embedded devices
 Home-page: https://github.com/edge-ml/python
 Author: KIT/TECO
 Author-email: KIT/TECO <info@edge-ml.org>
 Project-URL: Home, https://edge-ml.org
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `edge-ml-0.3/src/edgeml/Dataset.py` & `edge-ml-0.3.1/src/edgeml/Dataset.py`

 * *Files identical despite different names*

### Comparing `edge-ml-0.3/src/edgeml/Labeling.py` & `edge-ml-0.3.1/src/edgeml/Labeling.py`

 * *Files identical despite different names*

### Comparing `edge-ml-0.3/src/edgeml/TimeSeries.py` & `edge-ml-0.3.1/src/edgeml/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `edge-ml-0.3/src/edgeml/edgeml.py` & `edge-ml-0.3.1/src/edgeml/edgeml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import requests as req
 from edgeml.consts import getProjectEndpoint, initDatasetIncrement, addDatasetIncrement
 from edgeml.Dataset import Dataset
 import time
 
-
-print(initDatasetIncrement)
-
 class DatasetReceiver:
 
     def __init__(self, backendURL, readKey=None, writeKey=None):
         self.backendURL = backendURL
         self._readKey=readKey
         self._writeKey=writeKey
         res = req.get(backendURL + getProjectEndpoint + readKey)
```

### Comparing `edge-ml-0.3/tests/test_predictor.py` & `edge-ml-0.3.1/tests/test_predictor.py`

 * *Files identical despite different names*

