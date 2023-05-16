# Comparing `tmp/causaltensor-0.1.4.tar.gz` & `tmp/causaltensor-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/tianyipeng/Documents/Operations Research Code/21-08 Low-rank Matrix Code Library/Package Publication/causaltensor/dist/.", last modified: Sun Jan  1 16:47:51 2023, max compression
+gzip compressed data, was "/Users/tianyipeng/Documents/Operations Research Code/21-08 Low-rank Matrix Code Library/Package Publication/causaltensor/dist/.", last modified: Tue May 16 16:57:49 2023, max compression
```

## Comparing `causaltensor-0.1.4.tar` & `causaltensor-0.1.5.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 tianyipeng   (501) staff       (20)        0 2023-01-01 16:47:51.000000 causaltensor-0.1.4/
--rw-r--r--   0 tianyipeng   (501) staff       (20)     1068 2022-12-23 18:44:37.000000 causaltensor-0.1.4/LICENSE
--rw-r--r--   0 tianyipeng   (501) staff       (20)     4598 2023-01-01 16:47:51.000000 causaltensor-0.1.4/PKG-INFO
--rw-r--r--   0 tianyipeng   (501) staff       (20)     2744 2023-01-01 16:45:27.000000 causaltensor-0.1.4/README.md
--rw-r--r--   0 tianyipeng   (501) staff       (20)      980 2022-12-31 16:05:12.000000 causaltensor-0.1.4/pyproject.toml
--rw-r--r--   0 tianyipeng   (501) staff       (20)       38 2023-01-01 16:47:51.000000 causaltensor-0.1.4/setup.cfg
--rw-r--r--   0 tianyipeng   (501) staff       (20)       49 2022-12-24 00:56:31.000000 causaltensor-0.1.4/setup.py
-drwxr-xr-x   0 tianyipeng   (501) staff       (20)        0 2023-01-01 16:47:51.000000 causaltensor-0.1.4/src/
-drwxr-xr-x   0 tianyipeng   (501) staff       (20)        0 2023-01-01 16:47:51.000000 causaltensor-0.1.4/src/causaltensor/
--rw-r--r--   0 tianyipeng   (501) staff       (20)       92 2022-10-04 05:06:34.000000 causaltensor-0.1.4/src/causaltensor/__init__.py
-drwxr-xr-x   0 tianyipeng   (501) staff       (20)        0 2023-01-01 16:47:51.000000 causaltensor-0.1.4/src/causaltensor/cauest/
--rw-r--r--   0 tianyipeng   (501) staff       (20)     1973 2021-02-06 06:50:53.000000 causaltensor-0.1.4/src/causaltensor/cauest/CovariancePCA.py
--rw-r--r--   0 tianyipeng   (501) staff       (20)     1545 2022-12-25 19:22:55.000000 causaltensor-0.1.4/src/causaltensor/cauest/DID.py
--rw-r--r--   0 tianyipeng   (501) staff       (20)     3961 2022-12-30 00:46:40.000000 causaltensor-0.1.4/src/causaltensor/cauest/DebiasConvex.py
--rw-r--r--   0 tianyipeng   (501) staff       (20)     2829 2021-05-26 20:33:00.000000 causaltensor-0.1.4/src/causaltensor/cauest/DebiasConvexMissing.py
--rw-r--r--   0 tianyipeng   (501) staff       (20)     1776 2021-06-04 00:15:51.000000 causaltensor-0.1.4/src/causaltensor/cauest/DebiasConvexMultipleTreatment.py
--rw-r--r--   0 tianyipeng   (501) staff       (20)     4996 2023-01-01 06:26:26.000000 causaltensor-0.1.4/src/causaltensor/cauest/MCNNM.py
--rw-r--r--   0 tianyipeng   (501) staff       (20)     2388 2021-02-09 04:45:49.000000 causaltensor-0.1.4/src/causaltensor/cauest/RobustSyntheticControl.py
--rw-r--r--   0 tianyipeng   (501) staff       (20)     4192 2022-12-25 19:50:50.000000 causaltensor-0.1.4/src/causaltensor/cauest/SDID.py
--rw-r--r--   0 tianyipeng   (501) staff       (20)       90 2022-12-26 03:46:31.000000 causaltensor-0.1.4/src/causaltensor/cauest/__init__.py
-drwxr-xr-x   0 tianyipeng   (501) staff       (20)        0 2023-01-01 16:47:51.000000 causaltensor-0.1.4/src/causaltensor/matcomple/
--rw-r--r--   0 tianyipeng   (501) staff       (20)     2241 2022-12-23 17:22:59.000000 causaltensor-0.1.4/src/causaltensor/matcomple/ALS_solver.py
--rw-r--r--   0 tianyipeng   (501) staff       (20)       52 2022-10-04 05:07:43.000000 causaltensor-0.1.4/src/causaltensor/matcomple/__init__.py
--rw-r--r--   0 tianyipeng   (501) staff       (20)      301 2022-10-04 05:12:40.000000 causaltensor-0.1.4/src/causaltensor/matcomple/hard_impute.py
-drwxr-xr-x   0 tianyipeng   (501) staff       (20)        0 2023-01-01 16:47:51.000000 causaltensor-0.1.4/src/causaltensor/matlib/
--rw-r--r--   0 tianyipeng   (501) staff       (20)       89 2022-07-14 18:23:15.000000 causaltensor-0.1.4/src/causaltensor/matlib/__init__.py
--rw-r--r--   0 tianyipeng   (501) staff       (20)     1399 2022-07-14 16:57:40.000000 causaltensor-0.1.4/src/causaltensor/matlib/generation.py
--rw-r--r--   0 tianyipeng   (501) staff       (20)     3398 2021-12-06 21:52:31.000000 causaltensor-0.1.4/src/causaltensor/matlib/generation_treatment_pattern.py
--rw-r--r--   0 tianyipeng   (501) staff       (20)     1843 2022-10-04 05:14:13.000000 causaltensor-0.1.4/src/causaltensor/matlib/util.py
-drwxr-xr-x   0 tianyipeng   (501) staff       (20)        0 2023-01-01 16:47:51.000000 causaltensor-0.1.4/src/causaltensor/sample_data/
--rw-r--r--   0 tianyipeng   (501) staff       (20)       20 2022-12-25 18:05:57.000000 causaltensor-0.1.4/src/causaltensor/sample_data/__init__.py
--rw-r--r--   0 tianyipeng   (501) staff       (20)       81 2022-12-30 00:50:32.000000 causaltensor-0.1.4/src/causaltensor/sample_data/fetch.py
-drwxr-xr-x   0 tianyipeng   (501) staff       (20)        0 2023-01-01 16:47:51.000000 causaltensor-0.1.4/src/causaltensor.egg-info/
--rw-r--r--   0 tianyipeng   (501) staff       (20)     4598 2023-01-01 16:47:51.000000 causaltensor-0.1.4/src/causaltensor.egg-info/PKG-INFO
--rw-r--r--   0 tianyipeng   (501) staff       (20)      999 2023-01-01 16:47:51.000000 causaltensor-0.1.4/src/causaltensor.egg-info/SOURCES.txt
--rw-r--r--   0 tianyipeng   (501) staff       (20)        1 2023-01-01 16:47:51.000000 causaltensor-0.1.4/src/causaltensor.egg-info/dependency_links.txt
--rw-r--r--   0 tianyipeng   (501) staff       (20)       67 2023-01-01 16:47:51.000000 causaltensor-0.1.4/src/causaltensor.egg-info/requires.txt
--rw-r--r--   0 tianyipeng   (501) staff       (20)       13 2023-01-01 16:47:51.000000 causaltensor-0.1.4/src/causaltensor.egg-info/top_level.txt
+drwxr-xr-x   0 tianyipeng   (501) staff       (20)        0 2023-05-16 16:57:49.000000 causaltensor-0.1.5/
+-rw-r--r--   0 tianyipeng   (501) staff       (20)     1068 2022-12-23 18:44:37.000000 causaltensor-0.1.5/LICENSE
+-rw-r--r--   0 tianyipeng   (501) staff       (20)     4598 2023-05-16 16:57:49.000000 causaltensor-0.1.5/PKG-INFO
+-rw-r--r--   0 tianyipeng   (501) staff       (20)     2744 2023-01-01 16:45:27.000000 causaltensor-0.1.5/README.md
+-rw-r--r--   0 tianyipeng   (501) staff       (20)      980 2023-05-16 16:57:35.000000 causaltensor-0.1.5/pyproject.toml
+-rw-r--r--   0 tianyipeng   (501) staff       (20)       38 2023-05-16 16:57:49.000000 causaltensor-0.1.5/setup.cfg
+-rw-r--r--   0 tianyipeng   (501) staff       (20)       49 2022-12-24 00:56:31.000000 causaltensor-0.1.5/setup.py
+drwxr-xr-x   0 tianyipeng   (501) staff       (20)        0 2023-05-16 16:57:49.000000 causaltensor-0.1.5/src/
+drwxr-xr-x   0 tianyipeng   (501) staff       (20)        0 2023-05-16 16:57:49.000000 causaltensor-0.1.5/src/causaltensor/
+-rw-r--r--   0 tianyipeng   (501) staff       (20)       92 2022-10-04 05:06:34.000000 causaltensor-0.1.5/src/causaltensor/__init__.py
+drwxr-xr-x   0 tianyipeng   (501) staff       (20)        0 2023-05-16 16:57:49.000000 causaltensor-0.1.5/src/causaltensor/cauest/
+-rw-r--r--   0 tianyipeng   (501) staff       (20)     1973 2021-02-06 06:50:53.000000 causaltensor-0.1.5/src/causaltensor/cauest/CovariancePCA.py
+-rw-r--r--   0 tianyipeng   (501) staff       (20)     1563 2023-01-27 17:50:18.000000 causaltensor-0.1.5/src/causaltensor/cauest/DID.py
+-rw-r--r--   0 tianyipeng   (501) staff       (20)     3961 2022-12-30 00:46:40.000000 causaltensor-0.1.5/src/causaltensor/cauest/DebiasConvex.py
+-rw-r--r--   0 tianyipeng   (501) staff       (20)     2829 2021-05-26 20:33:00.000000 causaltensor-0.1.5/src/causaltensor/cauest/DebiasConvexMissing.py
+-rw-r--r--   0 tianyipeng   (501) staff       (20)     4996 2023-01-01 06:26:26.000000 causaltensor-0.1.5/src/causaltensor/cauest/MCNNM.py
+-rw-r--r--   0 tianyipeng   (501) staff       (20)     2784 2023-05-16 16:31:49.000000 causaltensor-0.1.5/src/causaltensor/cauest/Multiple_Interventions.py
+-rw-r--r--   0 tianyipeng   (501) staff       (20)     2388 2021-02-09 04:45:49.000000 causaltensor-0.1.5/src/causaltensor/cauest/RobustSyntheticControl.py
+-rw-r--r--   0 tianyipeng   (501) staff       (20)     1776 2021-06-04 00:15:51.000000 causaltensor-0.1.5/src/causaltensor/cauest/Row_Specific_Treatments.py
+-rw-r--r--   0 tianyipeng   (501) staff       (20)     4192 2022-12-25 19:50:50.000000 causaltensor-0.1.5/src/causaltensor/cauest/SDID.py
+-rw-r--r--   0 tianyipeng   (501) staff       (20)      128 2023-05-16 16:15:08.000000 causaltensor-0.1.5/src/causaltensor/cauest/__init__.py
+drwxr-xr-x   0 tianyipeng   (501) staff       (20)        0 2023-05-16 16:57:49.000000 causaltensor-0.1.5/src/causaltensor/matcomple/
+-rw-r--r--   0 tianyipeng   (501) staff       (20)     2241 2022-12-23 17:22:59.000000 causaltensor-0.1.5/src/causaltensor/matcomple/ALS_solver.py
+-rw-r--r--   0 tianyipeng   (501) staff       (20)       52 2022-10-04 05:07:43.000000 causaltensor-0.1.5/src/causaltensor/matcomple/__init__.py
+-rw-r--r--   0 tianyipeng   (501) staff       (20)      301 2022-10-04 05:12:40.000000 causaltensor-0.1.5/src/causaltensor/matcomple/hard_impute.py
+drwxr-xr-x   0 tianyipeng   (501) staff       (20)        0 2023-05-16 16:57:49.000000 causaltensor-0.1.5/src/causaltensor/matlib/
+-rw-r--r--   0 tianyipeng   (501) staff       (20)       89 2022-07-14 18:23:15.000000 causaltensor-0.1.5/src/causaltensor/matlib/__init__.py
+-rw-r--r--   0 tianyipeng   (501) staff       (20)     1399 2022-07-14 16:57:40.000000 causaltensor-0.1.5/src/causaltensor/matlib/generation.py
+-rw-r--r--   0 tianyipeng   (501) staff       (20)     3398 2021-12-06 21:52:31.000000 causaltensor-0.1.5/src/causaltensor/matlib/generation_treatment_pattern.py
+-rw-r--r--   0 tianyipeng   (501) staff       (20)     1843 2022-10-04 05:14:13.000000 causaltensor-0.1.5/src/causaltensor/matlib/util.py
+drwxr-xr-x   0 tianyipeng   (501) staff       (20)        0 2023-05-16 16:57:49.000000 causaltensor-0.1.5/src/causaltensor/sample_data/
+-rw-r--r--   0 tianyipeng   (501) staff       (20)       20 2022-12-25 18:05:57.000000 causaltensor-0.1.5/src/causaltensor/sample_data/__init__.py
+-rw-r--r--   0 tianyipeng   (501) staff       (20)       81 2022-12-30 00:50:32.000000 causaltensor-0.1.5/src/causaltensor/sample_data/fetch.py
+drwxr-xr-x   0 tianyipeng   (501) staff       (20)        0 2023-05-16 16:57:49.000000 causaltensor-0.1.5/src/causaltensor.egg-info/
+-rw-r--r--   0 tianyipeng   (501) staff       (20)     4598 2023-05-16 16:57:49.000000 causaltensor-0.1.5/src/causaltensor.egg-info/PKG-INFO
+-rw-r--r--   0 tianyipeng   (501) staff       (20)     1043 2023-05-16 16:57:49.000000 causaltensor-0.1.5/src/causaltensor.egg-info/SOURCES.txt
+-rw-r--r--   0 tianyipeng   (501) staff       (20)        1 2023-05-16 16:57:49.000000 causaltensor-0.1.5/src/causaltensor.egg-info/dependency_links.txt
+-rw-r--r--   0 tianyipeng   (501) staff       (20)       67 2023-05-16 16:57:49.000000 causaltensor-0.1.5/src/causaltensor.egg-info/requires.txt
+-rw-r--r--   0 tianyipeng   (501) staff       (20)       13 2023-05-16 16:57:49.000000 causaltensor-0.1.5/src/causaltensor.egg-info/top_level.txt
```

### Comparing `causaltensor-0.1.4/LICENSE` & `causaltensor-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `causaltensor-0.1.4/PKG-INFO` & `causaltensor-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causaltensor
-Version: 0.1.4
+Version: 0.1.5
 Summary: Package for causal inference in panels
 Author-email: Tianyi Peng <tianyipeng95@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Tianyi Peng
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `causaltensor-0.1.4/README.md` & `causaltensor-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `causaltensor-0.1.4/pyproject.toml` & `causaltensor-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "causaltensor"
-version = "0.1.4"
+version = "0.1.5"
 description = "Package for causal inference in panels"
 readme = "README.md"
 authors = [{ name = "Tianyi Peng", email = "tianyipeng95@gmail.com"}]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `causaltensor-0.1.4/src/causaltensor/cauest/CovariancePCA.py` & `causaltensor-0.1.5/src/causaltensor/cauest/CovariancePCA.py`

 * *Files identical despite different names*

### Comparing `causaltensor-0.1.4/src/causaltensor/cauest/DID.py` & `causaltensor-0.1.5/src/causaltensor/cauest/DID.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-def DID(O, Z, tau_star = 0):
+def DID(O, Z, tau_star = 0, output_var=False):
     n1 = O.shape[0]
     n2 = O.shape[1]
 
     a = np.zeros((n1, 1))
     b = np.zeros((n2, 1))
     tau = tau_star
 
