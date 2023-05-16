# Comparing `tmp/roboidai-1.1.8.tar.gz` & `tmp/roboidai-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\roboidai-1.1.8.tar", last modified: Sun Dec 27 08:52:04 2020, max compression
+gzip compressed data, was "dist\roboidai-1.1.9.tar", last modified: Thu Feb  4 22:23:17 2021, max compression
```

## Comparing `roboidai-1.1.8.tar` & `roboidai-1.1.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2020-12-27 08:52:04.822537 roboidai-1.1.8/
--rw-rw-rw-   0        0        0      802 2020-08-22 18:46:05.000000 roboidai-1.1.8/LICENSE
--rw-rw-rw-   0        0        0      241 2020-12-17 17:34:48.000000 roboidai-1.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0      649 2020-12-27 08:52:04.823536 roboidai-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      197 2020-12-17 17:05:23.000000 roboidai-1.1.8/README.md
--rw-rw-rw-   0        0        0      175 2020-12-27 07:18:14.000000 roboidai-1.1.8/requirements.txt
-drwxrwxrwx   0        0        0        0 2020-12-27 08:52:04.684529 roboidai-1.1.8/roboidai/
--rw-rw-rw-   0        0        0     2041 2020-12-27 07:17:52.000000 roboidai-1.1.8/roboidai/__init__.py
--rw-rw-rw-   0        0        0    15510 2020-12-27 08:36:55.000000 roboidai-1.1.8/roboidai/_camera.py
-drwxrwxrwx   0        0        0        0 2020-12-27 08:52:04.712530 roboidai-1.1.8/roboidai/_image/
--rw-rw-rw-   0        0        0        0 2020-12-25 13:05:51.000000 roboidai-1.1.8/roboidai/_image/__init__.py
--rw-rw-rw-   0        0        0     7799 2020-12-27 08:39:08.000000 roboidai-1.1.8/roboidai/_image/_age_gender.py
--rw-rw-rw-   0        0        0     7548 2020-12-27 08:39:49.000000 roboidai-1.1.8/roboidai/_image/_face_detector.py
--rw-rw-rw-   0        0        0     7215 2020-12-27 08:40:26.000000 roboidai-1.1.8/roboidai/_image/_face_marker.py
--rw-rw-rw-   0        0        0    20191 2020-12-27 08:41:03.000000 roboidai-1.1.8/roboidai/_image/_object_detector.py
--rw-rw-rw-   0        0        0     5794 2020-12-27 08:41:40.000000 roboidai-1.1.8/roboidai/_image/_tool.py
--rw-rw-rw-   0        0        0     3970 2020-12-27 08:37:36.000000 roboidai-1.1.8/roboidai/_keyevent.py
-drwxrwxrwx   0        0        0        0 2020-12-27 08:52:04.756533 roboidai-1.1.8/roboidai/_model/
--rw-rw-rw-   0        0        0 10666211 2020-12-25 13:05:51.000000 roboidai-1.1.8/roboidai/_model/face.caffemodel
--rw-rw-rw-   0        0        0    28091 2020-12-25 13:05:51.000000 roboidai-1.1.8/roboidai/_model/face.prototxt
--rw-rw-rw-   0        0        0      620 2020-12-25 13:05:51.000000 roboidai-1.1.8/roboidai/_model/object_labels.txt
-drwxrwxrwx   0        0        0        0 2020-12-27 08:52:04.764533 roboidai-1.1.8/roboidai/_tm/
--rw-rw-rw-   0        0        0        0 2020-12-25 13:05:51.000000 roboidai-1.1.8/roboidai/_tm/__init__.py
--rw-rw-rw-   0        0        0     5662 2020-12-27 08:42:30.000000 roboidai-1.1.8/roboidai/_tm/_image.py
--rw-rw-rw-   0        0        0     4294 2020-12-27 08:38:18.000000 roboidai-1.1.8/roboidai/_window.py
-drwxrwxrwx   0        0        0        0 2020-12-27 08:52:04.815536 roboidai-1.1.8/roboidai/lab/
--rw-rw-rw-   0        0        0     2894 2020-12-26 17:03:26.000000 roboidai-1.1.8/roboidai/lab/__init__.py
--rw-rw-rw-   0        0        0     6405 2020-12-27 08:43:58.000000 roboidai-1.1.8/roboidai/lab/_image.py
--rw-rw-rw-   0        0        0     6729 2020-12-27 08:44:40.000000 roboidai-1.1.8/roboidai/lab/_line_recorder.py
--rw-rw-rw-   0        0        0     8838 2020-12-27 08:45:18.000000 roboidai-1.1.8/roboidai/lab/_q_world.py
--rw-rw-rw-   0        0        0     5141 2020-12-27 08:45:54.000000 roboidai-1.1.8/roboidai/lab/_track.py
--rw-rw-rw-   0        0        0     1453 2020-12-25 13:05:51.000000 roboidai-1.1.8/roboidai/lab/_tree.py
--rw-rw-rw-   0        0        0     7341 2020-12-27 08:46:48.000000 roboidai-1.1.8/roboidai/lab/_zoo.py
-drwxrwxrwx   0        0        0        0 2020-12-27 08:52:04.820536 roboidai-1.1.8/roboidai/lab/ko/
--rw-rw-rw-   0        0        0     2966 2020-12-26 17:03:24.000000 roboidai-1.1.8/roboidai/lab/ko/__init__.py
-drwxrwxrwx   0        0        0        0 2020-12-27 08:52:04.698529 roboidai-1.1.8/roboidai.egg-info/
--rw-rw-rw-   0        0        0      649 2020-12-27 08:52:02.000000 roboidai-1.1.8/roboidai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      866 2020-12-27 08:52:02.000000 roboidai-1.1.8/roboidai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-12-27 08:52:02.000000 roboidai-1.1.8/roboidai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-12-27 08:52:02.000000 roboidai-1.1.8/roboidai.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       99 2020-12-27 08:52:02.000000 roboidai-1.1.8/roboidai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2020-12-27 08:52:02.000000 roboidai-1.1.8/roboidai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2020-12-27 08:52:04.826537 roboidai-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0      682 2020-12-27 07:17:41.000000 roboidai-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-02-04 22:23:17.189968 roboidai-1.1.9/
+-rw-rw-rw-   0        0        0      802 2020-08-22 18:46:05.000000 roboidai-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0      161 2021-02-04 22:15:50.000000 roboidai-1.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      649 2021-02-04 22:23:17.190968 roboidai-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2020-12-17 17:05:23.000000 roboidai-1.1.9/README.md
+-rw-rw-rw-   0        0        0      185 2021-02-04 22:14:16.000000 roboidai-1.1.9/requirements.txt
+drwxrwxrwx   0        0        0        0 2021-02-04 22:23:17.093962 roboidai-1.1.9/roboidai/
+-rw-rw-rw-   0        0        0     2139 2021-02-04 22:17:17.000000 roboidai-1.1.9/roboidai/__init__.py
+-rw-rw-rw-   0        0        0    15510 2020-12-27 08:36:55.000000 roboidai-1.1.9/roboidai/_camera.py
+drwxrwxrwx   0        0        0        0 2021-02-04 22:23:17.130964 roboidai-1.1.9/roboidai/_image/
+-rw-rw-rw-   0        0        0        0 2020-12-25 13:05:51.000000 roboidai-1.1.9/roboidai/_image/__init__.py
+-rw-rw-rw-   0        0        0     7799 2020-12-27 08:39:08.000000 roboidai-1.1.9/roboidai/_image/_age_gender.py
+-rw-rw-rw-   0        0        0     7548 2020-12-27 08:39:49.000000 roboidai-1.1.9/roboidai/_image/_face_detector.py
+-rw-rw-rw-   0        0        0     7215 2020-12-27 08:40:26.000000 roboidai-1.1.9/roboidai/_image/_face_marker.py
+-rw-rw-rw-   0        0        0    29139 2021-02-04 22:20:33.000000 roboidai-1.1.9/roboidai/_image/_face_mesh.py
+-rw-rw-rw-   0        0        0    12595 2021-02-04 22:21:12.000000 roboidai-1.1.9/roboidai/_image/_hand_pose.py
+-rw-rw-rw-   0        0        0    20191 2020-12-27 08:41:03.000000 roboidai-1.1.9/roboidai/_image/_object_detector.py
+-rw-rw-rw-   0        0        0     5794 2020-12-27 08:41:40.000000 roboidai-1.1.9/roboidai/_image/_tool.py
+-rw-rw-rw-   0        0        0     3970 2020-12-27 08:37:36.000000 roboidai-1.1.9/roboidai/_keyevent.py
+drwxrwxrwx   0        0        0        0 2021-02-04 22:23:17.132964 roboidai-1.1.9/roboidai/_model/
+-rw-rw-rw-   0        0        0      620 2020-12-25 13:05:51.000000 roboidai-1.1.9/roboidai/_model/object_labels.txt
+drwxrwxrwx   0        0        0        0 2021-02-04 22:23:17.140965 roboidai-1.1.9/roboidai/_tm/
+-rw-rw-rw-   0        0        0        0 2020-12-25 13:05:51.000000 roboidai-1.1.9/roboidai/_tm/__init__.py
+-rw-rw-rw-   0        0        0     5662 2020-12-27 08:42:30.000000 roboidai-1.1.9/roboidai/_tm/_image.py
+-rw-rw-rw-   0        0        0     4294 2020-12-27 08:38:18.000000 roboidai-1.1.9/roboidai/_window.py
+drwxrwxrwx   0        0        0        0 2021-02-04 22:23:17.183967 roboidai-1.1.9/roboidai/lab/
+-rw-rw-rw-   0        0        0     2894 2020-12-26 17:03:26.000000 roboidai-1.1.9/roboidai/lab/__init__.py
+-rw-rw-rw-   0        0        0     6405 2020-12-27 08:43:58.000000 roboidai-1.1.9/roboidai/lab/_image.py
+-rw-rw-rw-   0        0        0     6729 2020-12-27 08:44:40.000000 roboidai-1.1.9/roboidai/lab/_line_recorder.py
+-rw-rw-rw-   0        0        0     8838 2020-12-27 08:45:18.000000 roboidai-1.1.9/roboidai/lab/_q_world.py
+-rw-rw-rw-   0        0        0     5141 2020-12-27 08:45:54.000000 roboidai-1.1.9/roboidai/lab/_track.py
+-rw-rw-rw-   0        0        0     1453 2020-12-25 13:05:51.000000 roboidai-1.1.9/roboidai/lab/_tree.py
+-rw-rw-rw-   0        0        0     7341 2020-12-27 08:46:48.000000 roboidai-1.1.9/roboidai/lab/_zoo.py
+drwxrwxrwx   0        0        0        0 2021-02-04 22:23:17.187968 roboidai-1.1.9/roboidai/lab/ko/
+-rw-rw-rw-   0        0        0     2966 2020-12-26 17:03:24.000000 roboidai-1.1.9/roboidai/lab/ko/__init__.py
+drwxrwxrwx   0        0        0        0 2021-02-04 22:23:17.107963 roboidai-1.1.9/roboidai.egg-info/
+-rw-rw-rw-   0        0        0      649 2021-02-04 22:23:13.000000 roboidai-1.1.9/roboidai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2021-02-04 22:23:13.000000 roboidai-1.1.9/roboidai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-02-04 22:23:13.000000 roboidai-1.1.9/roboidai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-02-04 22:23:13.000000 roboidai-1.1.9/roboidai.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      101 2021-02-04 22:23:13.000000 roboidai-1.1.9/roboidai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2021-02-04 22:23:13.000000 roboidai-1.1.9/roboidai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2021-02-04 22:23:17.192968 roboidai-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      687 2021-02-04 22:14:14.000000 roboidai-1.1.9/setup.py
```

### Comparing `roboidai-1.1.8/LICENSE` & `roboidai-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `roboidai-1.1.8/PKG-INFO` & `roboidai-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboidai
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python Package for Roboid AI
 Home-page: UNKNOWN
 Author: Kwang-Hyun Park
 Author-email: akaii@kw.ac.kr
 License: UNKNOWN
 Description: # roboidai
```

