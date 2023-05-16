# Comparing `tmp/ecoengine-0.0.4.tar.gz` & `tmp/ecoengine-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoengine-0.0.4.tar", last modified: Wed Apr 19 19:39:24 2023, max compression
+gzip compressed data, was "ecoengine-0.0.5.tar", last modified: Tue May 16 20:16:06 2023, max compression
```

## Comparing `ecoengine-0.0.4.tar` & `ecoengine-0.0.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:24.928132 ecoengine-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-19 19:38:51.000000 ecoengine-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-19 19:39:24.928132 ecoengine-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-19 19:38:51.000000 ecoengine-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-19 19:38:51.000000 ecoengine-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-19 19:39:24.932132 ecoengine-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-19 19:38:51.000000 ecoengine-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:24.916132 ecoengine-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:24.920132 ecoengine-0.0.4/src/ecoengine/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:24.920132 ecoengine-0.0.4/src/ecoengine/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/constants/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:24.920132 ecoengine-0.0.4/src/ecoengine/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:24.924131 ecoengine-0.0.4/src/ecoengine/data/load_shapes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/apartment.json
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/elementary_school.json
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/food_service_a.json
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/food_service_b.json
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/junior_high.json
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/mens_dorm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/motel.json
--rw-r--r--   0 runner    (1001) docker     (123)    47218 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/multi_family.json
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/nursing_home.json
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/office_building.json
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/senior_high.json
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/womens_dorm.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:24.928132 ecoengine-0.0.4/src/ecoengine/engine/
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/engine/BuildingCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/engine/EcosizerEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/engine/SystemCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:24.928132 ecoengine-0.0.4/src/ecoengine/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/objects/Building.py
--rw-r--r--   0 runner    (1001) docker     (123)    23618 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/objects/SystemConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/objects/systemConfigUtils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:24.928132 ecoengine-0.0.4/src/ecoengine/objects/systems/
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/objects/systems/ParallelLoopTank.py
--rw-r--r--   0 runner    (1001) docker     (123)    16890 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/objects/systems/SwingTank.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/objects/systems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:24.920132 ecoengine-0.0.4/src/ecoengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-19 19:39:24.000000 ecoengine-0.0.4/src/ecoengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-19 19:39:24.000000 ecoengine-0.0.4/src/ecoengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:39:24.000000 ecoengine-0.0.4/src/ecoengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-19 19:39:24.000000 ecoengine-0.0.4/src/ecoengine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 19:39:24.000000 ecoengine-0.0.4/src/ecoengine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:16:06.776467 ecoengine-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-16 20:15:31.000000 ecoengine-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-16 20:16:06.776467 ecoengine-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-16 20:15:31.000000 ecoengine-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 20:15:31.000000 ecoengine-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-16 20:16:06.776467 ecoengine-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 20:15:31.000000 ecoengine-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:16:06.768467 ecoengine-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:16:06.772467 ecoengine-0.0.5/src/ecoengine/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:16:06.772467 ecoengine-0.0.5/src/ecoengine/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/constants/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:16:06.772467 ecoengine-0.0.5/src/ecoengine/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:16:06.772467 ecoengine-0.0.5/src/ecoengine/data/load_shapes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/apartment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/elementary_school.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/food_service_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/food_service_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/junior_high.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/mens_dorm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/motel.json
+-rw-r--r--   0 runner    (1001) docker     (123)    47218 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/multi_family.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/nursing_home.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/office_building.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/senior_high.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/data/load_shapes/womens_dorm.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:16:06.772467 ecoengine-0.0.5/src/ecoengine/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/engine/BuildingCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/engine/EcosizerEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/engine/SystemCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:16:06.772467 ecoengine-0.0.5/src/ecoengine/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/objects/Building.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23658 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/objects/SystemConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/objects/systemConfigUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:16:06.772467 ecoengine-0.0.5/src/ecoengine/objects/systems/
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/objects/systems/ParallelLoopTank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/objects/systems/SwingTank.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 20:15:31.000000 ecoengine-0.0.5/src/ecoengine/objects/systems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:16:06.772467 ecoengine-0.0.5/src/ecoengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-16 20:16:06.000000 ecoengine-0.0.5/src/ecoengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-16 20:16:06.000000 ecoengine-0.0.5/src/ecoengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:16:06.000000 ecoengine-0.0.5/src/ecoengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-16 20:16:06.000000 ecoengine-0.0.5/src/ecoengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 20:16:06.000000 ecoengine-0.0.5/src/ecoengine.egg-info/top_level.txt
```

### Comparing `ecoengine-0.0.4/PKG-INFO` & `ecoengine-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoengine
-Version: 0.0.4
+Version: 0.0.5
 Summary: A software for sizing Heat Pump Water Heaters for buildings
 Home-page: https://ecosizer.ecotope.com/sizer/
 Author: Nolan
 Author-email: nolan@ecotope.com
 Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecoengine-0.0.4/README.md` & `ecoengine-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.4/setup.cfg` & `ecoengine-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ecoengine
