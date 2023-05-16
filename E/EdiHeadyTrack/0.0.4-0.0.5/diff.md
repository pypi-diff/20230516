# Comparing `tmp/EdiHeadyTrack-0.0.4.tar.gz` & `tmp/EdiHeadyTrack-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/thomas/Library/CloudStorage/OneDrive-UniversityofEdinburgh/PhD/1. Working/1. Computational/EdiHeadyTrack - PACKAGE SOURC", last modified: Tue May 16 08:43:58 2023, max compression
+gzip compressed data, was "/Users/thomas/Library/CloudStorage/OneDrive-UniversityofEdinburgh/PhD/1. Working/1. Computational/EdiHeadyTrack - PACKAGE SOURC", last modified: Tue May 16 08:50:06 2023, max compression
```

## Comparing `EdiHeadyTrack-0.0.4.tar` & `EdiHeadyTrack-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 08:43:58.153594 EdiHeadyTrack-0.0.4/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 08:43:58.151364 EdiHeadyTrack-0.0.4/EdiHeadyTrack/
--rwxr-xr-x   0 thomas     (501) staff       (20)      475 2023-05-16 08:36:57.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack/__init__.py
--rwxr-xr-x   0 thomas     (501) staff       (20)     8554 2023-05-12 13:09:34.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack/calibration.py
--rw-r--r--   0 thomas     (501) staff       (20)     2883 2023-05-12 13:12:59.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack/camera.py
--rwxr-xr-x   0 thomas     (501) staff       (20)    15161 2023-05-16 08:42:22.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack/facedetector.py
--rw-r--r--   0 thomas     (501) staff       (20)     2763 2023-05-10 12:57:57.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack/filter.py
--rw-r--r--   0 thomas     (501) staff       (20)     5891 2023-05-12 13:40:15.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack/head.py
--rw-r--r--   0 thomas     (501) staff       (20)     3370 2023-05-10 12:57:57.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack/imu.py
--rw-r--r--   0 thomas     (501) staff       (20)     1029 2023-05-16 07:56:28.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack/load_sample.py
--rw-r--r--   0 thomas     (501) staff       (20)     9604 2023-05-16 08:43:03.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack/plot.py
--rw-r--r--   0 thomas     (501) staff       (20)     1492 2023-05-10 12:57:57.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack/sensordata.py
--rw-r--r--   0 thomas     (501) staff       (20)     3278 2023-05-12 13:26:00.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack/video.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 08:43:58.152484 EdiHeadyTrack-0.0.4/EdiHeadyTrack.egg-info/
--rw-r--r--   0 thomas     (501) staff       (20)     4383 2023-05-16 08:43:58.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)      588 2023-05-16 08:43:58.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (501) staff       (20)        1 2023-05-16 08:43:58.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (501) staff       (20)       78 2023-05-16 08:43:58.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack.egg-info/requires.txt
--rw-r--r--   0 thomas     (501) staff       (20)       19 2023-05-16 08:43:58.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack.egg-info/top_level.txt
--rw-r--r--   0 thomas     (501) staff       (20)    35149 2023-05-12 10:53:25.000000 EdiHeadyTrack-0.0.4/LICENSE
--rw-r--r--   0 thomas     (501) staff       (20)       33 2023-05-16 08:07:20.000000 EdiHeadyTrack-0.0.4/MANIFEST.in
--rw-r--r--   0 thomas     (501) staff       (20)     4383 2023-05-16 08:43:58.153744 EdiHeadyTrack-0.0.4/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)     3867 2023-05-12 14:52:31.000000 EdiHeadyTrack-0.0.4/README.md
--rw-r--r--   0 thomas     (501) staff       (20)       89 2023-05-12 09:37:25.000000 EdiHeadyTrack-0.0.4/pyproject.toml
--rw-r--r--   0 thomas     (501) staff       (20)      712 2023-05-16 08:43:58.154283 EdiHeadyTrack-0.0.4/setup.cfg
--rw-r--r--   0 thomas     (501) staff       (20)       77 2023-05-16 07:05:13.000000 EdiHeadyTrack-0.0.4/setup.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 08:43:58.153291 EdiHeadyTrack-0.0.4/test/
--rw-r--r--   0 thomas     (501) staff       (20)        0 2023-04-20 09:19:02.000000 EdiHeadyTrack-0.0.4/test/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)     1274 2023-04-20 09:19:02.000000 EdiHeadyTrack-0.0.4/test/test_calibrating.py
--rw-r--r--   0 thomas     (501) staff       (20)      230 2023-04-20 09:19:02.000000 EdiHeadyTrack-0.0.4/test/test_logging.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 08:50:06.138376 EdiHeadyTrack-0.0.5/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 08:50:06.136115 EdiHeadyTrack-0.0.5/EdiHeadyTrack/
+-rwxr-xr-x   0 thomas     (501) staff       (20)      475 2023-05-16 08:36:57.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack/__init__.py
+-rwxr-xr-x   0 thomas     (501) staff       (20)     8554 2023-05-12 13:09:34.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack/calibration.py
+-rw-r--r--   0 thomas     (501) staff       (20)     2883 2023-05-12 13:12:59.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack/camera.py
+-rwxr-xr-x   0 thomas     (501) staff       (20)    15161 2023-05-16 08:42:22.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack/facedetector.py
+-rw-r--r--   0 thomas     (501) staff       (20)     2763 2023-05-10 12:57:57.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack/filter.py
+-rw-r--r--   0 thomas     (501) staff       (20)     5891 2023-05-12 13:40:15.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack/head.py
+-rw-r--r--   0 thomas     (501) staff       (20)     3370 2023-05-10 12:57:57.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack/imu.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1029 2023-05-16 07:56:28.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack/load_sample.py
+-rw-r--r--   0 thomas     (501) staff       (20)     9604 2023-05-16 08:43:03.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack/plot.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1492 2023-05-10 12:57:57.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack/sensordata.py
+-rw-r--r--   0 thomas     (501) staff       (20)     3278 2023-05-12 13:26:00.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack/video.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 08:50:06.137314 EdiHeadyTrack-0.0.5/EdiHeadyTrack.egg-info/
+-rw-r--r--   0 thomas     (501) staff       (20)     4383 2023-05-16 08:50:06.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)      588 2023-05-16 08:50:06.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        1 2023-05-16 08:50:06.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       78 2023-05-16 08:50:06.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack.egg-info/requires.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       19 2023-05-16 08:50:06.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack.egg-info/top_level.txt
+-rw-r--r--   0 thomas     (501) staff       (20)    35149 2023-05-12 10:53:25.000000 EdiHeadyTrack-0.0.5/LICENSE
+-rw-r--r--   0 thomas     (501) staff       (20)       33 2023-05-16 08:07:20.000000 EdiHeadyTrack-0.0.5/MANIFEST.in
+-rw-r--r--   0 thomas     (501) staff       (20)     4383 2023-05-16 08:50:06.138482 EdiHeadyTrack-0.0.5/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)     3867 2023-05-12 14:52:31.000000 EdiHeadyTrack-0.0.5/README.md
+-rw-r--r--   0 thomas     (501) staff       (20)       89 2023-05-12 09:37:25.000000 EdiHeadyTrack-0.0.5/pyproject.toml
+-rw-r--r--   0 thomas     (501) staff       (20)      712 2023-05-16 08:50:06.138933 EdiHeadyTrack-0.0.5/setup.cfg
+-rw-r--r--   0 thomas     (501) staff       (20)       76 2023-05-16 08:44:42.000000 EdiHeadyTrack-0.0.5/setup.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 08:50:06.138094 EdiHeadyTrack-0.0.5/test/
+-rw-r--r--   0 thomas     (501) staff       (20)        0 2023-04-20 09:19:02.000000 EdiHeadyTrack-0.0.5/test/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1274 2023-04-20 09:19:02.000000 EdiHeadyTrack-0.0.5/test/test_calibrating.py
+-rw-r--r--   0 thomas     (501) staff       (20)      230 2023-04-20 09:19:02.000000 EdiHeadyTrack-0.0.5/test/test_logging.py
```

### Comparing `EdiHeadyTrack-0.0.4/EdiHeadyTrack/calibration.py` & `EdiHeadyTrack-0.0.5/EdiHeadyTrack/calibration.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.4/EdiHeadyTrack/camera.py` & `EdiHeadyTrack-0.0.5/EdiHeadyTrack/camera.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.4/EdiHeadyTrack/facedetector.py` & `EdiHeadyTrack-0.0.5/EdiHeadyTrack/facedetector.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.4/EdiHeadyTrack/filter.py` & `EdiHeadyTrack-0.0.5/EdiHeadyTrack/filter.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.4/EdiHeadyTrack/head.py` & `EdiHeadyTrack-0.0.5/EdiHeadyTrack/head.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.4/EdiHeadyTrack/imu.py` & `EdiHeadyTrack-0.0.5/EdiHeadyTrack/imu.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.4/EdiHeadyTrack/load_sample.py` & `EdiHeadyTrack-0.0.5/EdiHeadyTrack/load_sample.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.4/EdiHeadyTrack/plot.py` & `EdiHeadyTrack-0.0.5/EdiHeadyTrack/plot.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.4/EdiHeadyTrack/sensordata.py` & `EdiHeadyTrack-0.0.5/EdiHeadyTrack/sensordata.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.4/EdiHeadyTrack/video.py` & `EdiHeadyTrack-0.0.5/EdiHeadyTrack/video.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.4/EdiHeadyTrack.egg-info/PKG-INFO` & `EdiHeadyTrack-0.0.5/EdiHeadyTrack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdiHeadyTrack
-Version: 0.0.4
+Version: 0.0.5
 Summary: Automatic, markerless measurement of head kinematics using mediapipe and OpenCV
 Home-page: https://github.com/isDynamics/EdiHeadyTrack
 Author: Thomas Aston
 Author-email: thomas.aston@ed.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdiHeadyTrack Version: 0.0.4 Summary: Automatic,
