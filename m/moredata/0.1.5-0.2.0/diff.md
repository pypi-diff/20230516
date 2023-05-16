# Comparing `tmp/moredata-0.1.5.tar.gz` & `tmp/moredata-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moredata-0.1.5.tar", last modified: Wed Aug 10 21:57:51 2022, max compression
+gzip compressed data, was "moredata-0.2.0.tar", last modified: Tue May 16 15:07:30 2023, max compression
```

## Comparing `moredata-0.1.5.tar` & `moredata-0.2.0.tar`

### file list

```diff
@@ -1,51 +1,47 @@
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2022-08-10 21:57:51.436146 moredata-0.1.5/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1524 2022-01-16 23:26:40.000000 moredata-0.1.5/LICENSE.txt
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      329 2022-08-10 21:57:51.436146 moredata-0.1.5/PKG-INFO
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1888 2022-03-07 16:27:31.000000 moredata-0.1.5/README.md
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2022-08-10 21:57:51.428146 moredata-0.1.5/moredata/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      972 2022-02-22 21:23:43.000000 moredata-0.1.5/moredata/__init__.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2022-08-10 21:57:51.428146 moredata-0.1.5/moredata/datasets/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      667 2022-08-10 21:57:20.000000 moredata-0.1.5/moredata/datasets/__init__.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2022-08-10 21:57:51.432146 moredata-0.1.5/moredata/datasets/airbnb/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)  6371452 2022-02-23 12:47:32.000000 moredata-0.1.5/moredata/datasets/airbnb/airbnb-berlin-extra.csv
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)  1298509 2022-02-23 12:47:32.000000 moredata-0.1.5/moredata/datasets/airbnb/airbnb-berlin-host.csv
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)  2340410 2022-02-23 12:47:32.000000 moredata-0.1.5/moredata/datasets/airbnb/airbnb-berlin-main.csv
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2022-08-10 21:57:51.436146 moredata-0.1.5/moredata/enricher/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      143 2022-02-22 21:23:43.000000 moredata-0.1.5/moredata/enricher/__init__.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2022-08-10 21:57:51.436146 moredata-0.1.5/moredata/enricher/api_connector/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       40 2022-01-16 23:26:40.000000 moredata-0.1.5/moredata/enricher/api_connector/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     4333 2022-08-10 21:26:20.000000 moredata-0.1.5/moredata/enricher/api_connector/api_connector.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2022-08-10 21:57:51.436146 moredata-0.1.5/moredata/enricher/elasticsearch_connector/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       98 2022-02-22 21:23:43.000000 moredata-0.1.5/moredata/enricher/elasticsearch_connector/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1698 2022-02-22 21:23:43.000000 moredata-0.1.5/moredata/enricher/elasticsearch_connector/elasticsearch_connector.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     5138 2022-08-09 21:59:44.000000 moredata-0.1.5/moredata/enricher/elasticsearch_connector/index_handler.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     6042 2022-02-26 01:23:31.000000 moredata-0.1.5/moredata/enricher/elasticsearch_connector/pipeline_handler.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2742 2022-02-26 01:23:31.000000 moredata-0.1.5/moredata/enricher/elasticsearch_connector/policy_handler.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1391 2022-08-10 21:26:20.000000 moredata-0.1.5/moredata/enricher/enricher.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2335 2022-08-10 21:26:20.000000 moredata-0.1.5/moredata/enricher/enricher_builder.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2022-08-10 21:57:51.436146 moredata-0.1.5/moredata/enricher/osm/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       79 2022-02-22 21:23:43.000000 moredata-0.1.5/moredata/enricher/osm/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     5054 2022-08-10 21:26:20.000000 moredata-0.1.5/moredata/enricher/osm/functional_region_connector.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     6965 2022-08-10 21:26:20.000000 moredata-0.1.5/moredata/enricher/osm/osm_places_connector.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2022-08-10 21:57:51.436146 moredata-0.1.5/moredata/enricher/sql_connector/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       29 2022-02-22 21:23:43.000000 moredata-0.1.5/moredata/enricher/sql_connector/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     4590 2022-08-10 21:26:20.000000 moredata-0.1.5/moredata/enricher/sql_connector/sql_connector.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2022-08-10 21:57:51.436146 moredata-0.1.5/moredata/models/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       20 2022-02-22 21:23:43.000000 moredata-0.1.5/moredata/models/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1711 2022-08-10 21:26:20.000000 moredata-0.1.5/moredata/models/data.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2022-08-10 21:57:51.436146 moredata-0.1.5/moredata/parser/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1172 2022-08-09 21:59:44.000000 moredata-0.1.5/moredata/parser/__init__.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2022-08-10 21:57:51.436146 moredata-0.1.5/moredata/tests/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        0 2022-01-16 23:26:40.000000 moredata-0.1.5/moredata/tests/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      414 2022-02-22 21:23:43.000000 moredata-0.1.5/moredata/tests/test_datasets.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2022-08-10 21:57:51.436146 moredata-0.1.5/moredata/utils/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     3727 2022-08-10 21:26:20.000000 moredata-0.1.5/moredata/utils/__init__.py
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2260 2022-08-09 21:59:44.000000 moredata-0.1.5/moredata/utils/osm_downloader.py
-drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2022-08-10 21:57:51.428146 moredata-0.1.5/moredata.egg-info/
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      329 2022-08-10 21:57:51.000000 moredata-0.1.5/moredata.egg-info/PKG-INFO
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1315 2022-08-10 21:57:51.000000 moredata-0.1.5/moredata.egg-info/SOURCES.txt
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        1 2022-08-10 21:57:51.000000 moredata-0.1.5/moredata.egg-info/dependency_links.txt
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      645 2022-08-10 21:57:51.000000 moredata-0.1.5/moredata.egg-info/requires.txt
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        9 2022-08-10 21:57:51.000000 moredata-0.1.5/moredata.egg-info/top_level.txt
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      108 2022-08-10 21:57:51.436146 moredata-0.1.5/setup.cfg
--rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1462 2022-08-10 21:53:37.000000 moredata-0.1.5/setup.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.247055 moredata-0.2.0/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1524 2022-01-16 23:26:40.000000 moredata-0.2.0/LICENSE.txt
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      457 2023-05-16 15:07:30.247055 moredata-0.2.0/PKG-INFO
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1892 2023-05-16 14:20:50.000000 moredata-0.2.0/README.md
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.243055 moredata-0.2.0/moredata/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      972 2022-02-22 21:23:43.000000 moredata-0.2.0/moredata/__init__.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.243055 moredata-0.2.0/moredata/datasets/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      633 2022-08-10 22:04:01.000000 moredata-0.2.0/moredata/datasets/__init__.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.243055 moredata-0.2.0/moredata/enricher/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      143 2022-02-22 21:23:43.000000 moredata-0.2.0/moredata/enricher/__init__.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.243055 moredata-0.2.0/moredata/enricher/api_connector/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       40 2022-01-16 23:26:40.000000 moredata-0.2.0/moredata/enricher/api_connector/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     4333 2022-08-10 21:26:20.000000 moredata-0.2.0/moredata/enricher/api_connector/api_connector.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.247055 moredata-0.2.0/moredata/enricher/elasticsearch_connector/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       98 2022-02-22 21:23:43.000000 moredata-0.2.0/moredata/enricher/elasticsearch_connector/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1698 2022-02-22 21:23:43.000000 moredata-0.2.0/moredata/enricher/elasticsearch_connector/elasticsearch_connector.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     5138 2022-08-09 21:59:44.000000 moredata-0.2.0/moredata/enricher/elasticsearch_connector/index_handler.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     6042 2022-02-26 01:23:31.000000 moredata-0.2.0/moredata/enricher/elasticsearch_connector/pipeline_handler.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2742 2022-02-26 01:23:31.000000 moredata-0.2.0/moredata/enricher/elasticsearch_connector/policy_handler.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1391 2022-08-10 21:26:20.000000 moredata-0.2.0/moredata/enricher/enricher.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2340 2023-03-24 00:39:22.000000 moredata-0.2.0/moredata/enricher/enricher_builder.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.247055 moredata-0.2.0/moredata/enricher/osm/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       79 2022-02-22 21:23:43.000000 moredata-0.2.0/moredata/enricher/osm/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     5807 2023-05-16 14:15:55.000000 moredata-0.2.0/moredata/enricher/osm/functional_region_connector.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     7398 2023-05-16 14:22:06.000000 moredata-0.2.0/moredata/enricher/osm/osm_places_connector.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.247055 moredata-0.2.0/moredata/enricher/sql_connector/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       29 2022-02-22 21:23:43.000000 moredata-0.2.0/moredata/enricher/sql_connector/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     4590 2022-08-10 21:26:20.000000 moredata-0.2.0/moredata/enricher/sql_connector/sql_connector.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.247055 moredata-0.2.0/moredata/models/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)       20 2022-02-22 21:23:43.000000 moredata-0.2.0/moredata/models/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1807 2023-05-16 14:17:33.000000 moredata-0.2.0/moredata/models/data.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.247055 moredata-0.2.0/moredata/parser/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1168 2023-05-16 14:27:49.000000 moredata-0.2.0/moredata/parser/__init__.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.247055 moredata-0.2.0/moredata/tests/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        0 2022-01-16 23:26:40.000000 moredata-0.2.0/moredata/tests/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      414 2022-02-22 21:23:43.000000 moredata-0.2.0/moredata/tests/test_datasets.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.247055 moredata-0.2.0/moredata/utils/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     3727 2023-05-16 14:22:23.000000 moredata-0.2.0/moredata/utils/__init__.py
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     2260 2023-05-16 14:22:23.000000 moredata-0.2.0/moredata/utils/osm_downloader.py
+drwxrwxr-x   0 gegen07   (1000) gegen07   (1000)        0 2023-05-16 15:07:30.243055 moredata-0.2.0/moredata.egg-info/
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      457 2023-05-16 15:07:30.000000 moredata-0.2.0/moredata.egg-info/PKG-INFO
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1170 2023-05-16 15:07:30.000000 moredata-0.2.0/moredata.egg-info/SOURCES.txt
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        1 2023-05-16 15:07:30.000000 moredata-0.2.0/moredata.egg-info/dependency_links.txt
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1299 2023-05-16 15:07:30.000000 moredata-0.2.0/moredata.egg-info/requires.txt
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)        9 2023-05-16 15:07:30.000000 moredata-0.2.0/moredata.egg-info/top_level.txt
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)      108 2023-05-16 15:07:30.247055 moredata-0.2.0/setup.cfg
+-rw-rw-r--   0 gegen07   (1000) gegen07   (1000)     1546 2023-05-16 15:00:39.000000 moredata-0.2.0/setup.py
```

### Comparing `moredata-0.1.5/LICENSE.txt` & `moredata-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `moredata-0.1.5/README.md` & `moredata-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 The first step is to clone/download the repository and open the project folder in the terminal. After that, execute this code to install all the necessary requirements:
     
     $ pip install moredata
     $ pip install jupyter-notebook
 
 Then go to examples directory and open a new jupyter-notebook in examples directory:
 
-$ cd examples/
+    $ cd examples/
 
 If you want to run elasticsearch or SQL example you should have installed docker or have elasticsearch/MySQL in your machine, then:
 
     $ cd examples/
     $ cd elasticsearch_connector
     $ docker-compose up
```

