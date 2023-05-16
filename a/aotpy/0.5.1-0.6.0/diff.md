# Comparing `tmp/aotpy-0.5.1.tar.gz` & `tmp/aotpy-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aotpy-0.5.1.tar", last modified: Wed May 10 15:48:30 2023, max compression
+gzip compressed data, was "aotpy-0.6.0.tar", last modified: Tue May 16 13:18:11 2023, max compression
```

## Comparing `aotpy-0.5.1.tar` & `aotpy-0.6.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 15:48:30.018127 aotpy-0.5.1/
--rw-rw-rw-   0        0        0     1592 2022-07-17 01:57:35.000000 aotpy-0.5.1/LICENSE
--rw-rw-rw-   0        0        0     2991 2023-05-10 15:48:30.018127 aotpy-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     2198 2023-05-02 22:45:22.000000 aotpy-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 15:48:29.936101 aotpy-0.5.1/aotpy/
--rw-rw-rw-   0        0        0      521 2023-05-03 10:25:00.000000 aotpy-0.5.1/aotpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 15:48:29.965396 aotpy-0.5.1/aotpy/core/
--rw-rw-rw-   0        0        0      580 2023-04-19 14:10:55.000000 aotpy-0.5.1/aotpy/core/__init__.py
--rw-rw-rw-   0        0        0     1073 2023-05-02 09:36:00.000000 aotpy-0.5.1/aotpy/core/aberration.py
--rw-rw-rw-   0        0        0     3967 2023-05-03 10:26:29.000000 aotpy-0.5.1/aotpy/core/ao_system.py
--rw-rw-rw-   0        0        0     2227 2023-05-02 09:36:11.000000 aotpy-0.5.1/aotpy/core/atmosphere.py
--rw-rw-rw-   0        0        0      618 2023-05-03 10:52:05.000000 aotpy-0.5.1/aotpy/core/base.py
--rw-rw-rw-   0        0        0     1177 2023-05-02 18:40:00.000000 aotpy-0.5.1/aotpy/core/geometry.py
--rw-rw-rw-   0        0        0     1840 2023-05-02 13:49:09.000000 aotpy-0.5.1/aotpy/core/image.py
--rw-rw-rw-   0        0        0     4706 2023-05-02 09:40:01.000000 aotpy-0.5.1/aotpy/core/loop.py
--rw-rw-rw-   0        0        0     8912 2023-05-02 18:10:07.000000 aotpy-0.5.1/aotpy/core/optical_sensor.py
--rw-rw-rw-   0        0        0     2701 2023-05-02 09:42:13.000000 aotpy-0.5.1/aotpy/core/source.py
--rw-rw-rw-   0        0        0     4059 2023-05-02 18:40:18.000000 aotpy-0.5.1/aotpy/core/telescope.py
--rw-rw-rw-   0        0        0      708 2023-05-02 09:43:33.000000 aotpy-0.5.1/aotpy/core/time.py
--rw-rw-rw-   0        0        0     2728 2023-05-02 09:43:55.000000 aotpy-0.5.1/aotpy/core/wavefront_corrector.py
-drwxrwxrwx   0        0        0        0 2023-05-10 15:48:29.967349 aotpy-0.5.1/aotpy/io/
--rw-rw-rw-   0        0        0      436 2023-05-02 11:33:11.000000 aotpy-0.5.1/aotpy/io/__init__.py
--rw-rw-rw-   0        0        0     2785 2023-05-02 11:47:25.000000 aotpy-0.5.1/aotpy/io/base.py
-drwxrwxrwx   0        0        0        0 2023-05-10 15:48:30.008363 aotpy-0.5.1/aotpy/io/fits/
--rw-rw-rw-   0        0        0      200 2023-05-02 13:23:11.000000 aotpy-0.5.1/aotpy/io/fits/__init__.py
--rw-rw-rw-   0        0        0    27401 2023-05-03 11:20:21.000000 aotpy-0.5.1/aotpy/io/fits/_keywords.py
--rw-rw-rw-   0        0        0    43132 2023-05-03 10:32:11.000000 aotpy-0.5.1/aotpy/io/fits/reader.py
--rw-rw-rw-   0        0        0     8760 2023-05-03 10:32:11.000000 aotpy-0.5.1/aotpy/io/fits/utils.py
--rw-rw-rw-   0        0        0    31576 2023-05-03 10:58:25.000000 aotpy-0.5.1/aotpy/io/fits/writer.py
-drwxrwxrwx   0        0        0        0 2023-05-10 15:48:30.015198 aotpy-0.5.1/aotpy/translators/
--rw-rw-rw-   0        0        0      358 2023-05-02 17:59:07.000000 aotpy-0.5.1/aotpy/translators/__init__.py
--rw-rw-rw-   0        0        0    11862 2023-05-03 11:33:12.000000 aotpy-0.5.1/aotpy/translators/aof.py
--rw-rw-rw-   0        0        0      979 2023-05-02 18:03:17.000000 aotpy-0.5.1/aotpy/translators/base.py
--rw-rw-rw-   0        0        0     7404 2023-05-02 17:56:25.000000 aotpy-0.5.1/aotpy/translators/ciao.py
--rw-rw-rw-   0        0        0     8553 2023-05-02 18:43:53.000000 aotpy-0.5.1/aotpy/translators/eso.py
--rw-rw-rw-   0        0        0     6487 2023-05-02 17:55:46.000000 aotpy-0.5.1/aotpy/translators/naomi.py
-drwxrwxrwx   0        0        0        0 2023-05-10 15:48:29.950748 aotpy-0.5.1/aotpy.egg-info/
--rw-rw-rw-   0        0        0     2991 2023-05-10 15:48:29.000000 aotpy-0.5.1/aotpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      847 2023-05-10 15:48:29.000000 aotpy-0.5.1/aotpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 15:48:29.000000 aotpy-0.5.1/aotpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2023-05-10 15:48:29.000000 aotpy-0.5.1/aotpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-10 15:48:29.000000 aotpy-0.5.1/aotpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 15:48:30.017151 aotpy-0.5.1/data/
--rw-rw-rw-   0        0        0      105 2023-05-02 18:50:46.000000 aotpy-0.5.1/data/__init__.py
--rw-rw-rw-   0        0        0      108 2021-11-05 13:42:41.000000 aotpy-0.5.1/pyproject.toml
--rw-rw-rw-   0        0        0      982 2023-05-10 15:48:30.020080 aotpy-0.5.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 13:18:11.782788 aotpy-0.6.0/
+-rw-rw-rw-   0        0        0     1592 2022-07-17 01:57:35.000000 aotpy-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     2991 2023-05-16 13:18:11.782788 aotpy-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2198 2023-05-02 22:45:22.000000 aotpy-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 13:18:11.557841 aotpy-0.6.0/aotpy/
+-rw-rw-rw-   0        0        0      521 2023-05-03 10:25:00.000000 aotpy-0.6.0/aotpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:18:11.704111 aotpy-0.6.0/aotpy/core/
+-rw-rw-rw-   0        0        0      555 2023-05-08 11:52:45.000000 aotpy-0.6.0/aotpy/core/__init__.py
+-rw-rw-rw-   0        0        0     1073 2023-05-02 09:36:00.000000 aotpy-0.6.0/aotpy/core/aberration.py
+-rw-rw-rw-   0        0        0     3967 2023-05-03 10:26:29.000000 aotpy-0.6.0/aotpy/core/ao_system.py
+-rw-rw-rw-   0        0        0     3050 2023-05-08 11:38:37.000000 aotpy-0.6.0/aotpy/core/atmosphere.py
+-rw-rw-rw-   0        0        0      618 2023-05-03 10:52:05.000000 aotpy-0.6.0/aotpy/core/base.py
+-rw-rw-rw-   0        0        0     1177 2023-05-02 18:40:00.000000 aotpy-0.6.0/aotpy/core/geometry.py
+-rw-rw-rw-   0        0        0     1840 2023-05-02 13:49:09.000000 aotpy-0.6.0/aotpy/core/image.py
+-rw-rw-rw-   0        0        0     5293 2023-05-03 17:08:11.000000 aotpy-0.6.0/aotpy/core/loop.py
+-rw-rw-rw-   0        0        0    11452 2023-05-08 11:39:26.000000 aotpy-0.6.0/aotpy/core/optical_sensor.py
+-rw-rw-rw-   0        0        0     2701 2023-05-02 09:42:13.000000 aotpy-0.6.0/aotpy/core/source.py
+-rw-rw-rw-   0        0        0     4887 2023-05-08 11:39:26.000000 aotpy-0.6.0/aotpy/core/telescope.py
+-rw-rw-rw-   0        0        0      708 2023-05-02 09:43:33.000000 aotpy-0.6.0/aotpy/core/time.py
+-rw-rw-rw-   0        0        0     3554 2023-05-08 11:39:26.000000 aotpy-0.6.0/aotpy/core/wavefront_corrector.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:18:11.707039 aotpy-0.6.0/aotpy/io/
+-rw-rw-rw-   0        0        0      436 2023-05-02 11:33:11.000000 aotpy-0.6.0/aotpy/io/__init__.py
+-rw-rw-rw-   0        0        0     2785 2023-05-02 11:47:25.000000 aotpy-0.6.0/aotpy/io/base.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:18:11.739264 aotpy-0.6.0/aotpy/io/fits/
+-rw-rw-rw-   0        0        0      200 2023-05-02 13:23:11.000000 aotpy-0.6.0/aotpy/io/fits/__init__.py
+-rw-rw-rw-   0        0        0    26711 2023-05-16 13:12:55.000000 aotpy-0.6.0/aotpy/io/fits/_keywords.py
+-rw-rw-rw-   0        0        0    42036 2023-05-08 12:12:15.000000 aotpy-0.6.0/aotpy/io/fits/reader.py
+-rw-rw-rw-   0        0        0     8760 2023-05-03 10:32:11.000000 aotpy-0.6.0/aotpy/io/fits/utils.py
+-rw-rw-rw-   0        0        0    31083 2023-05-08 11:41:08.000000 aotpy-0.6.0/aotpy/io/fits/writer.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:18:11.770093 aotpy-0.6.0/aotpy/translators/
+-rw-rw-rw-   0        0        0      358 2023-05-02 17:59:07.000000 aotpy-0.6.0/aotpy/translators/__init__.py
+-rw-rw-rw-   0        0        0    11052 2023-05-15 11:30:25.000000 aotpy-0.6.0/aotpy/translators/aof.py
+-rw-rw-rw-   0        0        0      979 2023-05-02 18:03:17.000000 aotpy-0.6.0/aotpy/translators/base.py
+-rw-rw-rw-   0        0        0     6842 2023-05-15 12:17:23.000000 aotpy-0.6.0/aotpy/translators/ciao.py
+-rw-rw-rw-   0        0        0    14284 2023-05-15 11:20:25.000000 aotpy-0.6.0/aotpy/translators/eris.py
+-rw-rw-rw-   0        0        0     9095 2023-05-15 14:15:02.000000 aotpy-0.6.0/aotpy/translators/eso.py
+-rw-rw-rw-   0        0        0     7175 2023-05-16 13:06:00.000000 aotpy-0.6.0/aotpy/translators/naomi.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:18:11.593232 aotpy-0.6.0/aotpy.egg-info/
+-rw-rw-rw-   0        0        0     2991 2023-05-16 13:18:11.000000 aotpy-0.6.0/aotpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      873 2023-05-16 13:18:11.000000 aotpy-0.6.0/aotpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 13:18:11.000000 aotpy-0.6.0/aotpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2023-05-16 13:18:11.000000 aotpy-0.6.0/aotpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-16 13:18:11.000000 aotpy-0.6.0/aotpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 13:18:11.780865 aotpy-0.6.0/data/
+-rw-rw-rw-   0        0        0      105 2023-05-02 18:50:46.000000 aotpy-0.6.0/data/__init__.py
+-rw-rw-rw-   0        0        0      108 2021-11-05 13:42:41.000000 aotpy-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0      982 2023-05-16 13:18:11.791588 aotpy-0.6.0/setup.cfg
```

### Comparing `aotpy-0.5.1/LICENSE` & `aotpy-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.1/PKG-INFO` & `aotpy-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aotpy
-Version: 0.5.1
+Version: 0.6.0
 Summary: Helper package for handling Adaptive Optics Telemetry (AOT) standard files
 Home-page: https://github.com/kYwzor/aotpy
 Author: Tiago Gomes
 Author-email: tiagogomes@fe.up.pt
 Project-URL: Bug Tracker, https://github.com/kYwzor/aotpy/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aotpy-0.5.1/README.md` & `aotpy-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.1/aotpy/__init__.py` & `aotpy-0.6.0/aotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.1/aotpy/core/__init__.py` & `aotpy-0.6.0/aotpy/core/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 Note that all these functions and objects are available in the main ``aotpy`` namespace.
 """
 
 from .aberration import *
 from .ao_system import *
 from .atmosphere import *
 from .base import *
-from .geometry import *
 from .image import *
 from .loop import *
 from .optical_sensor import *
 from .source import *
 from .telescope import *
 from .time import *
 from .wavefront_corrector import *
```

### Comparing `aotpy-0.5.1/aotpy/core/aberration.py` & `aotpy-0.6.0/aotpy/core/aberration.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.1/aotpy/core/ao_system.py` & `aotpy-0.6.0/aotpy/core/ao_system.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.1/aotpy/core/base.py` & `aotpy-0.6.0/aotpy/core/base.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.1/aotpy/core/geometry.py` & `aotpy-0.6.0/aotpy/core/geometry.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.1/aotpy/core/image.py` & `aotpy-0.6.0/aotpy/core/image.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.1/aotpy/core/loop.py` & `aotpy-0.6.0/aotpy/core/loop.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,23 @@
 
 @dataclass(kw_only=True)
 class ControlLoop(Loop):
     """Contains data relevant to a control loop (relation between one wavefront sensor and one wavefront corrector)."""
 
     input_sensor: WavefrontSensor
 
+    modes: Image = None
+    """Set of :math:`m` different :math:`h \\times w` arrays, each representing the orthonormal basis of the
+    corresponding mode. (Dimensions :math:`m \\times h \\times w`, dimensionless quantity, using data type flt)"""
+
+    modal_coefficients: Image = None
+    """Sequence of coefficients of the modes to be corrected on the wavefront corrector. Each of the :math:`t` frames
+    contains the coefficients respective to each of the :math:`m` modes being corrected.
+    (Dimensions :math:`t \\times m`, in user defined units, using data type flt)"""
+
     control_matrix: Image = None
     """Linear relationship between the wavefront sensor measurements (:math:`d \\times s_v`) and the corrector commands 
     (:math:`a_v`). (Dimensions :math:`a_v \\times d \\times s_v`, in user defined units, using data type flt)"""
 
     measurements_to_modes: Image = None
     """Linear relationship between the wavefront sensor measurements (:math:`d \\times s_v`) and the modes to be
     corrected (:math:`m`). (Dimensions :math:`m \\times d \\times s_v`, in user defined units, using data type flt)"""
```

### Comparing `aotpy-0.5.1/aotpy/core/optical_sensor.py` & `aotpy-0.6.0/aotpy/core/optical_sensor.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 This includes scoring cameras and wavefront sensors, and their respective detectors.
 """
 
 from dataclasses import dataclass, field
 
 from .aberration import Aberration
 from .base import Referenceable, Coordinates
