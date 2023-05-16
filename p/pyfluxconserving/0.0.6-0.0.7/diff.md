# Comparing `tmp/pyfluxconserving-0.0.6.tar.gz` & `tmp/pyfluxconserving-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfluxconserving-0.0.6.tar", last modified: Thu Feb 23 11:52:42 2023, max compression
+gzip compressed data, was "pyfluxconserving-0.0.7.tar", last modified: Thu Feb 23 11:54:46 2023, max compression
```

## Comparing `pyfluxconserving-0.0.6.tar` & `pyfluxconserving-0.0.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-02-23 11:52:42.660730 pyfluxconserving-0.0.6/
--rw-r--r--   0 jean      (1000) users      (100)      894 2023-02-09 12:42:43.000000 pyfluxconserving-0.0.6/LICENSE.txt
--rw-r--r--   0 jean      (1000) users      (100)    14994 2023-02-23 11:52:42.660730 pyfluxconserving-0.0.6/PKG-INFO
--rw-r--r--   0 jean      (1000) users      (100)    14508 2023-02-23 11:33:27.000000 pyfluxconserving-0.0.6/README.md
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-02-23 11:52:42.656730 pyfluxconserving-0.0.6/pyfluxconserving.egg-info/
--rw-r--r--   0 jean      (1000) users      (100)    14994 2023-02-23 11:52:42.000000 pyfluxconserving-0.0.6/pyfluxconserving.egg-info/PKG-INFO
--rw-r--r--   0 jean      (1000) users      (100)      775 2023-02-23 11:52:42.000000 pyfluxconserving-0.0.6/pyfluxconserving.egg-info/SOURCES.txt
--rw-r--r--   0 jean      (1000) users      (100)        1 2023-02-23 11:52:42.000000 pyfluxconserving-0.0.6/pyfluxconserving.egg-info/dependency_links.txt
--rw-r--r--   0 jean      (1000) users      (100)       17 2023-02-23 11:52:42.000000 pyfluxconserving-0.0.6/pyfluxconserving.egg-info/requires.txt
--rw-r--r--   0 jean      (1000) users      (100)       17 2023-02-23 11:52:42.000000 pyfluxconserving-0.0.6/pyfluxconserving.egg-info/top_level.txt
--rw-r--r--   0 jean      (1000) users      (100)       38 2023-02-23 11:52:42.660730 pyfluxconserving-0.0.6/setup.cfg
--rw-r--r--   0 jean      (1000) users      (100)     1578 2023-02-23 11:52:20.000000 pyfluxconserving-0.0.6/setup.py
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-02-23 11:52:42.656730 pyfluxconserving-0.0.6/src/
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-02-23 11:52:42.656730 pyfluxconserving-0.0.6/src/fortran/
--rwxrwxrwx   0 jean      (1000) users      (100)    30528 2023-02-16 11:45:00.000000 pyfluxconserving-0.0.6/src/fortran/AkimaSpline.f90
--rwxr-xr-x   0 jean      (1000) users      (100)     1473 2023-02-16 10:55:29.000000 pyfluxconserving-0.0.6/src/fortran/DataTypes.f90
--rwxr-xr-x   0 jean      (1000) users      (100)    34014 2023-02-20 18:33:19.000000 pyfluxconserving-0.0.6/src/fortran/FluxConSpec.f90
--rwxrwxrwx   0 jean      (1000) users      (100)     6629 2023-02-16 11:50:43.000000 pyfluxconserving-0.0.6/src/fortran/Interpolado.f90
--rwxr-xr-x   0 jean      (1000) users      (100)     7586 2023-02-16 11:50:20.000000 pyfluxconserving-0.0.6/src/fortran/LINdexerpol.f90
--rwxr-xr-x   0 jean      (1000) users      (100)    11154 2023-02-12 17:59:45.000000 pyfluxconserving-0.0.6/src/fortran/LINinterpol.f90
--rwxr-xr-x   0 jean      (1000) users      (100)     8245 2023-02-16 11:48:58.000000 pyfluxconserving-0.0.6/src/fortran/SPLINE1DArr.f90
--rwxrwxrwx   0 jean      (1000) users      (100)    25721 2023-02-20 14:25:30.000000 pyfluxconserving-0.0.6/src/fortran/SPLINE3DFor.f90
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-02-23 11:52:42.660730 pyfluxconserving-0.0.6/src/python/
--rwxr--r--   0 jean      (1000) users      (100)    27805 2023-02-20 16:21:46.000000 pyfluxconserving-0.0.6/src/python/PyAkimaSpline.py
--rwxrwxrwx   0 jean      (1000) users      (100)    24871 2023-02-20 16:22:02.000000 pyfluxconserving-0.0.6/src/python/PyFluxConSpec.py
--rwxrw-rw-   0 jean      (1000) users      (100)    16685 2023-02-20 16:21:37.000000 pyfluxconserving-0.0.6/src/python/PyInterpolado.py
--rwxrw-rw-   0 jean      (1000) users      (100)    16617 2023-02-20 16:21:26.000000 pyfluxconserving-0.0.6/src/python/PyLINdexerpol.py
--rwxrw-rw-   0 jean      (1000) users      (100)    18028 2023-02-20 16:23:39.000000 pyfluxconserving-0.0.6/src/python/PyLINinterpol.py
--rwxrwxrwx   0 jean      (1000) users      (100)     8043 2022-04-14 17:45:45.000000 pyfluxconserving-0.0.6/src/python/PyLinear__int.py
--rwxr--r--   0 jean      (1000) users      (100)    16669 2023-02-20 16:25:03.000000 pyfluxconserving-0.0.6/src/python/PySPLINE1DArr.py
--rwxr--r--   0 jean      (1000) users      (100)    25688 2023-02-20 16:26:02.000000 pyfluxconserving-0.0.6/src/python/PySPLINE3DFor.py
--rw-r--r--   0 jean      (1000) users      (100)        0 2023-02-16 11:55:15.000000 pyfluxconserving-0.0.6/src/python/__init__.py
--rwxrwxrwx   0 jean      (1000) users      (100)     1146 2019-09-06 10:48:20.000000 pyfluxconserving-0.0.6/src/python/califa_cmap_alternative.py
--rwxrwxrwx   0 jean      (1000) users      (100)     4098 2023-02-20 12:31:02.000000 pyfluxconserving-0.0.6/src/python/fluxconserve.py
--rw-r--r--   0 jean      (1000) users      (100)        6 2023-02-23 11:52:05.000000 pyfluxconserving-0.0.6/version.txt
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-02-23 11:54:46.124727 pyfluxconserving-0.0.7/
+-rw-r--r--   0 jean      (1000) users      (100)      894 2023-02-09 12:42:43.000000 pyfluxconserving-0.0.7/LICENSE.txt
+-rw-r--r--   0 jean      (1000) users      (100)    15108 2023-02-23 11:54:46.124727 pyfluxconserving-0.0.7/PKG-INFO
+-rw-r--r--   0 jean      (1000) users      (100)    14508 2023-02-23 11:33:27.000000 pyfluxconserving-0.0.7/README.md
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-02-23 11:54:46.120727 pyfluxconserving-0.0.7/pyfluxconserving.egg-info/
+-rw-r--r--   0 jean      (1000) users      (100)    15108 2023-02-23 11:54:45.000000 pyfluxconserving-0.0.7/pyfluxconserving.egg-info/PKG-INFO
+-rw-r--r--   0 jean      (1000) users      (100)      775 2023-02-23 11:54:46.000000 pyfluxconserving-0.0.7/pyfluxconserving.egg-info/SOURCES.txt
+-rw-r--r--   0 jean      (1000) users      (100)        1 2023-02-23 11:54:45.000000 pyfluxconserving-0.0.7/pyfluxconserving.egg-info/dependency_links.txt
+-rw-r--r--   0 jean      (1000) users      (100)       17 2023-02-23 11:54:46.000000 pyfluxconserving-0.0.7/pyfluxconserving.egg-info/requires.txt
+-rw-r--r--   0 jean      (1000) users      (100)       17 2023-02-23 11:54:46.000000 pyfluxconserving-0.0.7/pyfluxconserving.egg-info/top_level.txt
+-rw-r--r--   0 jean      (1000) users      (100)       38 2023-02-23 11:54:46.124727 pyfluxconserving-0.0.7/setup.cfg
+-rw-r--r--   0 jean      (1000) users      (100)     1692 2023-02-23 11:54:16.000000 pyfluxconserving-0.0.7/setup.py
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-02-23 11:54:46.120727 pyfluxconserving-0.0.7/src/
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-02-23 11:54:46.124727 pyfluxconserving-0.0.7/src/fortran/
+-rwxrwxrwx   0 jean      (1000) users      (100)    30528 2023-02-16 11:45:00.000000 pyfluxconserving-0.0.7/src/fortran/AkimaSpline.f90
+-rwxr-xr-x   0 jean      (1000) users      (100)     1473 2023-02-16 10:55:29.000000 pyfluxconserving-0.0.7/src/fortran/DataTypes.f90
+-rwxr-xr-x   0 jean      (1000) users      (100)    34014 2023-02-20 18:33:19.000000 pyfluxconserving-0.0.7/src/fortran/FluxConSpec.f90
+-rwxrwxrwx   0 jean      (1000) users      (100)     6629 2023-02-16 11:50:43.000000 pyfluxconserving-0.0.7/src/fortran/Interpolado.f90
+-rwxr-xr-x   0 jean      (1000) users      (100)     7586 2023-02-16 11:50:20.000000 pyfluxconserving-0.0.7/src/fortran/LINdexerpol.f90
+-rwxr-xr-x   0 jean      (1000) users      (100)    11154 2023-02-12 17:59:45.000000 pyfluxconserving-0.0.7/src/fortran/LINinterpol.f90
+-rwxr-xr-x   0 jean      (1000) users      (100)     8245 2023-02-16 11:48:58.000000 pyfluxconserving-0.0.7/src/fortran/SPLINE1DArr.f90
+-rwxrwxrwx   0 jean      (1000) users      (100)    25721 2023-02-20 14:25:30.000000 pyfluxconserving-0.0.7/src/fortran/SPLINE3DFor.f90
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-02-23 11:54:46.124727 pyfluxconserving-0.0.7/src/python/
+-rwxr--r--   0 jean      (1000) users      (100)    27805 2023-02-20 16:21:46.000000 pyfluxconserving-0.0.7/src/python/PyAkimaSpline.py
+-rwxrwxrwx   0 jean      (1000) users      (100)    24871 2023-02-20 16:22:02.000000 pyfluxconserving-0.0.7/src/python/PyFluxConSpec.py
+-rwxrw-rw-   0 jean      (1000) users      (100)    16685 2023-02-20 16:21:37.000000 pyfluxconserving-0.0.7/src/python/PyInterpolado.py
+-rwxrw-rw-   0 jean      (1000) users      (100)    16617 2023-02-20 16:21:26.000000 pyfluxconserving-0.0.7/src/python/PyLINdexerpol.py
+-rwxrw-rw-   0 jean      (1000) users      (100)    18028 2023-02-20 16:23:39.000000 pyfluxconserving-0.0.7/src/python/PyLINinterpol.py
+-rwxrwxrwx   0 jean      (1000) users      (100)     8043 2022-04-14 17:45:45.000000 pyfluxconserving-0.0.7/src/python/PyLinear__int.py
+-rwxr--r--   0 jean      (1000) users      (100)    16669 2023-02-20 16:25:03.000000 pyfluxconserving-0.0.7/src/python/PySPLINE1DArr.py
+-rwxr--r--   0 jean      (1000) users      (100)    25688 2023-02-20 16:26:02.000000 pyfluxconserving-0.0.7/src/python/PySPLINE3DFor.py
+-rw-r--r--   0 jean      (1000) users      (100)        0 2023-02-16 11:55:15.000000 pyfluxconserving-0.0.7/src/python/__init__.py
+-rwxrwxrwx   0 jean      (1000) users      (100)     1146 2019-09-06 10:48:20.000000 pyfluxconserving-0.0.7/src/python/califa_cmap_alternative.py
+-rwxrwxrwx   0 jean      (1000) users      (100)     4098 2023-02-20 12:31:02.000000 pyfluxconserving-0.0.7/src/python/fluxconserve.py
+-rw-r--r--   0 jean      (1000) users      (100)        6 2023-02-23 11:54:21.000000 pyfluxconserving-0.0.7/version.txt
```

### Comparing `pyfluxconserving-0.0.6/LICENSE.txt` & `pyfluxconserving-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.6/PKG-INFO` & `pyfluxconserving-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyfluxconserving
-Version: 0.0.6
-Summary: Flux-conserving legacy routines in Fortran and Python
+Version: 0.0.7
+Summary: FluxConserving is a set of Fortran 2003+ legacy routines with Python. There are some options for the flux-conserving algorithm. It also includes interpolation scripts.
 Home-page: https://github.com/neutrinomuon/Pyfluxconserving
 Author: Jean Gomes
 Author-email: antineutrinomuon@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Fortran
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: pyfluxconserving Version: 0.0.6 Summary: Flux-
-conserving legacy routines in Fortran and Python Home-page: https://github.com/
-neutrinomuon/Pyfluxconserving Author: Jean Gomes Author-email:
-antineutrinomuon@gmail.com License: UNKNOWN Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Fortran
-Classifier: Operating System :: OS Independent Description-Content-Type: text/
-markdown License-File: LICENSE.txt ### FluxConserving #### A Fortran legacy
-package to easily compute the flux-density conservation Obs.: A Fortran legacy
-Interpolation routines also furnished
+Metadata-Version: 2.1 Name: pyfluxconserving Version: 0.0.7 Summary:
+FluxConserving is a set of Fortran 2003+ legacy routines with Python. There are
+some options for the flux-conserving algorithm. It also includes interpolation
+scripts. Home-page: https://github.com/neutrinomuon/Pyfluxconserving Author:
+Jean Gomes Author-email: antineutrinomuon@gmail.com License: UNKNOWN Platform:
+UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Fortran Classifier: Operating System :: OS Independent Description-
+Content-Type: text/markdown License-File: LICENSE.txt ### FluxConserving #### A
+Fortran legacy package to easily compute the flux-density conservation Obs.: A
+Fortran legacy Interpolation routines also furnished
 email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com),
 [jean@astro.up.pt](mailto:jean@astro.up.pt) Â© Copyright Â® J.G. - Jean Gomes
 ===============================================================================
 [![My Skills](https://skillicons.dev/
 icons?i=python,fortran,c,numpy&theme=light)](https://skillicons.dev)
 [![python3](https://img.shields.io/pypi/pyversions/pyfluxconserving)](https://
 img.shields.io/pypi/pyversions/pyfluxconserving) [![badgetlicense](https://
```

### Comparing `pyfluxconserving-0.0.6/README.md` & `pyfluxconserving-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.6/pyfluxconserving.egg-info/PKG-INFO` & `pyfluxconserving-0.0.7/pyfluxconserving.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyfluxconserving
-Version: 0.0.6
-Summary: Flux-conserving legacy routines in Fortran and Python
+Version: 0.0.7
+Summary: FluxConserving is a set of Fortran 2003+ legacy routines with Python. There are some options for the flux-conserving algorithm. It also includes interpolation scripts.
 Home-page: https://github.com/neutrinomuon/Pyfluxconserving
 Author: Jean Gomes
 Author-email: antineutrinomuon@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Fortran
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: pyfluxconserving Version: 0.0.6 Summary: Flux-
-conserving legacy routines in Fortran and Python Home-page: https://github.com/
-neutrinomuon/Pyfluxconserving Author: Jean Gomes Author-email:
-antineutrinomuon@gmail.com License: UNKNOWN Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Fortran
-Classifier: Operating System :: OS Independent Description-Content-Type: text/
-markdown License-File: LICENSE.txt ### FluxConserving #### A Fortran legacy
-package to easily compute the flux-density conservation Obs.: A Fortran legacy
-Interpolation routines also furnished
+Metadata-Version: 2.1 Name: pyfluxconserving Version: 0.0.7 Summary:
+FluxConserving is a set of Fortran 2003+ legacy routines with Python. There are
+some options for the flux-conserving algorithm. It also includes interpolation
+scripts. Home-page: https://github.com/neutrinomuon/Pyfluxconserving Author:
+Jean Gomes Author-email: antineutrinomuon@gmail.com License: UNKNOWN Platform:
+UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Fortran Classifier: Operating System :: OS Independent Description-
+Content-Type: text/markdown License-File: LICENSE.txt ### FluxConserving #### A
+Fortran legacy package to easily compute the flux-density conservation Obs.: A
+Fortran legacy Interpolation routines also furnished
 email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com),
 [jean@astro.up.pt](mailto:jean@astro.up.pt) Â© Copyright Â® J.G. - Jean Gomes
 ===============================================================================
 [![My Skills](https://skillicons.dev/
 icons?i=python,fortran,c,numpy&theme=light)](https://skillicons.dev)
 [![python3](https://img.shields.io/pypi/pyversions/pyfluxconserving)](https://
 img.shields.io/pypi/pyversions/pyfluxconserving) [![badgetlicense](https://
```

### Comparing `pyfluxconserving-0.0.6/pyfluxconserving.egg-info/SOURCES.txt` & `pyfluxconserving-0.0.7/pyfluxconserving.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.6/src/fortran/AkimaSpline.f90` & `pyfluxconserving-0.0.7/src/fortran/AkimaSpline.f90`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.6/src/fortran/DataTypes.f90` & `pyfluxconserving-0.0.7/src/fortran/DataTypes.f90`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.6/src/fortran/FluxConSpec.f90` & `pyfluxconserving-0.0.7/src/fortran/FluxConSpec.f90`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.6/src/fortran/Interpolado.f90` & `pyfluxconserving-0.0.7/src/fortran/Interpolado.f90`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.6/src/fortran/LINdexerpol.f90` & `pyfluxconserving-0.0.7/src/fortran/LINdexerpol.f90`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.6/src/fortran/LINinterpol.f90` & `pyfluxconserving-0.0.7/src/fortran/LINinterpol.f90`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.6/src/fortran/SPLINE1DArr.f90` & `pyfluxconserving-0.0.7/src/fortran/SPLINE1DArr.f90`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.6/src/fortran/SPLINE3DFor.f90` & `pyfluxconserving-0.0.7/src/fortran/SPLINE3DFor.f90`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.6/src/python/PyAkimaSpline.py` & `pyfluxconserving-0.0.7/src/python/PyAkimaSpline.py`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.6/src/python/PyFluxConSpec.py` & `pyfluxconserving-0.0.7/src/python/PyFluxConSpec.py`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.6/src/python/PyInterpolado.py` & `pyfluxconserving-0.0.7/src/python/PyInterpolado.py`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.6/src/python/PyLINdexerpol.py` & `pyfluxconserving-0.0.7/src/python/PyLINdexerpol.py`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.6/src/python/PyLINinterpol.py` & `pyfluxconserving-0.0.7/src/python/PyLINinterpol.py`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.6/src/python/PyLinear__int.py` & `pyfluxconserving-0.0.7/src/python/PyLinear__int.py`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.6/src/python/PySPLINE1DArr.py` & `pyfluxconserving-0.0.7/src/python/PySPLINE1DArr.py`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.6/src/python/PySPLINE3DFor.py` & `pyfluxconserving-0.0.7/src/python/PySPLINE3DFor.py`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.6/src/python/califa_cmap_alternative.py` & `pyfluxconserving-0.0.7/src/python/califa_cmap_alternative.py`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.6/src/python/fluxconserve.py` & `pyfluxconserving-0.0.7/src/python/fluxconserve.py`

 * *Files identical despite different names*

