# Comparing `tmp/dymoval-0.8.8.tar.gz` & `tmp/dymoval-0.8.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dymoval-0.8.8.tar", last modified: Tue May 16 08:26:34 2023, max compression
+gzip compressed data, was "dymoval-0.8.81.tar", last modified: Tue May 16 12:25:37 2023, max compression
```

## Comparing `dymoval-0.8.8.tar` & `dymoval-0.8.81.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1536 2023-05-16 08:21:52.083500 dymoval-0.8.8/LICENSE
--rw-r--r--   0        0        0     4475 2023-05-15 07:01:30.761752 dymoval-0.8.8/README.md
--rw-r--r--   0        0        0     1922 2023-05-16 08:26:34.691499 dymoval-0.8.8/pyproject.toml
--rw-r--r--   0        0        0      125 2023-05-14 20:41:41.380658 dymoval-0.8.8/src/dymoval/__init__.py
--rw-r--r--   0        0        0     1332 2023-05-15 08:02:53.628954 dymoval-0.8.8/src/dymoval/config.py
--rw-r--r--   0        0        0   112805 2023-05-14 20:41:41.381154 dymoval-0.8.8/src/dymoval/dataset.py
--rw-r--r--   0        0        0     2543 2023-05-15 10:15:47.636362 dymoval-0.8.8/src/dymoval/utils.py
--rw-r--r--   0        0        0    32835 2023-05-14 20:41:41.381401 dymoval-0.8.8/src/dymoval/validation.py
--rw-r--r--   0        0        0    65913 2023-05-14 20:41:41.381658 dymoval-0.8.8/src/tutorial/DCMotor.fmu
--rw-r--r--   0        0        0  1136010 2023-05-14 20:41:41.386937 dymoval-0.8.8/src/tutorial/DCMotor.svg
--rw-r--r--   0        0        0   963816 2023-05-14 20:41:41.391006 dymoval-0.8.8/src/tutorial/DCMotorLogs.h5
--rw-r--r--   0        0        0      798 2023-05-14 20:41:41.391222 dymoval-0.8.8/src/tutorial/DCMotorModel.py
--rw-r--r--   0        0        0        0 2023-05-14 20:41:41.391250 dymoval-0.8.8/src/tutorial/__init__.py
--rw-r--r--   0        0        0    34918 2023-05-14 20:41:41.391446 dymoval-0.8.8/src/tutorial/tutorial.ipynb
--rw-r--r--   0        0        0        0 2023-05-14 20:41:41.391484 dymoval-0.8.8/tests/__init__.py
--rw-r--r--   0        0        0    12028 2023-05-14 20:41:41.391579 dymoval-0.8.8/tests/fixture_data.py
--rw-r--r--   0        0        0    54384 2023-05-14 20:41:41.391755 dymoval-0.8.8/tests/test_dataset.py
--rw-r--r--   0        0        0    12437 2023-05-14 20:41:41.391860 dymoval-0.8.8/tests/test_initializers.py
--rw-r--r--   0        0        0     3216 2023-05-14 20:41:41.391927 dymoval-0.8.8/tests/test_utils.py
--rw-r--r--   0        0        0    26580 2023-05-14 20:41:41.392032 dymoval-0.8.8/tests/test_validation.py
--rw-r--r--   0        0        0     7503 1970-01-01 00:00:00.000000 dymoval-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0     1536 2023-05-16 08:21:52.083500 dymoval-0.8.81/LICENSE
+-rw-r--r--   0        0        0     4475 2023-05-15 07:01:30.761752 dymoval-0.8.81/README.md
+-rw-r--r--   0        0        0     1923 2023-05-16 12:25:37.651342 dymoval-0.8.81/pyproject.toml
+-rw-r--r--   0        0        0      125 2023-05-14 20:41:41.380658 dymoval-0.8.81/src/dymoval/__init__.py
+-rw-r--r--   0        0        0     1332 2023-05-15 08:02:53.628954 dymoval-0.8.81/src/dymoval/config.py
+-rw-r--r--   0        0        0   112805 2023-05-14 20:41:41.381154 dymoval-0.8.81/src/dymoval/dataset.py
+-rw-r--r--   0        0        0     2543 2023-05-15 10:15:47.636362 dymoval-0.8.81/src/dymoval/utils.py
+-rw-r--r--   0        0        0    32835 2023-05-14 20:41:41.381401 dymoval-0.8.81/src/dymoval/validation.py
+-rw-r--r--   0        0        0    65913 2023-05-14 20:41:41.381658 dymoval-0.8.81/src/tutorial/DCMotor.fmu
+-rw-r--r--   0        0        0  1136010 2023-05-14 20:41:41.386937 dymoval-0.8.81/src/tutorial/DCMotor.svg
+-rw-r--r--   0        0        0   963816 2023-05-14 20:41:41.391006 dymoval-0.8.81/src/tutorial/DCMotorLogs.h5
+-rw-r--r--   0        0        0      798 2023-05-14 20:41:41.391222 dymoval-0.8.81/src/tutorial/DCMotorModel.py
+-rw-r--r--   0        0        0        0 2023-05-14 20:41:41.391250 dymoval-0.8.81/src/tutorial/__init__.py
+-rw-r--r--   0        0        0    34918 2023-05-14 20:41:41.391446 dymoval-0.8.81/src/tutorial/tutorial.ipynb
+-rw-r--r--   0        0        0     6148 2023-05-16 12:22:44.602879 dymoval-0.8.81/tests/.DS_Store
+-rw-r--r--   0        0        0    12028 2023-05-14 20:41:41.391579 dymoval-0.8.81/tests/fixture_data.py
+-rw-r--r--   0        0        0    54384 2023-05-14 20:41:41.391755 dymoval-0.8.81/tests/test_dataset.py
+-rw-r--r--   0        0        0    12437 2023-05-14 20:41:41.391860 dymoval-0.8.81/tests/test_initializers.py
+-rw-r--r--   0        0        0     3216 2023-05-14 20:41:41.391927 dymoval-0.8.81/tests/test_utils.py
+-rw-r--r--   0        0        0    26580 2023-05-14 20:41:41.392032 dymoval-0.8.81/tests/test_validation.py
+-rw-r--r--   0        0        0     7504 1970-01-01 00:00:00.000000 dymoval-0.8.81/PKG-INFO
```

### Comparing `dymoval-0.8.8/LICENSE` & `dymoval-0.8.81/LICENSE`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.8/README.md` & `dymoval-0.8.81/README.md`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.8/pyproject.toml` & `dymoval-0.8.81/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "dymoval"
-version = "0.8.8"
+version = "0.8.81"
 requires-python = ">=3.10"
 dependencies = [
     "pandas",
     "matplotlib",
     "scipy",
     "control",
     "pathlib",
```

### Comparing `dymoval-0.8.8/src/dymoval/config.py` & `dymoval-0.8.81/src/dymoval/config.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.8/src/dymoval/dataset.py` & `dymoval-0.8.81/src/dymoval/dataset.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.8/src/dymoval/utils.py` & `dymoval-0.8.81/src/dymoval/utils.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.8/src/dymoval/validation.py` & `dymoval-0.8.81/src/dymoval/validation.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.8/src/tutorial/DCMotor.fmu` & `dymoval-0.8.81/src/tutorial/DCMotor.fmu`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.8/src/tutorial/DCMotor.svg` & `dymoval-0.8.81/src/tutorial/DCMotor.svg`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.8/src/tutorial/DCMotorLogs.h5` & `dymoval-0.8.81/src/tutorial/DCMotorLogs.h5`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.8/src/tutorial/DCMotorModel.py` & `dymoval-0.8.81/src/tutorial/DCMotorModel.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.8/src/tutorial/tutorial.ipynb` & `dymoval-0.8.81/src/tutorial/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.8/tests/fixture_data.py` & `dymoval-0.8.81/tests/fixture_data.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.8/tests/test_dataset.py` & `dymoval-0.8.81/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.8/tests/test_initializers.py` & `dymoval-0.8.81/tests/test_initializers.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.8/tests/test_utils.py` & `dymoval-0.8.81/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.8/tests/test_validation.py` & `dymoval-0.8.81/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.8/PKG-INFO` & `dymoval-0.8.81/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dymoval
-Version: 0.8.8
+Version: 0.8.81
 Summary: Dymoval is a Python package for validating models and analyzing datasets.
 Keywords: data-analysis modeling model validation dataset data
 Author-Email: Ubaldo Tiberi <ubaldo.tiberi@volvo.com>, Ubaldo Tiberi <ubaldo.tiberi@gmail.com>
 License: BSD 3-Clause License
         
         Author: Ubaldo Tiberi.
         Copyright (c) 2023, Ubaldo Tiberi
```

