# Comparing `tmp/pymca-5.8.1-py2.py3-none-any.whl.zip` & `tmp/pymca-5.8.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5534 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat     5827 b- defN 23-Jan-25 16:17 pymca-5.8.1.data/scripts/pymca_launcher
--rw-rw-rw-  2.0 fat       31 b- defN 16-Dec-03 05:23 pymca-5.8.1.data/scripts/pymca_launcher.bat
--rw-rw-rw-  2.0 fat     1817 b- defN 23-Jan-25 16:17 pymca-5.8.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1855 b- defN 23-Jan-25 16:17 pymca-5.8.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jan-25 16:17 pymca-5.8.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jan-25 16:17 pymca-5.8.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      570 b- defN 23-Jan-25 16:17 pymca-5.8.1.dist-info/RECORD
-7 files, 10211 bytes uncompressed, 4518 bytes compressed:  55.8%
+Zip file size: 5501 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat     5930 b- defN 23-May-16 09:41 pymca-5.8.2.data/scripts/pymca_launcher
+-rw-rw-rw-  2.0 fat       31 b- defN 23-May-16 09:38 pymca-5.8.2.data/scripts/pymca_launcher.bat
+-rw-rw-rw-  2.0 fat     1817 b- defN 23-May-16 09:41 pymca-5.8.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1775 b- defN 23-May-16 09:41 pymca-5.8.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-May-16 09:41 pymca-5.8.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-May-16 09:41 pymca-5.8.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      570 b- defN 23-May-16 09:41 pymca-5.8.2.dist-info/RECORD
+7 files, 10239 bytes uncompressed, 4485 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: pymca-5.8.1.data/scripts/pymca_launcher
+Filename: pymca-5.8.2.data/scripts/pymca_launcher
 Comment: 
 
-Filename: pymca-5.8.1.data/scripts/pymca_launcher.bat
+Filename: pymca-5.8.2.data/scripts/pymca_launcher.bat
 Comment: 
 
-Filename: pymca-5.8.1.dist-info/LICENSE
+Filename: pymca-5.8.2.dist-info/LICENSE
 Comment: 
 
-Filename: pymca-5.8.1.dist-info/METADATA
+Filename: pymca-5.8.2.dist-info/METADATA
 Comment: 
 
-Filename: pymca-5.8.1.dist-info/WHEEL
+Filename: pymca-5.8.2.dist-info/WHEEL
 Comment: 
 
-Filename: pymca-5.8.1.dist-info/top_level.txt
+Filename: pymca-5.8.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pymca-5.8.1.dist-info/RECORD
+Filename: pymca-5.8.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pymca-5.8.1.dist-info/LICENSE` & `pymca-5.8.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pymca-5.8.1.dist-info/METADATA` & `pymca-5.8.2.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 Metadata-Version: 2.1
 Name: pymca
-Version: 5.8.1
+Version: 5.8.2
 Summary: pymca
-Home-page: UNKNOWN
 Author: V.A. Sole - ESRF
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -23,18 +20,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
-Requires-Dist: PyMca5 (>=5.8.1)
+Requires-Dist: PyMca5 (>=5.8.2)
 Requires-Dist: h5py
 Requires-Dist: numpy
-Requires-Dist: PyOpenGL
 Requires-Dist: matplotlib
 
 pymca
 =====
 
 At this point this module just makes sure that pip install pymca install current PyMca5 version. It is more natural for the user to type pip install pymca than pip install PyMca5.
 
@@ -60,9 +56,7 @@
 
 
 License
 -------
 
 This code is licensed under the MIT license.
 
-
-
```