-version = 0.0.4
+version = 0.0.5
 author = Nolan
 author_email = nolan@ecotope.com
 description = A software for sizing Heat Pump Water Heaters for buildings
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://ecosizer.ecotope.com/sizer/
 project_urls =
```

### Comparing `ecoengine-0.0.4/src/ecoengine/__init__.py` & `ecoengine-0.0.5/src/ecoengine/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.4/src/ecoengine/data/load_shapes/apartment.json` & `ecoengine-0.0.5/src/ecoengine/data/load_shapes/apartment.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.4/src/ecoengine/data/load_shapes/elementary_school.json` & `ecoengine-0.0.5/src/ecoengine/data/load_shapes/elementary_school.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.4/src/ecoengine/data/load_shapes/food_service_a.json` & `ecoengine-0.0.5/src/ecoengine/data/load_shapes/food_service_a.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.4/src/ecoengine/data/load_shapes/food_service_b.json` & `ecoengine-0.0.5/src/ecoengine/data/load_shapes/food_service_b.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.4/src/ecoengine/data/load_shapes/junior_high.json` & `ecoengine-0.0.5/src/ecoengine/data/load_shapes/junior_high.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.4/src/ecoengine/data/load_shapes/mens_dorm.json` & `ecoengine-0.0.5/src/ecoengine/data/load_shapes/mens_dorm.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.4/src/ecoengine/data/load_shapes/motel.json` & `ecoengine-0.0.5/src/ecoengine/data/load_shapes/motel.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.4/src/ecoengine/data/load_shapes/multi_family.json` & `ecoengine-0.0.5/src/ecoengine/data/load_shapes/multi_family.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.4/src/ecoengine/data/load_shapes/nursing_home.json` & `ecoengine-0.0.5/src/ecoengine/data/load_shapes/nursing_home.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.4/src/ecoengine/data/load_shapes/office_building.json` & `ecoengine-0.0.5/src/ecoengine/data/load_shapes/office_building.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.4/src/ecoengine/data/load_shapes/senior_high.json` & `ecoengine-0.0.5/src/ecoengine/data/load_shapes/senior_high.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.4/src/ecoengine/data/load_shapes/womens_dorm.json` & `ecoengine-0.0.5/src/ecoengine/data/load_shapes/womens_dorm.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.4/src/ecoengine/engine/BuildingCreator.py` & `ecoengine-0.0.5/src/ecoengine/engine/BuildingCreator.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.4/src/ecoengine/engine/EcosizerEngine.py` & `ecoengine-0.0.5/src/ecoengine/engine/EcosizerEngine.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     def getSizingResults(self):
         """
         Returns the minimum primary volume and heating capacity sizing results
 
         Returns
         -------
         list
-            self.PVol_G_atStorageT, self.PCap_kBTUhr (also self.TMVol_G, self.TMCap_kBTUhr if there is a TM system)
+            self.PVol_G_atStorageT, self.PCap_kBTUhr (also self.TMVol_G, self.TMCap_kBTUhr if there is a TM system and self.CA_TMVol_G if SwingTank)
         """
         return self.system.getSizingResults()
 
     def primaryCurve(self):
         """
         Sizes the primary system curve. Will catch the point at which the aquatstat
         fraction is too small for system and cuts the return arrays to match cutoff point.
```

### Comparing `ecoengine-0.0.4/src/ecoengine/engine/SystemCreator.py` & `ecoengine-0.0.5/src/ecoengine/engine/SystemCreator.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.4/src/ecoengine/engine/__init__.py` & `ecoengine-0.0.5/src/ecoengine/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.4/src/ecoengine/objects/Building.py` & `ecoengine-0.0.5/src/ecoengine/objects/Building.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.4/src/ecoengine/objects/SystemConfig.py` & `ecoengine-0.0.5/src/ecoengine/objects/SystemConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
 
         # To per minute from per hour
         G_hw = np.array(hrToMinList(G_hw)) / 60
         D_hw = np.array(hrToMinList(D_hw)) / 60
 
         # Init the "simulation"
         V0 = np.ceil(Pvolume * self.percentUseable)
-        Vtrig = np.ceil(Pvolume * (1 - self.aquaFract)) + 1 # To prevent negatives with any of that rounding math.
+        Vtrig = np.ceil(Pvolume * (1 - self.aquaFract)) + 1 # To prevent negatives with any of that rounding math. TODO Nolan is sus of that +1
         pV = [V0] + [0] * (len(G_hw) - 1)
 
         pheating = False
 
         return G_hw, D_hw, V0, Vtrig, pV, pheating
     
     def _setLoadShift(self, loadShiftSchedule, loadShiftPercent=1):
@@ -437,15 +437,15 @@
         if pheating:
             Vnew = Vcurr + hw_in - hw_out # If heating, generate HW and lose HW
             did_run = hw_in
 
         else:  # Else not heating,
             Vnew = Vcurr - hw_out # So lose HW
             if Vnew < Vtrig: # If should heat
-                time_missed = (Vtrig - Vnew)/hw_out # Volume below turn on / rate of draw gives time below tigger
+                time_missed = (Vtrig - Vnew)/hw_out # Volume below turn on / rate of draw gives time below tigger (aquastat)
                 Vnew += hw_in * time_missed # Start heating
                 did_run = hw_in * time_missed
                 pheating = True
 
         if Vnew > V0: # If overflow
             time_over = (Vnew - V0) / (hw_in - hw_out) # Volume over generated / rate of generation gives time above full
             Vnew = V0 - hw_out * time_over # Make full with missing volume
```

### Comparing `ecoengine-0.0.4/src/ecoengine/objects/__init__.py` & `ecoengine-0.0.5/src/ecoengine/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.4/src/ecoengine/objects/systemConfigUtils.py` & `ecoengine-0.0.5/src/ecoengine/objects/systemConfigUtils.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.4/src/ecoengine/objects/systems/ParallelLoopTank.py` & `ecoengine-0.0.5/src/ecoengine/objects/systems/ParallelLoopTank.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.4/src/ecoengine/objects/systems/SwingTank.py` & `ecoengine-0.0.5/src/ecoengine/objects/systems/SwingTank.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from plotly.subplots import make_subplots
 
 class SwingTank(SystemConfig):
 
     #Assuming that these swing sizing methodologies will be dropped in next code cycle so they likely can be removed, it not we will need to implement additional swing sizing
     Table_Napts = [0, 12, 24, 48, 96]
     sizingTable = [40, 50, 80, 100, 120, 160, 175, 240, 350] #multiples of standard tank sizes
+    sizingTable_CA = [80, 96, 168, 288, 480]
 
     def __init__(self, safetyTM, building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract,
                  doLoadShift = False, loadShiftPercent = 1, loadShiftSchedule = None):
         # check Saftey factor
         if not (isinstance(safetyTM, float) or isinstance(safetyTM, int)) or safetyTM <= 1.:
             raise Exception("The saftey factor for the temperature maintenance system must be greater than 1 or the system will never keep up with the losses.")
         # check building because recirc losses needed before super().__init__()
@@ -23,30 +24,31 @@
             raise Exception("Error: Building is not valid.")
         #check if recirc losses require tank larger than 350 gallons
         if building.recirc_loss / (watt_per_gal_recirc_factor * W_TO_BTUHR) > max(self.sizingTable):
             raise Exception("Recirculation losses are too high, consider using multiple central plants.")
 
         self.safetyTM = safetyTM
         self.TMVol_G = min([x for x in self.sizingTable if x >= (building.recirc_loss / (watt_per_gal_recirc_factor * W_TO_BTUHR))])
+        self.CA_TMVol_G = min([x for x in self.sizingTable_CA if x >= (building.recirc_loss / (watt_per_gal_recirc_factor * W_TO_BTUHR))])
         self.element_deadband_F = 8.
         self.TMCap_kBTUhr = self.safetyTM * building.recirc_loss / 1000.
         
         super().__init__(building, storageT_F, defrostFactor, percentUseable, compRuntime_hr, aquaFract, 
                  doLoadShift, loadShiftPercent, loadShiftSchedule)
     
     def getSizingResults(self):
         """
         Returns the minimum primary volume and heating capacity sizing results
 
         Returns
         -------
         list
