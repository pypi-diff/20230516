# Comparing `tmp/dis_tp-0.0.1.tar.gz` & `tmp/dis_tp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dis_tp-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dis_tp-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dis_tp-0.0.1.tar` & `dis_tp-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      382 2023-01-27 18:05:09.270364 dis_tp-0.0.1/README.md
--rw-r--r--   0        0        0     1291 2023-05-16 13:43:36.034335 dis_tp-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6108 2023-03-01 11:39:47.904195 dis_tp-0.0.1/src/dis_tp/Harmonics.py
--rwxr-xr-x   0        0        0    12829 2023-05-15 12:21:45.316582 dis_tp-0.0.1/src/dis_tp/Initialize.py
--rw-r--r--   0        0        0     2042 2023-03-01 11:39:47.904647 dis_tp-0.0.1/src/dis_tp/InverseMellin.py
--rwxr-xr-x   0        0        0     5038 2023-03-03 15:26:20.310552 dis_tp-0.0.1/src/dis_tp/MassiveCoeffFunc.py
--rwxr-xr-x   0        0        0     6668 2023-04-13 13:13:45.524709 dis_tp-0.0.1/src/dis_tp/MasslessCoeffFunc.py
--rwxr-xr-x   0        0        0     9872 2023-03-03 15:26:20.310824 dis_tp-0.0.1/src/dis_tp/MatchingFunc.py
--rwxr-xr-x   0        0        0     2577 2023-04-13 13:27:07.004573 dis_tp-0.0.1/src/dis_tp/ReadTxt.py
--rw-r--r--   0        0        0     2338 2023-03-01 11:39:47.906649 dis_tp-0.0.1/src/dis_tp/Splitting_funcs.py
--rwxr-xr-x   0        0        0     6024 2023-05-09 09:50:38.860127 dis_tp-0.0.1/src/dis_tp/TildeCoeffFunc.py
--rwxr-xr-x   0        0        0     3893 2023-04-13 13:13:45.525692 dis_tp-0.0.1/src/dis_tp/TildeCoeffFunc_light.py
--rw-r--r--   0        0        0      107 2022-10-29 12:56:08.209737 dis_tp-0.0.1/src/dis_tp/__init__.py
--rw-r--r--   0        0        0       55 2023-03-01 11:39:47.907109 dis_tp-0.0.1/src/dis_tp/cli/__init__.py
--rw-r--r--   0        0        0      215 2023-03-01 11:39:47.907253 dis_tp-0.0.1/src/dis_tp/cli/base.py
--rw-r--r--   0        0        0     5378 2023-05-15 12:21:45.317376 dis_tp-0.0.1/src/dis_tp/cli/compute.py
--rw-r--r--   0        0        0     2529 2023-05-15 12:21:45.318913 dis_tp-0.0.1/src/dis_tp/cli/grids.py
--rw-r--r--   0        0        0     2910 2023-03-01 11:39:47.907673 dis_tp-0.0.1/src/dis_tp/configs.py
--rw-r--r--   0        0        0     9580 2023-05-15 16:26:08.507519 dis_tp-0.0.1/src/dis_tp/io.py
--rw-r--r--   0        0        0     5566 2023-05-15 12:21:45.319679 dis_tp-0.0.1/src/dis_tp/k_factors.py
--rw-r--r--   0        0        0     1319 2023-03-01 11:39:47.908241 dis_tp-0.0.1/src/dis_tp/logging.py
--rw-r--r--   0        0        0     2562 2023-04-13 13:13:45.526821 dis_tp-0.0.1/src/dis_tp/parameters.py
--rw-r--r--   0        0        0    20827 2023-05-15 16:26:07.917731 dis_tp-0.0.1/src/dis_tp/plot.py
--rw-r--r--   0        0        0     4978 2023-05-15 12:21:45.320439 dis_tp-0.0.1/src/dis_tp/runner.py
--rw-r--r--   0        0        0       36 2023-03-01 11:39:47.908868 dis_tp-0.0.1/src/dis_tp/structure_functions/__init__.py
--rw-r--r--   0        0        0    30552 2023-05-09 15:15:38.294537 dis_tp-0.0.1/src/dis_tp/structure_functions/f2.py
--rw-r--r--   0        0        0    23748 2023-05-09 15:15:38.312802 dis_tp-0.0.1/src/dis_tp/structure_functions/fl.py
--rwxr-xr-x   0        0        0     4688 2023-03-03 15:26:20.311875 dis_tp-0.0.1/src/dis_tp/structure_functions/heavy_tools.py
--rw-r--r--   0        0        0     2693 2023-03-01 11:39:47.909463 dis_tp-0.0.1/src/dis_tp/structure_functions/light_tools.py
--rw-r--r--   0        0        0     1461 1970-01-01 00:00:00.000000 dis_tp-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      393 2023-05-16 14:50:03.623751 dis_tp-0.1.2/README.md
+-rw-r--r--   0        0        0     1291 2023-05-16 14:50:03.627751 dis_tp-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6108 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/Harmonics.py
+-rwxr-xr-x   0        0        0    12829 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/Initialize.py
+-rw-r--r--   0        0        0     2042 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/InverseMellin.py
+-rwxr-xr-x   0        0        0     5038 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/MassiveCoeffFunc.py
+-rwxr-xr-x   0        0        0     6668 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/MasslessCoeffFunc.py
+-rwxr-xr-x   0        0        0     9872 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/MatchingFunc.py
+-rwxr-xr-x   0        0        0     2577 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/ReadTxt.py
+-rw-r--r--   0        0        0     2338 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/Splitting_funcs.py
+-rwxr-xr-x   0        0        0     6024 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/TildeCoeffFunc.py
+-rwxr-xr-x   0        0        0     3893 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/TildeCoeffFunc_light.py
+-rw-r--r--   0        0        0      107 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/__init__.py
+-rw-r--r--   0        0        0       55 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/cli/__init__.py
+-rw-r--r--   0        0        0      215 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/cli/base.py
+-rw-r--r--   0        0        0     5378 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/cli/compute.py
+-rw-r--r--   0        0        0     2529 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/cli/grids.py
+-rw-r--r--   0        0        0     2910 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/configs.py
+-rw-r--r--   0        0        0     9580 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/io.py
+-rw-r--r--   0        0        0     5566 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/k_factors.py
+-rw-r--r--   0        0        0     1319 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/logging.py
+-rw-r--r--   0        0        0     2562 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/parameters.py
+-rw-r--r--   0        0        0    20827 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/plot.py
+-rw-r--r--   0        0        0     4978 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/runner.py
+-rw-r--r--   0        0        0       36 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/structure_functions/__init__.py
+-rw-r--r--   0        0        0    30552 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/structure_functions/f2.py
+-rw-r--r--   0        0        0    23748 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/structure_functions/fl.py
+-rwxr-xr-x   0        0        0     4688 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/structure_functions/heavy_tools.py
+-rw-r--r--   0        0        0     2693 2023-05-16 14:50:03.627751 dis_tp-0.1.2/src/dis_tp/structure_functions/light_tools.py
+-rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 dis_tp-0.1.2/PKG-INFO
```

### Comparing `dis_tp-0.0.1/pyproject.toml` & `dis_tp-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.7.1,<4"]
 
 [project]
 name = "dis_tp"
