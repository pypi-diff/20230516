# Comparing `tmp/geci-nerd-0.3.1.tar.gz` & `tmp/geci-nerd-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geci-nerd-0.3.1.tar", last modified: Thu Mar  3 22:46:26 2022, max compression
+gzip compressed data, was "geci-nerd-0.4.0.tar", last modified: Tue May 16 00:50:39 2023, max compression
```

## Comparing `geci-nerd-0.3.1.tar` & `geci-nerd-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 22:46:26.442128 geci-nerd-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-03-03 22:29:34.000000 geci-nerd-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-03-03 22:46:26.442128 geci-nerd-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1775 2022-03-03 22:29:34.000000 geci-nerd-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 22:46:26.438128 geci-nerd-0.3.1/geci_nerd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-03-03 22:46:26.000000 geci-nerd-0.3.1/geci_nerd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-03-03 22:46:26.000000 geci-nerd-0.3.1/geci_nerd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-03 22:46:26.000000 geci-nerd-0.3.1/geci_nerd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-03-03 22:46:26.000000 geci-nerd-0.3.1/geci_nerd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-03-03 22:46:26.000000 geci-nerd-0.3.1/geci_nerd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 22:46:26.438128 geci-nerd-0.3.1/nerd/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-03-03 22:29:34.000000 geci-nerd-0.3.1/nerd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 22:46:26.442128 geci-nerd-0.3.1/nerd/calibration/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-03-03 22:29:34.000000 geci-nerd-0.3.1/nerd/calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2022-03-03 22:29:34.000000 geci-nerd-0.3.1/nerd/calibration/best_density_function.py
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-03-03 22:29:34.000000 geci-nerd-0.3.1/nerd/calibration/fit_flow_rate.py
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-03-03 22:29:34.000000 geci-nerd-0.3.1/nerd/calibration/get_swath_width.py
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-03-03 22:29:34.000000 geci-nerd-0.3.1/nerd/calibration/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1018 2022-03-03 22:29:34.000000 geci-nerd-0.3.1/nerd/calibration/rmse.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 22:46:26.442128 geci-nerd-0.3.1/nerd/density_functions/
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-03-03 22:29:34.000000 geci-nerd-0.3.1/nerd/density_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-03-03 22:29:34.000000 geci-nerd-0.3.1/nerd/density_functions/density_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 22:46:26.442128 geci-nerd-0.3.1/nerd/io/
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2022-03-03 22:29:34.000000 geci-nerd-0.3.1/nerd/io/Nerd.py
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-03-03 22:29:34.000000 geci-nerd-0.3.1/nerd/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-03-03 22:29:34.000000 geci-nerd-0.3.1/nerd/io/geo2utm.py
--rw-r--r--   0 runner    (1001) docker     (121)     2290 2022-03-03 22:29:34.000000 geci-nerd-0.3.1/nerd/io/import_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-03 22:46:26.442128 geci-nerd-0.3.1/nerd/mapping/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-03-03 22:29:34.000000 geci-nerd-0.3.1/nerd/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9496 2022-03-03 22:29:34.000000 geci-nerd-0.3.1/nerd/mapping/tiling.py
--rw-r--r--   0 runner    (1001) docker     (121)     1593 2022-03-03 22:29:34.000000 geci-nerd-0.3.1/nerd/solver.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-03 22:46:26.442128 geci-nerd-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-03-03 22:29:34.000000 geci-nerd-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:50:39.291138 geci-nerd-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-16 00:50:39.291138 geci-nerd-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:50:39.283137 geci-nerd-0.4.0/geci_nerd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-16 00:50:39.000000 geci-nerd-0.4.0/geci_nerd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-16 00:50:39.000000 geci-nerd-0.4.0/geci_nerd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:50:39.000000 geci-nerd-0.4.0/geci_nerd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-16 00:50:39.000000 geci-nerd-0.4.0/geci_nerd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-16 00:50:39.000000 geci-nerd-0.4.0/geci_nerd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:50:39.283137 geci-nerd-0.4.0/nerd/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/nerd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:50:39.287137 geci-nerd-0.4.0/nerd/calibration/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/nerd/calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/nerd/calibration/best_density_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/nerd/calibration/fit_flow_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/nerd/calibration/get_swath_width.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/nerd/calibration/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/nerd/calibration/rmse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:50:39.287137 geci-nerd-0.4.0/nerd/density_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/nerd/density_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/nerd/density_functions/density_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:50:39.287137 geci-nerd-0.4.0/nerd/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/nerd/io/Nerd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/nerd/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/nerd/io/geo2utm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/nerd/io/import_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:50:39.287137 geci-nerd-0.4.0/nerd/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/nerd/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/nerd/mapping/tiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/nerd/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 00:50:39.291138 geci-nerd-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:50:39.291138 geci-nerd-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/tests/test_blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/tests/test_fit_flow_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/tests/test_geo2utm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/tests/test_import_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15541 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/tests/test_nerd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/tests/test_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/tests/test_triangular.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-16 00:31:42.000000 geci-nerd-0.4.0/tests/test_uniform.py
```

### Comparing `geci-nerd-0.3.1/LICENSE` & `geci-nerd-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geci-nerd-0.3.1/PKG-INFO` & `geci-nerd-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 Metadata-Version: 2.1
 Name: geci-nerd