-from .geometry import Geometry
 from .image import Image
 from .source import Source
 
 __all__ = ['Detector', 'ScoringCamera', 'WavefrontSensor', 'ShackHartmann', 'Pyramid']
 
 
 @dataclass(kw_only=True)
@@ -99,29 +98,46 @@
     readout_rate: float = None
     r'Inverse of the time required to digitize a single pixel (in px s\ :math:`^{-1}` units)'
 
     frame_rate: float = None
     r"""Inverse of the time needed for the detector to acquire an image and then completely read it out.
     (in frame s\ :math:`^{-1}` units)"""
 
-    geometry: Geometry = None
+    transformation_matrix: Image = None
+    r"""Matrix that defines 2-dimensional affine transformations over time (:math:`t`) using homogeneous coordinates.
+    Any combination of translation, reflection, scale, rotation and shearing can be described via a single
+    :math:`3 \times 3` matrix :math:`M` such that :math:`P' = MP`, where :math:`P` is a
+    :math:`\begin{bmatrix}x & y & 1 \end{bmatrix}` vector (with :math:`x` and :math:`y` being the original horizontal 
+    and vertical coordinates, respectively) and :math:`P'` is a :math:`\begin{bmatrix}x' & y' & 1 \end{bmatrix}`, where
+    :math:`x'` and :math:`y'` are the transformed coordinates. All geometry information must be described relative to
+    the same reference origin point, from which transformations may occur.
+    (Dimensions :math:`3 \times 3 \times t`, dimensionless quantity, using data type flt)"""
 
 
 @dataclass(kw_only=True)
 class ScoringCamera(Referenceable):
     """Contains data regarding a scoring camera in the system."""
 
     pupil_mask: Image = None
     """Binary image that describes the shape of the pupil. A 1 indicates the presence of the pupil, while a 0 indicates
     the opposite. (Dimensions :math:`h \\times w`, dimensionless quantity, using data type int)"""
 
     wavelength: float = None
     """'Observation wavelength  (in m units)'"""
 
-    geometry: Geometry = None
+    transformation_matrix: Image = None
+    r"""Matrix that defines 2-dimensional affine transformations over time (:math:`t`) using homogeneous coordinates.
+    Any combination of translation, reflection, scale, rotation and shearing can be described via a single
+    :math:`3 \times 3` matrix :math:`M` such that :math:`P' = MP`, where :math:`P` is a
+    :math:`\begin{bmatrix}x & y & 1 \end{bmatrix}` vector (with :math:`x` and :math:`y` being the original horizontal 
+    and vertical coordinates, respectively) and :math:`P'` is a :math:`\begin{bmatrix}x' & y' & 1 \end{bmatrix}`, where
+    :math:`x'` and :math:`y'` are the transformed coordinates. All geometry information must be described relative to
+    the same reference origin point, from which transformations may occur.
+    (Dimensions :math:`3 \times 3 \times t`, dimensionless quantity, using data type flt)"""
+
     detector: Detector = None
     aberration: Aberration = None
 
 
 @dataclass(kw_only=True)
 class WavefrontSensor(Referenceable):
     """Abstract class that contains data related to one wavefront sensor in the system."""
@@ -160,15 +176,24 @@
 
     wavelength: float = None
     'Wavelength being sensed. (in m units)'
 
     optical_gain: Image = None
     'WFS optical gain over time. (Dimensions :math:`t`, dimensionless quantity, using data type flt)'
 
-    geometry: Geometry = None
+    transformation_matrix: Image = None
+    r"""Matrix that defines 2-dimensional affine transformations over time (:math:`t`) using homogeneous coordinates.
+    Any combination of translation, reflection, scale, rotation and shearing can be described via a single
+    :math:`3 \times 3` matrix :math:`M` such that :math:`P' = MP`, where :math:`P` is a
+    :math:`\begin{bmatrix}x & y & 1 \end{bmatrix}` vector (with :math:`x` and :math:`y` being the original horizontal 
+    and vertical coordinates, respectively) and :math:`P'` is a :math:`\begin{bmatrix}x' & y' & 1 \end{bmatrix}`, where
+    :math:`x'` and :math:`y'` are the transformed coordinates. All geometry information must be described relative to
+    the same reference origin point, from which transformations may occur.
+    (Dimensions :math:`3 \times 3 \times t`, dimensionless quantity, using data type flt)"""
+
     detector: Detector = None
     aberration: Aberration = None
     non_common_path_aberration: Aberration = None
 
     def __post_init__(self):
         if self.__class__ == WavefrontSensor:
             raise TypeError("Cannot instantiate abstract class.")
```

### Comparing `aotpy-0.5.1/aotpy/core/source.py` & `aotpy-0.6.0/aotpy/core/source.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.1/aotpy/core/telescope.py` & `aotpy-0.6.0/aotpy/core/telescope.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 
 
 from dataclasses import dataclass, field
 
 from .aberration import Aberration
 from .base import Referenceable, Coordinates
-from .geometry import Geometry
 
 __all__ = ['Segments', 'Monolithic', 'CircularSegments', 'HexagonalSegments', 'Telescope', 'MainTelescope',
            'LaserLaunchTelescope']
 
 from .image import Image
 
 
@@ -83,15 +82,25 @@
     """Diameter of the largest circle that can be contained in the pupil (inscribed circle).
     On monolithic circular pupils this is equivalent to `enclosing_diameter`. (in m units)"""
 
     obstruction_diameter: float = None
     'Diameter of the smallest circle that fully contains the central obstruction. (in m units)'
 
     segments: Segments = field(default_factory=Monolithic)
-    geometry: Geometry = None
+
+    transformation_matrix: Image = None
+    r"""Matrix that defines 2-dimensional affine transformations over time (:math:`t`) using homogeneous coordinates.
+    Any combination of translation, reflection, scale, rotation and shearing can be described via a single
+    :math:`3 \times 3` matrix :math:`M` such that :math:`P' = MP`, where :math:`P` is a
+    :math:`\begin{bmatrix}x & y & 1 \end{bmatrix}` vector (with :math:`x` and :math:`y` being the original horizontal 
+    and vertical coordinates, respectively) and :math:`P'` is a :math:`\begin{bmatrix}x' & y' & 1 \end{bmatrix}`, where
+    :math:`x'` and :math:`y'` are the transformed coordinates. All geometry information must be described relative to
+    the same reference origin point, from which transformations may occur.
+    (Dimensions :math:`3 \times 3 \times t`, dimensionless quantity, using data type flt)"""
+
     aberration: Aberration = None  # static_map
 
     def __post_init__(self):
         if self.__class__ == Telescope:
             raise TypeError("Cannot instantiate abstract class.")