-version = "0.0.1"
+version = "0.1.2"
 authors = [
     {name = "Andrea Barontini", email = "andrea.barontini@mi.infn.it"},
     {name = "Niccolò Laurenti", email = "niccolo.laurenti@mi.infn.it"},
 ]
 description = "Python package for producing matched DIS predictions"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `dis_tp-0.0.1/src/dis_tp/Harmonics.py` & `dis_tp-0.1.2/src/dis_tp/Harmonics.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/src/dis_tp/Initialize.py` & `dis_tp-0.1.2/src/dis_tp/Initialize.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/src/dis_tp/InverseMellin.py` & `dis_tp-0.1.2/src/dis_tp/InverseMellin.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/src/dis_tp/MassiveCoeffFunc.py` & `dis_tp-0.1.2/src/dis_tp/MassiveCoeffFunc.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/src/dis_tp/MasslessCoeffFunc.py` & `dis_tp-0.1.2/src/dis_tp/MasslessCoeffFunc.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/src/dis_tp/MatchingFunc.py` & `dis_tp-0.1.2/src/dis_tp/MatchingFunc.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/src/dis_tp/ReadTxt.py` & `dis_tp-0.1.2/src/dis_tp/ReadTxt.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/src/dis_tp/Splitting_funcs.py` & `dis_tp-0.1.2/src/dis_tp/Splitting_funcs.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/src/dis_tp/TildeCoeffFunc.py` & `dis_tp-0.1.2/src/dis_tp/TildeCoeffFunc.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/src/dis_tp/TildeCoeffFunc_light.py` & `dis_tp-0.1.2/src/dis_tp/TildeCoeffFunc_light.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/src/dis_tp/cli/compute.py` & `dis_tp-0.1.2/src/dis_tp/cli/compute.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/src/dis_tp/cli/grids.py` & `dis_tp-0.1.2/src/dis_tp/cli/grids.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/src/dis_tp/configs.py` & `dis_tp-0.1.2/src/dis_tp/configs.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/src/dis_tp/io.py` & `dis_tp-0.1.2/src/dis_tp/io.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/src/dis_tp/k_factors.py` & `dis_tp-0.1.2/src/dis_tp/k_factors.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/src/dis_tp/logging.py` & `dis_tp-0.1.2/src/dis_tp/logging.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/src/dis_tp/parameters.py` & `dis_tp-0.1.2/src/dis_tp/parameters.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/src/dis_tp/plot.py` & `dis_tp-0.1.2/src/dis_tp/plot.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/src/dis_tp/runner.py` & `dis_tp-0.1.2/src/dis_tp/runner.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/src/dis_tp/structure_functions/f2.py` & `dis_tp-0.1.2/src/dis_tp/structure_functions/f2.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/src/dis_tp/structure_functions/fl.py` & `dis_tp-0.1.2/src/dis_tp/structure_functions/fl.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/src/dis_tp/structure_functions/heavy_tools.py` & `dis_tp-0.1.2/src/dis_tp/structure_functions/heavy_tools.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/src/dis_tp/structure_functions/light_tools.py` & `dis_tp-0.1.2/src/dis_tp/structure_functions/light_tools.py`

 * *Files identical despite different names*

