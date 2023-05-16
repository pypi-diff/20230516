# Comparing `tmp/EdiHeadyTrack-0.0.3.tar.gz` & `tmp/EdiHeadyTrack-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/thomas/Library/CloudStorage/OneDrive-UniversityofEdinburgh/PhD/1. Working/1. Computational/EdiHeadyTrack - PACKAGE SOURC", last modified: Tue May 16 08:29:47 2023, max compression
+gzip compressed data, was "/Users/thomas/Library/CloudStorage/OneDrive-UniversityofEdinburgh/PhD/1. Working/1. Computational/EdiHeadyTrack - PACKAGE SOURC", last modified: Tue May 16 08:43:58 2023, max compression
```

## Comparing `EdiHeadyTrack-0.0.3.tar` & `EdiHeadyTrack-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 08:29:47.865460 EdiHeadyTrack-0.0.3/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 08:29:47.863145 EdiHeadyTrack-0.0.3/EdiHeadyTrack/
--rwxr-xr-x   0 thomas     (501) staff       (20)      501 2023-05-12 08:33:18.000000 EdiHeadyTrack-0.0.3/EdiHeadyTrack/__init__.py
--rwxr-xr-x   0 thomas     (501) staff       (20)     8554 2023-05-12 13:09:34.000000 EdiHeadyTrack-0.0.3/EdiHeadyTrack/calibration.py
--rw-r--r--   0 thomas     (501) staff       (20)     2883 2023-05-12 13:12:59.000000 EdiHeadyTrack-0.0.3/EdiHeadyTrack/camera.py
--rwxr-xr-x   0 thomas     (501) staff       (20)    15120 2023-05-10 12:57:57.000000 EdiHeadyTrack-0.0.3/EdiHeadyTrack/facedetector.py
--rw-r--r--   0 thomas     (501) staff       (20)     2763 2023-05-10 12:57:57.000000 EdiHeadyTrack-0.0.3/EdiHeadyTrack/filter.py
--rw-r--r--   0 thomas     (501) staff       (20)     5891 2023-05-12 13:40:15.000000 EdiHeadyTrack-0.0.3/EdiHeadyTrack/head.py
--rw-r--r--   0 thomas     (501) staff       (20)     3370 2023-05-10 12:57:57.000000 EdiHeadyTrack-0.0.3/EdiHeadyTrack/imu.py
--rw-r--r--   0 thomas     (501) staff       (20)     1029 2023-05-16 07:56:28.000000 EdiHeadyTrack-0.0.3/EdiHeadyTrack/load_sample.py
--rw-r--r--   0 thomas     (501) staff       (20)     9616 2023-05-12 14:02:08.000000 EdiHeadyTrack-0.0.3/EdiHeadyTrack/plot.py
--rw-r--r--   0 thomas     (501) staff       (20)     1492 2023-05-10 12:57:57.000000 EdiHeadyTrack-0.0.3/EdiHeadyTrack/sensordata.py
--rw-r--r--   0 thomas     (501) staff       (20)     3278 2023-05-12 13:26:00.000000 EdiHeadyTrack-0.0.3/EdiHeadyTrack/video.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 08:29:47.864373 EdiHeadyTrack-0.0.3/EdiHeadyTrack.egg-info/
--rw-r--r--   0 thomas     (501) staff       (20)     4383 2023-05-16 08:29:47.000000 EdiHeadyTrack-0.0.3/EdiHeadyTrack.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)      588 2023-05-16 08:29:47.000000 EdiHeadyTrack-0.0.3/EdiHeadyTrack.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (501) staff       (20)        1 2023-05-16 08:29:47.000000 EdiHeadyTrack-0.0.3/EdiHeadyTrack.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (501) staff       (20)       78 2023-05-16 08:29:47.000000 EdiHeadyTrack-0.0.3/EdiHeadyTrack.egg-info/requires.txt
--rw-r--r--   0 thomas     (501) staff       (20)       19 2023-05-16 08:29:47.000000 EdiHeadyTrack-0.0.3/EdiHeadyTrack.egg-info/top_level.txt
--rw-r--r--   0 thomas     (501) staff       (20)    35149 2023-05-12 10:53:25.000000 EdiHeadyTrack-0.0.3/LICENSE
--rw-r--r--   0 thomas     (501) staff       (20)       33 2023-05-16 08:07:20.000000 EdiHeadyTrack-0.0.3/MANIFEST.in
--rw-r--r--   0 thomas     (501) staff       (20)     4383 2023-05-16 08:29:47.865582 EdiHeadyTrack-0.0.3/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)     3867 2023-05-12 14:52:31.000000 EdiHeadyTrack-0.0.3/README.md
--rw-r--r--   0 thomas     (501) staff       (20)       89 2023-05-12 09:37:25.000000 EdiHeadyTrack-0.0.3/pyproject.toml
--rw-r--r--   0 thomas     (501) staff       (20)      712 2023-05-16 08:29:47.866043 EdiHeadyTrack-0.0.3/setup.cfg
--rw-r--r--   0 thomas     (501) staff       (20)       77 2023-05-16 07:05:13.000000 EdiHeadyTrack-0.0.3/setup.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 08:29:47.865081 EdiHeadyTrack-0.0.3/test/
--rw-r--r--   0 thomas     (501) staff       (20)        0 2023-04-20 09:19:02.000000 EdiHeadyTrack-0.0.3/test/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)     1274 2023-04-20 09:19:02.000000 EdiHeadyTrack-0.0.3/test/test_calibrating.py
--rw-r--r--   0 thomas     (501) staff       (20)      230 2023-04-20 09:19:02.000000 EdiHeadyTrack-0.0.3/test/test_logging.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 08:43:58.153594 EdiHeadyTrack-0.0.4/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 08:43:58.151364 EdiHeadyTrack-0.0.4/EdiHeadyTrack/
+-rwxr-xr-x   0 thomas     (501) staff       (20)      475 2023-05-16 08:36:57.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack/__init__.py
+-rwxr-xr-x   0 thomas     (501) staff       (20)     8554 2023-05-12 13:09:34.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack/calibration.py
+-rw-r--r--   0 thomas     (501) staff       (20)     2883 2023-05-12 13:12:59.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack/camera.py
+-rwxr-xr-x   0 thomas     (501) staff       (20)    15161 2023-05-16 08:42:22.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack/facedetector.py
+-rw-r--r--   0 thomas     (501) staff       (20)     2763 2023-05-10 12:57:57.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack/filter.py
+-rw-r--r--   0 thomas     (501) staff       (20)     5891 2023-05-12 13:40:15.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack/head.py
+-rw-r--r--   0 thomas     (501) staff       (20)     3370 2023-05-10 12:57:57.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack/imu.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1029 2023-05-16 07:56:28.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack/load_sample.py
+-rw-r--r--   0 thomas     (501) staff       (20)     9604 2023-05-16 08:43:03.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack/plot.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1492 2023-05-10 12:57:57.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack/sensordata.py
+-rw-r--r--   0 thomas     (501) staff       (20)     3278 2023-05-12 13:26:00.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack/video.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 08:43:58.152484 EdiHeadyTrack-0.0.4/EdiHeadyTrack.egg-info/
+-rw-r--r--   0 thomas     (501) staff       (20)     4383 2023-05-16 08:43:58.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)      588 2023-05-16 08:43:58.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        1 2023-05-16 08:43:58.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       78 2023-05-16 08:43:58.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack.egg-info/requires.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       19 2023-05-16 08:43:58.000000 EdiHeadyTrack-0.0.4/EdiHeadyTrack.egg-info/top_level.txt
+-rw-r--r--   0 thomas     (501) staff       (20)    35149 2023-05-12 10:53:25.000000 EdiHeadyTrack-0.0.4/LICENSE
+-rw-r--r--   0 thomas     (501) staff       (20)       33 2023-05-16 08:07:20.000000 EdiHeadyTrack-0.0.4/MANIFEST.in
+-rw-r--r--   0 thomas     (501) staff       (20)     4383 2023-05-16 08:43:58.153744 EdiHeadyTrack-0.0.4/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)     3867 2023-05-12 14:52:31.000000 EdiHeadyTrack-0.0.4/README.md
+-rw-r--r--   0 thomas     (501) staff       (20)       89 2023-05-12 09:37:25.000000 EdiHeadyTrack-0.0.4/pyproject.toml
+-rw-r--r--   0 thomas     (501) staff       (20)      712 2023-05-16 08:43:58.154283 EdiHeadyTrack-0.0.4/setup.cfg
+-rw-r--r--   0 thomas     (501) staff       (20)       77 2023-05-16 07:05:13.000000 EdiHeadyTrack-0.0.4/setup.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 08:43:58.153291 EdiHeadyTrack-0.0.4/test/
+-rw-r--r--   0 thomas     (501) staff       (20)        0 2023-04-20 09:19:02.000000 EdiHeadyTrack-0.0.4/test/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1274 2023-04-20 09:19:02.000000 EdiHeadyTrack-0.0.4/test/test_calibrating.py
+-rw-r--r--   0 thomas     (501) staff       (20)      230 2023-04-20 09:19:02.000000 EdiHeadyTrack-0.0.4/test/test_logging.py
```

### Comparing `EdiHeadyTrack-0.0.3/EdiHeadyTrack/calibration.py` & `EdiHeadyTrack-0.0.4/EdiHeadyTrack/calibration.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.3/EdiHeadyTrack/camera.py` & `EdiHeadyTrack-0.0.4/EdiHeadyTrack/camera.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.3/EdiHeadyTrack/facedetector.py` & `EdiHeadyTrack-0.0.4/EdiHeadyTrack/facedetector.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #                                                                              #
 #                                                         :::      ::::::::    #
 #    facedetector.py                                    :+:      :+:    :+:    #
 #                                                     +:+ +:+         +:+      #
 #    By: taston <thomas.aston@ed.ac.uk>             +#+  +:+       +#+         #
 #                                                 +#+#+#+#+#+   +#+            #
 #    Created: 2023/02/10 16:43:13 by taston            #+#    #+#              #