-            self.PVol_G_atStorageT, self.PCap_kBTUhr, self.TMVol_G, self.TMCap_kBTUhr
+            self.PVol_G_atStorageT, self.PCap_kBTUhr, self.TMVol_G, self.TMCap_kBTUhr, self.CA_TMVol_G
         """
-        return [self.PVol_G_atStorageT, self.PCap_kBTUhr, self.TMVol_G, self.TMCap_kBTUhr]
+        return [self.PVol_G_atStorageT, self.PCap_kBTUhr, self.TMVol_G, self.TMCap_kBTUhr, self.CA_TMVol_G]
     
     def _calcRunningVol(self, heatHrs, onOffArr, loadshape, effMixFract = 0.):
         """
         Function to find the running volume for the hot water storage tank, which
         is needed for calculating the total volume for primary sizing and in the event of load shift sizing
         represents the entire volume.
```

### Comparing `ecoengine-0.0.4/src/ecoengine.egg-info/PKG-INFO` & `ecoengine-0.0.5/src/ecoengine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoengine
-Version: 0.0.4
+Version: 0.0.5
 Summary: A software for sizing Heat Pump Water Heaters for buildings
 Home-page: https://ecosizer.ecotope.com/sizer/
 Author: Nolan
 Author-email: nolan@ecotope.com
 Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecoengine-0.0.4/src/ecoengine.egg-info/SOURCES.txt` & `ecoengine-0.0.5/src/ecoengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

