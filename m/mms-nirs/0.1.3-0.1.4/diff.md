# Comparing `tmp/mms_nirs-0.1.3.tar.gz` & `tmp/mms_nirs-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mms_nirs-0.1.3.tar", max compression
+gzip compressed data, was "mms_nirs-0.1.4.tar", max compression
```

## Comparing `mms_nirs-0.1.3.tar` & `mms_nirs-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      143 2023-05-03 11:01:49.168314 mms_nirs-0.1.3/README.md
--rw-r--r--   0        0        0      662 2023-05-09 17:15:42.681482 mms_nirs-0.1.3/mms_nirs/UCLN/DefaultValues.py
--rw-r--r--   0        0        0     3304 2023-05-09 17:15:42.681482 mms_nirs-0.1.3/mms_nirs/UCLN/UCLN.py
--rw-r--r--   0        0        0      132 2023-05-09 15:01:31.364702 mms_nirs-0.1.3/mms_nirs/UCLN/__init__.py
--rw-r--r--   0        0        0     3876 2023-05-09 17:15:42.681482 mms_nirs-0.1.3/mms_nirs/UCLN/defaults.csv
--rw-r--r--   0        0        0        0 2023-05-02 14:50:03.986089 mms_nirs-0.1.3/mms_nirs/__init__.py
--rw-r--r--   0        0        0      892 2023-05-09 17:17:07.741448 mms_nirs-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      794 1970-01-01 00:00:00.000000 mms_nirs-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-05-03 11:01:49.168314 mms_nirs-0.1.4/README.md
+-rw-r--r--   0        0        0      662 2023-05-09 17:15:42.681482 mms_nirs-0.1.4/mms_nirs/UCLN/DefaultValues.py
+-rw-r--r--   0        0        0     3309 2023-05-16 10:47:43.079500 mms_nirs-0.1.4/mms_nirs/UCLN/UCLN.py
+-rw-r--r--   0        0        0      152 2023-05-16 10:47:43.079500 mms_nirs-0.1.4/mms_nirs/UCLN/__init__.py
+-rw-r--r--   0        0        0     3876 2023-05-09 17:15:42.681482 mms_nirs-0.1.4/mms_nirs/UCLN/defaults.csv
+-rw-r--r--   0        0        0        0 2023-05-02 14:50:03.986089 mms_nirs-0.1.4/mms_nirs/__init__.py
+-rw-r--r--   0        0        0      892 2023-05-16 10:48:10.839500 mms_nirs-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      794 1970-01-01 00:00:00.000000 mms_nirs-0.1.4/PKG-INFO
```

### Comparing `mms_nirs-0.1.3/mms_nirs/UCLN/DefaultValues.py` & `mms_nirs-0.1.4/mms_nirs/UCLN/DefaultValues.py`

 * *Files identical despite different names*

### Comparing `mms_nirs-0.1.3/mms_nirs/UCLN/UCLN.py` & `mms_nirs-0.1.4/mms_nirs/UCLN/UCLN.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Literal, Optional, TypedDict, Tuple
+from typing import Literal, Optional, Tuple, TypedDict
+
 import numpy as np
 from numpy import linalg
 from scipy.interpolate import interp1d
 
 
 class DifferentialPathlengthFactors(TypedDict):
     baby_head: float
@@ -27,15 +28,15 @@
 
     def __init__(
         self,
         extinction_coefficients: np.ndarray,
         wavelength_dependency_of_pathlength: np.ndarray,
         optode_dist: float,
         dpf_type: DpfType,
-        wavelengths: Tuple[int, int],
+        wavelengths: Tuple[float, float],
     ) -> None:
         self.extinction_coefficients = extinction_coefficients
         self.wavelength_dependency = wavelength_dependency_of_pathlength
         self.optode_dist = optode_dist
         self.dpf: float = self._dpf_dict[dpf_type]
 
         (min_wavelength, max_wavelength) = wavelengths
```

### Comparing `mms_nirs-0.1.3/mms_nirs/UCLN/defaults.csv` & `mms_nirs-0.1.4/mms_nirs/UCLN/defaults.csv`

 * *Files identical despite different names*

### Comparing `mms_nirs-0.1.3/pyproject.toml` & `mms_nirs-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mms-nirs"
-version = "0.1.3"
+version = "0.1.4"
 description = "Algorithms used in the multimodal spectroscopy group to process NIRS data"
 authors = ["Josh Buckland, <joshua.russell-buckland@ucl.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "mms_nirs" }]
 
 [tool.poetry.dependencies]
```

### Comparing `mms_nirs-0.1.3/PKG-INFO` & `mms_nirs-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mms-nirs
-Version: 0.1.3
+Version: 0.1.4
 Summary: Algorithms used in the multimodal spectroscopy group to process NIRS data
 License: MIT
 Author: Josh Buckland,
 Author-email: joshua.russell-buckland@ucl.ac.uk
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

