# Comparing `tmp/coolpandas-0.2.2.tar.gz` & `tmp/coolpandas-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolpandas-0.2.2.tar", last modified: Tue Nov 22 21:42:23 2022, max compression
+gzip compressed data, was "coolpandas-0.3.0.tar", last modified: Tue May 16 10:28:05 2023, max compression
```

## Comparing `coolpandas-0.2.2.tar` & `coolpandas-0.3.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 21:42:23.783657 coolpandas-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2022-11-22 21:42:13.000000 coolpandas-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1389 2022-11-22 21:42:23.783657 coolpandas-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      560 2022-11-22 21:42:13.000000 coolpandas-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 21:42:23.779657 coolpandas-0.2.2/coolpandas/
--rw-r--r--   0 runner    (1001) docker     (122)       90 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 21:42:23.779657 coolpandas-0.2.2/coolpandas/eda/
--rw-r--r--   0 runner    (1001) docker     (122)      599 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/eda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1083 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/eda/correlation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4067 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/eda/distribution.py
--rw-r--r--   0 runner    (1001) docker     (122)     2181 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/eda/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2614 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/eda/features_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     4604 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/eda/geo_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/eda/missing_values.py
--rw-r--r--   0 runner    (1001) docker     (122)      336 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/eda/random_state.py
--rw-r--r--   0 runner    (1001) docker     (122)      967 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/eda/shape.py
--rw-r--r--   0 runner    (1001) docker     (122)      692 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/eda/summary.py
--rw-r--r--   0 runner    (1001) docker     (122)     2471 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/eda/value_counts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 21:42:23.783657 coolpandas-0.2.2/coolpandas/evaluate/
--rw-r--r--   0 runner    (1001) docker     (122)       91 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1578 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/evaluate/confusion_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 21:42:23.783657 coolpandas-0.2.2/coolpandas/plot/
--rw-r--r--   0 runner    (1001) docker     (122)      152 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1002 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/plot/barplot.py
--rw-r--r--   0 runner    (1001) docker     (122)     1052 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/plot/distplot.py
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/plot/geoplot.py
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/plot/mapplot.py
--rw-r--r--   0 runner    (1001) docker     (122)     1255 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/plot/style.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 21:42:23.783657 coolpandas-0.2.2/coolpandas/transform/
--rw-r--r--   0 runner    (1001) docker     (122)      184 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      713 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/transform/bin.py
--rw-r--r--   0 runner    (1001) docker     (122)      461 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/transform/epoch.py
--rw-r--r--   0 runner    (1001) docker     (122)      593 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/transform/missing_values.py
--rw-r--r--   0 runner    (1001) docker     (122)     1762 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/transform/outliers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 21:42:23.783657 coolpandas-0.2.2/coolpandas/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      336 2022-11-22 21:42:13.000000 coolpandas-0.2.2/coolpandas/utils/random_state.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 21:42:23.779657 coolpandas-0.2.2/coolpandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1389 2022-11-22 21:42:23.000000 coolpandas-0.2.2/coolpandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2022-11-22 21:42:23.000000 coolpandas-0.2.2/coolpandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-22 21:42:23.000000 coolpandas-0.2.2/coolpandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      198 2022-11-22 21:42:23.000000 coolpandas-0.2.2/coolpandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2022-11-22 21:42:23.000000 coolpandas-0.2.2/coolpandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1543 2022-11-22 21:42:13.000000 coolpandas-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-22 21:42:23.783657 coolpandas-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:28:05.200110 coolpandas-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-16 10:27:55.000000 coolpandas-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-16 10:28:05.200110 coolpandas-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-16 10:27:55.000000 coolpandas-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:28:05.196109 coolpandas-0.3.0/coolpandas/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:28:05.196109 coolpandas-0.3.0/coolpandas/eda/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/eda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/eda/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/eda/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/eda/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/eda/features_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/eda/geo_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/eda/missing_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/eda/random_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/eda/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/eda/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/eda/value_counts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:28:05.196109 coolpandas-0.3.0/coolpandas/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/evaluate/confusion_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:28:05.196109 coolpandas-0.3.0/coolpandas/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/plot/barplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/plot/distplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/plot/geoplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/plot/lineplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/plot/mapplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/plot/style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:28:05.200110 coolpandas-0.3.0/coolpandas/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/transform/bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/transform/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/transform/missing_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/transform/outliers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:28:05.200110 coolpandas-0.3.0/coolpandas/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-16 10:27:55.000000 coolpandas-0.3.0/coolpandas/utils/random_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:28:05.196109 coolpandas-0.3.0/coolpandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-16 10:28:05.000000 coolpandas-0.3.0/coolpandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-16 10:28:05.000000 coolpandas-0.3.0/coolpandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 10:28:05.000000 coolpandas-0.3.0/coolpandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-16 10:28:05.000000 coolpandas-0.3.0/coolpandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-16 10:28:05.000000 coolpandas-0.3.0/coolpandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-16 10:27:55.000000 coolpandas-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 10:28:05.200110 coolpandas-0.3.0/setup.cfg
```

### Comparing `coolpandas-0.2.2/LICENSE` & `coolpandas-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coolpandas-0.2.2/PKG-INFO` & `coolpandas-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coolpandas
-Version: 0.2.2
+Version: 0.3.0
 Summary: A Python package for Exploratory Data Analysis.
 Author-email: Avel Docquin <adocquin@outlook.com>
 Project-URL: Homepage, https://github.com/adocquin/coolpandas
 Project-URL: Bug Tracker, https://github.com/adocquin/coolpandas/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `coolpandas-0.2.2/README.md` & `coolpandas-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `coolpandas-0.2.2/coolpandas/eda/__init__.py` & `coolpandas-0.3.0/coolpandas/eda/__init__.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.2.2/coolpandas/eda/correlation.py` & `coolpandas-0.3.0/coolpandas/eda/correlation.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.2.2/coolpandas/eda/distribution.py` & `coolpandas-0.3.0/coolpandas/eda/distribution.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.2.2/coolpandas/eda/features_type.py` & `coolpandas-0.3.0/coolpandas/eda/features_type.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.2.2/coolpandas/eda/geo_distance.py` & `coolpandas-0.3.0/coolpandas/eda/geo_distance.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.2.2/coolpandas/eda/missing_values.py` & `coolpandas-0.3.0/coolpandas/eda/missing_values.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.2.2/coolpandas/eda/shape.py` & `coolpandas-0.3.0/coolpandas/eda/shape.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.2.2/coolpandas/eda/summary.py` & `coolpandas-0.3.0/coolpandas/eda/summary.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.2.2/coolpandas/eda/value_counts.py` & `coolpandas-0.3.0/coolpandas/eda/value_counts.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.2.2/coolpandas/evaluate/confusion_matrix.py` & `coolpandas-0.3.0/coolpandas/evaluate/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.2.2/coolpandas/plot/barplot.py` & `coolpandas-0.3.0/coolpandas/plot/barplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.2.2/coolpandas/plot/distplot.py` & `coolpandas-0.3.0/coolpandas/plot/distplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.2.2/coolpandas/plot/geoplot.py` & `coolpandas-0.3.0/coolpandas/plot/geoplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.2.2/coolpandas/plot/mapplot.py` & `coolpandas-0.3.0/coolpandas/plot/mapplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.2.2/coolpandas/plot/style.py` & `coolpandas-0.3.0/coolpandas/plot/style.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.2.2/coolpandas/transform/bin.py` & `coolpandas-0.3.0/coolpandas/transform/bin.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.2.2/coolpandas/transform/missing_values.py` & `coolpandas-0.3.0/coolpandas/transform/missing_values.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.2.2/coolpandas/transform/outliers.py` & `coolpandas-0.3.0/coolpandas/transform/outliers.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.2.2/coolpandas.egg-info/PKG-INFO` & `coolpandas-0.3.0/coolpandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coolpandas