@@ -34,15 +34,15 @@
     one_col = np.ones((n1, 1))
     M = a.dot(one_row)+one_col.dot(b.T)
 
     for T1 in range(2000):
         a_new = np.sum(Omega*(O-tau*Z-one_col.dot(b.T)), axis=1).reshape((n1, 1)) / np.sum(Omega, axis=1).reshape((n1, 1))
         b_new = np.sum(Omega*(O-tau*Z-a_new.dot(one_row)), axis=0).reshape((n2, 1)) / np.sum(Omega, axis=0).reshape((n2, 1))
 
-        if (np.sum((b_new - b)**2) < 1e-5 * np.sum(b**2) and np.sum((a_new - a)**2) < 1e-5 * np.sum(a**2)):
+        if (np.sum((b_new - b)**2) < 1e-7 * np.sum(b**2) and np.sum((a_new - a)**2) < 1e-7 * np.sum(a**2)):
             break
         a = a_new
         b = b_new
         M = a.dot(one_row)+one_col.dot(b.T)
         tau = np.sum(Omega*Z*(O-M))/np.sum(Omega*Z)
 
         if debug:
```

### Comparing `causaltensor-0.1.4/src/causaltensor/cauest/DebiasConvex.py` & `causaltensor-0.1.5/src/causaltensor/cauest/DebiasConvex.py`

 * *Files identical despite different names*

### Comparing `causaltensor-0.1.4/src/causaltensor/cauest/DebiasConvexMissing.py` & `causaltensor-0.1.5/src/causaltensor/cauest/DebiasConvexMissing.py`

 * *Files identical despite different names*

### Comparing `causaltensor-0.1.4/src/causaltensor/cauest/DebiasConvexMultipleTreatment.py` & `causaltensor-0.1.5/src/causaltensor/cauest/Row_Specific_Treatments.py`

 * *Files identical despite different names*

### Comparing `causaltensor-0.1.4/src/causaltensor/cauest/MCNNM.py` & `causaltensor-0.1.5/src/causaltensor/cauest/MCNNM.py`

 * *Files identical despite different names*

### Comparing `causaltensor-0.1.4/src/causaltensor/cauest/RobustSyntheticControl.py` & `causaltensor-0.1.5/src/causaltensor/cauest/RobustSyntheticControl.py`

 * *Files identical despite different names*

### Comparing `causaltensor-0.1.4/src/causaltensor/cauest/SDID.py` & `causaltensor-0.1.5/src/causaltensor/cauest/SDID.py`

 * *Files identical despite different names*

### Comparing `causaltensor-0.1.4/src/causaltensor/matcomple/ALS_solver.py` & `causaltensor-0.1.5/src/causaltensor/matcomple/ALS_solver.py`

 * *Files identical despite different names*

### Comparing `causaltensor-0.1.4/src/causaltensor/matlib/generation.py` & `causaltensor-0.1.5/src/causaltensor/matlib/generation.py`

 * *Files identical despite different names*

### Comparing `causaltensor-0.1.4/src/causaltensor/matlib/generation_treatment_pattern.py` & `causaltensor-0.1.5/src/causaltensor/matlib/generation_treatment_pattern.py`

 * *Files identical despite different names*

### Comparing `causaltensor-0.1.4/src/causaltensor/matlib/util.py` & `causaltensor-0.1.5/src/causaltensor/matlib/util.py`

 * *Files identical despite different names*

### Comparing `causaltensor-0.1.4/src/causaltensor.egg-info/PKG-INFO` & `causaltensor-0.1.5/src/causaltensor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causaltensor
-Version: 0.1.4
+Version: 0.1.5
 Summary: Package for causal inference in panels
 Author-email: Tianyi Peng <tianyipeng95@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Tianyi Peng
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `causaltensor-0.1.4/src/causaltensor.egg-info/SOURCES.txt` & `causaltensor-0.1.5/src/causaltensor.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 src/causaltensor.egg-info/dependency_links.txt
 src/causaltensor.egg-info/requires.txt
 src/causaltensor.egg-info/top_level.txt
 src/causaltensor/cauest/CovariancePCA.py
 src/causaltensor/cauest/DID.py
 src/causaltensor/cauest/DebiasConvex.py
 src/causaltensor/cauest/DebiasConvexMissing.py
-src/causaltensor/cauest/DebiasConvexMultipleTreatment.py
 src/causaltensor/cauest/MCNNM.py
+src/causaltensor/cauest/Multiple_Interventions.py
 src/causaltensor/cauest/RobustSyntheticControl.py
+src/causaltensor/cauest/Row_Specific_Treatments.py
 src/causaltensor/cauest/SDID.py
 src/causaltensor/cauest/__init__.py
 src/causaltensor/matcomple/ALS_solver.py
 src/causaltensor/matcomple/__init__.py
 src/causaltensor/matcomple/hard_impute.py
 src/causaltensor/matlib/__init__.py
 src/causaltensor/matlib/generation.py
```