### Comparing `moredata-0.1.5/moredata/__init__.py` & `moredata-0.2.0/moredata/__init__.py`

 * *Files identical despite different names*

### Comparing `moredata-0.1.5/moredata/datasets/__init__.py` & `moredata-0.2.0/moredata/datasets/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 
 __all__ = ["available", "get_path"]
 
 _module_path = os.path.dirname(__file__)
 _available_csv = {
-    "airbnb-berlin-main": "./airbnb/airbnb-berlin-main.csv",
-    "airbnb-berlin-host": "./airbnb/airbnb-berlin-host.csv",
-    "airbnb-berlin-extra": "./airbnb/airbnb-berlin-extra.csv",
+    "airbnb-berlin-main": "airbnb-berlin-main.csv",
+    "airbnb-berlin-host": "airbnb-berlin-host.csv",
+    "airbnb-berlin-extra": "airbnb-berlin-extra.csv",
 }
 available = list(_available_csv.keys())
 
 
 def get_path(dataset):
     if dataset in _available_csv:
-        return os.path.abspath(os.path.join(_module_path, _available_csv[dataset]))
+        return os.path.abspath(os.path.join(_module_path, dataset + ".csv"))
     else:
         msg = "The dataset '{data}' is not available. ".format(data=dataset)
         msg += "Available datasets are {}".format(", ".join(available))
         raise ValueError(msg)
