# Comparing `tmp/PyTraffic-1.0.6.tar.gz` & `tmp/PyTraffic-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTraffic-1.0.6.tar", last modified: Sat May 13 11:15:48 2023, max compression
+gzip compressed data, was "PyTraffic-1.0.7.tar", last modified: Tue May 16 07:14:48 2023, max compression
```

## Comparing `PyTraffic-1.0.6.tar` & `PyTraffic-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 11:15:48.765765 PyTraffic-1.0.6/
--rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PyTraffic-1.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0      126 2023-05-13 07:33:47.000000 PyTraffic-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     3994 2023-05-13 11:15:48.764769 PyTraffic-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-13 11:15:48.738838 PyTraffic-1.0.6/PyTraffic/
--rw-rw-rw-   0        0        0      800 2023-05-13 11:13:39.000000 PyTraffic-1.0.6/PyTraffic/Density.py
--rw-rw-rw-   0        0        0     4126 2023-05-13 11:14:06.000000 PyTraffic-1.0.6/PyTraffic/LicensePlate.py
--rw-rw-rw-   0        0        0       59 2023-05-13 05:58:41.000000 PyTraffic-1.0.6/PyTraffic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 11:15:48.760781 PyTraffic-1.0.6/PyTraffic/models/
--rw-rw-rw-   0        0        0   118802 2023-03-06 15:47:42.000000 PyTraffic-1.0.6/PyTraffic/models/cars.xml
--rw-rw-rw-   0        0        0    78136 2023-05-13 06:54:47.000000 PyTraffic-1.0.6/PyTraffic/models/license_plate_opencv.xml
-drwxrwxrwx   0        0        0        0 2023-05-13 11:15:48.752800 PyTraffic-1.0.6/PyTraffic.egg-info/
--rw-rw-rw-   0        0        0     3994 2023-05-13 11:15:48.000000 PyTraffic-1.0.6/PyTraffic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-05-13 11:15:48.000000 PyTraffic-1.0.6/PyTraffic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 11:15:48.000000 PyTraffic-1.0.6/PyTraffic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-05-13 11:15:48.000000 PyTraffic-1.0.6/PyTraffic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-13 11:15:48.000000 PyTraffic-1.0.6/PyTraffic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3438 2023-05-13 11:14:49.000000 PyTraffic-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-13 11:15:48.765765 PyTraffic-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1050 2023-05-13 11:14:45.000000 PyTraffic-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:14:48.964353 PyTraffic-1.0.7/
+-rw-rw-rw-   0        0        0     1091 2023-05-10 06:48:15.000000 PyTraffic-1.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      149 2023-05-16 06:43:09.000000 PyTraffic-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4701 2023-05-16 07:14:48.963352 PyTraffic-1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-16 07:14:48.933432 PyTraffic-1.0.7/PyTraffic/
+-rw-rw-rw-   0        0        0     3645 2023-05-16 06:40:04.000000 PyTraffic-1.0.7/PyTraffic/LicensePlate.py
+-rw-rw-rw-   0        0        0     3150 2023-05-14 06:05:25.000000 PyTraffic-1.0.7/PyTraffic/VehicleDetection.py
+-rw-rw-rw-   0        0        0       59 2023-05-13 05:58:41.000000 PyTraffic-1.0.7/PyTraffic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:14:48.958366 PyTraffic-1.0.7/PyTraffic/models/
+-rw-rw-rw-   0        0        0   118802 2023-03-06 15:47:42.000000 PyTraffic-1.0.7/PyTraffic/models/haarcascade_car.xml
+-rw-rw-rw-   0        0        0    78136 2023-05-13 06:54:47.000000 PyTraffic-1.0.7/PyTraffic/models/haarcascade_russian_plate_number.xml
+drwxrwxrwx   0        0        0        0 2023-05-16 07:14:48.949406 PyTraffic-1.0.7/PyTraffic.egg-info/
+-rw-rw-rw-   0        0        0     4701 2023-05-16 07:14:47.000000 PyTraffic-1.0.7/PyTraffic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2023-05-16 07:14:47.000000 PyTraffic-1.0.7/PyTraffic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 07:14:47.000000 PyTraffic-1.0.7/PyTraffic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-16 07:14:47.000000 PyTraffic-1.0.7/PyTraffic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-16 07:14:47.000000 PyTraffic-1.0.7/PyTraffic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4127 2023-05-14 05:43:08.000000 PyTraffic-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 07:14:48.965346 PyTraffic-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1063 2023-05-16 06:40:35.000000 PyTraffic-1.0.7/setup.py
```

### Comparing `PyTraffic-1.0.6/LICENSE.txt` & `PyTraffic-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyTraffic-1.0.6/PKG-INFO` & `PyTraffic-1.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: PyTraffic
-Version: 1.0.6
+Version: 1.0.7
 Summary: PyTraffic is a Python module to work on traffic-related functions and use cases.
 Home-page: https://github.com/Anikethc/PyTraffic
 Download-URL: https://pypi.org/project/PyTraffic
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
-Keywords: Traffic,Traffic Density,License Plates,Speed,Speed Calculation
+Keywords: Traffic,Traffic Density,License Plates,Vehicles,Vehicle Detection
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # PyTraffic
 
 ## Introduction
 
 PyTraffic is a Python module to work on traffic-related functions and use cases.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pytraffic-docs).
 
 ## Module Information
 
 **Name** - PyTraffic</br>