```

### Comparing `aotpy-0.5.1/aotpy/core/time.py` & `aotpy-0.6.0/aotpy/core/time.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.1/aotpy/io/base.py` & `aotpy-0.6.0/aotpy/io/base.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.1/aotpy/io/fits/_keywords.py` & `aotpy-0.6.0/aotpy/io/fits/_keywords.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This module contains data that defines the AOT FITS format itself, including the specific FITS keywords and tables used.
 Not meant to be imported by users.
 """
 
 import re
 from dataclasses import dataclass
 
-CURRENT_AOT_VERSION = '0.5'
+CURRENT_AOT_VERSION = '0.6'
 
 
 @dataclass
 class AOTField:
     name: str
     format: str
     unit: str
@@ -57,15 +57,14 @@
 UNIT_PIXELS = 'pix'
 UNIT_DECIBELS = 'dB'
 UNIT_FRAME = 'frame'
 UNIT_HERTZ = 'Hz'
 UNIT_ARCSEC = 'arcsec'
 
 TIME_TABLE = 'AOT_TIME'
-GEOMETRY_TABLE = 'AOT_GEOMETRY'
 ATMOSPHERIC_PARAMETERS_TABLE = 'AOT_ATMOSPHERIC_PARAMETERS'
 ABERRATIONS_TABLE = 'AOT_ABERRATIONS'
 TELESCOPES_TABLE = 'AOT_TELESCOPES'
 SOURCES_TABLE = 'AOT_SOURCES'
 SOURCES_SODIUM_LGS_TABLE = 'AOT_SOURCES_SODIUM_LGS'
 SOURCES_RAYLEIGH_LGS_TABLE = 'AOT_SOURCES_RAYLEIGH_LGS'
 DETECTORS_TABLE = 'AOT_DETECTORS'
@@ -75,27 +74,27 @@
 WAVEFRONT_SENSORS_PYRAMID_TABLE = 'AOT_WAVEFRONT_SENSORS_PYRAMID'
 WAVEFRONT_CORRECTORS_TABLE = 'AOT_WAVEFRONT_CORRECTORS'
 WAVEFRONT_CORRECTORS_DM_TABLE = 'AOT_WAVEFRONT_CORRECTORS_DM'
 LOOPS_TABLE = 'AOT_LOOPS'
 LOOPS_CONTROL_TABLE = 'AOT_LOOPS_CONTROL'
 LOOPS_OFFLOAD_TABLE = 'AOT_LOOPS_OFFLOAD'
 
-MANDATORY_TABLE_SET = {TIME_TABLE, GEOMETRY_TABLE, ATMOSPHERIC_PARAMETERS_TABLE, ABERRATIONS_TABLE, TELESCOPES_TABLE,
-                       SOURCES_TABLE, DETECTORS_TABLE, SCORING_CAMERAS_TABLE, WAVEFRONT_SENSORS_TABLE,
-                       WAVEFRONT_CORRECTORS_TABLE, LOOPS_TABLE}
+MANDATORY_TABLE_SET = {TIME_TABLE, ATMOSPHERIC_PARAMETERS_TABLE, ABERRATIONS_TABLE, TELESCOPES_TABLE, SOURCES_TABLE,
+                       DETECTORS_TABLE, SCORING_CAMERAS_TABLE, WAVEFRONT_SENSORS_TABLE, WAVEFRONT_CORRECTORS_TABLE,
+                       LOOPS_TABLE}
 
 SECONDARY_TABLE_SET = {SOURCES_SODIUM_LGS_TABLE, SOURCES_RAYLEIGH_LGS_TABLE, WAVEFRONT_SENSORS_SHACK_HARTMANN_TABLE,
                        WAVEFRONT_SENSORS_PYRAMID_TABLE, WAVEFRONT_CORRECTORS_DM_TABLE, LOOPS_CONTROL_TABLE,
                        LOOPS_OFFLOAD_TABLE}
 TABLE_SET = MANDATORY_TABLE_SET | SECONDARY_TABLE_SET
-TABLE_SEQUENCE = [TIME_TABLE, GEOMETRY_TABLE, ATMOSPHERIC_PARAMETERS_TABLE, ABERRATIONS_TABLE, TELESCOPES_TABLE,
-                  SOURCES_TABLE, SOURCES_SODIUM_LGS_TABLE, SOURCES_RAYLEIGH_LGS_TABLE, DETECTORS_TABLE,
-                  SCORING_CAMERAS_TABLE, WAVEFRONT_SENSORS_TABLE, WAVEFRONT_SENSORS_SHACK_HARTMANN_TABLE,
-                  WAVEFRONT_SENSORS_PYRAMID_TABLE, WAVEFRONT_CORRECTORS_TABLE, WAVEFRONT_CORRECTORS_DM_TABLE,
-                  LOOPS_TABLE, LOOPS_CONTROL_TABLE, LOOPS_OFFLOAD_TABLE]
+TABLE_SEQUENCE = [TIME_TABLE, ATMOSPHERIC_PARAMETERS_TABLE, ABERRATIONS_TABLE, TELESCOPES_TABLE, SOURCES_TABLE,
+                  SOURCES_SODIUM_LGS_TABLE, SOURCES_RAYLEIGH_LGS_TABLE, DETECTORS_TABLE, SCORING_CAMERAS_TABLE,
+                  WAVEFRONT_SENSORS_TABLE, WAVEFRONT_SENSORS_SHACK_HARTMANN_TABLE, WAVEFRONT_SENSORS_PYRAMID_TABLE,
+                  WAVEFRONT_CORRECTORS_TABLE, WAVEFRONT_CORRECTORS_DM_TABLE, LOOPS_TABLE, LOOPS_CONTROL_TABLE,
+                  LOOPS_OFFLOAD_TABLE]
 TABLE_FIELDS: dict[str, AOTFieldDict] = {}
 
 # AOSystem keywords
 AOT_VERSION = 'AOT-VERS'
 AOT_AO_MODE = 'AO-MODE'
 AOT_AO_MODE_SET = {'SCAO', 'SLAO', 'GLAO', 'MOAO', 'LTAO', 'MCAO'}
 AOT_TIMESYS = 'TIMESYS'
@@ -106,48 +105,32 @@
 AOT_TEMPORAL_ERROR = 'TEMP-ERR'
 AOT_CONFIG = 'CONFIG'
 AOT_HEADER_SET = {AOT_VERSION, AOT_AO_MODE, AOT_TIMESYS, AOT_DATE_BEG, AOT_DATE_END, AOT_STREHL_RATIO,
                   AOT_TEMPORAL_ERROR, AOT_CONFIG}
 
 REFERENCE_UID = 'UID'
 TIME_REFERENCE = 'TIME_UID'
-GEOMETRY_REFERENCE = 'GEOMETRY_UID'
 ABERRATION_REFERENCE = 'ABERRATION_UID'
 LASER_LAUNCH_TELESCOPE_REFERENCE = 'LLT_UID'
 DETECTOR_REFERENCE = 'DETECTOR_UID'
 SOURCE_REFERENCE = 'SOURCE_UID'
 NCPA_REFERENCE = 'NCPA_UID'
 TELESCOPE_REFERENCE = 'TELESCOPE_UID'
+TRANSFORMATION_MATRIX = 'TRANSFORMATION_MATRIX'
 
 # AOT_TIME fields
 TIME_TIMESTAMPS = 'TIMESTAMPS'
 TIME_FRAME_NUMBERS = 'FRAME_NUMBERS'
 TIME_FIELDS = AOTFieldDict(
     AOTField(name=REFERENCE_UID, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS, mandatory=True, unique=True),
     AOTField(name=TIME_TIMESTAMPS, format=LIST_FORMAT, unit=UNIT_SECONDS),
     AOTField(name=TIME_FRAME_NUMBERS, format=LIST_FORMAT, unit=UNIT_COUNT)
 )
 TABLE_FIELDS[TIME_TABLE] = TIME_FIELDS
 
-# AOT_GEOMETRY fields
-GEOMETRY_ROTATION = 'ROTATION'
-GEOMETRY_TRANSLATION_X = 'TRANSLATION_X'
-GEOMETRY_TRANSLATION_Y = 'TRANSLATION_Y'
-GEOMETRY_MAGNIFICATION_X = 'MAGNIFICATION_X'
-GEOMETRY_MAGNIFICATION_Y = 'MAGNIFICATION_Y'
-GEOMETRY_FIELDS = AOTFieldDict(
-    AOTField(name=REFERENCE_UID, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS, mandatory=True, unique=True),
-    AOTField(name=TIME_REFERENCE, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
-    AOTField(name=GEOMETRY_ROTATION, format=LIST_FORMAT, unit=UNIT_RADIANS),
-    AOTField(name=GEOMETRY_TRANSLATION_X, format=LIST_FORMAT, unit=UNIT_METERS),
-    AOTField(name=GEOMETRY_TRANSLATION_Y, format=LIST_FORMAT, unit=UNIT_METERS),
-    AOTField(name=GEOMETRY_MAGNIFICATION_X, format=LIST_FORMAT, unit=UNIT_DIMENSIONLESS),
-    AOTField(name=GEOMETRY_MAGNIFICATION_Y, format=LIST_FORMAT, unit=UNIT_DIMENSIONLESS)
-)
-TABLE_FIELDS[GEOMETRY_TABLE] = GEOMETRY_FIELDS
 
 # AOT_ATMOSPHERIC_PARAMETERS fields
 ATMOSPHERIC_PARAMETERS_WAVELENGTH = 'WAVELENGTH'
 ATMOSPHERIC_PARAMETERS_R0 = 'R0'
 ATMOSPHERIC_PARAMETERS_FWHM = 'FWHM'
 ATMOSPHERIC_PARAMETERS_TAU0 = 'TAU0'
 ATMOSPHERIC_PARAMETERS_THETA0 = 'THETA0'
@@ -165,15 +148,15 @@
     AOTField(name=ATMOSPHERIC_PARAMETERS_TAU0, format=LIST_FORMAT, unit=UNIT_SECONDS),
     AOTField(name=ATMOSPHERIC_PARAMETERS_THETA0, format=LIST_FORMAT, unit=UNIT_RADIANS),
     AOTField(name=ATMOSPHERIC_PARAMETERS_LAYERS_WEIGHT, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=ATMOSPHERIC_PARAMETERS_LAYERS_HEIGHT, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=ATMOSPHERIC_PARAMETERS_LAYERS_L0, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=ATMOSPHERIC_PARAMETERS_LAYERS_WIND_SPEED, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=ATMOSPHERIC_PARAMETERS_LAYERS_WIND_DIRECTION, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
-    AOTField(name=GEOMETRY_REFERENCE, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS)
+    AOTField(name=TRANSFORMATION_MATRIX, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS)
 )
 TABLE_FIELDS[ATMOSPHERIC_PARAMETERS_TABLE] = ATMOSPHERIC_PARAMETERS_FIELDS
 
 # AOT_ABERRATIONS fields
 ABERRATION_MODES = 'MODES'
 ABERRATION_COEFFICIENTS = 'COEFFICIENTS'
 ABERRATION_X_OFFSETS = 'X_OFFSETS'
@@ -216,15 +199,15 @@
     AOTField(name=TELESCOPE_ENCLOSING_D, format=FLOAT_FORMAT, unit=UNIT_METERS),
     AOTField(name=TELESCOPE_INSCRIBED_D, format=FLOAT_FORMAT, unit=UNIT_METERS),
     AOTField(name=TELESCOPE_OBSTRUCTION_D, format=FLOAT_FORMAT, unit=UNIT_METERS),
     AOTField(name=TELESCOPE_SEGMENTS_TYPE, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS, mandatory=True),
     AOTField(name=TELESCOPE_SEGMENTS_SIZE, format=FLOAT_FORMAT, unit=UNIT_METERS),
     AOTField(name=TELESCOPE_SEGMENTS_X, format=LIST_FORMAT, unit=UNIT_METERS),
     AOTField(name=TELESCOPE_SEGMENTS_Y, format=LIST_FORMAT, unit=UNIT_METERS),
-    AOTField(name=GEOMETRY_REFERENCE, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
+    AOTField(name=TRANSFORMATION_MATRIX, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=ABERRATION_REFERENCE, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS)
 )
 TABLE_FIELDS[TELESCOPES_TABLE] = TELESCOPE_FIELDS
 TELESCOPE_TYPE_MAIN = 'Main Telescope'
 TELESCOPE_TYPE_LLT = 'Laser Launch Telescope'
 TELESCOPE_SEGMENT_TYPE_MONOLITHIC = 'Monolithic'
 TELESCOPE_SEGMENT_TYPE_HEXAGON = 'Hexagon'
@@ -324,26 +307,26 @@
     AOTField(name=DETECTOR_GAIN, format=FLOAT_FORMAT, unit=UNIT_ELECTRONS),
     AOTField(name=DETECTOR_EXCESS_NOISE, format=FLOAT_FORMAT, unit=UNIT_ELECTRONS),
     AOTField(name=DETECTOR_FILTER, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=DETECTOR_BAD_PIXEL_MAP, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=DETECTOR_DYNAMIC_RANGE, format=FLOAT_FORMAT, unit=UNIT_DECIBELS),
     AOTField(name=DETECTOR_READOUT_RATE, format=STRING_FORMAT, unit=f'{UNIT_PIXELS}*{UNIT_SECONDS}^-1'),
     AOTField(name=DETECTOR_FRAME_RATE, format=STRING_FORMAT, unit=f'{UNIT_FRAME}*{UNIT_SECONDS}^-1'),
-    AOTField(name=GEOMETRY_REFERENCE, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS)
+    AOTField(name=TRANSFORMATION_MATRIX, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS)
 )
 TABLE_FIELDS[DETECTORS_TABLE] = DETECTOR_FIELDS
 
 # AOT_SCORING_CAMERAS fields
 SCORING_CAMERA_PUPIL_MASK = 'PUPIL_MASK'
 SCORING_CAMERA_WAVELENGTH = 'WAVELENGTH'
 SCORING_CAMERA_FIELDS = AOTFieldDict(
     AOTField(name=REFERENCE_UID, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS, mandatory=True, unique=True),
     AOTField(name=SCORING_CAMERA_PUPIL_MASK, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=SCORING_CAMERA_WAVELENGTH, format=FLOAT_FORMAT, unit=UNIT_METERS),
-    AOTField(name=GEOMETRY_REFERENCE, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
+    AOTField(name=TRANSFORMATION_MATRIX, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=DETECTOR_REFERENCE, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=ABERRATION_REFERENCE, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS)
 )
 TABLE_FIELDS[SCORING_CAMERAS_TABLE] = SCORING_CAMERA_FIELDS
 
 # AOT_WAVEFRONT_SENSORS
 WAVEFRONT_SENSOR_TYPE = 'TYPE'
@@ -369,15 +352,15 @@
     AOTField(name=WAVEFRONT_SENSOR_SUBAPERTURE_MASK, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=WAVEFRONT_SENSOR_MASK_X_OFFSETS, format=LIST_FORMAT, unit=UNIT_PIXELS),
     AOTField(name=WAVEFRONT_SENSOR_MASK_Y_OFFSETS, format=LIST_FORMAT, unit=UNIT_PIXELS),
     AOTField(name=WAVEFRONT_SENSOR_SUBAPERTURE_SIZE, format=STRING_FORMAT, unit=UNIT_PIXELS),
     AOTField(name=WAVEFRONT_SENSOR_SUBAPERTURE_INTENSITIES, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=WAVEFRONT_SENSOR_WAVELENGTH, format=FLOAT_FORMAT, unit=UNIT_METERS),
     AOTField(name=WAVEFRONT_SENSOR_OPTICAL_GAIN, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
-    AOTField(name=GEOMETRY_REFERENCE, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
+    AOTField(name=TRANSFORMATION_MATRIX, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=DETECTOR_REFERENCE, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=ABERRATION_REFERENCE, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=NCPA_REFERENCE, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS)
 )
 TABLE_FIELDS[WAVEFRONT_SENSORS_TABLE] = WAVEFRONT_SENSOR_FIELDS
 WAVEFRONT_SENSOR_TYPE_SHACK_HARTMANN = 'Shack-Hartmann'
 WAVEFRONT_SENSOR_TYPE_PYRAMID = 'Pyramid'
@@ -415,15 +398,15 @@
     AOTField(name=REFERENCE_UID, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS, mandatory=True, unique=True),
     AOTField(name=WAVEFRONT_CORRECTOR_TYPE, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS, mandatory=True),
     AOTField(name=TELESCOPE_REFERENCE, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS, mandatory=True),
     AOTField(name=WAVEFRONT_CORRECTOR_N_VALID_ACTUATORS, format=INTEGER_FORMAT, unit=UNIT_COUNT),
     AOTField(name=WAVEFRONT_CORRECTOR_PUPIL_MASK, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=WAVEFRONT_CORRECTOR_TFZ_NUM, format=LIST_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=WAVEFRONT_CORRECTOR_TFZ_DEN, format=LIST_FORMAT, unit=UNIT_DIMENSIONLESS),
-    AOTField(name=GEOMETRY_REFERENCE, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
+    AOTField(name=TRANSFORMATION_MATRIX, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=ABERRATION_REFERENCE, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS)
 )
 TABLE_FIELDS[WAVEFRONT_CORRECTORS_TABLE] = WAVEFRONT_CORRECTOR_FIELDS
 WAVEFRONT_CORRECTOR_TYPE_DM = 'Deformable Mirror'
 WAVEFRONT_CORRECTOR_TYPE_TTM = 'Tip-Tilt Mirror'
 WAVEFRONT_CORRECTOR_TYPE_LS = 'Linear Stage'
 
@@ -468,24 +451,28 @@
 LOOPS_TYPE_CONTROL = 'Control Loop'
 LOOPS_TYPE_OFFLOAD = 'Offload Loop'
 LOOPS_STATUS_OPEN = 'Open'
 LOOPS_STATUS_CLOSED = 'Closed'
 
 # AOT_LOOPS_CONTROL fields
 LOOPS_CONTROL_INPUT_SENSOR = 'INPUT_SENSOR_UID'
+LOOPS_CONTROL_MODES = 'MODES'
+LOOPS_CONTROL_MODAL_COEFFICIENTS = 'MODAL_COEFFICIENTS'
 LOOPS_CONTROL_CONTROL_MATRIX = 'CONTROL_MATRIX'
 LOOPS_CONTROL_MEASUREMENTS_TO_MODES = 'MEASUREMENTS_TO_MODES'
 LOOPS_CONTROL_MODES_TO_COMMANDS = 'MODES_TO_COMMANDS'
 LOOPS_CONTROL_INTERACTION_MATRIX = 'INTERACTION_MATRIX'
 LOOPS_CONTROL_COMMANDS_TO_MODES = 'COMMANDS_TO_MODES'
 LOOPS_CONTROL_MODES_TO_MEASUREMENTS = 'MODES_TO_MEASUREMENTS'
 LOOPS_CONTROL_RESIDUAL_COMMANDS = 'RESIDUAL_COMMANDS'
 LOOPS_CONTROL_FIELDS = AOTFieldDict(
     AOTField(name=REFERENCE_UID, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS, mandatory=True, unique=True),
     AOTField(name=LOOPS_CONTROL_INPUT_SENSOR, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS, mandatory=True),
+    AOTField(name=LOOPS_CONTROL_MODES, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
+    AOTField(name=LOOPS_CONTROL_MODAL_COEFFICIENTS, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=LOOPS_CONTROL_CONTROL_MATRIX, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=LOOPS_CONTROL_MEASUREMENTS_TO_MODES, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=LOOPS_CONTROL_MODES_TO_COMMANDS, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=LOOPS_CONTROL_INTERACTION_MATRIX, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=LOOPS_CONTROL_COMMANDS_TO_MODES, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=LOOPS_CONTROL_MODES_TO_MEASUREMENTS, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS),
     AOTField(name=LOOPS_CONTROL_RESIDUAL_COMMANDS, format=STRING_FORMAT, unit=UNIT_DIMENSIONLESS)
```

### Comparing `aotpy-0.5.1/aotpy/io/fits/reader.py` & `aotpy-0.6.0/aotpy/io/fits/reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,25 +79,23 @@
 class FITSReader(SystemReader):
     def _initialize_data(self) -> None:
         """
         Initialize data structures necessary for reading the file.
         """
         self._images: dict[str, list] = {}
         self._time: dict[str, list] = {}
-        self._geometries: dict[str, list] = {}
         self._aberrations: dict[str, list] = {}
         self._telescopes: dict[str, list] = {}
         self._sources: dict[str, list] = {}
         self._detectors: dict[str, list] = {}
         self._wfss: dict[str, list] = {}
         self._wfcs: dict[str, list] = {}
 
         self._table_to_dict = {
             kw.TIME_TABLE: self._time,
-            kw.GEOMETRY_TABLE: self._geometries,
             kw.ABERRATIONS_TABLE: self._aberrations,
             kw.TELESCOPES_TABLE: self._telescopes,
             kw.SOURCES_TABLE: self._sources,
             kw.DETECTORS_TABLE: self._detectors,
             kw.WAVEFRONT_SENSORS_TABLE: self._wfss,
             kw.WAVEFRONT_CORRECTORS_TABLE: self._wfcs
         }
@@ -131,15 +129,15 @@
                             raise ValueError(f"Image name '{hdu.name}' appears repeated in file.")
                         if hdu.data is None:
                             warnings.warn(f"Image HDU '{hdu.name}' was ignored for having no data.")
                         self._images[hdu.name] = [image_from_hdu(hdu), False]
                     else:
                         self._extra_hdus.append(hdu)
             if self._extra_hdus and not self._extra_data_flag:
-                warnings.warn(f"""File contains non-standard HDUs that were ignored: """
+                warnings.warn(f"""File contains non-AOT HDUs that were ignored: """
                               f"""{', '.join([f"'{x.name}'" for x in self._extra_hdus])}""")
 
             for name, count in table_count.items():
                 if name in kw.MANDATORY_TABLE_SET and count != 1:
                     raise ValueError(f"Mandatory table '{name}' must appear exactly once in file.")
                 if count > 1:
                     raise ValueError(f"Secondary table '{name}' cannot appear repeated in file.")
@@ -149,15 +147,14 @@
 
             self._handle_time(hdus)
 
             for tup in self._images.values():
                 image = tup[0]
                 image.time = self._handle_reference(image._time, kw.TIME_TABLE)
 
-            self._handle_geometry(hdus)
             self._handle_atmosphere(hdus)
             self._handle_aberrations(hdus)
             self._handle_telescopes(hdus)
             self._handle_sources(hdus)
             self._handle_detectors(hdus)
             self._handle_scoring_cameras(hdus)
             self._handle_wavefront_sensors(hdus)
@@ -227,15 +224,15 @@
         except KeyError:
             config = None
 
         for card in self._primary_header.cards:
             if card.keyword not in kw.AOT_HEADER_SET and keyword_is_relevant(card.keyword):
                 self._extra_header.append(card)
         if self._extra_header and not self._extra_data_flag:
-            warnings.warn(f"""Header contains non-standard keywords that were ignored: """
+            warnings.warn(f"""Header contains non-AOT keywords that were ignored: """
                           f"""{', '.join([f"'{x.keyword}'" for x in self._extra_header])}""")
 
         return aotpy.AOSystem(ao_mode=ao_mode, date_beginning=beg, date_end=end, strehl_ratio=strehl_ratio,
                               temporal_error=temporal_error, config=config)
 
     def _check_bintable(self, hdus: fits.HDUList, table_name: str):
         fields = kw.TABLE_FIELDS[table_name]
@@ -258,83 +255,90 @@
                     u = table.data[col.name]
                     if len(np.unique(u)) != len(u):
                         raise ValueError(
                             f"Column '{col.name}' in table '{table_name}' must have unique values.")
             else:
                 self._extra_columns.setdefault(table_name, []).append(col)
         if table_name in self._extra_columns and not self._extra_data_flag:
-            warnings.warn(f"""Table '{table_name}' contains non-standard columns that were ignored: """
+            warnings.warn(f"""Table '{table_name}' contains non-AOT columns that were ignored: """
                           f"""{', '.join([f"'{x.name}'" for x in self._extra_columns[table_name]])}""")
 
         for name, count in field_count.items():
             if count < 1:
                 warnings.warn(f"Column '{name}' missing in table '{table_name}'.")
             if count > 1:
                 raise ValueError(f"Column '{name}' cannot appear repeated in table '{table_name}'.")
 
         seq = [field_name for field_name, count in field_count.items() if count > 0]
         if seq != [col.name for col, _ in zip(table.columns.columns, seq)]:
-            warnings.warn(f"Non-standard column sequence in table '{table_name}'.")
+            warnings.warn(f"Non-AOT column sequence in table '{table_name}'.")
 
-    def _handle_reference(self, ref: str, table: str = None):
+    def _handle_image(self, ref: str):
         if ref is None:
             return None
         fullmatch = _reference_pattern.fullmatch(ref)
         if fullmatch is None:
-            warnings.warn(f"Reference '{ref}' was ignored: not properly formatted.")
+            warnings.warn(f"Image reference '{ref}' was ignored: not properly formatted.")
             return None
         prefix, name, index = fullmatch.groups()
 
-        if table is None:
-            match prefix:
-                case kw.INTERNAL_REFERENCE:
+        match prefix:
+            case kw.INTERNAL_REFERENCE:
+                try:
+                    aux = self._images[name]
+                    aux[1] = True
+                    return aux[0]
+                except KeyError:
+                    warnings.warn(f"Could not find internal image referenced by '{ref}'.")
+                    return None
+            case kw.FILE_REFERENCE | kw.URL_REFERENCE:
+                if index is not None:
                     try:
-                        aux = self._images[name]
-                        aux[1] = True
-                        return aux[0]
-                    except KeyError:
-                        warnings.warn(f"Could not find internal image referenced by '{ref}'.")
-                        return None
-                case kw.FILE_REFERENCE | kw.URL_REFERENCE:
-                    if index is not None:
-                        try:
-                            index = int(index)
-                        except ValueError:
-                            warnings.warn(f"Index in file reference '{ref}' was ignored: not properly formatted.")
-                            index = None
-                    if prefix == kw.FILE_REFERENCE:
-                        image = FITSFileImage(name, index)
-                    else:
-                        image = FITSURLImage(name, index)
+                        index = int(index)
+                    except ValueError:
+                        warnings.warn(f"Index in file reference '{ref}' was ignored: not properly formatted.")
+                        index = None
+                if prefix == kw.FILE_REFERENCE:
+                    image = FITSFileImage(name, index)
+                else:
+                    image = FITSURLImage(name, index)
 
-                    image.time = self._handle_reference(image._time, kw.TIME_TABLE)
-                    return image
+                image.time = self._handle_reference(image._time, kw.TIME_TABLE)
+                return image
+            case _:
+                warnings.warn(f"Reference '{ref}' was ignored: expected an image reference.")
+                return None
 
-            warnings.warn(f"Image reference '{ref}' was ignored: not properly formatted.")
+    def _handle_reference(self, ref: str, table: str):
+        if ref is None:
+            return None
+        fullmatch = _reference_pattern.fullmatch(ref)
+        if fullmatch is None:
+            warnings.warn(f"Row reference '{ref}' was ignored: not properly formatted.")
             return None
+        prefix, name, index = fullmatch.groups()
 
-        if prefix == kw.ROW_REFERENCE:
-            d = self._table_to_dict[table]
-            try:
-                aux = d[name]
-                aux[1] = True
-                return aux[0]
-            except KeyError:
-                warnings.warn(f"Could not find row referenced by '{ref}'. Ignoring reference.")
-                return None
+        if prefix != kw.ROW_REFERENCE:
+            warnings.warn(f"Reference '{ref}' was ignored: expected a row reference.")
+            return None
 
-        warnings.warn(f"Row reference '{ref}' was ignored: not properly formatted.")
-        return None
+        d = self._table_to_dict[table]
+        try:
+            aux = d[name]
+            aux[1] = True
+            return aux[0]
+        except KeyError:
+            warnings.warn(f"Could not find row referenced by '{ref}'. Ignoring reference.")
+            return None
 
     def _check_usage(self):
         # We don't need to check the usage of atmosphere parameters, sources, scoring cameras, wavefront sensors,
         # wavefront correctors or loops, since they are always referenced by the AOSystem class
         a = [(self._images, 'image extensions'),
              (self._time, 'time rows'),
-             (self._geometries, 'geometry rows'),
              (self._aberrations, 'aberration rows'),
              (self._telescopes, 'telescope rows'),
              (self._detectors, 'detector rows')]
 
         for d, name in a:
             unused = {k: v[0] for k, v in d.items() if not v[1]}
             if unused:
@@ -353,34 +357,14 @@
 
             self._time[data[kw.REFERENCE_UID]] = [aotpy.Time(
                 uid=data[kw.REFERENCE_UID],
                 timestamps=data[kw.TIME_TIMESTAMPS],
                 frame_numbers=data[kw.TIME_FRAME_NUMBERS]
             ), False]
 
-    def _handle_geometry(self, hdus: fits.HDUList):
-        self._check_bintable(hdus, kw.GEOMETRY_TABLE)
-
-        table = hdus[kw.GEOMETRY_TABLE]
-        columns = table.columns
-        for row in table.data:
-            data = _convert_row(columns, row, kw.GEOMETRY_FIELDS)
-
-            self._geometries[data[kw.REFERENCE_UID]] = [aotpy.Geometry(
-                uid=data[kw.REFERENCE_UID],
-                time=self._handle_reference(data[kw.TIME_REFERENCE], kw.TIME_TABLE),
-                sequence=[aotpy.GeometryInstant(
-                    rotation=rotation,
-                    translation=aotpy.Coordinates(translation_x, translation_y),
-                    magnification=aotpy.Coordinates(magnification_x, magnification_y),
-                ) for rotation, translation_x, translation_y, magnification_x, magnification_y in
-                    zip(data[kw.GEOMETRY_ROTATION], data[kw.GEOMETRY_TRANSLATION_X], data[kw.GEOMETRY_TRANSLATION_Y],
-                        data[kw.GEOMETRY_MAGNIFICATION_X], data[kw.GEOMETRY_MAGNIFICATION_Y])]
-            ), False]
-
     def _handle_atmosphere(self, hdus: fits.HDUList):
         self._check_bintable(hdus, kw.ATMOSPHERIC_PARAMETERS_TABLE)
 
         table = hdus[kw.ATMOSPHERIC_PARAMETERS_TABLE]
         columns = table.columns
         for row in table.data:
             data = _convert_row(columns, row, kw.ATMOSPHERIC_PARAMETERS_FIELDS)
@@ -390,35 +374,35 @@
                     uid=data[kw.REFERENCE_UID],
                     wavelength=data[kw.ATMOSPHERIC_PARAMETERS_WAVELENGTH],
                     time=self._handle_reference(data[kw.TIME_REFERENCE], kw.TIME_TABLE),
                     r0=data[kw.ATMOSPHERIC_PARAMETERS_R0],
                     fwhm=data[kw.ATMOSPHERIC_PARAMETERS_FWHM],
                     tau0=data[kw.ATMOSPHERIC_PARAMETERS_TAU0],
                     theta0=data[kw.ATMOSPHERIC_PARAMETERS_THETA0],
-                    layers_weight=self._handle_reference(data[kw.ATMOSPHERIC_PARAMETERS_LAYERS_WEIGHT]),
-                    layers_height=self._handle_reference(data[kw.ATMOSPHERIC_PARAMETERS_LAYERS_HEIGHT]),
-                    layers_l0=self._handle_reference(data[kw.ATMOSPHERIC_PARAMETERS_LAYERS_L0]),
-                    layers_wind_speed=self._handle_reference(data[kw.ATMOSPHERIC_PARAMETERS_LAYERS_WIND_SPEED]),
-                    layers_wind_direction=self._handle_reference(data[kw.ATMOSPHERIC_PARAMETERS_LAYERS_WIND_DIRECTION]),
-                    geometry=self._handle_reference(data[kw.GEOMETRY_REFERENCE], kw.GEOMETRY_TABLE)
+                    layers_weight=self._handle_image(data[kw.ATMOSPHERIC_PARAMETERS_LAYERS_WEIGHT]),
+                    layers_height=self._handle_image(data[kw.ATMOSPHERIC_PARAMETERS_LAYERS_HEIGHT]),
+                    layers_l0=self._handle_image(data[kw.ATMOSPHERIC_PARAMETERS_LAYERS_L0]),
+                    layers_wind_speed=self._handle_image(data[kw.ATMOSPHERIC_PARAMETERS_LAYERS_WIND_SPEED]),
+                    layers_wind_direction=self._handle_image(data[kw.ATMOSPHERIC_PARAMETERS_LAYERS_WIND_DIRECTION]),
+                    transformation_matrix=self._handle_image(data[kw.TRANSFORMATION_MATRIX])
                 )
             )
 
     def _handle_aberrations(self, hdus: fits.HDUList):
         self._check_bintable(hdus, kw.ABERRATIONS_TABLE)
 
         table = hdus[kw.ABERRATIONS_TABLE]
         columns = table.columns
         for row in table.data:
             data = _convert_row(columns, row, kw.ABERRATION_FIELDS)
 
             self._aberrations[data[kw.REFERENCE_UID]] = [aotpy.Aberration(
                 uid=data[kw.REFERENCE_UID],
-                modes=self._handle_reference(data[kw.ABERRATION_MODES]),
-                coefficients=self._handle_reference(data[kw.ABERRATION_COEFFICIENTS]),
+                modes=self._handle_image(data[kw.ABERRATION_MODES]),
+                coefficients=self._handle_image(data[kw.ABERRATION_COEFFICIENTS]),
                 offsets=[aotpy.Coordinates(x, y)
                          for x, y in zip(data[kw.ABERRATION_X_OFFSETS], data[kw.ABERRATION_Y_OFFSETS])],
             ), False]
 
     def _handle_telescopes(self, hdus: fits.HDUList):
         self._check_bintable(hdus, kw.TELESCOPES_TABLE)
 
@@ -443,15 +427,15 @@
                 continue
 
             tel.latitude = data[kw.TELESCOPE_LATITUDE]
             tel.longitude = data[kw.TELESCOPE_LONGITUDE]
             tel.elevation = data[kw.TELESCOPE_ELEVATION]
             tel.azimuth = data[kw.TELESCOPE_AZIMUTH]
             tel.parallactic = data[kw.TELESCOPE_PARALLACTIC]
-            tel.pupil_mask = self._handle_reference(data[kw.TELESCOPE_PUPIL_MASK])
+            tel.pupil_mask = self._handle_image(data[kw.TELESCOPE_PUPIL_MASK])
             tel.pupil_angle = data[kw.TELESCOPE_PUPIL_ANGLE]
             tel.enclosing_diameter = data[kw.TELESCOPE_ENCLOSING_D]
             tel.inscribed_diameter = data[kw.TELESCOPE_INSCRIBED_D]
             tel.obstruction_diameter = data[kw.TELESCOPE_OBSTRUCTION_D]
 
             t = data[kw.TELESCOPE_SEGMENTS_TYPE]
             if t == kw.TELESCOPE_SEGMENT_TYPE_MONOLITHIC:
@@ -465,15 +449,15 @@
                     warnings.warn(f"Ignored unknown segment type '{t}'.")
                     seg = aotpy.Monolithic()
                 seg.size = data[kw.TELESCOPE_SEGMENTS_SIZE]
                 seg.coordinates = [aotpy.Coordinates(x, y)
                                    for x, y in zip(data[kw.TELESCOPE_SEGMENTS_X], data[kw.TELESCOPE_SEGMENTS_Y])]
 
             tel.segments = seg
-            tel.geometry = self._handle_reference(data[kw.GEOMETRY_REFERENCE], kw.GEOMETRY_TABLE)
+            tel.transformation_matrix = self._handle_image(data[kw.TRANSFORMATION_MATRIX])
             tel.aberration = self._handle_reference(data[kw.ABERRATION_REFERENCE], kw.ABERRATIONS_TABLE)
 
     def _handle_sources(self, hdus: fits.HDUList):
         self._check_bintable(hdus, kw.SOURCES_TABLE)
 
         table = hdus[kw.SOURCES_TABLE]
         existing_types = table.data['TYPE']
@@ -507,15 +491,15 @@
                     raise ValueError(f"Source '{uid}' not found in table '{kw.SOURCES_SODIUM_LGS_TABLE}' even"
                                      f" though it is of type '{t}'")
 
                 other_data = _convert_row(hdus[kw.SOURCES_SODIUM_LGS_TABLE].columns, f, kw.SOURCE_SODIUM_LGS_FIELDS)
                 src = aotpy.SodiumLaserGuideStar(
                     uid=uid,
                     height=other_data[kw.SOURCE_SODIUM_LGS_HEIGHT],
-                    profile=self._handle_reference(other_data[kw.SOURCE_SODIUM_LGS_PROFILE]),
+                    profile=self._handle_image(other_data[kw.SOURCE_SODIUM_LGS_PROFILE]),
                     altitudes=other_data[kw.SOURCE_SODIUM_LGS_ALTITUDES],
                     laser_launch_telescope=self._handle_reference(other_data[kw.LASER_LAUNCH_TELESCOPE_REFERENCE],
                                                                   kw.TELESCOPES_TABLE)
                 )
             elif t == kw.SOURCE_TYPE_RAYLEIGH_LASER_GUIDE_STAR:
                 # Try to find uid in secondary table
                 f = next((x for x in hdus[kw.SOURCES_RAYLEIGH_LGS_TABLE].data if x[kw.REFERENCE_UID] == uid), None)
@@ -553,51 +537,51 @@
             data = _convert_row(columns, row, kw.DETECTOR_FIELDS)
 
             self._detectors[data[kw.REFERENCE_UID]] = [aotpy.Detector(
                 uid=data[kw.REFERENCE_UID],
                 type=data[kw.DETECTOR_TYPE],
                 sampling_technique=data[kw.DETECTOR_SAMPLING_TECHNIQUE],
                 shutter_type=data[kw.DETECTOR_SHUTTER_TYPE],
-                flat_field=self._handle_reference(data[kw.DETECTOR_FLAT_FIELD]),
+                flat_field=self._handle_image(data[kw.DETECTOR_FLAT_FIELD]),
                 readout_noise=data[kw.DETECTOR_READOUT_NOISE],
-                pixel_intensities=self._handle_reference(data[kw.DETECTOR_PIXEL_INTENSITIES]),
+                pixel_intensities=self._handle_image(data[kw.DETECTOR_PIXEL_INTENSITIES]),
                 integration_time=data[kw.DETECTOR_INTEGRATION_TIME],
                 coadds=data[kw.DETECTOR_COADDS],
-                dark=self._handle_reference(data[kw.DETECTOR_DARK]),
-                weight_map=self._handle_reference(data[kw.DETECTOR_WEIGHT_MAP]),
+                dark=self._handle_image(data[kw.DETECTOR_DARK]),
+                weight_map=self._handle_image(data[kw.DETECTOR_WEIGHT_MAP]),
                 quantum_efficiency=data[kw.DETECTOR_QUANTUM_EFFICIENCY],
                 pixel_scale=data[kw.DETECTOR_PIXEL_SCALE],
                 binning=data[kw.DETECTOR_BINNING],
                 bandwidth=data[kw.DETECTOR_BANDWIDTH],
                 transmission_wavelength=data[kw.DETECTOR_TRANSMISSION_WAVELENGTH],
                 transmission=data[kw.DETECTOR_TRANSMISSION],
-                sky_background=self._handle_reference(data[kw.DETECTOR_SKY_BACKGROUND]),
+                sky_background=self._handle_image(data[kw.DETECTOR_SKY_BACKGROUND]),
                 gain=data[kw.DETECTOR_GAIN],
                 excess_noise=data[kw.DETECTOR_EXCESS_NOISE],
                 filter=data[kw.DETECTOR_FILTER],
-                bad_pixel_map=self._handle_reference(data[kw.DETECTOR_BAD_PIXEL_MAP]),
+                bad_pixel_map=self._handle_image(data[kw.DETECTOR_BAD_PIXEL_MAP]),
                 dynamic_range=data[kw.DETECTOR_DYNAMIC_RANGE],
                 readout_rate=data[kw.DETECTOR_READOUT_RATE],
                 frame_rate=data[kw.DETECTOR_FRAME_RATE],
-                geometry=self._handle_reference(data[kw.GEOMETRY_REFERENCE], kw.GEOMETRY_TABLE),
+                transformation_matrix=self._handle_image(data[kw.TRANSFORMATION_MATRIX])
             ), False]
 
     def _handle_scoring_cameras(self, hdus: fits.HDUList):
         self._check_bintable(hdus, kw.SCORING_CAMERAS_TABLE)
 
         table = hdus[kw.SCORING_CAMERAS_TABLE]
         columns = table.columns
         for row in table.data:
             data = _convert_row(columns, row, kw.SCORING_CAMERA_FIELDS)
 
             self._system.scoring_cameras.append(aotpy.ScoringCamera(
                 uid=data[kw.REFERENCE_UID],
-                pupil_mask=self._handle_reference(data[kw.SCORING_CAMERA_PUPIL_MASK]),
+                pupil_mask=self._handle_image(data[kw.SCORING_CAMERA_PUPIL_MASK]),
                 wavelength=data[kw.SCORING_CAMERA_WAVELENGTH],
-                geometry=self._handle_reference(data[kw.GEOMETRY_REFERENCE], kw.GEOMETRY_TABLE),
+                transformation_matrix=self._handle_image(data[kw.TRANSFORMATION_MATRIX]),
                 detector=self._handle_reference(data[kw.DETECTOR_REFERENCE], kw.DETECTORS_TABLE),
                 aberration=self._handle_reference(data[kw.ABERRATION_REFERENCE], kw.ABERRATIONS_TABLE),
             ))
 
     def _handle_wavefront_sensors(self, hdus: fits.HDUList):
         self._check_bintable(hdus, kw.WAVEFRONT_SENSORS_TABLE)
 
@@ -640,17 +624,16 @@
                     warnings.warn(f"Unexpected value for '{kw.WAVEFRONT_SENSOR_DIMENSIONS}' in wavefront sensor '{uid}'"
                                   f" of type '{t}'. Expected 2, got {dimensions}.")
                 wfs = aotpy.ShackHartmann(
                     uid=uid,
                     source=source,
                     n_valid_subapertures=n_valid_subapertures,
                     centroiding_algorithm=other_data[kw.WAVEFRONT_SENSOR_SHACK_HARTMANN_CENTROIDING_ALGORITHM],
-                    centroid_gains=self._handle_reference(
-                        other_data[kw.WAVEFRONT_SENSOR_SHACK_HARTMANN_CENTROID_GAINS]),
-                    spot_fwhm=self._handle_reference(other_data[kw.WAVEFRONT_SENSOR_SHACK_HARTMANN_SPOT_FWHM])
+                    centroid_gains=self._handle_image(other_data[kw.WAVEFRONT_SENSOR_SHACK_HARTMANN_CENTROID_GAINS]),
+                    spot_fwhm=self._handle_image(other_data[kw.WAVEFRONT_SENSOR_SHACK_HARTMANN_SPOT_FWHM])
                 )
             elif t == kw.WAVEFRONT_SENSOR_TYPE_PYRAMID:
                 # Try to find uid in secondary table
                 f = next((x for x in hdus[kw.WAVEFRONT_SENSORS_PYRAMID_TABLE].data if x[kw.REFERENCE_UID] == uid), None)
                 if f is None:
                     raise ValueError(f"Wavefront sensor '{uid}' not found in table "
                                      f"'{kw.WAVEFRONT_SENSORS_PYRAMID_TABLE}' even though it is of type '{t}'")
@@ -665,24 +648,24 @@
                     n_sides=other_data[kw.WAVEFRONT_SENSOR_PYRAMID_N_SIDES],
                     modulation=other_data[kw.WAVEFRONT_SENSOR_PYRAMID_MODULATION]
                 )
             else:
                 warnings.warn(f"Skipped wavefront sensor '{uid}': unknown type '{t}'.")
                 continue
 
-            wfs.measurements = self._handle_reference(data[kw.WAVEFRONT_SENSOR_MEASUREMENTS])
-            wfs.ref_measurements = self._handle_reference(data[kw.WAVEFRONT_SENSOR_REF_MEASUREMENTS])
-            wfs.subaperture_mask = self._handle_reference(data[kw.WAVEFRONT_SENSOR_SUBAPERTURE_MASK])
+            wfs.measurements = self._handle_image(data[kw.WAVEFRONT_SENSOR_MEASUREMENTS])
+            wfs.ref_measurements = self._handle_image(data[kw.WAVEFRONT_SENSOR_REF_MEASUREMENTS])
+            wfs.subaperture_mask = self._handle_image(data[kw.WAVEFRONT_SENSOR_SUBAPERTURE_MASK])
             wfs.mask_offsets = [aotpy.Coordinates(x, y) for x, y in zip(data[kw.WAVEFRONT_SENSOR_MASK_X_OFFSETS],
                                                                         data[kw.WAVEFRONT_SENSOR_MASK_Y_OFFSETS])]
             wfs.subaperture_size = data[kw.WAVEFRONT_SENSOR_SUBAPERTURE_SIZE]
-            wfs.subaperture_intensities = self._handle_reference(data[kw.WAVEFRONT_SENSOR_SUBAPERTURE_INTENSITIES])
+            wfs.subaperture_intensities = self._handle_image(data[kw.WAVEFRONT_SENSOR_SUBAPERTURE_INTENSITIES])
             wfs.wavelength = data[kw.WAVEFRONT_SENSOR_WAVELENGTH]
-            wfs.optical_gain = self._handle_reference(data[kw.WAVEFRONT_SENSOR_OPTICAL_GAIN])
-            wfs.geometry = self._handle_reference(data[kw.GEOMETRY_REFERENCE], kw.GEOMETRY_TABLE)
+            wfs.optical_gain = self._handle_image(data[kw.WAVEFRONT_SENSOR_OPTICAL_GAIN])
+            wfs.transformation_matrix = self._handle_image(data[kw.TRANSFORMATION_MATRIX])
             wfs.detector = self._handle_reference(data[kw.DETECTOR_REFERENCE], kw.DETECTORS_TABLE)
             wfs.aberration = self._handle_reference(data[kw.ABERRATION_REFERENCE], kw.ABERRATIONS_TABLE)
             wfs.non_common_path_aberration = self._handle_reference(data[kw.NCPA_REFERENCE], kw.ABERRATIONS_TABLE)
 
             self._wfss[uid] = [wfs, True]  # wavefront sensors are always referenced by AOSystem
             self._system.wavefront_sensors.append(wfs)
 
@@ -718,15 +701,15 @@
                 cor = aotpy.DeformableMirror(
                     uid=uid,
                     telescope=telescope,
                     n_valid_actuators=data[kw.WAVEFRONT_CORRECTOR_N_VALID_ACTUATORS],
                     actuator_coordinates=[aotpy.Coordinates(x, y) for x, y in
                                           zip(other_data[kw.WAVEFRONT_CORRECTOR_DM_ACTUATORS_X],
                                               other_data[kw.WAVEFRONT_CORRECTOR_DM_ACTUATORS_Y])],
-                    influence_function=self._handle_reference(other_data[kw.WAVEFRONT_CORRECTOR_DM_INFLUENCE_FUNCTION]),
+                    influence_function=self._handle_image(other_data[kw.WAVEFRONT_CORRECTOR_DM_INFLUENCE_FUNCTION]),
                     stroke=other_data[kw.WAVEFRONT_CORRECTOR_DM_STROKE]
                 )
             elif t == kw.WAVEFRONT_CORRECTOR_TYPE_TTM:
                 cor = aotpy.TipTiltMirror(
                     uid=uid,
                     telescope=telescope
                 )
@@ -735,18 +718,18 @@
                     uid=uid,
                     telescope=telescope
                 )
             else:
                 warnings.warn(f"Skipped wavefront corrector '{uid}': unknown type '{t}'.")
                 continue
 
-            cor.pupil_mask = self._handle_reference(data[kw.WAVEFRONT_CORRECTOR_PUPIL_MASK])
+            cor.pupil_mask = self._handle_image(data[kw.WAVEFRONT_CORRECTOR_PUPIL_MASK])
             cor.tfz_num = data[kw.WAVEFRONT_CORRECTOR_TFZ_NUM]
             cor.tfz_den = data[kw.WAVEFRONT_CORRECTOR_TFZ_DEN]
-            cor.geometry = self._handle_reference(data[kw.GEOMETRY_REFERENCE], kw.GEOMETRY_TABLE)
+            cor.transformation_matrix = self._handle_image(data[kw.TRANSFORMATION_MATRIX])
             cor.aberration = self._handle_reference(data[kw.ABERRATION_REFERENCE], kw.ABERRATIONS_TABLE)
 
             self._wfcs[uid] = [cor, True]  # wavefront corectors are always referenced by AOSystem
             self._system.wavefront_correctors.append(cor)
 
     def _handle_loops(self, hdus: fits.HDUList):
         self._check_bintable(hdus, kw.LOOPS_TABLE)
@@ -783,36 +766,38 @@
 
                 other_data = _convert_row(hdus[kw.LOOPS_CONTROL_TABLE].columns, f, kw.LOOPS_CONTROL_FIELDS)
                 loop = aotpy.ControlLoop(
                     uid=uid,
                     commanded_corrector=commanded,
                     input_sensor=self._handle_reference(other_data[kw.LOOPS_CONTROL_INPUT_SENSOR],
                                                         kw.WAVEFRONT_SENSORS_TABLE),
-                    control_matrix=self._handle_reference(other_data[kw.LOOPS_CONTROL_CONTROL_MATRIX]),
-                    measurements_to_modes=self._handle_reference(other_data[kw.LOOPS_CONTROL_MEASUREMENTS_TO_MODES]),
-                    modes_to_commands=self._handle_reference(other_data[kw.LOOPS_CONTROL_MODES_TO_COMMANDS]),
-                    interaction_matrix=self._handle_reference(other_data[kw.LOOPS_CONTROL_INTERACTION_MATRIX]),
-                    commands_to_modes=self._handle_reference(other_data[kw.LOOPS_CONTROL_COMMANDS_TO_MODES]),
-                    modes_to_measurements=self._handle_reference(other_data[kw.LOOPS_CONTROL_MODES_TO_MEASUREMENTS]),
-                    residual_commands=self._handle_reference(other_data[kw.LOOPS_CONTROL_RESIDUAL_COMMANDS])
+                    modes=self._handle_image(other_data[kw.LOOPS_CONTROL_MODES]),
+                    modal_coefficients=self._handle_image(other_data[kw.LOOPS_CONTROL_MODAL_COEFFICIENTS]),
+                    control_matrix=self._handle_image(other_data[kw.LOOPS_CONTROL_CONTROL_MATRIX]),
+                    measurements_to_modes=self._handle_image(other_data[kw.LOOPS_CONTROL_MEASUREMENTS_TO_MODES]),
+                    modes_to_commands=self._handle_image(other_data[kw.LOOPS_CONTROL_MODES_TO_COMMANDS]),
+                    interaction_matrix=self._handle_image(other_data[kw.LOOPS_CONTROL_INTERACTION_MATRIX]),
+                    commands_to_modes=self._handle_image(other_data[kw.LOOPS_CONTROL_COMMANDS_TO_MODES]),
+                    modes_to_measurements=self._handle_image(other_data[kw.LOOPS_CONTROL_MODES_TO_MEASUREMENTS]),
+                    residual_commands=self._handle_image(other_data[kw.LOOPS_CONTROL_RESIDUAL_COMMANDS])
                 )
             elif t == kw.LOOPS_TYPE_OFFLOAD:
                 # Try to find uid in secondary table
                 f = next((x for x in hdus[kw.LOOPS_OFFLOAD_TABLE].data if x[kw.REFERENCE_UID] == uid), None)
                 if f is None:
                     raise ValueError(f"Loop '{uid}' not found in table "
                                      f"'{kw.LOOPS_OFFLOAD_TABLE}' even though it is of type '{t}'")
 
                 other_data = _convert_row(hdus[kw.LOOPS_OFFLOAD_TABLE].columns, f, kw.LOOPS_OFFLOAD_FIELDS)
                 loop = aotpy.OffloadLoop(
                     uid=uid,
                     commanded_corrector=commanded,
                     input_corrector=self._handle_reference(other_data[kw.LOOPS_OFFLOAD_INPUT_CORRECTOR],
                                                            kw.WAVEFRONT_CORRECTORS_TABLE),
-                    offload_matrix=self._handle_reference(other_data[kw.LOOPS_OFFLOAD_OFFLOAD_MATRIX])
+                    offload_matrix=self._handle_image(other_data[kw.LOOPS_OFFLOAD_OFFLOAD_MATRIX])
                 )
             else:
                 warnings.warn(f"Skipped loop '{uid}': unknown type '{t}'.")
                 continue
 
             loop.time = self._handle_reference(data[kw.TIME_REFERENCE], kw.TIME_TABLE)
             if (status := data[kw.LOOPS_STATUS]) is None:
@@ -820,15 +805,15 @@
             elif status == kw.LOOPS_STATUS_CLOSED:
                 loop.closed = True
             elif status == kw.LOOPS_STATUS_OPEN:
                 loop.closed = False
             else:
                 warnings.warn(f"Ignored unknown loop status '{status}'.")
                 loop.closed = None
-            loop.commands = self._handle_reference(data[kw.LOOPS_COMMANDS])
-            loop.ref_commands = self._handle_reference(data[kw.LOOPS_REF_COMMANDS])
+            loop.commands = self._handle_image(data[kw.LOOPS_COMMANDS])
+            loop.ref_commands = self._handle_image(data[kw.LOOPS_REF_COMMANDS])
             loop.framerate = data[kw.LOOPS_FRAMERATE]
             loop.delay = data[kw.LOOPS_DELAY]
-            loop.time_filter_num = self._handle_reference(data[kw.LOOPS_TIME_FILTER_NUM])
-            loop.time_filter_den = self._handle_reference(data[kw.LOOPS_TIME_FILTER_DEN])
+            loop.time_filter_num = self._handle_image(data[kw.LOOPS_TIME_FILTER_NUM])
+            loop.time_filter_den = self._handle_image(data[kw.LOOPS_TIME_FILTER_DEN])
 
             self._system.loops.append(loop)
```

### Comparing `aotpy-0.5.1/aotpy/io/fits/utils.py` & `aotpy-0.6.0/aotpy/io/fits/utils.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.1/aotpy/io/fits/writer.py` & `aotpy-0.6.0/aotpy/io/fits/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,29 +187,14 @@
                 if image is self._images[image.name]:
                     # Image has already been handled before
                     return reference
                 raise ValueError(f'Repeated image name {image.name}.')
             self._images[image.name] = image
             return reference
 
-    def _handle_geometry(self, geo: aotpy.Geometry) -> str | None:
-        if geo is None:
-            return None
-        row = {
-            kw.REFERENCE_UID: geo.uid,
-            kw.TIME_REFERENCE: self._handle_time(geo.time),
-            kw.GEOMETRY_ROTATION: [i.rotation for i in geo.sequence],
-            kw.GEOMETRY_TRANSLATION_X: [i.translation.x for i in geo.sequence],
-            kw.GEOMETRY_TRANSLATION_Y: [i.translation.y for i in geo.sequence],
-            kw.GEOMETRY_MAGNIFICATION_X: [i.magnification.x for i in geo.sequence],
-            kw.GEOMETRY_MAGNIFICATION_Y: [i.magnification.y for i in geo.sequence]
-        }
-        self._add_to_table(kw.GEOMETRY_TABLE, geo, row)
-        return self._create_row_reference(geo.uid)
-
     def _handle_atmospheric_parameters(self, atm: aotpy.AtmosphericParameters) -> None:
         if atm is None:
             raise ValueError("'AOSystem.atmosphere_params' list cannot contain 'None' items.")
 
         row = {
             kw.REFERENCE_UID: atm.uid,
             kw.ATMOSPHERIC_PARAMETERS_WAVELENGTH: atm.wavelength,
@@ -219,15 +204,15 @@
             kw.ATMOSPHERIC_PARAMETERS_TAU0: atm.tau0,
             kw.ATMOSPHERIC_PARAMETERS_THETA0: atm.theta0,
             kw.ATMOSPHERIC_PARAMETERS_LAYERS_WEIGHT: self._handle_image(atm.layers_weight),
             kw.ATMOSPHERIC_PARAMETERS_LAYERS_HEIGHT: self._handle_image(atm.layers_height),
             kw.ATMOSPHERIC_PARAMETERS_LAYERS_L0: self._handle_image(atm.layers_l0),
             kw.ATMOSPHERIC_PARAMETERS_LAYERS_WIND_SPEED: self._handle_image(atm.layers_wind_speed),
             kw.ATMOSPHERIC_PARAMETERS_LAYERS_WIND_DIRECTION: self._handle_image(atm.layers_wind_direction),
-            kw.GEOMETRY_REFERENCE: self._handle_geometry(atm.geometry),
+            kw.TRANSFORMATION_MATRIX: self._handle_image(atm.transformation_matrix),
         }
         self._add_to_table(kw.ATMOSPHERIC_PARAMETERS_TABLE, atm, row)
 
     def _handle_aberration(self, abr: aotpy.Aberration) -> str | None:
         if abr is None:
             return None
 
@@ -291,15 +276,15 @@
             kw.TELESCOPE_ENCLOSING_D: tel.enclosing_diameter,
             kw.TELESCOPE_INSCRIBED_D: tel.inscribed_diameter,
             kw.TELESCOPE_OBSTRUCTION_D: tel.obstruction_diameter,
             kw.TELESCOPE_SEGMENTS_TYPE: segments_type,
             kw.TELESCOPE_SEGMENTS_SIZE: segments_size,
             kw.TELESCOPE_SEGMENTS_X: segments_x,
             kw.TELESCOPE_SEGMENTS_Y: segments_y,
-            kw.GEOMETRY_REFERENCE: self._handle_geometry(tel.geometry),
+            kw.TRANSFORMATION_MATRIX: self._handle_image(tel.transformation_matrix),
             kw.ABERRATION_REFERENCE: self._handle_aberration(tel.aberration)
         }
         if self._add_to_table(kw.TELESCOPES_TABLE, tel, row) and referenced and main:
             raise ValueError(
                 "Telescope references cannot reference a 'MainTelescope' object that is not AOSystem.main_telescope.")
         return self._create_row_reference(tel.uid)
 
@@ -374,28 +359,28 @@
             kw.DETECTOR_GAIN: det.gain,
             kw.DETECTOR_EXCESS_NOISE: det.excess_noise,
             kw.DETECTOR_FILTER: det.filter,
             kw.DETECTOR_BAD_PIXEL_MAP: self._handle_image(det.bad_pixel_map),
             kw.DETECTOR_DYNAMIC_RANGE: det.dynamic_range,
             kw.DETECTOR_READOUT_RATE: det.readout_rate,
             kw.DETECTOR_FRAME_RATE: det.frame_rate,
-            kw.GEOMETRY_REFERENCE: self._handle_geometry(det.geometry)
+            kw.TRANSFORMATION_MATRIX: self._handle_image(det.transformation_matrix),
         }
         self._add_to_table(kw.DETECTORS_TABLE, det, row)
         return self._create_row_reference(det.uid)
 
     def _handle_scoring_camera(self, cam: aotpy.ScoringCamera) -> None:
         if cam is None:
             raise ValueError("'AOSystem.scoring_cameras' list cannot contain 'None' items.")
 
         row = {
             kw.REFERENCE_UID: cam.uid,
             kw.SCORING_CAMERA_PUPIL_MASK: self._handle_image(cam.pupil_mask),
             kw.SCORING_CAMERA_WAVELENGTH: cam.wavelength,
-            kw.GEOMETRY_REFERENCE: self._handle_geometry(cam.geometry),
+            kw.TRANSFORMATION_MATRIX: self._handle_image(cam.transformation_matrix),
             kw.DETECTOR_REFERENCE: self._handle_detector(cam.detector),
             kw.ABERRATION_REFERENCE: self._handle_aberration(cam.aberration)
         }
         self._add_to_table(kw.SCORING_CAMERAS_TABLE, cam, row)
 
     def _handle_wavefront_sensor(self, wfs: aotpy.WavefrontSensor, referenced: bool) -> str | None:
         if wfs is None:
@@ -434,18 +419,18 @@
             kw.WAVEFRONT_SENSOR_SUBAPERTURE_MASK: self._handle_image(wfs.subaperture_mask),
             kw.WAVEFRONT_SENSOR_MASK_X_OFFSETS: [off.x for off in wfs.mask_offsets],
             kw.WAVEFRONT_SENSOR_MASK_Y_OFFSETS: [off.y for off in wfs.mask_offsets],
             kw.WAVEFRONT_SENSOR_SUBAPERTURE_SIZE: wfs.subaperture_size,
             kw.WAVEFRONT_SENSOR_SUBAPERTURE_INTENSITIES: self._handle_image(wfs.subaperture_intensities),
             kw.WAVEFRONT_SENSOR_WAVELENGTH: wfs.wavelength,
             kw.WAVEFRONT_SENSOR_OPTICAL_GAIN: self._handle_image(wfs.optical_gain),
-            kw.GEOMETRY_REFERENCE: self._handle_geometry(wfs.geometry),
+            kw.TRANSFORMATION_MATRIX: self._handle_image(wfs.transformation_matrix),
             kw.DETECTOR_REFERENCE: self._handle_detector(wfs.detector),
             kw.ABERRATION_REFERENCE: self._handle_aberration(wfs.aberration),
-            kw.NCPA_REFERENCE: self._handle_aberration(wfs.aberration)
+            kw.NCPA_REFERENCE: self._handle_aberration(wfs.non_common_path_aberration)
         }
         if self._add_to_table(kw.WAVEFRONT_SENSORS_TABLE, wfs, row) and referenced:
             raise ValueError(
                 f"Wavefront Sensor '{wfs.uid}' is referenced but not present in 'AOSystem.wavefront_sensors'")
         return self._create_row_reference(wfs.uid)
 
     def _handle_wavefront_corrector(self, cor: aotpy.WavefrontCorrector, referenced: bool) -> str | None:
@@ -474,15 +459,15 @@
             kw.REFERENCE_UID: cor.uid,
             kw.WAVEFRONT_CORRECTOR_TYPE: cor_type,
             kw.TELESCOPE_REFERENCE: self._handle_telescope(cor.telescope, True),
             kw.WAVEFRONT_CORRECTOR_N_VALID_ACTUATORS: cor.n_valid_actuators,
             kw.WAVEFRONT_CORRECTOR_PUPIL_MASK: self._handle_image(cor.pupil_mask),
             kw.WAVEFRONT_CORRECTOR_TFZ_NUM: cor.tfz_num,
             kw.WAVEFRONT_CORRECTOR_TFZ_DEN: cor.tfz_den,
-            kw.GEOMETRY_REFERENCE: self._handle_geometry(cor.geometry),
+            kw.TRANSFORMATION_MATRIX: self._handle_image(cor.transformation_matrix),
             kw.ABERRATION_REFERENCE: self._handle_aberration(cor.aberration)
         }
         if self._add_to_table(kw.WAVEFRONT_CORRECTORS_TABLE, cor, row) and referenced:
             raise ValueError(
                 f"Wavefront Corrector '{cor.uid}' is referenced but not present in 'AOSystem.wavefront_correctors'")
         return self._create_row_reference(cor.uid)
 
@@ -491,14 +476,16 @@
             raise ValueError("'AOSystem.loops' list cannot contain 'None' items.")
 
         if isinstance(loop, aotpy.ControlLoop):
             loop_type = kw.LOOPS_TYPE_CONTROL
             row = {
                 kw.REFERENCE_UID: loop.uid,
                 kw.LOOPS_CONTROL_INPUT_SENSOR: self._handle_wavefront_sensor(loop.input_sensor, True),
+                kw.LOOPS_CONTROL_MODES: self._handle_image(loop.modes),
+                kw.LOOPS_CONTROL_MODAL_COEFFICIENTS: self._handle_image(loop.modal_coefficients),
                 kw.LOOPS_CONTROL_CONTROL_MATRIX: self._handle_image(loop.control_matrix),
                 kw.LOOPS_CONTROL_MEASUREMENTS_TO_MODES: self._handle_image(loop.measurements_to_modes),
                 kw.LOOPS_CONTROL_MODES_TO_COMMANDS: self._handle_image(loop.modes_to_commands),
                 kw.LOOPS_CONTROL_INTERACTION_MATRIX: self._handle_image(loop.interaction_matrix),
                 kw.LOOPS_CONTROL_COMMANDS_TO_MODES: self._handle_image(loop.commands_to_modes),
                 kw.LOOPS_CONTROL_MODES_TO_MEASUREMENTS: self._handle_image(loop.modes_to_measurements),
                 kw.LOOPS_CONTROL_RESIDUAL_COMMANDS: self._handle_image(loop.residual_commands)
```

### Comparing `aotpy-0.5.1/aotpy/translators/aof.py` & `aotpy-0.6.0/aotpy/translators/aof.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         path_lgs = Path(path_lgs)
         lgs_loop_frame = fits.getdata(path_lgs / f'{path_lgs.name}.fits', extname='LGSLoopFrame')
 
         self.dsm_valid = fits.getdata(path_lgs / 'RTC.USED_ACT_MAP.fits')[0] - 1
         # We have to subtract one because the array uses one-based indexing unlike Python
 
         self.dsm = aotpy.DeformableMirror(
-            uid=f'DSM',
+            uid='DSM',
             telescope=self.system.main_telescope,
             n_valid_actuators=self.dsm_valid.size,
         )
         self.system.wavefront_correctors.append(self.dsm)
 
         lgs_timestamps = lgs_loop_frame['Seconds'] + lgs_loop_frame['USeconds'] / 1.e6
         self.system.date_beginning = datetime.utcfromtimestamp(lgs_timestamps[0])
@@ -77,25 +77,17 @@
         proj_map = fits.getdata(path_lgs / f'JitCtr.PROJ_MAP_SCALED.fits')
         im_list = np.split(fits.getdata(path_lgs / f'RTC.IMref4Atm.fits')[:, self.dsm_valid], 4, axis=0)
         for i in range(1, 5):
             llt = aotpy.LaserLaunchTelescope(f'LLT{i}')
             lgs = aotpy.SodiumLaserGuideStar(uid=f'LGS{i}', laser_launch_telescope=llt)
             self.system.sources.append(lgs)
 
-            gradients = lgs_loop_frame[f'WFS{i}_Gradients']
-            # AOF gradients are ordered tip1, tilt1, tip2, tilt2, etc., so even numbers are tip and odd numbers are tilt
-            # We separate them, select the valid subapertures and then stack them
-            tip = gradients[:, ::2]
-            tilt = gradients[:, 1::2]
-            gradients = np.stack([tip, tilt], axis=1)
-
-            reference = fits.getdata(path_lgs / f'LGSAcq.DET{i}.REFSLP_WITH_OFFSETS.fits')[0]
-            tip = reference[::2]
-            tilt = reference[1::2]
-            reference = np.stack([tip, tilt], axis=0)
+            gradients = self._stack_slopes(lgs_loop_frame[f'WFS{i}_Gradients'], slope_axis=1)
+            reference = self._stack_slopes(fits.getdata(path_lgs / f'LGSAcq.DET{i}.REFSLP_WITH_OFFSETS.fits'),
+                                           slope_axis=1)[0]
             wfs = aotpy.ShackHartmann(
                 uid=f'LGS WFS{i}',
                 source=lgs,
                 n_valid_subapertures=n_valid_subapertures,
                 measurements=aotpy.Image(f'WFS{i}_Gradients', gradients),
                 ref_measurements=aotpy.Image(f'LGSAcq.DET{i}.REFSLP_WITH_OFFSETS', reference),
                 subaperture_mask=subaperture_mask,
@@ -105,23 +97,16 @@
             wfs.detector = aotpy.Detector(
                 uid=f'LGS DET{i}',
                 dark=image_from_file(path_lgs / f'LGSAcq.DET{i}.DARK.fits'),
                 weight_map=image_from_file(path_lgs / f'LGSAcq.DET{i}.WEIGHT.fits')
             )
             self.system.wavefront_sensors.append(wfs)
 
-            cm = fits.getdata(path_lgs / f'LGSRecn.REC{i}.HOCM.fits')[self.dsm_valid]
-            tip = cm[:, ::2]
-            tilt = cm[:, 1::2]
-            cm = np.stack([tip, tilt], axis=1)
-
-            im = im_list[i - 1]
-            tip = im[::2]
-            tilt = im[1::2]
-            im = np.stack([tip, tilt], axis=1)
+            cm = self._stack_slopes(fits.getdata(path_lgs / f'LGSRecn.REC{i}.HOCM.fits')[self.dsm_valid], slope_axis=1)
+            im = self._stack_slopes(im_list[i - 1], slope_axis=0)
             self.system.loops.append(aotpy.ControlLoop(
                 uid=f'High-order loop {i}',
                 input_sensor=wfs,
                 commanded_corrector=self.dsm,
                 commands=dsm_positions,
                 time=lgs_time,
                 framerate=1000,
@@ -132,18 +117,15 @@
             ))
 
             jit = aotpy.TipTiltMirror(
                 uid=f'Jitter{i}',
                 telescope=llt
             )
 
-            cm = fits.getdata(path_lgs / f'JitRecnOptimiser.JitCM{i}.fits')
-            tip = cm[:, ::2]
-            tilt = cm[:, 1::2]
-            cm = np.stack([tip, tilt], axis=1)
+            cm = self._stack_slopes(fits.getdata(path_lgs / f'JitRecnOptimiser.JitCM{i}.fits'), slope_axis=1)
             self.system.loops.append(aotpy.ControlLoop(
                 uid=f'Jitter loop {i}',
                 input_sensor=wfs,
                 commanded_corrector=jit,
                 commands=aotpy.Image(f'Jitter{i}_Positions', lgs_loop_frame[f'Jitter{i}_Positions']),
                 ref_commands=aotpy.Image(f'Jit{i}Ctr.ACT_POS_REF_MAP_WITH_OFFSETS', jit_ref[(i - 1) * 2: i * 2]),
                 time=lgs_time,
@@ -185,23 +167,16 @@
             ngs_timestamps_list = ngs_timestamps.tolist()
         ho_frame_numbers = ir_loop_frame['HOFrameCounter']
         ir_time = aotpy.Time('NGS Loop Time', timestamps=ngs_timestamps_list, frame_numbers=ho_frame_numbers.tolist())
 
         ngs = aotpy.NaturalGuideStar('NGS')
         self.system.sources.append(ngs)
 
-        gradients = ir_loop_frame['WFS_Gradients']
-        tip = gradients[:, ::2]
-        tilt = gradients[:, 1::2]
-        gradients = np.stack([tip, tilt], axis=1)
-
-        reference = fits.getdata(path_ir / 'IRAcq.DET1.REFSLP_WITH_OFFSETS.fits')[0]
-        tip = reference[::2]
-        tilt = reference[1::2]
-        reference = np.stack([tip, tilt], axis=0)
+        gradients = self._stack_slopes(ir_loop_frame['WFS_Gradients'], slope_axis=1)
+        reference = self._stack_slopes(fits.getdata(path_ir / 'IRAcq.DET1.REFSLP_WITH_OFFSETS.fits'), slope_axis=1)[0]
         ngs_wfs = aotpy.ShackHartmann(
             uid='NGS WFS1',
             n_valid_subapertures=4,  # All subapertures are valid
             subaperture_mask=aotpy.Image('NGS_WFS_SUBAPERTURE_MASK', np.array([[1, 3], [2, 4]])),
             source=ngs,
             measurements=aotpy.Image('NGS_WFS_Gradients', gradients),
             ref_measurements=aotpy.Image('IRAcq.DET1.REFSLP_WITH_OFFSETS', reference),
@@ -223,23 +198,19 @@
                               frame_numbers=ho_frame_numbers[pix_time_mask].tolist())
 
         ngs_wfs.detector = aotpy.Detector(
             uid='NGS DET1',
             dark=image_from_file(path_ir / 'IRAcq.DET1.DARK.fits'),
             weight_map=image_from_file(path_ir / 'IRAcq.DET1.WEIGHT.fits'),
             pixel_intensities=aotpy.Image(name='NGS Pixels',
-                                          data=self.get_pixel_data_from_table(pix_loop_frame),
+                                          data=self._get_pixel_data_from_table(pix_loop_frame),
                                           time=pix_time)
         )
 
-        s2m = fits.getdata(path_ir / 'IRCtr.SENSOR_2_MODES.fits')
-        tip = s2m[:, ::2]
-        tilt = s2m[:, 1::2]
-        s2m = np.stack([tip, tilt], axis=1)
-
+        s2m = self._stack_slopes(fits.getdata(path_ir / 'IRCtr.SENSOR_2_MODES.fits'), slope_axis=1)
         m2c = fits.getdata(path_ir / 'IRCtr.MODES_2_ACT.fits')[self.dsm_valid]
         self.system.loops.append(aotpy.ControlLoop(
             uid='Low-order loop',
             input_sensor=ngs_wfs,
             commanded_corrector=self.dsm,
             commands=aotpy.Image('LO_Positions', ir_loop_frame['LO_Positions'][:, self.dsm_valid]),
             measurements_to_modes=aotpy.Image('IRCtr.SENSOR_2_MODES', s2m),
```

### Comparing `aotpy-0.5.1/aotpy/translators/base.py` & `aotpy-0.6.0/aotpy/translators/base.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.5.1/aotpy/translators/ciao.py` & `aotpy-0.6.0/aotpy/translators/ciao.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,98 +37,79 @@
             ao_mode='SCAO',
             strehl_ratio=main_hdr['ESO AOS ATM SR'],
             temporal_error=main_hdr['ESO AOS ATM TERR']
         )
         self.system.main_telescope = aotpy.MainTelescope(
             uid=f'ESO VLT AT{at_number}',
             elevation=main_hdr['ESO TEL ALT'],
-            azimuth=self.azimuth_conversion(main_hdr['ESO TEL AZ']),
+            azimuth=self._azimuth_conversion(main_hdr['ESO TEL AZ']),
             parallactic=main_hdr['ESO TEL PRLTIC']
         )
 
         ngs = aotpy.NaturalGuideStar('NGS',
                                      right_ascension=main_hdr['RA'],
                                      declination=main_hdr['DEC'])
 
         main_timestamps = main_loop_frame['Seconds'] + main_loop_frame['USeconds'] / 1.e6
         self.system.date_beginning = datetime.utcfromtimestamp(main_timestamps[0])
         self.system.date_end = datetime.utcfromtimestamp(main_timestamps[-1])
         main_frame_numbers = main_loop_frame['FrameCounter']
         loop_time = aotpy.Time('Loop Time', timestamps=main_timestamps.tolist(),
                                frame_numbers=main_frame_numbers.tolist())
 
-        wfs = aotpy.ShackHartmann('WFS', source=ngs, n_valid_subapertures=68,
-                                  detector=aotpy.Detector('SAPHIRA'))
-
-        gradients = main_loop_frame['Gradients']
-        # AOF gradients are ordered tip1, tilt1, tip2, tilt2, etc., so even numbers are tip and odd numbers are tilt
-        # We separate them, select the valid subapertures and then stack them
-        tip = gradients[:, ::2]
-        tilt = gradients[:, 1::2]
-        gradients = np.stack([tip, tilt], axis=1)
-        wfs.measurements = aotpy.Image('Gradients', gradients, time=loop_time)
-
-        reference = fits.getdata(path / 'Acq.DET1.REFSLP_0001.fits')[0]
-        tip = reference[::2]
-        tilt = reference[1::2]
-        reference = np.stack([tip, tilt], axis=0)
-        wfs.ref_measurements = aotpy.Image('Acq.DET1.REFSLP', reference)
-
-        wfs.subaperture_intensities = aotpy.Image(f'Intensities', main_loop_frame['Intensities'], time=loop_time)
+        gradients = self._stack_slopes(main_loop_frame['Gradients'], slope_axis=1)
+        reference = self._stack_slopes(fits.getdata(path / 'Acq.DET1.REFSLP_0001.fits'), slope_axis=1)[0]
+        wfs = aotpy.ShackHartmann(
+            uid='WFS',
+            source=ngs,
+            n_valid_subapertures=68,
+            detector=aotpy.Detector('SAPHIRA'),
+            measurements=aotpy.Image('Gradients', gradients, time=loop_time),
+            ref_measurements=aotpy.Image('Acq.DET1.REFSLP', reference),
+            subaperture_intensities=aotpy.Image(f'Intensities', main_loop_frame['Intensities'], time=loop_time),
+            centroiding_algorithm=main_hdr['ESO AOS ACQ CENTROID ALGO']
+        )
 
         pix_loop_frame = fits.getdata(path / 'CIAO_PIXELS_0001.fits')
         wfs.detector.pixel_intensities = aotpy.Image(
             'Pixels',
-            data=self.get_pixel_data_from_table(pix_loop_frame),
+            data=self._get_pixel_data_from_table(pix_loop_frame),
             time=aotpy.Time('Pixel time', frame_numbers=pix_loop_frame['FrameCounter'].tolist())
         )
 
-        wfs.centroiding_algorithm = main_hdr['ESO AOS ACQ CENTROID ALGO']
-
         ho_dm = aotpy.DeformableMirror('High Order Deformable Mirror (HODM)', telescope=self.system.main_telescope,
                                        n_valid_actuators=60)
         ittm = aotpy.TipTiltMirror('Image Tip-Tilt Mirror (ITTM)', telescope=self.system.main_telescope)
 
-        cm = fits.getdata(path / 'Recn.REC1.CM_0001.fits')
-        tip = cm[:, ::2]
-        tilt = cm[:, 1::2]
-        cm = np.stack([tip, tilt], axis=1)
+        cm = self._stack_slopes(fits.getdata(path / 'Recn.REC1.CM_0001.fits'), slope_axis=1)
         ho_cm = cm[: ho_dm.n_valid_actuators]
         tt_cm = cm[ho_dm.n_valid_actuators:]
 
-        s2m = fits.getdata(path / 'RecnOptimiser.S2M_0001.fits')
+        s2m = self._stack_slopes(fits.getdata(path / 'RecnOptimiser.S2M_0001.fits'), slope_axis=1)
         if main_hdr['ESO AOS CM MODES CONTROLLED'] != s2m.shape[0]:
             warnings.warn("Keyword 'ESO AOS CM MODES CONTROLLED' does not match modes in measurements to modes matrix")
-        tip = s2m[:, ::2]
-        tilt = s2m[:, 1::2]
-        s2m = np.stack([tip, tilt], axis=1)
         s2m = aotpy.Image('RecnOptimiser.S2M', s2m)
 
         m2c = fits.getdata(path / 'RecnOptimiser.M2V_0001.fits')
         ho_m2c = m2c[:ho_dm.n_valid_actuators]
         tt_m2c = m2c[ho_dm.n_valid_actuators:]
 
-        ho_im = fits.getdata(path / 'RecnOptimiser.HO_IM_0001.fits')
-        tip = ho_im[::2]
-        tilt = ho_im[1::2]
-        ho_im = np.stack([tip, tilt], axis=1)
-        ho_im = aotpy.Image('RecnOptimiser.HO_IM', ho_im)
-
+        ho_im = self._stack_slopes(fits.getdata(path / 'RecnOptimiser.HO_IM_0001.fits'), slope_axis=0)
         ho_loop = aotpy.ControlLoop(
             'HO Loop',
             input_sensor=wfs,
             commanded_corrector=ho_dm,
             time=loop_time,
             commands=aotpy.Image('HODM positions', main_loop_frame['HODM_Positions'], time=loop_time),
             ref_commands=aotpy.Image('HOCtr.ACT_POS_REF_MAP',
                                      fits.getdata(path / 'HOCtr.ACT_POS_REF_MAP_0001.fits')[0]),
             control_matrix=aotpy.Image('HO Control Matrix', ho_cm),
             measurements_to_modes=s2m,
             modes_to_commands=aotpy.Image('HO modes to commands', ho_m2c),
-            interaction_matrix=ho_im,
+            interaction_matrix=aotpy.Image('RecnOptimiser.HO_IM', ho_im),
             framerate=main_hdr['ESO AOS LOOP RATE'],
             closed=main_hdr['ESO AOS HO LOOP ST']
         )
 
         tt_loop = aotpy.ControlLoop(
             'TT Loop',
             input_sensor=wfs,
```

### Comparing `aotpy-0.5.1/aotpy/translators/eso.py` & `aotpy-0.6.0/aotpy/translators/eso.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         WHERE midpoint_date between '{beg}' and '{end}'
         AND valid=1
         """
         res = tap.TAPService(ESO_TAP_OBS).search(query).to_table()
         return res
 
     @staticmethod