```

### Comparing `moredata-0.1.5/moredata/enricher/api_connector/api_connector.py` & `moredata-0.2.0/moredata/enricher/api_connector/api_connector.py`

 * *Files identical despite different names*

### Comparing `moredata-0.1.5/moredata/enricher/elasticsearch_connector/elasticsearch_connector.py` & `moredata-0.2.0/moredata/enricher/elasticsearch_connector/elasticsearch_connector.py`

 * *Files identical despite different names*

### Comparing `moredata-0.1.5/moredata/enricher/elasticsearch_connector/index_handler.py` & `moredata-0.2.0/moredata/enricher/elasticsearch_connector/index_handler.py`

 * *Files identical despite different names*

### Comparing `moredata-0.1.5/moredata/enricher/elasticsearch_connector/pipeline_handler.py` & `moredata-0.2.0/moredata/enricher/elasticsearch_connector/pipeline_handler.py`

 * *Files identical despite different names*

### Comparing `moredata-0.1.5/moredata/enricher/elasticsearch_connector/policy_handler.py` & `moredata-0.2.0/moredata/enricher/elasticsearch_connector/policy_handler.py`

 * *Files identical despite different names*

### Comparing `moredata-0.1.5/moredata/enricher/enricher.py` & `moredata-0.2.0/moredata/enricher/enricher.py`

 * *Files identical despite different names*

### Comparing `moredata-0.1.5/moredata/enricher/enricher_builder.py` & `moredata-0.2.0/moredata/enricher/enricher_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,8 +75,8 @@
         this method call all of enrichments functions that are 
         saved as array attribute in data class. 
 
         Returns
         -------
         This method returns the implementations of each :func:`~enricher.Enricher.enrich`.
         """
-        return pipe(self._data, [e.enrich for e in self._data.enrichers], **kwargs)
+        return pipe(self._data, [e.enrich for e in self._data.enrichers], **kwargs).data
```

### Comparing `moredata-0.1.5/moredata/enricher/osm/functional_region_connector.py` & `moredata-0.2.0/moredata/enricher/osm/functional_region_connector.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,18 +34,19 @@
     files: List[str]
 
     dict_keys: List[str]
 
     key: str
     """
 
