# Comparing `tmp/crossroads-schematization-0.0.8.tar.gz` & `tmp/crossroads-schematization-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossroads-schematization-0.0.8.tar", last modified: Tue May 16 13:36:38 2023, max compression
+gzip compressed data, was "crossroads-schematization-0.0.9.tar", last modified: Tue May 16 13:44:59 2023, max compression
```

## Comparing `crossroads-schematization-0.0.8.tar` & `crossroads-schematization-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-05-16 13:36:38.431705 crossroads-schematization-0.0.8/
--rw-r--r--   0 jm        (1000) jm        (1000)      107 2022-11-30 16:15:16.000000 crossroads-schematization-0.0.8/MANIFEST.in
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-05-16 13:36:38.431705 crossroads-schematization-0.0.8/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.0.8/README.md
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-05-16 13:36:38.427705 crossroads-schematization-0.0.8/crossroads_schematization.egg-info/
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-05-16 13:36:38.000000 crossroads-schematization-0.0.8/crossroads_schematization.egg-info/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)      794 2023-05-16 13:36:38.000000 crossroads-schematization-0.0.8/crossroads_schematization.egg-info/SOURCES.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-05-16 13:36:38.000000 crossroads-schematization-0.0.8/crossroads_schematization.egg-info/dependency_links.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-05-16 13:36:38.000000 crossroads-schematization-0.0.8/crossroads_schematization.egg-info/entry_points.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-05-16 13:36:38.000000 crossroads-schematization-0.0.8/crossroads_schematization.egg-info/top_level.txt
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-05-16 13:36:38.431705 crossroads-schematization-0.0.8/crschem/
--rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-05-16 13:34:46.000000 crossroads-schematization-0.0.8/crschem/__init__.py
--rw-r--r--   0 jm        (1000) jm        (1000)     5853 2022-12-02 09:57:06.000000 crossroads-schematization-0.0.8/crschem/cmd.py
--rw-r--r--   0 jm        (1000) jm        (1000)    37904 2023-05-16 13:20:22.000000 crossroads-schematization-0.0.8/crschem/crossroad.py
--rw-r--r--   0 jm        (1000) jm        (1000)    21458 2023-05-16 13:06:22.000000 crossroads-schematization-0.0.8/crschem/crossroad_schematization.py
--rw-r--r--   0 jm        (1000) jm        (1000)     5393 2023-05-12 08:32:50.000000 crossroads-schematization-0.0.8/crschem/processing.py
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-05-16 13:36:38.431705 crossroads-schematization-0.0.8/crschem/resources/
--rw-r--r--   0 jm        (1000) jm        (1000)     2425 2022-10-28 13:53:49.000000 crossroads-schematization-0.0.8/crschem/resources/crossing.svg
--rw-r--r--   0 jm        (1000) jm        (1000)    23130 2023-02-06 15:35:04.000000 crossroads-schematization-0.0.8/crschem/resources/rendering-areas.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    29217 2023-01-16 14:33:05.000000 crossroads-schematization-0.0.8/crschem/resources/rendering-nodes-crossings.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    22244 2023-01-16 15:35:19.000000 crossroads-schematization-0.0.8/crschem/resources/rendering-nodes-islands.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    22752 2023-02-06 15:36:47.000000 crossroads-schematization-0.0.8/crschem/resources/rendering-nodes-space.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    35242 2023-01-16 09:30:00.000000 crossroads-schematization-0.0.8/crschem/resources/rendering-nodes.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    28654 2023-02-06 15:35:25.000000 crossroads-schematization-0.0.8/crschem/resources/rendering-polylines-space.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    28635 2023-01-16 09:29:31.000000 crossroads-schematization-0.0.8/crschem/resources/rendering-polylines.qml
--rw-r--r--   0 jm        (1000) jm        (1000)     7371 2022-11-10 14:22:27.000000 crossroads-schematization-0.0.8/crschem/resources/tactile-a5.qpt
--rw-r--r--   0 jm        (1000) jm        (1000)     7350 2023-05-16 08:27:12.000000 crossroads-schematization-0.0.8/crschem/utils.py
--rw-r--r--   0 jm        (1000) jm        (1000)       36 2023-05-15 13:14:07.000000 crossroads-schematization-0.0.8/requirements.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-05-16 13:36:38.431705 crossroads-schematization-0.0.8/setup.cfg
--rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.0.8/setup.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-05-16 13:44:59.007081 crossroads-schematization-0.0.9/
+-rw-r--r--   0 jm        (1000) jm        (1000)      107 2022-11-30 16:15:16.000000 crossroads-schematization-0.0.9/MANIFEST.in
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-05-16 13:44:59.007081 crossroads-schematization-0.0.9/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.0.9/README.md
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-05-16 13:44:59.003081 crossroads-schematization-0.0.9/crossroads_schematization.egg-info/
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-05-16 13:44:58.000000 crossroads-schematization-0.0.9/crossroads_schematization.egg-info/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)      794 2023-05-16 13:44:58.000000 crossroads-schematization-0.0.9/crossroads_schematization.egg-info/SOURCES.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-05-16 13:44:58.000000 crossroads-schematization-0.0.9/crossroads_schematization.egg-info/dependency_links.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-05-16 13:44:58.000000 crossroads-schematization-0.0.9/crossroads_schematization.egg-info/entry_points.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-05-16 13:44:58.000000 crossroads-schematization-0.0.9/crossroads_schematization.egg-info/top_level.txt
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-05-16 13:44:59.003081 crossroads-schematization-0.0.9/crschem/
+-rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-05-16 13:44:31.000000 crossroads-schematization-0.0.9/crschem/__init__.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     5853 2022-12-02 09:57:06.000000 crossroads-schematization-0.0.9/crschem/cmd.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    37904 2023-05-16 13:20:22.000000 crossroads-schematization-0.0.9/crschem/crossroad.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    21474 2023-05-16 13:43:40.000000 crossroads-schematization-0.0.9/crschem/crossroad_schematization.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     5393 2023-05-12 08:32:50.000000 crossroads-schematization-0.0.9/crschem/processing.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-05-16 13:44:59.007081 crossroads-schematization-0.0.9/crschem/resources/
+-rw-r--r--   0 jm        (1000) jm        (1000)     2425 2022-10-28 13:53:49.000000 crossroads-schematization-0.0.9/crschem/resources/crossing.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)    23130 2023-02-06 15:35:04.000000 crossroads-schematization-0.0.9/crschem/resources/rendering-areas.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    29217 2023-01-16 14:33:05.000000 crossroads-schematization-0.0.9/crschem/resources/rendering-nodes-crossings.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    22244 2023-01-16 15:35:19.000000 crossroads-schematization-0.0.9/crschem/resources/rendering-nodes-islands.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    22752 2023-02-06 15:36:47.000000 crossroads-schematization-0.0.9/crschem/resources/rendering-nodes-space.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    35242 2023-01-16 09:30:00.000000 crossroads-schematization-0.0.9/crschem/resources/rendering-nodes.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    28654 2023-02-06 15:35:25.000000 crossroads-schematization-0.0.9/crschem/resources/rendering-polylines-space.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    28635 2023-01-16 09:29:31.000000 crossroads-schematization-0.0.9/crschem/resources/rendering-polylines.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)     7371 2022-11-10 14:22:27.000000 crossroads-schematization-0.0.9/crschem/resources/tactile-a5.qpt
+-rw-r--r--   0 jm        (1000) jm        (1000)     7350 2023-05-16 08:27:12.000000 crossroads-schematization-0.0.9/crschem/utils.py
+-rw-r--r--   0 jm        (1000) jm        (1000)       36 2023-05-15 13:14:07.000000 crossroads-schematization-0.0.9/requirements.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-05-16 13:44:59.007081 crossroads-schematization-0.0.9/setup.cfg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.0.9/setup.py
```

### Comparing `crossroads-schematization-0.0.8/PKG-INFO` & `crossroads-schematization-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.0.8
+Version: 0.0.9
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.0.8/README.md` & `crossroads-schematization-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.8/crossroads_schematization.egg-info/PKG-INFO` & `crossroads-schematization-0.0.9/crossroads_schematization.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.0.8
+Version: 0.0.9
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.0.8/crossroads_schematization.egg-info/SOURCES.txt` & `crossroads-schematization-0.0.9/crossroads_schematization.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.8/crschem/cmd.py` & `crossroads-schematization-0.0.9/crschem/cmd.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.8/crschem/crossroad.py` & `crossroads-schematization-0.0.9/crschem/crossroad.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.8/crschem/crossroad_schematization.py` & `crossroads-schematization-0.0.9/crschem/crossroad_schematization.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,16 @@
         'traffic_signals',
         'traffic_signals:direction',
         'traffic_signals:sound',
         'button_operated'
         #sidewalk informations
         'kerb',
         #island informations