-Version: 0.3.1
+Version: 0.4.0
 Summary: Numerical Estimation of Rodenticide Density (NERD)
 Home-page: https://github.com/IslasGECI/nerd
 Author: Ciencia de Datos • GECI
 Author-email: ciencia.datos@islas.org.mx
-License: UNKNOWN
-Platform: UNKNOWN
 License-File: LICENSE
 
 The eradication of rodents is central to island conservation efforts and the aerial broadcast of rodenticide bait is the preferred dispersal method. To improve accuracy and expedite the evaluation of aerial operations, we developed an algorithm for the numerical estimation of rodenticide density (NERD). The NERD algorithm performs calculations with increased accuracy, displaying results almost in real-time. NERD describes the relationship between bait density, the mass flow rate of rodenticide through the bait bucket, and helicopter speed and produces maps of bait density on the ground. NERD also facilitates the planning of helicopter flight paths and allows for the instant identification of areas with low or high bait density.
-
```

### Comparing `geci-nerd-0.3.1/geci_nerd.egg-info/PKG-INFO` & `geci-nerd-0.4.0/geci_nerd.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 Metadata-Version: 2.1
 Name: geci-nerd
-Version: 0.3.1
+Version: 0.4.0
 Summary: Numerical Estimation of Rodenticide Density (NERD)
 Home-page: https://github.com/IslasGECI/nerd
 Author: Ciencia de Datos • GECI
 Author-email: ciencia.datos@islas.org.mx
-License: UNKNOWN
-Platform: UNKNOWN
 License-File: LICENSE
 
 The eradication of rodents is central to island conservation efforts and the aerial broadcast of rodenticide bait is the preferred dispersal method. To improve accuracy and expedite the evaluation of aerial operations, we developed an algorithm for the numerical estimation of rodenticide density (NERD). The NERD algorithm performs calculations with increased accuracy, displaying results almost in real-time. NERD describes the relationship between bait density, the mass flow rate of rodenticide through the bait bucket, and helicopter speed and produces maps of bait density on the ground. NERD also facilitates the planning of helicopter flight paths and allows for the instant identification of areas with low or high bait density.
-
```

### Comparing `geci-nerd-0.3.1/nerd/calibration/best_density_function.py` & `geci-nerd-0.4.0/nerd/calibration/best_density_function.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 import inspect
 import numpy as np
 from . import get_rmse_from_function_array
 from .. import density_functions as df
 
 
 def get_density_functions_array():
-    return [
-        getattr(df, elemento) for elemento in dir(df) if inspect.isfunction(getattr(df, elemento))
-    ]
+    return [getattr(df, element) for element in dir(df) if inspect.isfunction(getattr(df, element))]
 
 
 def select_best_density_function_from_array(
     distance,
     density,
     aperture_diameter_data,
     helicopter_speed_data,
@@ -25,16 +23,16 @@
         density,
         aperture_diameter_data,
         helicopter_speed_data,
         swath_width,
         density_functions,
         flow_rate_function,
     )