-    def __init__(self, files, key, dict_keys=[]):
+    def __init__(self, files, key, radius=0, dict_keys=[]):
         self.key = key
         self.dict_keys = dict_keys
         self.files = files
+        self.radius = radius
 
         self._df = []
         if self.files is not None:
             read_temp = []
             for file in self.files:
                 read_temp.append(pd.read_csv(file))
             self._df = pd.concat(read_temp)
@@ -82,15 +83,15 @@
             else:
                 point[self.key] += amount
         else:
             raise Exception(
                 "area_point polygon was not found. Please use function geodesic_point_buffer present in utils package and try again."
             )
 
-    def enrichJsonData(self, data, **kwargs):
+    def enrich_json_data(self, data, **kwargs):
         for d in data.parse(**kwargs):
 
             if not self.dict_keys:
                 points = d
             else:
                 points = d[self.dict_keys[0]]
                 for k in range(1, len(self.dict_keys)):
@@ -103,35 +104,59 @@
                 for point in points:
                     self._enrich_point(point)
             else:
                 self._enrich_point(points)
 
             yield d
 
-    def enrich_geopandas_data(self, data):
-        self._df = self._df.set_crs(epsg=4326).to_crs(epsg=3857)
+    def _buffer_with_crs(self, data, new_crs=None):
+        if new_crs is None:
+            new_crs = "EPSG:3857"
+
+        if data.crs is None:
+            data = data.set_crs("EPSG:4326")
+
+        data["geometry_not_buffered"] = data["geometry"].copy()
+
+        if data.crs != new_crs:
+            data = data.to_crs(new_crs)
+
+        data["geometry"] = data["geometry"].buffer(self.radius)
+
+        data = data.to_crs("EPSG:4326")
+
+        return data
+
+    def enrich_geopandas_data(self, data: geopandas.GeoDataFrame, **kwargs):
+        self._df = self._df.set_crs("EPSG:4326")
         data.reset_index(inplace=True)
 
