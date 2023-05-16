# Comparing `tmp/e2enetworks-0.0.5.tar.gz` & `tmp/e2enetworks-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2enetworks-0.0.5.tar", last modified: Mon May 15 12:39:36 2023, max compression
+gzip compressed data, was "e2enetworks-0.0.7.tar", last modified: Tue May 16 06:57:43 2023, max compression
```

## Comparing `e2enetworks-0.0.5.tar` & `e2enetworks-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 12:39:36.255056 e2enetworks-0.0.5/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)    10786 2023-05-15 06:38:48.000000 e2enetworks-0.0.5/LICENSE.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-15 12:39:36.255121 e2enetworks-0.0.5/PKG-INFO
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     4748 2023-05-15 07:01:23.000000 e2enetworks-0.0.5/README.rst
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 12:39:36.252917 e2enetworks-0.0.5/e2enetworks/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:31:42.000000 e2enetworks-0.0.5/e2enetworks/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 12:39:36.253605 e2enetworks-0.0.5/e2enetworks/cloud/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:31:42.000000 e2enetworks-0.0.5/e2enetworks/cloud/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 12:39:36.254154 e2enetworks-0.0.5/e2enetworks/cloud/aiplatform/
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 12:39:36.254460 e2enetworks-0.0.5/e2enetworks/cloud/aiplatform/Dataset/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      404 2023-05-15 12:30:25.000000 e2enetworks-0.0.5/e2enetworks/cloud/aiplatform/Dataset/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 12:39:36.254675 e2enetworks-0.0.5/e2enetworks/cloud/aiplatform/EndPoint/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      497 2023-05-15 12:30:25.000000 e2enetworks-0.0.5/e2enetworks/cloud/aiplatform/EndPoint/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 12:39:36.254859 e2enetworks-0.0.5/e2enetworks/cloud/aiplatform/Model/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      492 2023-05-15 12:30:25.000000 e2enetworks-0.0.5/e2enetworks/cloud/aiplatform/Model/__init__.py
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      169 2023-05-15 11:02:21.000000 e2enetworks-0.0.5/e2enetworks/cloud/aiplatform/__init__.py
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      382 2023-05-15 11:27:01.000000 e2enetworks-0.0.5/e2enetworks/cloud/aiplatform/init.py
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      147 2023-05-15 07:31:42.000000 e2enetworks-0.0.5/e2enetworks/cloud/test.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 12:39:36.253421 e2enetworks-0.0.5/e2enetworks.egg-info/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-15 12:39:35.000000 e2enetworks-0.0.5/e2enetworks.egg-info/PKG-INFO
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      485 2023-05-15 12:39:36.000000 e2enetworks-0.0.5/e2enetworks.egg-info/SOURCES.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        1 2023-05-15 12:39:36.000000 e2enetworks-0.0.5/e2enetworks.egg-info/dependency_links.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)       12 2023-05-15 12:39:36.000000 e2enetworks-0.0.5/e2enetworks.egg-info/top_level.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)       67 2023-05-15 12:39:36.255332 e2enetworks-0.0.5/setup.cfg
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1833 2023-05-15 12:39:27.000000 e2enetworks-0.0.5/setup.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 06:57:43.358964 e2enetworks-0.0.7/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)    10786 2023-05-15 06:38:48.000000 e2enetworks-0.0.7/LICENSE.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-16 06:57:43.359040 e2enetworks-0.0.7/PKG-INFO
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     4748 2023-05-15 07:01:23.000000 e2enetworks-0.0.7/README.rst
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 06:57:43.356580 e2enetworks-0.0.7/e2enetworks/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:31:42.000000 e2enetworks-0.0.7/e2enetworks/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 06:57:43.357395 e2enetworks-0.0.7/e2enetworks/cloud/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:31:42.000000 e2enetworks-0.0.7/e2enetworks/cloud/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 06:57:43.357978 e2enetworks-0.0.7/e2enetworks/cloud/aiplatform/
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 06:57:43.358322 e2enetworks-0.0.7/e2enetworks/cloud/aiplatform/Dataset/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      840 2023-05-16 06:50:34.000000 e2enetworks-0.0.7/e2enetworks/cloud/aiplatform/Dataset/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 06:57:43.358543 e2enetworks-0.0.7/e2enetworks/cloud/aiplatform/EndPoint/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      290 2023-05-16 06:13:24.000000 e2enetworks-0.0.7/e2enetworks/cloud/aiplatform/EndPoint/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 06:57:43.358777 e2enetworks-0.0.7/e2enetworks/cloud/aiplatform/Model/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      388 2023-05-16 06:13:24.000000 e2enetworks-0.0.7/e2enetworks/cloud/aiplatform/Model/__init__.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      220 2023-05-16 06:52:59.000000 e2enetworks-0.0.7/e2enetworks/cloud/aiplatform/__init__.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      275 2023-05-16 06:15:26.000000 e2enetworks-0.0.7/e2enetworks/cloud/aiplatform/init.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      147 2023-05-15 07:31:42.000000 e2enetworks-0.0.7/e2enetworks/cloud/test.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      142 2023-05-16 06:50:03.000000 e2enetworks-0.0.7/e2enetworks/constants.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 06:57:43.357191 e2enetworks-0.0.7/e2enetworks.egg-info/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-16 06:57:43.000000 e2enetworks-0.0.7/e2enetworks.egg-info/PKG-INFO
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      510 2023-05-16 06:57:43.000000 e2enetworks-0.0.7/e2enetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        1 2023-05-16 06:57:43.000000 e2enetworks-0.0.7/e2enetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)       12 2023-05-16 06:57:43.000000 e2enetworks-0.0.7/e2enetworks.egg-info/top_level.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)       67 2023-05-16 06:57:43.359248 e2enetworks-0.0.7/setup.cfg
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1833 2023-05-16 06:57:12.000000 e2enetworks-0.0.7/setup.py
```

### Comparing `e2enetworks-0.0.5/LICENSE.txt` & `e2enetworks-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `e2enetworks-0.0.5/PKG-INFO` & `e2enetworks-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 0.0.5
+Version: 0.0.7
 Summary: E2E Networks Plugins
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
```

### Comparing `e2enetworks-0.0.5/README.rst` & `e2enetworks-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `e2enetworks-0.0.5/e2enetworks.egg-info/PKG-INFO` & `e2enetworks-0.0.7/e2enetworks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 0.0.5
+Version: 0.0.7
 Summary: E2E Networks Plugins
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
```

### Comparing `e2enetworks-0.0.5/setup.py` & `e2enetworks-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 from os import path
 
-version = "0.0.5"
+version = "0.0.7"
 install_requires = [
 
 ]
 # read the contents of your README file
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.rst")) as f:
```