-Version: 0.2.2
+Version: 0.3.0
 Summary: A Python package for Exploratory Data Analysis.
 Author-email: Avel Docquin <adocquin@outlook.com>
 Project-URL: Homepage, https://github.com/adocquin/coolpandas
 Project-URL: Bug Tracker, https://github.com/adocquin/coolpandas/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `coolpandas-0.2.2/coolpandas.egg-info/SOURCES.txt` & `coolpandas-0.3.0/coolpandas.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 coolpandas/eda/value_counts.py
 coolpandas/evaluate/__init__.py
 coolpandas/evaluate/confusion_matrix.py
 coolpandas/plot/__init__.py
 coolpandas/plot/barplot.py
 coolpandas/plot/distplot.py
 coolpandas/plot/geoplot.py
+coolpandas/plot/lineplot.py
 coolpandas/plot/mapplot.py
 coolpandas/plot/style.py
 coolpandas/transform/__init__.py
 coolpandas/transform/bin.py
 coolpandas/transform/epoch.py
 coolpandas/transform/missing_values.py
 coolpandas/transform/outliers.py
```

### Comparing `coolpandas-0.2.2/pyproject.toml` & `coolpandas-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coolpandas"
-version = "0.2.2"
+version = "0.3.0"
 authors = [
   { name="Avel Docquin", email="adocquin@outlook.com" },
   ]
 description = "A Python package for Exploratory Data Analysis."
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