+Metadata-Version: 2.1 Name: EdiHeadyTrack Version: 0.0.5 Summary: Automatic,
 markerless measurement of head kinematics using mediapipe and OpenCV Home-page:
 https://github.com/isDynamics/EdiHeadyTrack Author: Thomas Aston Author-email:
 thomas.aston@ed.ac.uk Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown License-File: LICENSE [![License: GPL
 v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/
```

### Comparing `EdiHeadyTrack-0.0.4/EdiHeadyTrack.egg-info/SOURCES.txt` & `EdiHeadyTrack-0.0.5/EdiHeadyTrack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.4/LICENSE` & `EdiHeadyTrack-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.4/PKG-INFO` & `EdiHeadyTrack-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdiHeadyTrack
-Version: 0.0.4
+Version: 0.0.5
 Summary: Automatic, markerless measurement of head kinematics using mediapipe and OpenCV
 Home-page: https://github.com/isDynamics/EdiHeadyTrack
 Author: Thomas Aston
 Author-email: thomas.aston@ed.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdiHeadyTrack Version: 0.0.4 Summary: Automatic,
+Metadata-Version: 2.1 Name: EdiHeadyTrack Version: 0.0.5 Summary: Automatic,
 markerless measurement of head kinematics using mediapipe and OpenCV Home-page:
 https://github.com/isDynamics/EdiHeadyTrack Author: Thomas Aston Author-email:
 thomas.aston@ed.ac.uk Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown License-File: LICENSE [![License: GPL
 v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/
```

### Comparing `EdiHeadyTrack-0.0.4/README.md` & `EdiHeadyTrack-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.4/setup.cfg` & `EdiHeadyTrack-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = EdiHeadyTrack
-version = 0.0.4
+version = 0.0.5
 author = Thomas Aston
 author_email = thomas.aston@ed.ac.uk
 description = Automatic, markerless measurement of head kinematics using mediapipe and OpenCV
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/isDynamics/EdiHeadyTrack
 classifiers =
```

### Comparing `EdiHeadyTrack-0.0.4/test/test_calibrating.py` & `EdiHeadyTrack-0.0.5/test/test_calibrating.py`

 * *Files identical despite different names*

