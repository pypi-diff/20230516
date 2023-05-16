# Comparing `tmp/crmodel-0.4.2.tar.gz` & `tmp/crmodel-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crmodel-0.4.2.tar", last modified: Fri May 12 13:22:28 2023, max compression
+gzip compressed data, was "crmodel-0.4.3.tar", last modified: Tue May 16 15:09:09 2023, max compression
```

## Comparing `crmodel-0.4.2.tar` & `crmodel-0.4.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-05-12 13:22:28.212648 crmodel-0.4.2/
--rw-r--r--   0 jeremy     (501) staff       (20)    35147 2023-01-16 12:55:21.000000 crmodel-0.4.2/LICENSE
--rw-r--r--   0 jeremy     (501) staff       (20)       63 2023-01-16 12:55:21.000000 crmodel-0.4.2/MANIFEST.in
--rw-r--r--   0 jeremy     (501) staff       (20)     1717 2023-05-12 13:22:28.212494 crmodel-0.4.2/PKG-INFO
--rw-r--r--   0 jeremy     (501) staff       (20)     1111 2023-01-16 12:55:21.000000 crmodel-0.4.2/README.md
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-05-12 13:22:28.211490 crmodel-0.4.2/crmodel/
--rw-r--r--   0 jeremy     (501) staff       (20)     1071 2023-05-12 12:29:12.000000 crmodel-0.4.2/crmodel/config.py
--rw-r--r--   0 jeremy     (501) staff       (20)    18474 2023-05-12 13:20:50.000000 crmodel-0.4.2/crmodel/crmodel.py
--rw-r--r--   0 jeremy     (501) staff       (20)     7859 2023-05-12 13:09:16.000000 crmodel-0.4.2/crmodel/model.py
--rw-r--r--   0 jeremy     (501) staff       (20)     1769 2023-01-16 12:55:21.000000 crmodel-0.4.2/crmodel/segmentationReader.py
--rw-r--r--   0 jeremy     (501) staff       (20)     8394 2023-03-02 21:22:47.000000 crmodel-0.4.2/crmodel/utils.py
-drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-05-12 13:22:28.212292 crmodel-0.4.2/crmodel.egg-info/
--rw-r--r--   0 jeremy     (501) staff       (20)     1717 2023-05-12 13:22:28.000000 crmodel-0.4.2/crmodel.egg-info/PKG-INFO
--rw-r--r--   0 jeremy     (501) staff       (20)      310 2023-05-12 13:22:28.000000 crmodel-0.4.2/crmodel.egg-info/SOURCES.txt
--rw-r--r--   0 jeremy     (501) staff       (20)        1 2023-05-12 13:22:28.000000 crmodel-0.4.2/crmodel.egg-info/dependency_links.txt
--rw-r--r--   0 jeremy     (501) staff       (20)      121 2023-05-12 13:22:28.000000 crmodel-0.4.2/crmodel.egg-info/requires.txt
--rw-r--r--   0 jeremy     (501) staff       (20)        8 2023-05-12 13:22:28.000000 crmodel-0.4.2/crmodel.egg-info/top_level.txt
--rw-r--r--   0 jeremy     (501) staff       (20)      121 2023-05-12 12:16:26.000000 crmodel-0.4.2/requirements.txt
--rw-r--r--   0 jeremy     (501) staff       (20)       38 2023-05-12 13:22:28.212754 crmodel-0.4.2/setup.cfg
--rw-r--r--   0 jeremy     (501) staff       (20)     1092 2023-05-12 13:22:08.000000 crmodel-0.4.2/setup.py
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-05-16 15:09:09.313747 crmodel-0.4.3/
+-rw-r--r--   0 jeremy     (501) staff       (20)    35147 2023-01-16 12:55:21.000000 crmodel-0.4.3/LICENSE
+-rw-r--r--   0 jeremy     (501) staff       (20)       63 2023-01-16 12:55:21.000000 crmodel-0.4.3/MANIFEST.in
+-rw-r--r--   0 jeremy     (501) staff       (20)     1717 2023-05-16 15:09:09.313594 crmodel-0.4.3/PKG-INFO
+-rw-r--r--   0 jeremy     (501) staff       (20)     1111 2023-01-16 12:55:21.000000 crmodel-0.4.3/README.md
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-05-16 15:09:09.310396 crmodel-0.4.3/crmodel/
+-rw-r--r--   0 jeremy     (501) staff       (20)     1071 2023-05-12 12:29:12.000000 crmodel-0.4.3/crmodel/config.py
+-rw-r--r--   0 jeremy     (501) staff       (20)    18474 2023-05-12 13:20:50.000000 crmodel-0.4.3/crmodel/crmodel.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     7941 2023-05-16 14:50:35.000000 crmodel-0.4.3/crmodel/model.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     1769 2023-01-16 12:55:21.000000 crmodel-0.4.3/crmodel/segmentationReader.py
+-rw-r--r--   0 jeremy     (501) staff       (20)     8394 2023-03-02 21:22:47.000000 crmodel-0.4.3/crmodel/utils.py
+drwxr-xr-x   0 jeremy     (501) staff       (20)        0 2023-05-16 15:09:09.312638 crmodel-0.4.3/crmodel.egg-info/
+-rw-r--r--   0 jeremy     (501) staff       (20)     1717 2023-05-16 15:09:09.000000 crmodel-0.4.3/crmodel.egg-info/PKG-INFO
+-rw-r--r--   0 jeremy     (501) staff       (20)      310 2023-05-16 15:09:09.000000 crmodel-0.4.3/crmodel.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)        1 2023-05-16 15:09:09.000000 crmodel-0.4.3/crmodel.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)      121 2023-05-16 15:09:09.000000 crmodel-0.4.3/crmodel.egg-info/requires.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)        8 2023-05-16 15:09:09.000000 crmodel-0.4.3/crmodel.egg-info/top_level.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)      121 2023-05-12 12:16:26.000000 crmodel-0.4.3/requirements.txt
+-rw-r--r--   0 jeremy     (501) staff       (20)       38 2023-05-16 15:09:09.313810 crmodel-0.4.3/setup.cfg
+-rw-r--r--   0 jeremy     (501) staff       (20)     1092 2023-05-16 15:08:26.000000 crmodel-0.4.3/setup.py
```

### Comparing `crmodel-0.4.2/LICENSE` & `crmodel-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `crmodel-0.4.2/PKG-INFO` & `crmodel-0.4.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crmodel
-Version: 0.4.2
+Version: 0.4.3
 Summary: crmodel is a python package that produces the crossroadsdesriber model from OpenStreetMap. See doi.org/10.5194/agile-giss-3-40-2022 for further informations.
 Home-page: https://github.com/jeremyk6/crmodel
 Author: Jérémy Kalsron
 Author-email: jeremy.kalsron@gmail.com  
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crmodel-0.4.2/README.md` & `crmodel-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `crmodel-0.4.2/crmodel/config.py` & `crmodel-0.4.3/crmodel/config.py`

 * *Files identical despite different names*

### Comparing `crmodel-0.4.2/crmodel/crmodel.py` & `crmodel-0.4.3/crmodel/crmodel.py`

 * *Files identical despite different names*

### Comparing `crmodel-0.4.2/crmodel/model.py` & `crmodel-0.4.3/crmodel/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 def createCrosswalk(junction, node):
     # Does it have a tactile paving ?
     cw_tactile_paving = "unknown"
     if "tactile_paving" in node:
         cw_tactile_paving = node["tactile_paving"]
     junction = Crosswalk(junction, cw_tactile_paving, [])
     # Does it have a traffic light ?