-#    Updated: 2023/05/10 11:29:21 by taston           ###   ########.fr        #
+#    Updated: 2023/05/16 09:42:22 by taston           ###   ########.fr        #
 #                                                                              #
 # **************************************************************************** #
 
 import cv2
 import mediapipe as mp
 import numpy as np
 from numpy import genfromtxt
@@ -153,15 +153,15 @@
         while True:
             success, img = self.video.cap.read()
             if success:
                 progress_bar.update(1)
                 # current_frame = int(self.video.cap.get(1))
                 self.find_faces(img)
                 cv2.namedWindow("EdiHeadyTrack", cv2.WINDOW_NORMAL)
-                cv2.resizeWindow("EdiHeadyTrack", 640, 360)
+                cv2.resizeWindow("EdiHeadyTrack", int(self.video.width/2), int(self.video.height/2))
                 cv2.imshow("EdiHeadyTrack", img)
                 # cv2.imwrite(f'tracking frames/{current_frame}.png', img)
                 
                 if cv2.waitKey(5) & 0xFF == ord('q'):
                     progress_bar.close()
                     print('Face tracking interuppted...')
                     break
```

### Comparing `EdiHeadyTrack-0.0.3/EdiHeadyTrack/filter.py` & `EdiHeadyTrack-0.0.4/EdiHeadyTrack/filter.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.3/EdiHeadyTrack/head.py` & `EdiHeadyTrack-0.0.4/EdiHeadyTrack/head.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.3/EdiHeadyTrack/imu.py` & `EdiHeadyTrack-0.0.4/EdiHeadyTrack/imu.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.3/EdiHeadyTrack/load_sample.py` & `EdiHeadyTrack-0.0.4/EdiHeadyTrack/load_sample.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.3/EdiHeadyTrack/plot.py` & `EdiHeadyTrack-0.0.4/EdiHeadyTrack/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #                                                                              #
 #                                                         :::      ::::::::    #
 #    plot.py                                            :+:      :+:    :+:    #
 #                                                     +:+ +:+         +:+      #
 #    By: taston <thomas.aston@ed.ac.uk>             +#+  +:+       +#+         #
 #                                                 +#+#+#+#+#+   +#+            #
 #    Created: 2023/04/27 10:18:49 by taston            #+#    #+#              #