-**Version** - 1.0.6</br>
+**Version** - 1.0.7</br>
 **Description** - PyTraffic is a Python module to work on traffic-related functions and use cases.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyTraffic](https://github.com/Anikethc/PyTraffic)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyTraffic](https://pypi.org/project/PyTraffic)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pytraffic-docs](https://aniketh-chavare.gitbook.io/pytraffic-docs)
 
 ## License
@@ -63,34 +63,49 @@
 **Link:** Visit [here](https://www.tutorialspoint.com/how-to-detect-license-plates-using-opencv-python).<br>
 
 **Project:** Tutorial (Web Page)<br>
 **Used For:** LicensePlate (Sub-Module)<br>
 **Author:** Denis Kuria<br>
 **Link:** Visit [here](https://www.makeuseof.com/python-car-license-plates-detect-and-recognize).<br>
 
+**Project:** Tutorial (Web Page)<br>
+**Used For:** VehicleDetection (Sub-Module)<br>
+**Author:** Aman Preet Gulati<br>
+**Link:** Visit [here](https://www.analyticsvidhya.com/blog/2021/12/vehicle-detection-and-counting-system-using-opencv).<br>
+
+**Project:** Tutorial (Web Page)<br>
+**Used For:** VehicleDetection (Sub-Module)<br>
+**Author:** Vidhu Chaudhary<br>
+**Link:** Visit [here](https://www.codingninjas.com/codestudio/library/vehicle-detection-using-opencv).<br>
+
 **Project:** Python Module (opencv-python)<br>
-**Used For:** LicensePlate and Density (Sub-Modules)<br>
+**Used For:** LicensePlate and VehicleDetection (Sub-Modules)<br>
 **Author:** OpenCV<br>
 **Link:** Visit [here](https://github.com/opencv/opencv-python).<br>
 
 **Project:** Python Module (imutils)<br>
 **Used For:** LicensePlate (Sub-Module)<br>
 **Author:** PyImageSearch<br>
 **Link:** Visit [here](https://github.com/PyImageSearch/imutils).<br>
 
 **Project:** Python Module (Numpy)<br>
-**Used For:** LicensePlate (Sub-Module)<br>
+**Used For:** LicensePlate and VehicleDetection (Sub-Module)<br>
 **Author:** Numpy.org<br>
 **Link:** Visit [here](https://github.com/numpy/numpy).<br>
 
 **Project:** Python Module (PyTesseract)<br>
 **Used For:** LicensePlate (Sub-Module)<br>
 **Author:** madmaze<br>
 **Link:** Visit [here](https://github.com/madmaze/pytesseract).<br>
 
+**Project:** Python Module (Pillow)<br>
+**Used For:** VehicleDetection (Sub-Module)<br>
+**Author:** Python-Pillow<br>
+**Link:** Visit [here](https://github.com/python-pillow/Pillow).<br>
+
 ## Issues & Bugs
 
 If you encounter any issues or bugs, visit the 'Issues' tab and create an issue. I'll look into it and resolve it ASAP.
 
 ## Conclusion
 
 I hope you liked this module. Thank you!
```

### Comparing `PyTraffic-1.0.6/PyTraffic/LicensePlate.py` & `PyTraffic-1.0.7/PyTraffic/LicensePlate.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,109 +3,100 @@
 # Imports
 import os
 import cv2
 import imutils
 import numpy as np
 import pytesseract
 
-# Variables
-OpenCV = "OpenCV"
-Tesseract = "Tesseract"
-
-# Function 1 - Check Tesseract
-def checkTesseract():
-    programs = []
-
-    for item in winapps.list_installed():
-        programs.append(item.name)
-
-    return "Tesseract-OCR - open source OCR engine" in programs
-
-# Function 2 - Check License Plate
-def checkLicensePlate(method, imagePath, tesseractPath="None"):
+# Function 1 - Show License Plate
+def showLicensePlate(imagePath):
     # Set Directory
     directory = os.path.dirname(os.path.realpath(__file__))
     directory = directory.replace(os.sep, "/")
 
+    # Check if Path Exists
+    if (os.path.exists(imagePath)):
+        # Reading the Image
+        img = cv2.imread(imagePath)
+
+        # Converting the Images to Grayscale
+        gray = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
+        cascade = cv2.CascadeClassifier(directory + "/models/haarcascade_russian_plate_number.xml")
+
+        # Finding the Plates
+        plates = cascade.detectMultiScale(gray, 1.2, 5)
+        print('Number of Detected License Plates:', len(plates))
+
+        # Displaying Each License Plate
+        for (x,y,w,h) in plates:
+            cv2.rectangle(img, (x,y), (x+w, y+h), (0,255,0), 2)
+            gray_plates = gray[y:y+h, x:x+w]
+            color_plates = img[y:y+h, x:x+w]
+
+            cv2.imshow('Vehicle Image', img)
+            cv2.imshow('Number Plate', gray_plates)
+            cv2.waitKey(0)
+    else:
+        raise Exception("The image file path does not exist.")
+
+# Function 2 - Get License Plate Number
+def getLicensePlateNumber(imagePath, tesseractPath):
+    # Check if Path Exists
     if (os.path.exists(imagePath)):
-        if (method == "OpenCV"): # OpenCV
+        # Check for Tesseract
+        if (os.path.exists(tesseractPath)):
+            # Connecting to Tesseract
+            pytesseract.pytesseract.tesseract_cmd = tesseractPath
+
             # Reading the Image
-            img = cv2.imread(imagePath)
+            img = cv2.imread(imagePath, cv2.IMREAD_COLOR)
+            img = cv2.resize(img, (600,400))
 
-            # Converting the Images to Grayscale
-            gray = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-            cascade = cv2.CascadeClassifier(directory + "/models/license_plate_opencv.xml")
-
-            # Finding the Plates
-            plates = cascade.detectMultiScale(gray, 1.2, 5)
-            print('Number of Detected License Plates:', len(plates))
-
-            # Displaying Each License Plate
-            for (x,y,w,h) in plates:
-                cv2.rectangle(img, (x,y), (x+w, y+h), (0,255,0), 2)
-                gray_plates = gray[y:y+h, x:x+w]
-                color_plates = img[y:y+h, x:x+w]
-
-                cv2.imshow('Number Plate', gray_plates)
-                cv2.imshow('Number Plate Image', img)
-                cv2.waitKey(0)
-        elif (method == "Tesseract"): # Tesseract
-            # Check for Tesseract
-            if (os.path.exists(tesseractPath)):
-                # Connecting to Tesseract
-                pytesseract.pytesseract.tesseract_cmd = tesseractPath
-
-                # Reading the Image
-                img = cv2.imread(imagePath, cv2.IMREAD_COLOR)
-                img = cv2.resize(img, (600,400))
-
-                # Converting the Images to Grayscale
-                gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY) 
-                gray = cv2.bilateralFilter(gray, 13, 15, 15) 
-
-                # Finding Contours
-                edged = cv2.Canny(gray, 30, 200) 
-                contours = cv2.findContours(edged.copy(), cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)
-                contours = imutils.grab_contours(contours)
-                contours = sorted(contours, key = cv2.contourArea, reverse = True)[:10]
-                screenCnt = None
-
-                for c in contours:
-                    peri = cv2.arcLength(c, True)
-                    approx = cv2.approxPolyDP(c, 0.018 * peri, True)
-
-                    if len(approx) == 4:
-                        screenCnt = approx
-                        break
-
-                if screenCnt is None:
-                    detected = 0
-                else:
-                    detected = 1
-
-                if detected == 1:
-                    cv2.drawContours(img, [screenCnt], -1, (0, 0, 255), 3)
-
-                mask = np.zeros(gray.shape,np.uint8)
-                new_image = cv2.drawContours(mask,[screenCnt],0,255,-1,)
-                new_image = cv2.bitwise_and(img,img,mask=mask)
-
-                (x, y) = np.where(mask == 255)
-                (topx, topy) = (np.min(x), np.min(y))
-                (bottomx, bottomy) = (np.max(x), np.max(y))
-                Cropped = gray[topx:bottomx+1, topy:bottomy+1]
-
-                # License Plate Number
-                text = pytesseract.image_to_string(Cropped, config='--psm 11')
-
-                # Close OpenCV
-                cv2.waitKey(0)
-                cv2.destroyAllWindows()
+            # Converting the Image to Grayscale
+            gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY) 
+            gray = cv2.bilateralFilter(gray, 13, 15, 15) 
+
+            # Finding & Counting Contours
+            edged = cv2.Canny(gray, 30, 200) 
+            contours = cv2.findContours(edged.copy(), cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)
+            contours = imutils.grab_contours(contours)
+            contours = sorted(contours, key = cv2.contourArea, reverse = True)[:10]
+            screenCnt = None
+
+            for c in contours:
+                peri = cv2.arcLength(c, True)
+                approx = cv2.approxPolyDP(c, 0.018 * peri, True)
+
+                if len(approx) == 4:
+                    screenCnt = approx
+                    break
 
-                # Return the License Plate Number
-                return text
+            if screenCnt is None:
+                detected = 0
             else:
-                raise Exception("The 'tesseract.exe' file path does not exist. Make sure Tesseract-OCR is installed and the path given is correct.")
+                detected = 1
+
+            if detected == 1:
+                cv2.drawContours(img, [screenCnt], -1, (0, 0, 255), 3)
+
+            mask = np.zeros(gray.shape,np.uint8)
+            new_image = cv2.drawContours(mask,[screenCnt],0,255,-1,)
+            new_image = cv2.bitwise_and(img,img,mask=mask)
+
+            (x, y) = np.where(mask == 255)
+            (topx, topy) = (np.min(x), np.min(y))
+            (bottomx, bottomy) = (np.max(x), np.max(y))
+            Cropped = gray[topx:bottomx+1, topy:bottomy+1]
+
+            # License Plate Number
+            text = pytesseract.image_to_string(Cropped, config='--psm 11')
+
+            # Close OpenCV
+            cv2.waitKey(0)
+            cv2.destroyAllWindows()
+
+            # Return the License Plate Number
+            return text
         else:
-            raise Exception("Please use a valid method for identifying the license plate numbers.")
+            raise Exception("The 'tesseract.exe' file path does not exist. Make sure Tesseract-OCR is installed and the path given exists.")
     else:
-        raise Exception("The file path does not exist.")
+        raise Exception("The image file path does not exist.")
```

### Comparing `PyTraffic-1.0.6/PyTraffic/models/cars.xml` & `PyTraffic-1.0.7/PyTraffic/models/haarcascade_car.xml`

 * *Files identical despite different names*

### Comparing `PyTraffic-1.0.6/PyTraffic/models/license_plate_opencv.xml` & `PyTraffic-1.0.7/PyTraffic/models/haarcascade_russian_plate_number.xml`

 * *Files identical despite different names*

### Comparing `PyTraffic-1.0.6/PyTraffic.egg-info/PKG-INFO` & `PyTraffic-1.0.7/PyTraffic.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: PyTraffic
-Version: 1.0.6
+Version: 1.0.7
 Summary: PyTraffic is a Python module to work on traffic-related functions and use cases.
 Home-page: https://github.com/Anikethc/PyTraffic
 Download-URL: https://pypi.org/project/PyTraffic
 Author: Aniketh Chavare
 Author-email: anikethchavare@outlook.com
 License: MIT
-Keywords: Traffic,Traffic Density,License Plates,Speed,Speed Calculation
+Keywords: Traffic,Traffic Density,License Plates,Vehicles,Vehicle Detection
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # PyTraffic
 
 ## Introduction
 
 PyTraffic is a Python module to work on traffic-related functions and use cases.
 
 Read the docs on GitBook [here](https://aniketh-chavare.gitbook.io/pytraffic-docs).
 
 ## Module Information
 
 **Name** - PyTraffic</br>
-**Version** - 1.0.6</br>
+**Version** - 1.0.7</br>
 **Description** - PyTraffic is a Python module to work on traffic-related functions and use cases.</br>
 **Author** - Aniketh Chavare</br>
 **GitHub URL** - [https://github.com/Anikethc/PyTraffic](https://github.com/Anikethc/PyTraffic)</br>
 **Pypi.org URL** - [https://pypi.org/project/PyTraffic](https://pypi.org/project/PyTraffic)</br>
 **Docs URL** - [https://aniketh-chavare.gitbook.io/pytraffic-docs](https://aniketh-chavare.gitbook.io/pytraffic-docs)
 
 ## License
@@ -63,34 +63,49 @@
 **Link:** Visit [here](https://www.tutorialspoint.com/how-to-detect-license-plates-using-opencv-python).<br>
 
 **Project:** Tutorial (Web Page)<br>
 **Used For:** LicensePlate (Sub-Module)<br>
 **Author:** Denis Kuria<br>
 **Link:** Visit [here](https://www.makeuseof.com/python-car-license-plates-detect-and-recognize).<br>
 
+**Project:** Tutorial (Web Page)<br>
+**Used For:** VehicleDetection (Sub-Module)<br>
+**Author:** Aman Preet Gulati<br>
+**Link:** Visit [here](https://www.analyticsvidhya.com/blog/2021/12/vehicle-detection-and-counting-system-using-opencv).<br>
+
+**Project:** Tutorial (Web Page)<br>
+**Used For:** VehicleDetection (Sub-Module)<br>
+**Author:** Vidhu Chaudhary<br>
+**Link:** Visit [here](https://www.codingninjas.com/codestudio/library/vehicle-detection-using-opencv).<br>
+
 **Project:** Python Module (opencv-python)<br>
-**Used For:** LicensePlate and Density (Sub-Modules)<br>
+**Used For:** LicensePlate and VehicleDetection (Sub-Modules)<br>
 **Author:** OpenCV<br>
 **Link:** Visit [here](https://github.com/opencv/opencv-python).<br>
 
 **Project:** Python Module (imutils)<br>
 **Used For:** LicensePlate (Sub-Module)<br>
 **Author:** PyImageSearch<br>
 **Link:** Visit [here](https://github.com/PyImageSearch/imutils).<br>
 
 **Project:** Python Module (Numpy)<br>
-**Used For:** LicensePlate (Sub-Module)<br>
+**Used For:** LicensePlate and VehicleDetection (Sub-Module)<br>
 **Author:** Numpy.org<br>
 **Link:** Visit [here](https://github.com/numpy/numpy).<br>
 
 **Project:** Python Module (PyTesseract)<br>
 **Used For:** LicensePlate (Sub-Module)<br>
 **Author:** madmaze<br>
 **Link:** Visit [here](https://github.com/madmaze/pytesseract).<br>
 
+**Project:** Python Module (Pillow)<br>
+**Used For:** VehicleDetection (Sub-Module)<br>
+**Author:** Python-Pillow<br>
+**Link:** Visit [here](https://github.com/python-pillow/Pillow).<br>
+
 ## Issues & Bugs
 
 If you encounter any issues or bugs, visit the 'Issues' tab and create an issue. I'll look into it and resolve it ASAP.
 
 ## Conclusion
 
 I hope you liked this module. Thank you!
```

### Comparing `PyTraffic-1.0.6/setup.py` & `PyTraffic-1.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 # README.md
 with open("README.md") as readme_file:
     README = readme_file.read()
 
 # Setup Arguements
 setup_args = dict (
     name="PyTraffic",
-    version="1.0.6",
+    version="1.0.7",
     description="PyTraffic is a Python module to work on traffic-related functions and use cases.",
     long_description_content_type="text/markdown",
     long_description=README,
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     author="Aniketh Chavare",
     author_email="anikethchavare@outlook.com",
-    keywords=["Traffic", "Traffic Density", "License Plates", "Speed", "Speed Calculation"],
+    keywords=["Traffic", "Traffic Density", "License Plates", "Vehicles", "Vehicle Detection"],
     url="https://github.com/Anikethc/PyTraffic",
     download_url="https://pypi.org/project/PyTraffic"
 )
 
 # Install Requires
-install_requires = ["opencv-python", "imutils", "numpy", "pytesseract"]
+install_requires = ["opencv-python", "imutils", "numpy", "pytesseract", "pillow"]
 
 # Run the Setup File
 if __name__ == "__main__":
     setup(**setup_args, install_requires=install_requires)
```

