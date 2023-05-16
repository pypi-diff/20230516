# Comparing `tmp/e2enetworks-0.0.4.tar.gz` & `tmp/e2enetworks-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2enetworks-0.0.4.tar", last modified: Mon May 15 07:42:20 2023, max compression
+gzip compressed data, was "e2enetworks-0.0.5.tar", last modified: Mon May 15 12:39:36 2023, max compression
```

## Comparing `e2enetworks-0.0.4.tar` & `e2enetworks-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,25 @@
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:42:20.290674 e2enetworks-0.0.4/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)    10786 2023-05-15 06:38:48.000000 e2enetworks-0.0.4/LICENSE.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-15 07:42:20.290742 e2enetworks-0.0.4/PKG-INFO
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     4748 2023-05-15 07:01:23.000000 e2enetworks-0.0.4/README.rst
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:42:20.289860 e2enetworks-0.0.4/e2enetworks/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:31:42.000000 e2enetworks-0.0.4/e2enetworks/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:42:20.290427 e2enetworks-0.0.4/e2enetworks/cloud/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:31:42.000000 e2enetworks-0.0.4/e2enetworks/cloud/__init__.py
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      147 2023-05-15 07:31:42.000000 e2enetworks-0.0.4/e2enetworks/cloud/test.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:42:20.290258 e2enetworks-0.0.4/e2enetworks.egg-info/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-15 07:42:20.000000 e2enetworks-0.0.4/e2enetworks.egg-info/PKG-INFO
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      261 2023-05-15 07:42:20.000000 e2enetworks-0.0.4/e2enetworks.egg-info/SOURCES.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        1 2023-05-15 07:42:20.000000 e2enetworks-0.0.4/e2enetworks.egg-info/dependency_links.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)       12 2023-05-15 07:42:20.000000 e2enetworks-0.0.4/e2enetworks.egg-info/top_level.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)       67 2023-05-15 07:42:20.290945 e2enetworks-0.0.4/setup.cfg
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1833 2023-05-15 07:38:52.000000 e2enetworks-0.0.4/setup.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 12:39:36.255056 e2enetworks-0.0.5/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)    10786 2023-05-15 06:38:48.000000 e2enetworks-0.0.5/LICENSE.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-15 12:39:36.255121 e2enetworks-0.0.5/PKG-INFO
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     4748 2023-05-15 07:01:23.000000 e2enetworks-0.0.5/README.rst
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 12:39:36.252917 e2enetworks-0.0.5/e2enetworks/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:31:42.000000 e2enetworks-0.0.5/e2enetworks/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 12:39:36.253605 e2enetworks-0.0.5/e2enetworks/cloud/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:31:42.000000 e2enetworks-0.0.5/e2enetworks/cloud/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 12:39:36.254154 e2enetworks-0.0.5/e2enetworks/cloud/aiplatform/
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 12:39:36.254460 e2enetworks-0.0.5/e2enetworks/cloud/aiplatform/Dataset/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      404 2023-05-15 12:30:25.000000 e2enetworks-0.0.5/e2enetworks/cloud/aiplatform/Dataset/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 12:39:36.254675 e2enetworks-0.0.5/e2enetworks/cloud/aiplatform/EndPoint/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      497 2023-05-15 12:30:25.000000 e2enetworks-0.0.5/e2enetworks/cloud/aiplatform/EndPoint/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 12:39:36.254859 e2enetworks-0.0.5/e2enetworks/cloud/aiplatform/Model/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      492 2023-05-15 12:30:25.000000 e2enetworks-0.0.5/e2enetworks/cloud/aiplatform/Model/__init__.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      169 2023-05-15 11:02:21.000000 e2enetworks-0.0.5/e2enetworks/cloud/aiplatform/__init__.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      382 2023-05-15 11:27:01.000000 e2enetworks-0.0.5/e2enetworks/cloud/aiplatform/init.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      147 2023-05-15 07:31:42.000000 e2enetworks-0.0.5/e2enetworks/cloud/test.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 12:39:36.253421 e2enetworks-0.0.5/e2enetworks.egg-info/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-15 12:39:35.000000 e2enetworks-0.0.5/e2enetworks.egg-info/PKG-INFO
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      485 2023-05-15 12:39:36.000000 e2enetworks-0.0.5/e2enetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        1 2023-05-15 12:39:36.000000 e2enetworks-0.0.5/e2enetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)       12 2023-05-15 12:39:36.000000 e2enetworks-0.0.5/e2enetworks.egg-info/top_level.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)       67 2023-05-15 12:39:36.255332 e2enetworks-0.0.5/setup.cfg
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1833 2023-05-15 12:39:27.000000 e2enetworks-0.0.5/setup.py
```

### Comparing `e2enetworks-0.0.4/LICENSE.txt` & `e2enetworks-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `e2enetworks-0.0.4/PKG-INFO` & `e2enetworks-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 0.0.4
+Version: 0.0.5
 Summary: E2E Networks Plugins
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
```

### Comparing `e2enetworks-0.0.4/README.rst` & `e2enetworks-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `e2enetworks-0.0.4/e2enetworks.egg-info/PKG-INFO` & `e2enetworks-0.0.5/e2enetworks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 0.0.4
+Version: 0.0.5
 Summary: E2E Networks Plugins
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
```

### Comparing `e2enetworks-0.0.4/setup.py` & `e2enetworks-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 from os import path
 
-version = "0.0.4"
+version = "0.0.5"
 install_requires = [
 
 ]
 # read the contents of your README file
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.rst")) as f:
```