-    def azimuth_conversion(az: float):
+    def _azimuth_conversion(az: float):
         """
         Convert azimuth from ESO's reference frame to AOT's reference frame.
 
         ESO's azimuth is measured westwards from the south, while in AOT it is defined as being measured from the
         eastward from the north.
 
         Parameters
@@ -179,15 +179,15 @@
         az
             ESO azimuth to be converted
         """
         # We need to subtract the angle between north and south and then apply symmetry.
         return -(az - 180) % 360
 
     @staticmethod
-    def get_pixel_data_from_table(pix_loop_frame: fits.FITS_rec) -> np.ndarray:
+    def _get_pixel_data_from_table(pix_loop_frame: fits.FITS_rec) -> np.ndarray:
         """
         Get properly reshaped pixel data from FITS binary table data.
 
         Parameters
         ----------
         pix_loop_frame
             Binary table data containing pixel image.
@@ -196,7 +196,21 @@
         sizes_y = pix_loop_frame['WindowSizeY']
         if np.any(sizes_x != sizes_x[0]) or np.any(sizes_y != sizes_y[0]):
             warnings.warn('Pixel window size seems to change over time.')
         sizes_x = sizes_x[0]
         sizes_y = sizes_y[0]
 
         return pix_loop_frame['Pixels'][:, :sizes_x * sizes_y].reshape(-1, sizes_x, sizes_y)
+
+    @staticmethod
+    def _stack_slopes(data: np.ndarray, slope_axis: int) -> np.ndarray:
+        # ESO slopes are ordered tip1, tilt1, tip2, tilt2, etc., so even numbers are tip and odd numbers are tilt.
+        # We separate and then stack them.
+        if slope_axis == 0:
+            tip = data[::2]
+            tilt = data[1::2]
+        elif slope_axis == 1:
+            tip = data[:, ::2]
+            tilt = data[:, 1::2]
+        else:
+            raise NotImplementedError
+        return np.stack([tip, tilt], axis=1)
```

### Comparing `aotpy-0.5.1/aotpy/translators/naomi.py` & `aotpy-0.6.0/aotpy/translators/naomi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This module contains a class for translating data produced by ESO's NAOMI system.
 """
 
