# Comparing `tmp/dymoval-0.8.82.tar.gz` & `tmp/dymoval-0.8.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dymoval-0.8.82.tar", last modified: Tue May 16 13:51:52 2023, max compression
+gzip compressed data, was "dymoval-0.8.83.tar", last modified: Tue May 16 20:44:44 2023, max compression
```

## Comparing `dymoval-0.8.82.tar` & `dymoval-0.8.83.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1536 2023-05-16 08:21:52.083500 dymoval-0.8.82/LICENSE
--rw-r--r--   0        0        0     4475 2023-05-15 07:01:30.761752 dymoval-0.8.82/README.md
--rw-r--r--   0        0        0     1923 2023-05-16 13:51:52.290691 dymoval-0.8.82/pyproject.toml
--rw-r--r--   0        0        0      125 2023-05-14 20:41:41.380658 dymoval-0.8.82/src/dymoval/__init__.py
--rw-r--r--   0        0        0     1332 2023-05-15 08:02:53.628954 dymoval-0.8.82/src/dymoval/config.py
--rw-r--r--   0        0        0   112805 2023-05-14 20:41:41.381154 dymoval-0.8.82/src/dymoval/dataset.py
--rw-r--r--   0        0        0     2543 2023-05-15 10:15:47.636362 dymoval-0.8.82/src/dymoval/utils.py
--rw-r--r--   0        0        0    32835 2023-05-14 20:41:41.381401 dymoval-0.8.82/src/dymoval/validation.py
--rw-r--r--   0        0        0    65913 2023-05-14 20:41:41.381658 dymoval-0.8.82/src/tutorial/DCMotor.fmu
--rw-r--r--   0        0        0  1136010 2023-05-14 20:41:41.386937 dymoval-0.8.82/src/tutorial/DCMotor.svg
--rw-r--r--   0        0        0   963816 2023-05-14 20:41:41.391006 dymoval-0.8.82/src/tutorial/DCMotorLogs.h5
--rw-r--r--   0        0        0      798 2023-05-14 20:41:41.391222 dymoval-0.8.82/src/tutorial/DCMotorModel.py
--rw-r--r--   0        0        0        0 2023-05-14 20:41:41.391250 dymoval-0.8.82/src/tutorial/__init__.py
--rw-r--r--   0        0        0    34918 2023-05-14 20:41:41.391446 dymoval-0.8.82/src/tutorial/tutorial.ipynb
--rw-r--r--   0        0        0     6148 2023-05-16 12:22:44.602879 dymoval-0.8.82/tests/.DS_Store
--rw-r--r--   0        0        0    12028 2023-05-14 20:41:41.391579 dymoval-0.8.82/tests/fixture_data.py
--rw-r--r--   0        0        0    54383 2023-05-16 12:53:21.472851 dymoval-0.8.82/tests/test_dataset.py
--rw-r--r--   0        0        0    12436 2023-05-16 12:53:21.473084 dymoval-0.8.82/tests/test_initializers.py
--rw-r--r--   0        0        0     3215 2023-05-16 12:53:21.473265 dymoval-0.8.82/tests/test_utils.py
--rw-r--r--   0        0        0    26579 2023-05-16 12:53:21.473501 dymoval-0.8.82/tests/test_validation.py
--rw-r--r--   0        0        0     7504 1970-01-01 00:00:00.000000 dymoval-0.8.82/PKG-INFO
+-rw-r--r--   0        0        0     1536 2023-05-16 08:21:52.083500 dymoval-0.8.83/LICENSE
+-rw-r--r--   0        0        0     4475 2023-05-15 07:01:30.761752 dymoval-0.8.83/README.md
+-rw-r--r--   0        0        0     1908 2023-05-16 20:44:44.663459 dymoval-0.8.83/pyproject.toml
+-rw-r--r--   0        0        0      125 2023-05-14 20:41:41.380658 dymoval-0.8.83/src/dymoval/__init__.py
+-rw-r--r--   0        0        0     1332 2023-05-15 08:02:53.628954 dymoval-0.8.83/src/dymoval/config.py
+-rw-r--r--   0        0        0   112805 2023-05-14 20:41:41.381154 dymoval-0.8.83/src/dymoval/dataset.py
+-rw-r--r--   0        0        0     2543 2023-05-15 10:15:47.636362 dymoval-0.8.83/src/dymoval/utils.py
+-rw-r--r--   0        0        0    32835 2023-05-14 20:41:41.381401 dymoval-0.8.83/src/dymoval/validation.py
+-rw-r--r--   0        0        0    65913 2023-05-14 20:41:41.381658 dymoval-0.8.83/src/tutorial/DCMotor.fmu
+-rw-r--r--   0        0        0  1136010 2023-05-14 20:41:41.386937 dymoval-0.8.83/src/tutorial/DCMotor.svg
+-rw-r--r--   0        0        0   963816 2023-05-14 20:41:41.391006 dymoval-0.8.83/src/tutorial/DCMotorLogs.h5
+-rw-r--r--   0        0        0      798 2023-05-14 20:41:41.391222 dymoval-0.8.83/src/tutorial/DCMotorModel.py
+-rw-r--r--   0        0        0        0 2023-05-14 20:41:41.391250 dymoval-0.8.83/src/tutorial/__init__.py
+-rw-r--r--   0        0        0    34918 2023-05-14 20:41:41.391446 dymoval-0.8.83/src/tutorial/tutorial.ipynb
+-rw-r--r--   0        0        0     6148 2023-05-16 12:22:44.602879 dymoval-0.8.83/tests/.DS_Store
+-rw-r--r--   0        0        0    12028 2023-05-14 20:41:41.391579 dymoval-0.8.83/tests/fixture_data.py
+-rw-r--r--   0        0        0    54383 2023-05-16 12:53:21.472851 dymoval-0.8.83/tests/test_dataset.py
+-rw-r--r--   0        0        0    12436 2023-05-16 12:53:21.473084 dymoval-0.8.83/tests/test_initializers.py
+-rw-r--r--   0        0        0     3215 2023-05-16 12:53:21.473265 dymoval-0.8.83/tests/test_utils.py
+-rw-r--r--   0        0        0    26579 2023-05-16 12:53:21.473501 dymoval-0.8.83/tests/test_validation.py
+-rw-r--r--   0        0        0     7481 1970-01-01 00:00:00.000000 dymoval-0.8.83/PKG-INFO
```

### Comparing `dymoval-0.8.82/LICENSE` & `dymoval-0.8.83/LICENSE`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.82/README.md` & `dymoval-0.8.83/README.md`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.82/pyproject.toml` & `dymoval-0.8.83/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "dymoval"
-version = "0.8.82"
+version = "0.8.83"
 requires-python = ">=3.10"
 dependencies = [
     "pandas",
     "matplotlib",
     "scipy",
     "control",
-    "pathlib",
     "numpy",
     "tomli",
     "h5py",
 ]
 authors = [
     { name = "Ubaldo Tiberi", email = "ubaldo.tiberi@volvo.com" },
     { name = "Ubaldo Tiberi", email = "ubaldo.tiberi@gmail.com" },
```

### Comparing `dymoval-0.8.82/src/dymoval/config.py` & `dymoval-0.8.83/src/dymoval/config.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.82/src/dymoval/dataset.py` & `dymoval-0.8.83/src/dymoval/dataset.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.82/src/dymoval/utils.py` & `dymoval-0.8.83/src/dymoval/utils.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.82/src/dymoval/validation.py` & `dymoval-0.8.83/src/dymoval/validation.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.82/src/tutorial/DCMotor.fmu` & `dymoval-0.8.83/src/tutorial/DCMotor.fmu`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.82/src/tutorial/DCMotor.svg` & `dymoval-0.8.83/src/tutorial/DCMotor.svg`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.82/src/tutorial/DCMotorLogs.h5` & `dymoval-0.8.83/src/tutorial/DCMotorLogs.h5`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.82/src/tutorial/DCMotorModel.py` & `dymoval-0.8.83/src/tutorial/DCMotorModel.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.82/src/tutorial/tutorial.ipynb` & `dymoval-0.8.83/src/tutorial/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.82/tests/.DS_Store` & `dymoval-0.8.83/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.82/tests/fixture_data.py` & `dymoval-0.8.83/tests/fixture_data.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.82/tests/test_dataset.py` & `dymoval-0.8.83/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.82/tests/test_initializers.py` & `dymoval-0.8.83/tests/test_initializers.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.82/tests/test_utils.py` & `dymoval-0.8.83/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.82/tests/test_validation.py` & `dymoval-0.8.83/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.82/PKG-INFO` & `dymoval-0.8.83/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dymoval
-Version: 0.8.82
+Version: 0.8.83
 Summary: Dymoval is a Python package for validating models and analyzing datasets.
 Keywords: data-analysis modeling model validation dataset data
 Author-Email: Ubaldo Tiberi <ubaldo.tiberi@volvo.com>, Ubaldo Tiberi <ubaldo.tiberi@gmail.com>
 License: BSD 3-Clause License
         
         Author: Ubaldo Tiberi.
         Copyright (c) 2023, Ubaldo Tiberi
@@ -41,15 +41,14 @@
 Project-URL: Documentation, https://volvogroup.github.io/dymoval/
 Project-URL: Bug tracker, https://github.com/VolvoGroup/dymoval/issues
 Requires-Python: >=3.10
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: scipy
 Requires-Dist: control
-Requires-Dist: pathlib
 Requires-Dist: numpy
 Requires-Dist: tomli
 Requires-Dist: h5py
 Requires-Dist: pdm; extra == "build"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: furo; extra == "dev"
 Requires-Dist: sphinx-toolbox; extra == "dev"
```