+        if self.radius != 0:
+            data = self._buffer_with_crs(data, kwargs.get("new_crs", None))
+
         spatial_joined = geopandas.sjoin(
             data, self._df, how="inner", predicate="intersects"
         )
         different_indices = spatial_joined.index.value_counts()
 
         data.set_index("index", inplace=True)
 
         data[self.key] = different_indices
         data[self.key].fillna(0, inplace=True)
 
+        data["geometry"] = data["geometry_not_buffered"]
+        data.drop("geometry_not_buffered", axis=1, inplace=True)
+
         return GeopandasData.from_geodataframe(data)
 
     def enrich(self, data, **kwargs):
         """Method overrided of interface. It walk through the keys to reach at the data that will be used to intersect the polygons. It uses a R tree to index polygons and search faster. For optimization purposes we recommend to buffer the point, using ``geodesic_point_buffer`` function, creating, necessarily, a label named ``area_point``, and save the file with points buffered to use as base of enrichment. After buffer the points, you can use the Functional Region Connector to create your enrichment passing proper attributes."""
         self._get_polygons()
 
         if isinstance(data, GeopandasData):
-            return self.enrich_geopandas_data(data.data)
+            return self.enrich_geopandas_data(data.data, **kwargs)
 
         elif isinstance(data, DaskGeopandasData):
-            raise Exception("DaskGeopandasData not supported yet")
+            raise Exception("DaskGeopandasData not implemented")
 
         elif isinstance(data, JsonData):
-            return self.enrichJsonData(data, **kwargs)
+            return self.enrich_json_data(data, **kwargs)
```

### Comparing `moredata-0.1.5/moredata/enricher/osm/osm_places_connector.py` & `moredata-0.2.0/moredata/enricher/osm/osm_places_connector.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,18 +31,14 @@
 
     file: str, optional
         name of file in CSV of downloaded polygons with must columns: key, value, polygon.
 
     radius: numeric, optional
         radius to around of point to intersect the polygon.
 
-    buffered: boolean
-        True if the region is already buffered;
-        False if you want buffer the region;
-
     files: List[str]
 
     Attributes
     ----------
     dict_keys: List[str]
 
     key: str
@@ -59,56 +55,53 @@
     def __init__(
         self,
         key=None,
         value=None,
         dict_keys=[],
         place_name="Brasil",
         files=None,
-        radius=None,
+        radius=0,
         geometry_intersected=False,
-        buffered=False,
     ):
         self.key = key
         self.value = value
         self.place_name = place_name
         self.files = files
         self.radius = radius
         self.dict_keys = dict_keys
         self.geometry = geometry_intersected
-        self.buffered = buffered
 
         if self.files is not None:
             read_temp = []
             for file in self.files:
                 read_temp.append(pd.read_csv(file))
             self._df = pd.concat(read_temp)
             self._df["geometry"] = self._df["geometry"].apply(wkt.loads)
             self._df = geopandas.GeoDataFrame(self._df)
         if self.geometry:
             self._df["geometry_intersected"] = self._df.geometry
 
     def _get_polygons(self):
         self.array_polygons = []
-        for index, row in self._df.iterrows():
+        for _, row in self._df.iterrows():
             pol = row["geometry"]
             self.array_polygons.append(pol)
 
         self.idx = rtreeindex.Index()
         for pos, poly in enumerate(self.array_polygons):
             self.idx.insert(pos, poly.bounds)
 
     def _fence_check_local(self, point):
         polygon_metadata = []