-    if node["crossing"] == "traffic_signals":
+    if "crossing" in node and node["crossing"] == "traffic_signals":
         ptl_sound = "unknown"
         # Does it have sound ?
         if "traffic_signals:sound" in node:
             ptl_sound = node["traffic_signals:sound"]
         junction = Pedestrian_traffic_light(junction, ptl_sound)
     return junction
 
@@ -186,15 +186,15 @@
     junction = None
     if node_id in Junction._junctions.keys():
         junction = Junction._junctions[node_id]
     else :
         junction = Junction(node_id, node["x"], node["y"])
             
         # is it a crosswalk ?
-        if "crossing" in node and node["crossing"] != "no":
+        if ("crossing" in node and node["crossing"] != "no") or ("highway" in node and node["highway"] == "crossing"):
             if "foot" not in node or node["foot"] != "no":
                 junction = createCrosswalk(junction, node)
 
         # is it a traffic light ?
         if "traffic_signals" in node:
             junction = createTrafficSignal(junction, node)
```

### Comparing `crmodel-0.4.2/crmodel/segmentationReader.py` & `crmodel-0.4.3/crmodel/segmentationReader.py`

 * *Files identical despite different names*

### Comparing `crmodel-0.4.2/crmodel/utils.py` & `crmodel-0.4.3/crmodel/utils.py`

 * *Files identical despite different names*

### Comparing `crmodel-0.4.2/crmodel.egg-info/PKG-INFO` & `crmodel-0.4.3/crmodel.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crmodel
-Version: 0.4.2
+Version: 0.4.3
 Summary: crmodel is a python package that produces the crossroadsdesriber model from OpenStreetMap. See doi.org/10.5194/agile-giss-3-40-2022 for further informations.
 Home-page: https://github.com/jeremyk6/crmodel
 Author: Jérémy Kalsron
 Author-email: jeremy.kalsron@gmail.com  
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crmodel-0.4.2/setup.py` & `crmodel-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # The requirements file
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 # This call to setup() does all the work
 setup(
     name="crmodel",
-    version="0.4.2",
+    version="0.4.3",
     description="crmodel is a python package that produces the crossroadsdesriber model from OpenStreetMap. See doi.org/10.5194/agile-giss-3-40-2022 for further informations.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/jeremyk6/crmodel",
     author="Jérémy Kalsron",
     author_email="jeremy.kalsron@gmail.com  ",
     license="AGPL-3.0",
```