-#    Updated: 2023/05/12 15:02:08 by taston           ###   ########.fr        #
+#    Updated: 2023/05/16 09:43:03 by taston           ###   ########.fr        #
 #                                                                              #
 # **************************************************************************** #
 
 
 from .head import Head
 from .imu import IMU
 from .sensordata import SensorData
@@ -214,9 +214,9 @@
                                         boxcoords="offset points",
                                         pad=0.01,
                                         bboxprops =dict(edgecolor='white')
                                         )
 
                     ax1.add_artist(ab)
         
-        plt.savefig('EdiHeadyTrack/resources/comparison.png', bbox_inches='tight')
+        # plt.savefig('resources/comparison.png', bbox_inches='tight')
         plt.show()
```

### Comparing `EdiHeadyTrack-0.0.3/EdiHeadyTrack/sensordata.py` & `EdiHeadyTrack-0.0.4/EdiHeadyTrack/sensordata.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.3/EdiHeadyTrack/video.py` & `EdiHeadyTrack-0.0.4/EdiHeadyTrack/video.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.3/EdiHeadyTrack.egg-info/PKG-INFO` & `EdiHeadyTrack-0.0.4/EdiHeadyTrack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdiHeadyTrack
-Version: 0.0.3
+Version: 0.0.4
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
-Metadata-Version: 2.1 Name: EdiHeadyTrack Version: 0.0.3 Summary: Automatic,
+Metadata-Version: 2.1 Name: EdiHeadyTrack Version: 0.0.4 Summary: Automatic,
 markerless measurement of head kinematics using mediapipe and OpenCV Home-page:
 https://github.com/isDynamics/EdiHeadyTrack Author: Thomas Aston Author-email:
 thomas.aston@ed.ac.uk Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown License-File: LICENSE [![License: GPL
 v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/
```

### Comparing `EdiHeadyTrack-0.0.3/EdiHeadyTrack.egg-info/SOURCES.txt` & `EdiHeadyTrack-0.0.4/EdiHeadyTrack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.3/LICENSE` & `EdiHeadyTrack-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.3/PKG-INFO` & `EdiHeadyTrack-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdiHeadyTrack
-Version: 0.0.3
+Version: 0.0.4
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
-Metadata-Version: 2.1 Name: EdiHeadyTrack Version: 0.0.3 Summary: Automatic,
+Metadata-Version: 2.1 Name: EdiHeadyTrack Version: 0.0.4 Summary: Automatic,
 markerless measurement of head kinematics using mediapipe and OpenCV Home-page:
 https://github.com/isDynamics/EdiHeadyTrack Author: Thomas Aston Author-email:
 thomas.aston@ed.ac.uk Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown License-File: LICENSE [![License: GPL
 v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/
```

### Comparing `EdiHeadyTrack-0.0.3/README.md` & `EdiHeadyTrack-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.3/setup.cfg` & `EdiHeadyTrack-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = EdiHeadyTrack
-version = 0.0.3
+version = 0.0.4
 author = Thomas Aston
 author_email = thomas.aston@ed.ac.uk
 description = Automatic, markerless measurement of head kinematics using mediapipe and OpenCV
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/isDynamics/EdiHeadyTrack
 classifiers =
```

### Comparing `EdiHeadyTrack-0.0.3/test/test_calibrating.py` & `EdiHeadyTrack-0.0.4/test/test_calibrating.py`

 * *Files identical despite different names*