-        if self.buffered:
+        if "area_point" in point.keys() and point["area_point"] is not None:
             shp = wkt.loads(point["area_point"])
         elif self.radius is not None:
             shp = geodesic_point_buffer(
                 point["latitude"], point["longitude"], self.radius
             )
-
         else:
             shp = Point(point["longitude"], point["latitude"])
 
         for j in self.idx.intersection(shp.bounds):
             if self.radius is None:
                 if shp.within(shape(self.array_polygons[j])):
                     polygon_metadata.append(self._df.iloc[j].to_frame().T)
@@ -158,33 +151,54 @@
                 for point in points:
                     self._enrich_point(point)
             else:
                 self._enrich_point(points)
 
             yield d
 
-    def enrich_geopandas_data(self, data):
-        data = data.set_crs(epsg=4326).to_crs(epsg=3857)
-        data["geometry"] = data.buffer(self.radius)
-        data = data.to_crs(epsg=4326)
-        self._df = self._df.set_crs(epsg=4326)
-
-        spatial_joined = geopandas.sjoin(
-            data, self._df, how="left", predicate="intersects"
-        )
-        return spatial_joined
-
-    def enrich_dask_geopandas_data(self, data):
-        data = data.set_crs("EPSG:4326").to_crs("EPSG:3857")
-        data["geometry"] = data.buffer(self.radius)
-        data = data.to_crs("EPSG:4326")
+    def _buffer_with_crs(self, data, new_crs=None):
+        if new_crs is None:
+            new_crs = 3857
+
+        if data.crs is None:
+            data = data.set_crs(4326)
+
+        if data.crs != new_crs:
+            data = data.to_crs(new_crs)
+
+        data["geometry_not_buffered"] = data["geometry"]
+        data["geometry"] = data.geometry.buffer(self.radius)
+
+        data = data.to_crs(4326)
+
+        return data
+
+    def enrich_geopandas_data(self, data, **kwargs):
+        data = self._buffer_with_crs(data, kwargs.get("new_crs", None))
+
         self._df = self._df.set_crs("EPSG:4326")
 