### Comparing `dis_tp-0.0.1/PKG-INFO` & `dis_tp-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dis_tp
-Version: 0.0.1
+Version: 0.1.2
 Summary: Python package for producing matched DIS predictions
 Author-email: Andrea Barontini <andrea.barontini@mi.infn.it>, Niccolò Laurenti <niccolo.laurenti@mi.infn.it>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -24,11 +24,10 @@
 Requires-Dist: yadism == 0.12.4
 Requires-Dist: click ==8.1.3
 Requires-Dist: banana-hep ==0.6.7
 Requires-Dist: multiprocess == 0.70.14
 Requires-Dist: rich == 12.6.0
 
 # DIS_TP
-This is the python version of the code I used for my master's thesis. It computes the F2 and FL structure functions for DIS with heavy-quark prodction (at the moment
-assumed to be the b-quark) at NLO, NNLO and N3LO. It is also able to construct the scale varied result (at the moment only threshold scale variation
-is available) and obtain uncertainty bands based on that.
+This is the python version of the code I used for my master's thesis. It computes the F2 and FL structure functions for DIS with heavy-quark production at NLO, NNLO and N3LO. It is also able to construct the scale varied result (at the moment only threshold scale variation
+is available) and obtain uncertainty bands based on that and on coefficient function uncertainties (at N3LO).
```