-        'crossing:island'
+        'crossing:island',
+        'foot'
     ]
 
     # If the OSM data has been previously loaded, do not load it again
     def __init__(self, cr_input, 
                  osm_oriented = None,
                  osm_unoriented = None,
                  osm_buffer_size_meters = 200,
```

### Comparing `crossroads-schematization-0.0.8/crschem/processing.py` & `crossroads-schematization-0.0.9/crschem/processing.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.8/crschem/resources/crossing.svg` & `crossroads-schematization-0.0.9/crschem/resources/crossing.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.8/crschem/resources/rendering-areas.qml` & `crossroads-schematization-0.0.9/crschem/resources/rendering-areas.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.8/crschem/resources/rendering-nodes-crossings.qml` & `crossroads-schematization-0.0.9/crschem/resources/rendering-nodes-crossings.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.8/crschem/resources/rendering-nodes-islands.qml` & `crossroads-schematization-0.0.9/crschem/resources/rendering-nodes-islands.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.8/crschem/resources/rendering-nodes-space.qml` & `crossroads-schematization-0.0.9/crschem/resources/rendering-nodes-space.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.8/crschem/resources/rendering-nodes.qml` & `crossroads-schematization-0.0.9/crschem/resources/rendering-nodes.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.8/crschem/resources/rendering-polylines-space.qml` & `crossroads-schematization-0.0.9/crschem/resources/rendering-polylines-space.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.8/crschem/resources/rendering-polylines.qml` & `crossroads-schematization-0.0.9/crschem/resources/rendering-polylines.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.8/crschem/resources/tactile-a5.qpt` & `crossroads-schematization-0.0.9/crschem/resources/tactile-a5.qpt`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.8/crschem/utils.py` & `crossroads-schematization-0.0.9/crschem/utils.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.0.8/setup.py` & `crossroads-schematization-0.0.9/setup.py`

 * *Files identical despite different names*