-        joined = dask_geopandas.sjoin(data, self._df, predicate="intersects")
-        return joined
+        sj = geopandas.sjoin(data, self._df, how="left", predicate="intersects")
+
+        sj["geometry"] = sj["geometry_not_buffered"]
+        sj.drop(columns=["geometry_not_buffered"], inplace=True)
+
+        return GeopandasData.from_geodataframe(sj)
+
+    def enrich_dask_geopandas_data(self, data, **kwargs):
+        data = self._buffer_with_crs(data, kwargs.get("new_crs", None))
+
+        self._df = self._df.set_crs("EPSG:4326")
+
+        sj = dask_geopandas.sjoin(data, self._df, predicate="intersects")
+
+        sj["geometry"] = sj["geometry_not_buffered"]
+        sj = sj.drop(columns=["geometry_not_buffered"])
+
+        return DaskGeopandasData.from_dask_geodataframe(sj)
 
     def enrich(self, data, **kwargs):
         """Method overrided of interface. This method do enrichment using OSM data as a enricher. It walk through the keys to reach at the data that will be used to intersect the polygons. It uses a R tree to index polygons and search faster. If the radius attribute is passed the algorithm returns all polygons that intersect the point buffered with this radius else the algorithm returns all polygons that contains the point.
 
         Parameters
         ----------
         data: :obj:`Data`
@@ -193,14 +207,14 @@
         if self.files is None and self.key is not None and self.value is not None:
             osm_util = OSM_util()
             self._df = osm_util.get_places(self.place_name, self.key, self.value)
 
         self._get_polygons()
 
         if isinstance(data, GeopandasData):
-            return self.enrich_geopandas_data(data.data)
+            return self.enrich_geopandas_data(data.data, **kwargs)
 
         elif isinstance(data, DaskGeopandasData):
-            return self.enrich_dask_geopandas_data(data.data)
+            return self.enrich_dask_geopandas_data(data.data, **kwargs)
 
         elif isinstance(data, JsonData):
             return self.enrich_json_data(data, **kwargs)
```

### Comparing `moredata-0.1.5/moredata/enricher/sql_connector/sql_connector.py` & `moredata-0.2.0/moredata/enricher/sql_connector/sql_connector.py`

 * *Files identical despite different names*

### Comparing `moredata-0.1.5/moredata/models/data.py` & `moredata-0.2.0/moredata/models/data.py`

 * *Files 26% similar despite different names*

```diff
@@ -33,39 +33,45 @@
 
     def add(self, enricher):
         """add enricher in enrichers attribute"""
         self.enrichers.append(enricher)
 
 
 class GeopandasData(Data):
+    def __init__(self, data):
+        super().__init__()
+        self.data = data
+
     @classmethod
     def from_geodataframe(cls, geodataframe):
-        geopandas_data = GeopandasData()
-        geopandas_data.data = geodataframe
-        return geopandas_data
+        return GeopandasData(geodataframe)
 
     @classmethod
     def from_path(cls, path):
-        geopandas_data = GeopandasData()
-        geopandas_data.data = geopandas.read_file(path)
-        return geopandas_data
+        return GeopandasData(geopandas.read_file(path))
 
 
 class DaskGeopandasData(Data):
+    def __init__(self, data):
+        super().__init__()
+        self.data = data
+
     @classmethod
     def from_geodataframe(cls, geodataframe, npartitions=4):
-        dgd = DaskGeopandasData()
-        dgd.data = dask_geopandas.from_geopandas(geodataframe, npartitions)
-        return dgd
+        return DaskGeopandasData(
+            dask_geopandas.from_geopandas(geodataframe, npartitions)
+        )
+
+    @classmethod
+    def from_dask_geodataframe(cls, dask_geodataframe):
+        return DaskGeopandasData(dask_geodataframe)
 
     @classmethod
     def from_path(cls, path, npartitions=4):
-        dgd = DaskGeopandasData()
-        dgd.data = dask_geopandas.read_file(path, npartitions)
-        return dgd
+        return DaskGeopandasData(dask_geopandas.read_file(path, npartitions))
 
 
 class JsonData(Data):
     def __init__(self, data_file, parser):
         self.data_file = data_file
         self.parser = parser
```

### Comparing `moredata-0.1.5/moredata/parser/__init__.py` & `moredata-0.2.0/moredata/parser/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import csv
 from h3 import h3
 from ..utils import read_json_from_file, load_json
-from shapely.geometry import asPoint
+from shapely.geometry import Point
 from numpy import array
 
 
 def _add_geo_location(doc):
-    doc["geo_location"] = asPoint(array([doc["longitude"], doc["latitude"]])).wkt
+    doc["geo_location"] = Point(array([doc["longitude"], doc["latitude"]])).wkt
     return doc
 
 
 def _add_code_point(doc):
     doc["code_h3"] = h3.geo_to_h3(doc["latitude"], doc["longitude"], 8)
     return doc
```

### Comparing `moredata-0.1.5/moredata/utils/__init__.py` & `moredata-0.2.0/moredata/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `moredata-0.1.5/moredata/utils/osm_downloader.py` & `moredata-0.2.0/moredata/utils/osm_downloader.py`

 * *Files identical despite different names*

### Comparing `moredata-0.1.5/moredata.egg-info/SOURCES.txt` & `moredata-0.2.0/moredata.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 moredata/__init__.py
 moredata.egg-info/PKG-INFO
 moredata.egg-info/SOURCES.txt
 moredata.egg-info/dependency_links.txt
 moredata.egg-info/requires.txt
 moredata.egg-info/top_level.txt
 moredata/datasets/__init__.py
-moredata/datasets/airbnb/airbnb-berlin-extra.csv
-moredata/datasets/airbnb/airbnb-berlin-host.csv
-moredata/datasets/airbnb/airbnb-berlin-main.csv
 moredata/enricher/__init__.py
 moredata/enricher/enricher.py
 moredata/enricher/enricher_builder.py
 moredata/enricher/api_connector/__init__.py
 moredata/enricher/api_connector/api_connector.py
 moredata/enricher/elasticsearch_connector/__init__.py
 moredata/enricher/elasticsearch_connector/elasticsearch_connector.py
```

