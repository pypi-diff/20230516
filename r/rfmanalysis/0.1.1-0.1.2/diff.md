# Comparing `tmp/rfmanalysis-0.1.1.tar.gz` & `tmp/rfmanalysis-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfmanalysis-0.1.1.tar", last modified: Tue May 16 19:32:42 2023, max compression
+gzip compressed data, was "rfmanalysis-0.1.2.tar", last modified: Tue May 16 21:06:47 2023, max compression
```

## Comparing `rfmanalysis-0.1.1.tar` & `rfmanalysis-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 19:32:41.999552 rfmanalysis-0.1.1/
--rw-rw-rw-   0        0        0      184 2023-05-16 18:36:44.000000 rfmanalysis-0.1.1/AUTHORS.rst
--rw-rw-rw-   0        0        0     3690 2023-05-16 18:36:44.000000 rfmanalysis-0.1.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-05-16 18:36:44.000000 rfmanalysis-0.1.1/HISTORY.rst
--rw-rw-rw-   0        0        0     1098 2023-05-16 18:36:44.000000 rfmanalysis-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      273 2023-05-16 18:36:44.000000 rfmanalysis-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5269 2023-05-16 19:32:41.999552 rfmanalysis-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4105 2023-05-16 18:42:22.000000 rfmanalysis-0.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-16 19:32:41.953712 rfmanalysis-0.1.1/docs/
--rw-rw-rw-   0        0        0      632 2023-05-16 18:36:44.000000 rfmanalysis-0.1.1/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-05-16 18:36:44.000000 rfmanalysis-0.1.1/docs/authors.rst
--rw-rw-rw-   0        0        0     5019 2023-05-16 18:36:44.000000 rfmanalysis-0.1.1/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-05-16 18:36:44.000000 rfmanalysis-0.1.1/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-05-16 18:36:44.000000 rfmanalysis-0.1.1/docs/history.rst
--rw-rw-rw-   0        0        0      331 2023-05-16 18:36:44.000000 rfmanalysis-0.1.1/docs/index.rst
--rw-rw-rw-   0        0        0     1206 2023-05-16 18:36:44.000000 rfmanalysis-0.1.1/docs/installation.rst
--rwxrwxrwx   0        0        0      809 2023-05-16 18:36:44.000000 rfmanalysis-0.1.1/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-05-16 18:36:44.000000 rfmanalysis-0.1.1/docs/readme.rst
--rw-rw-rw-   0        0        0       87 2023-05-16 18:36:44.000000 rfmanalysis-0.1.1/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-05-16 19:32:41.957548 rfmanalysis-0.1.1/rfmanalysis/
--rw-rw-rw-   0        0        0      216 2023-05-16 19:14:34.000000 rfmanalysis-0.1.1/rfmanalysis/__init__.py
--rw-rw-rw-   0        0        0    10559 2023-05-16 16:19:14.000000 rfmanalysis-0.1.1/rfmanalysis/rfmanalysis.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:32:41.993909 rfmanalysis-0.1.1/rfmanalysis.egg-info/
--rw-rw-rw-   0        0        0     5269 2023-05-16 19:32:41.000000 rfmanalysis-0.1.1/rfmanalysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      524 2023-05-16 19:32:41.000000 rfmanalysis-0.1.1/rfmanalysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 19:32:41.000000 rfmanalysis-0.1.1/rfmanalysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-16 18:47:20.000000 rfmanalysis-0.1.1/rfmanalysis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-05-16 19:32:41.000000 rfmanalysis-0.1.1/rfmanalysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      454 2023-05-16 19:32:42.002210 rfmanalysis-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1658 2023-05-16 19:22:14.000000 rfmanalysis-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:32:41.998554 rfmanalysis-0.1.1/tests/
--rw-rw-rw-   0        0        0       42 2023-05-16 18:36:44.000000 rfmanalysis-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0      589 2023-05-16 18:36:44.000000 rfmanalysis-0.1.1/tests/test_rfmanalysis.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:06:47.007715 rfmanalysis-0.1.2/
+-rw-rw-rw-   0        0        0      184 2023-05-16 18:36:44.000000 rfmanalysis-0.1.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3690 2023-05-16 18:36:44.000000 rfmanalysis-0.1.2/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-05-16 18:36:44.000000 rfmanalysis-0.1.2/HISTORY.rst
+-rw-rw-rw-   0        0        0     1098 2023-05-16 18:36:44.000000 rfmanalysis-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-05-16 18:36:44.000000 rfmanalysis-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5269 2023-05-16 21:06:47.008076 rfmanalysis-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4105 2023-05-16 18:42:22.000000 rfmanalysis-0.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-16 21:06:46.930116 rfmanalysis-0.1.2/docs/
+-rw-rw-rw-   0        0        0      632 2023-05-16 18:36:44.000000 rfmanalysis-0.1.2/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-05-16 18:36:44.000000 rfmanalysis-0.1.2/docs/authors.rst
+-rw-rw-rw-   0        0        0     5019 2023-05-16 18:36:44.000000 rfmanalysis-0.1.2/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-05-16 18:36:44.000000 rfmanalysis-0.1.2/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-05-16 18:36:44.000000 rfmanalysis-0.1.2/docs/history.rst
+-rw-rw-rw-   0        0        0      331 2023-05-16 18:36:44.000000 rfmanalysis-0.1.2/docs/index.rst
+-rw-rw-rw-   0        0        0     1206 2023-05-16 18:36:44.000000 rfmanalysis-0.1.2/docs/installation.rst
+-rwxrwxrwx   0        0        0      809 2023-05-16 18:36:44.000000 rfmanalysis-0.1.2/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-05-16 18:36:44.000000 rfmanalysis-0.1.2/docs/readme.rst
+-rw-rw-rw-   0        0        0       87 2023-05-16 18:36:44.000000 rfmanalysis-0.1.2/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-05-16 21:06:46.937091 rfmanalysis-0.1.2/rfmanalysis/
+-rw-rw-rw-   0        0        0      201 2023-05-16 21:05:29.000000 rfmanalysis-0.1.2/rfmanalysis/__init__.py
+-rw-rw-rw-   0        0        0    10559 2023-05-16 16:19:14.000000 rfmanalysis-0.1.2/rfmanalysis/rfmanalysis.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:06:46.997707 rfmanalysis-0.1.2/rfmanalysis.egg-info/
+-rw-rw-rw-   0        0        0     5269 2023-05-16 21:06:46.000000 rfmanalysis-0.1.2/rfmanalysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      524 2023-05-16 21:06:46.000000 rfmanalysis-0.1.2/rfmanalysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 21:06:46.000000 rfmanalysis-0.1.2/rfmanalysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-16 18:47:20.000000 rfmanalysis-0.1.2/rfmanalysis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-05-16 21:06:46.000000 rfmanalysis-0.1.2/rfmanalysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      454 2023-05-16 21:06:47.021585 rfmanalysis-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1658 2023-05-16 21:05:38.000000 rfmanalysis-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 21:06:47.002432 rfmanalysis-0.1.2/tests/
+-rw-rw-rw-   0        0        0       42 2023-05-16 18:36:44.000000 rfmanalysis-0.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      589 2023-05-16 18:36:44.000000 rfmanalysis-0.1.2/tests/test_rfmanalysis.py
```

### Comparing `rfmanalysis-0.1.1/CONTRIBUTING.rst` & `rfmanalysis-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.1/LICENSE` & `rfmanalysis-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.1/PKG-INFO` & `rfmanalysis-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfmanalysis
-Version: 0.1.1
+Version: 0.1.2
 Summary: This repository contains a Python implementation of RFM (Recency, Frequency, Monetary) analysis, a customer segmentation technique used in marketing and customer relationship management. The RFM analysis helps identify customer segments based on their purchasing behavior, allowing businesses to tailor their marketing strategies and customer retention efforts.
 Home-page: https://github.com/emmayann/rfmanalysis
 Author: Emma Hovhannisyan
 Author-email: emmahovhannisyan02@gmail.com
 License: MIT license
 Keywords: rfmanalysis
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `rfmanalysis-0.1.1/README.rst` & `rfmanalysis-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.1/docs/Makefile` & `rfmanalysis-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.1/docs/conf.py` & `rfmanalysis-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.1/docs/installation.rst` & `rfmanalysis-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.1/docs/make.bat` & `rfmanalysis-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.1/rfmanalysis/rfmanalysis.py` & `rfmanalysis-0.1.2/rfmanalysis/rfmanalysis.py`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.1/rfmanalysis.egg-info/PKG-INFO` & `rfmanalysis-0.1.2/rfmanalysis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfmanalysis
-Version: 0.1.1
+Version: 0.1.2
 Summary: This repository contains a Python implementation of RFM (Recency, Frequency, Monetary) analysis, a customer segmentation technique used in marketing and customer relationship management. The RFM analysis helps identify customer segments based on their purchasing behavior, allowing businesses to tailor their marketing strategies and customer retention efforts.
 Home-page: https://github.com/emmayann/rfmanalysis
 Author: Emma Hovhannisyan
 Author-email: emmahovhannisyan02@gmail.com
 License: MIT license
 Keywords: rfmanalysis
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `rfmanalysis-0.1.1/rfmanalysis.egg-info/SOURCES.txt` & `rfmanalysis-0.1.2/rfmanalysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rfmanalysis-0.1.1/setup.py` & `rfmanalysis-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,10 +35,10 @@
     include_package_data=True,
     keywords='rfmanalysis',
     name='rfmanalysis',
     packages=find_packages(include=['rfmanalysis', 'rfmanalysis.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/emmayann/rfmanalysis',
-    version='0.1.1',
+    version='0.1.2',
     zip_safe=False,
 )
```

### Comparing `rfmanalysis-0.1.1/tests/test_rfmanalysis.py` & `rfmanalysis-0.1.2/tests/test_rfmanalysis.py`

 * *Files identical despite different names*