### Comparing `roboidai-1.1.8/roboidai/__init__.py` & `roboidai-1.1.9/roboidai/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,21 +16,23 @@
 # Free Software Foundation, Inc., 59 Temple Place, Suite 330,
 # Boston, MA  02111-1307  USA
 
 from roboidai._camera import Camera
 from roboidai._window import Window
 from roboidai._keyevent import KeyEvent
 from roboidai._image._face_detector import FaceDetector
+from roboidai._image._face_mesh import FaceMesh
+from roboidai._image._hand_pose import HandPose
 from roboidai._image._age_gender import AgeGenderDetector
 from roboidai._image._object_detector import ObjectDetector
 from roboidai._image._face_marker import FaceMarkerDetector
 from roboidai._image._tool import ImageTool
 from roboidai._tm._image import TmImage
 
-__version__ = "1.1.8"
+__version__ = "1.1.9"
 
 def version():
     import roboid
     import numpy as np
     import tensorflow as tf
     import cv2
     print('-' * 20)
```

### Comparing `roboidai-1.1.8/roboidai/_camera.py` & `roboidai-1.1.9/roboidai/_camera.py`

 * *Files identical despite different names*

### Comparing `roboidai-1.1.8/roboidai/_image/_age_gender.py` & `roboidai-1.1.9/roboidai/_image/_age_gender.py`

 * *Files identical despite different names*

### Comparing `roboidai-1.1.8/roboidai/_image/_face_detector.py` & `roboidai-1.1.9/roboidai/_image/_face_detector.py`

 * *Files identical despite different names*

### Comparing `roboidai-1.1.8/roboidai/_image/_face_marker.py` & `roboidai-1.1.9/roboidai/_image/_face_marker.py`

 * *Files identical despite different names*

### Comparing `roboidai-1.1.8/roboidai/_image/_object_detector.py` & `roboidai-1.1.9/roboidai/_image/_object_detector.py`

 * *Files identical despite different names*

### Comparing `roboidai-1.1.8/roboidai/_image/_tool.py` & `roboidai-1.1.9/roboidai/_image/_tool.py`

 * *Files identical despite different names*

### Comparing `roboidai-1.1.8/roboidai/_keyevent.py` & `roboidai-1.1.9/roboidai/_keyevent.py`

 * *Files identical despite different names*

### Comparing `roboidai-1.1.8/roboidai/_model/object_labels.txt` & `roboidai-1.1.9/roboidai/_model/object_labels.txt`

 * *Files identical despite different names*

### Comparing `roboidai-1.1.8/roboidai/_tm/_image.py` & `roboidai-1.1.9/roboidai/_tm/_image.py`

 * *Files identical despite different names*

### Comparing `roboidai-1.1.8/roboidai/_window.py` & `roboidai-1.1.9/roboidai/_window.py`

 * *Files identical despite different names*

### Comparing `roboidai-1.1.8/roboidai/lab/__init__.py` & `roboidai-1.1.9/roboidai/lab/__init__.py`

 * *Files identical despite different names*

### Comparing `roboidai-1.1.8/roboidai/lab/_image.py` & `roboidai-1.1.9/roboidai/lab/_image.py`

 * *Files identical despite different names*

### Comparing `roboidai-1.1.8/roboidai/lab/_line_recorder.py` & `roboidai-1.1.9/roboidai/lab/_line_recorder.py`

 * *Files identical despite different names*

### Comparing `roboidai-1.1.8/roboidai/lab/_q_world.py` & `roboidai-1.1.9/roboidai/lab/_q_world.py`

 * *Files identical despite different names*

### Comparing `roboidai-1.1.8/roboidai/lab/_track.py` & `roboidai-1.1.9/roboidai/lab/_track.py`

 * *Files identical despite different names*

### Comparing `roboidai-1.1.8/roboidai/lab/_tree.py` & `roboidai-1.1.9/roboidai/lab/_tree.py`

 * *Files identical despite different names*

### Comparing `roboidai-1.1.8/roboidai/lab/_zoo.py` & `roboidai-1.1.9/roboidai/lab/_zoo.py`

 * *Files identical despite different names*

### Comparing `roboidai-1.1.8/roboidai/lab/ko/__init__.py` & `roboidai-1.1.9/roboidai/lab/ko/__init__.py`

 * *Files identical despite different names*

### Comparing `roboidai-1.1.8/roboidai.egg-info/PKG-INFO` & `roboidai-1.1.9/roboidai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboidai
-Version: 1.1.8
+Version: 1.1.9
 Summary: Python Package for Roboid AI
 Home-page: UNKNOWN
 Author: Kwang-Hyun Park
 Author-email: akaii@kw.ac.kr
 License: UNKNOWN
 Description: # roboidai