+import importlib.resources
 import warnings
 from datetime import datetime
 from pathlib import Path
 
 import numpy as np
 from astropy.io import fits
 
@@ -28,101 +29,109 @@
     """
     def __init__(self, path: str, at_number: int):
         path = Path(path)
         self._at_number = at_number
 
         with fits.open(path / 'NAOMI_LOOP_0001.fits', extname='LoopFrame') as hdus:
             main_hdr = hdus[0].header
-            main_loop_frame = hdus['LoopFrame'].data
+            main_loop_frame: fits.FITS_rec = hdus['LoopFrame'].data
 
         self.system = aotpy.AOSystem(ao_mode='SCAO')
         self.system.main_telescope = aotpy.MainTelescope(
             uid=f'ESO VLT AT{at_number}',
             elevation=main_hdr['ESO TEL ALT'],
-            azimuth=self.azimuth_conversion(main_hdr['ESO TEL AZ']),
+            azimuth=self._azimuth_conversion(main_hdr['ESO TEL AZ']),
             parallactic=main_hdr['ESO TEL PRLTIC']
         )
+        naomi_data_path = importlib.resources.files('data') / 'NAOMI'
+        with importlib.resources.as_file(naomi_data_path / 'zernike_control_modes.fits') as p:
+            # Load file with the representation of the modes controlled in NAOMI (Zernike modes 2 to 15)
+            control_modes = aotpy.Image('CONTROL MODES', fits.getdata(p))
+
+        if main_hdr['ESO AOS CM MODES CONTROLLED'] != control_modes.data.shape[0]:
+            warnings.warn("Keyword 'ESO AOS CM MODES CONTROLLED' does not match expected number of control modes.")
 
         ngs = aotpy.NaturalGuideStar('NGS',
                                      right_ascension=main_hdr['RA'],
                                      declination=main_hdr['DEC'])
 
         main_timestamps = main_loop_frame['Seconds'] + main_loop_frame['USeconds'] / 1.e6
         self.system.date_beginning = datetime.utcfromtimestamp(main_timestamps[0])
         self.system.date_end = datetime.utcfromtimestamp(main_timestamps[-1])
         main_frame_numbers = main_loop_frame['FrameCounter']
         loop_time = aotpy.Time('Loop Time', timestamps=main_timestamps.tolist(),
                                frame_numbers=main_frame_numbers.tolist())
 
-        wfs = aotpy.ShackHartmann('WFS', source=ngs, n_valid_subapertures=12,
-                                  detector=aotpy.Detector('DET'))
+        gradients = self._stack_slopes(main_loop_frame['Gradients'], slope_axis=1)
+        reference = self._stack_slopes(fits.getdata(path / 'Acq.DET1.REFSLP_WITH_OFFSETS_0001.fits'), slope_axis=1)[0]
+        wfs = aotpy.ShackHartmann(
+            uid='WFS',
+            source=ngs,
+            n_valid_subapertures=12,
+            measurements=aotpy.Image('Gradients', gradients, time=loop_time),
+            ref_measurements=aotpy.Image('Acq.DET1.REFSLP_WITH_OFFSETS', reference),
+            subaperture_intensities=aotpy.Image(f'Intensities', main_loop_frame['Intensities'], time=loop_time)
+        )
 
-        gradients = main_loop_frame['Gradients']
-        # AOF gradients are ordered tip1, tilt1, tip2, tilt2, etc., so even numbers are tip and odd numbers are tilt
-        # We separate them, select the valid subapertures and then stack them
-        tip = gradients[:, ::2]
-        tilt = gradients[:, 1::2]
-        gradients = np.stack([tip, tilt], axis=1)
-
-        reference = fits.getdata(path / 'Acq.DET1.REFSLP_WITH_OFFSETS_0001.fits')[0]
-        tip = reference[::2]
-        tilt = reference[1::2]
-        reference = np.stack([tip, tilt], axis=0)
-
-        wfs.measurements = aotpy.Image('Gradients', gradients, time=loop_time)
-        wfs.ref_measurements = aotpy.Image('Acq.DET1.REFSLP_WITH_OFFSETS', reference)
-        wfs.subaperture_intensities = aotpy.Image(f'Intensities', main_loop_frame['Intensities'], time=loop_time)
-
-        wfs.detector.weight_map = image_from_file(path / 'Acq.DET1.WEIGHT_0001.fits')
-        wfs.detector.dark = image_from_file(path / 'Acq.DET1.DARK_0001.fits')
-        wfs.detector.flat_field = image_from_file(path / 'Acq.DET1.FLAT_0001.fits')
-        wfs.detector.bad_pixel_map = image_from_file(path / 'Acq.DET1.DEAD_0001.fits')
-        wfs.detector.sky_background = image_from_file(path / 'Acq.DET1.BACKGROUND_0001.fits')
+        wfs.non_common_path_aberration = aotpy.Aberration(
+            uid='NCPA',
+            modes=control_modes,
+            coefficients=image_from_file(path / 'Ctr.MODAL_OFFSETS_ROTATED_0001.fits')  # in DM modal space
+        )
+
+        wfs.detector = aotpy.Detector(
+            uid='DET',
+            weight_map=image_from_file(path / 'Acq.DET1.WEIGHT_0001.fits'),
+            dark=image_from_file(path / 'Acq.DET1.DARK_0001.fits'),
+            flat_field=image_from_file(path / 'Acq.DET1.FLAT_0001.fits'),
+            bad_pixel_map=image_from_file(path / 'Acq.DET1.DEAD_0001.fits'),
+            sky_background=image_from_file(path / 'Acq.DET1.BACKGROUND_0001.fits')
+        )
 
         pix_loop_frame = fits.getdata(path / 'NAOMI_PIXELS_0001.fits')
         wfs.detector.pixel_intensities = aotpy.Image(
             'Pixels',
-            data=self.get_pixel_data_from_table(pix_loop_frame),
+            data=self._get_pixel_data_from_table(pix_loop_frame),
             time=aotpy.Time('Pixel time', frame_numbers=pix_loop_frame['FrameCounter'].tolist())
         )
 
         dm = aotpy.DeformableMirror('DM', telescope=self.system.main_telescope, n_valid_actuators=241)
 
-        loop = aotpy.ControlLoop('Main Loop', input_sensor=wfs, commanded_corrector=dm, time=loop_time)
-        loop.time_filter_num = aotpy.Image('Ctr.TERM_A', fits.getdata(path / 'Ctr.TERM_A_0001.fits'))
-        loop.time_filter_den = aotpy.Image('Ctr.TERM_B', fits.getdata(path / 'Ctr.TERM_B_0001.fits'))
-
-        loop.commands = aotpy.Image('DM positions', main_loop_frame['Positions'], time=loop_time)
-        # loop.ref_commands = image_from_file(path / 'Ctr.ACT_POS_REF_MAP_0001.fits')
-        # loop.ref_commands.data = loop.ref_commands.data[0]
-        loop.ref_commands = aotpy.Image('Ctr.ACT_POS_REF_MAP', fits.getdata(path / 'Ctr.ACT_POS_REF_MAP_0001.fits'))
-
-        derotation_matrix = fits.getdata(path / 'RecnOptimiser.ROTATION_MATRIX_0001.fits').T
-
-        s2m = fits.getdata(path / 'Recn.REC1.CM_0001.fits')
-        s2m = s2m.T @ derotation_matrix
-        tip = s2m[::2]
-        tilt = s2m[1::2]
-        s2m = np.stack([tip, tilt], axis=1).T
-        loop.measurements_to_modes = aotpy.Image('Recn.REC1.CM', s2m)
-
-        loop.modes_to_commands = image_from_file(path / 'RTC.M2DM_SCALED_0001.fits')
-
-        if main_hdr['ESO AOS CM MODES CONTROLLED'] != s2m.shape[0]:
-            warnings.warn("Keyword 'ESO AOS CM MODES CONTROLLED' does not match modes in control matrix")
-
-        loop.commands_to_modes = image_from_file(path / 'RTC.DM2M_SCALED_0001.fits')
-        m2s = fits.getdata(path / 'ModalRecnCalibrat.REF_IM_0001.fits')
-        tip = m2s[::2]
-        tilt = m2s[1::2]
-        m2s = np.stack([tip, tilt], axis=1)
-        loop.modes_to_measurements = aotpy.Image('ModalRecnCalibrat.REF_IM', m2s)
-
-        loop.closed = main_hdr['ESO AOS LOOP ST']
-        loop.framerate = main_hdr['ESO AOS LOOP RATE']
+        modal_coefficients = main_loop_frame['ModalCoefficients']
+        modal_coefficients += fits.getdata(path / 'Ctr.MODAL_OFFSETS_ROTATED_0001.fits') * 2
+        # These are saved in the DM modal space. Need to add the rotated offsets to get the real coefficients that are
+        # then sent to the DM after M2DM conversion.
+        s2m = self._stack_slopes(fits.getdata(path / 'Recn.REC1.CM_0001.fits'), slope_axis=1)
+        # The S2M matrix is already rotated to to DM modes
+        m2s = self._stack_slopes(fits.getdata(path / 'ModalRecnCalibrat.REF_IM_0001.fits'), slope_axis=0)
+
+        try:
+            ref_commands = aotpy.Image('Ctr.ACT_POS_REF_MAP', fits.getdata(path / 'Ctr.ACT_POS_REF_MAP_0001.fits')[0])
+        except FileNotFoundError:
+            ref_commands = None
+            warnings.warn("Reference commands file not found ('Ctr.ACT_POS_REF_MAP_0001.fits').")
+
+        loop = aotpy.ControlLoop(
+            uid='Main Loop',
+            input_sensor=wfs,
+            commanded_corrector=dm,
+            time=loop_time,
+            time_filter_num=aotpy.Image('Ctr.TERM_A', fits.getdata(path / 'Ctr.TERM_A_0001.fits')),
+            time_filter_den=aotpy.Image('Ctr.TERM_B', fits.getdata(path / 'Ctr.TERM_B_0001.fits')),
+            commands=aotpy.Image('DM positions', main_loop_frame['Positions'], time=loop_time),
+            ref_commands=ref_commands,
+            modes=control_modes,
+            modal_coefficients=aotpy.Image('Modal Coefficients', modal_coefficients, time=loop_time),
+            measurements_to_modes=aotpy.Image('Recn.REC1.CM', s2m),
+            modes_to_commands=image_from_file(path / 'RTC.M2DM_SCALED_0001.fits'),
+            commands_to_modes=image_from_file(path / 'RTC.DM2M_SCALED_0001.fits'),
+            modes_to_measurements=aotpy.Image('ModalRecnCalibrat.REF_IM', m2s),
+            closed=main_hdr['ESO AOS LOOP ST'],
+            framerate=main_hdr['ESO AOS LOOP RATE']
+        )
 
         asm = aotpy.AtmosphericParameters(
             'ESO ASM (Astronomical Site Monitor)',
             wavelength=500e-9,
             fwhm=[main_hdr['ESO TEL AMBI FWHM']],
             tau0=[main_hdr['ESO TEL AMBI TAU0']],
             theta0=[main_hdr['ESO TEL AMBI THETA0']],
```

### Comparing `aotpy-0.5.1/aotpy.egg-info/PKG-INFO` & `aotpy-0.6.0/aotpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aotpy
-Version: 0.5.1
+Version: 0.6.0
 Summary: Helper package for handling Adaptive Optics Telemetry (AOT) standard files
 Home-page: https://github.com/kYwzor/aotpy
 Author: Tiago Gomes
 Author-email: tiagogomes@fe.up.pt
 Project-URL: Bug Tracker, https://github.com/kYwzor/aotpy/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aotpy-0.5.1/aotpy.egg-info/SOURCES.txt` & `aotpy-0.6.0/aotpy.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -28,10 +28,11 @@
 aotpy/io/fits/reader.py
 aotpy/io/fits/utils.py
 aotpy/io/fits/writer.py
 aotpy/translators/__init__.py
 aotpy/translators/aof.py
 aotpy/translators/base.py
 aotpy/translators/ciao.py
+aotpy/translators/eris.py
 aotpy/translators/eso.py
 aotpy/translators/naomi.py
 data/__init__.py
```

### Comparing `aotpy-0.5.1/setup.cfg` & `aotpy-0.6.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6f74 7079 0d0a 7665 7273 696f   = aotpy..versio
-00000020: 6e20 3d20 302e 352e 310d 0a61 7574 686f  n = 0.5.1..autho
+00000020: 6e20 3d20 302e 362e 300d 0a61 7574 686f  n = 0.6.0..autho
 00000030: 7220 3d20 5469 6167 6f20 476f 6d65 730d  r = Tiago Gomes.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 7469 6167 6f67 6f6d 6573 4066 652e 7570  tiagogomes@fe.up
 00000060: 2e70 740d 0a64 6573 6372 6970 7469 6f6e  .pt..description
 00000070: 203d 2048 656c 7065 7220 7061 636b 6167   = Helper packag
 00000080: 6520 666f 7220 6861 6e64 6c69 6e67 2041  e for handling A
 00000090: 6461 7074 6976 6520 4f70 7469 6373 2054  daptive Optics T
```