-    es_mejor_funcion = rmse == rmse.min()
-    return density_functions[np.where(es_mejor_funcion)[0][0]]
+    is_better_function = rmse == rmse.min()
+    return density_functions[np.where(is_better_function)[0][0]]
 
 
 def get_best_density_function(
     distance: np.array,
     density: np.array,
     aperture_diameter_data: float,
     helicopter_speed_data: float,
```

### Comparing `geci-nerd-0.3.1/nerd/calibration/fit_flow_rate.py` & `geci-nerd-0.4.0/nerd/calibration/fit_flow_rate.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,9 +6,9 @@
     """
     Fit quadratic model for flow rate (kg/s) as a function of aperture diameter (mm)
     :param aperture_diameters: Array of diameters of the bucket aperture in
         millimetres (mm)
     :param flow_rates: Array of mass flow rate of bait in kg per second (kg/s)
     :return: Function of mass flow rate with respect to aperture diameter
     """
-    coeficientes = np.polyfit(aperture_diameters, flow_rates, 2)
-    return np.poly1d(coeficientes)
+    coeficients = np.polyfit(aperture_diameters, flow_rates, 2)
+    return np.poly1d(coeficients)
```

### Comparing `geci-nerd-0.3.1/nerd/calibration/get_swath_width.py` & `geci-nerd-0.4.0/nerd/calibration/get_swath_width.py`

 * *Files identical despite different names*

### Comparing `geci-nerd-0.3.1/nerd/calibration/model.py` & `geci-nerd-0.4.0/nerd/calibration/model.py`

 * *Files identical despite different names*

### Comparing `geci-nerd-0.3.1/nerd/calibration/rmse.py` & `geci-nerd-0.4.0/nerd/calibration/rmse.py`

 * *Files identical despite different names*

### Comparing `geci-nerd-0.3.1/nerd/density_functions/density_functions.py` & `geci-nerd-0.4.0/nerd/density_functions/density_functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,29 +5,29 @@
     """
     Uniform distribution for density profiles
     :param distance: Distance from flight path
     :param width: Swath width
     :param parameter: Free parameter to be fitted
     :return:
     """
-    es_dentro = np.abs(distance) < width / 2
-    return np.double(es_dentro) * parameter
+    is_inside = np.abs(distance) < width / 2
+    return np.double(is_inside) * parameter
 
 
 def triangular(distance: float, width: float, parameter: float) -> float:
     """
     Triangular distribution for density profiles
     :param distance: Distance from flight path
     :param width: Swath width
     :param parameter: Free parameter to be fitted
     :return:
     """
     slope = -2 * parameter / width
-    es_dentro = np.abs(distance) < width / 2  # pragma: no mutate
-    return (slope * np.abs(distance) + parameter) * np.double(es_dentro)
+    is_inside = np.abs(distance) < width / 2  # pragma: no mutate
+    return (slope * np.abs(distance) + parameter) * np.double(is_inside)
 
 
 def normal(distance: float, width: float, parameter: float) -> float:
     """
     Normal distribution for density profiles
     :param distance: Distance from flight path
     :param width: Swath width
```

### Comparing `geci-nerd-0.3.1/nerd/io/Nerd.py` & `geci-nerd-0.4.0/nerd/io/Nerd.py`

 * *Files identical despite different names*

### Comparing `geci-nerd-0.3.1/nerd/io/import_data.py` & `geci-nerd-0.4.0/nerd/io/import_data.py`

 * *Files identical despite different names*

### Comparing `geci-nerd-0.3.1/nerd/mapping/tiling.py` & `geci-nerd-0.4.0/nerd/mapping/tiling.py`

 * *Files identical despite different names*

### Comparing `geci-nerd-0.3.1/nerd/solver.py` & `geci-nerd-0.4.0/nerd/solver.py`

 * *Files identical despite different names*

### Comparing `geci-nerd-0.3.1/setup.py` & `geci-nerd-0.4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     author="Ciencia de Datos • GECI",
     author_email="ciencia.datos@islas.org.mx",
     description="Numerical Estimation of Rodenticide Density (NERD)",
     long_description="The eradication of rodents is central to island conservation efforts and the aerial broadcast of rodenticide bait is the preferred dispersal method. To improve accuracy and expedite the evaluation of aerial operations, we developed an algorithm for the numerical estimation of rodenticide density (NERD). The NERD algorithm performs calculations with increased accuracy, displaying results almost in real-time. NERD describes the relationship between bait density, the mass flow rate of rodenticide through the bait bucket, and helicopter speed and produces maps of bait density on the ground. NERD also facilitates the planning of helicopter flight paths and allows for the instant identification of areas with low or high bait density.",
     name="geci-nerd",
     packages=find_packages(),
     url="https://github.com/IslasGECI/nerd",
-    version="0.3.1",
+    version="0.4.0",
     install_requires=[
         "descartes",
         "fiona",
         "geojsoncontour",
         "matplotlib",
         "numpy",
         "pandas",
```