```

### Comparing `roboidai-1.1.8/roboidai.egg-info/SOURCES.txt` & `roboidai-1.1.9/roboidai.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 roboidai.egg-info/not-zip-safe
 roboidai.egg-info/requires.txt
 roboidai.egg-info/top_level.txt
 roboidai/_image/__init__.py
 roboidai/_image/_age_gender.py
 roboidai/_image/_face_detector.py
 roboidai/_image/_face_marker.py
+roboidai/_image/_face_mesh.py
+roboidai/_image/_hand_pose.py
 roboidai/_image/_object_detector.py
 roboidai/_image/_tool.py
-roboidai/_model/face.caffemodel
-roboidai/_model/face.prototxt
 roboidai/_model/object_labels.txt
 roboidai/_tm/__init__.py
 roboidai/_tm/_image.py
 roboidai/lab/__init__.py
 roboidai/lab/_image.py
 roboidai/lab/_line_recorder.py
 roboidai/lab/_q_world.py
```

### Comparing `roboidai-1.1.8/setup.py` & `roboidai-1.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="roboidai",
-	version="1.1.8",
+	version="1.1.9",
 	author="Kwang-Hyun Park",
 	author_email="akaii@kw.ac.kr",
 	description="Python Package for Roboid AI",
 	long_description=open("README.md").read(),
 	long_description_content_type="text/markdown",
-	install_requires=["roboid", "ifaddr", "pyttsx3", "pynput", "pandas", "matplotlib", "scikit-learn", "numpy", "opencv-contrib-python", "tensorflow"],
+	install_requires=["roboid", "ifaddr", "pyttsx3", "pynput", "pandas", "matplotlib", "scikit-learn", "numpy", "mediapipe", "opencv-python", "tensorflow"],
 	packages=find_packages(exclude=["examples", "tests"]),
 	python_requires=">=3",
 	include_package_data=True,
 	zip_safe=False,
 	classifiers=[
 		"License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)"
 	]
```

