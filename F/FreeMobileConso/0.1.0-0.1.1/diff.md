# Comparing `tmp/FreeMobileConso-0.1.0.tar.gz` & `tmp/FreeMobileConso-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeMobileConso-0.1.0.tar", last modified: Sun May 14 12:38:01 2023, max compression
+gzip compressed data, was "FreeMobileConso-0.1.1.tar", last modified: Tue May 16 17:16:37 2023, max compression
```

## Comparing `FreeMobileConso-0.1.0.tar` & `FreeMobileConso-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-14 12:38:01.417204 FreeMobileConso-0.1.0/
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-14 12:38:01.416085 FreeMobileConso-0.1.0/FreeMobileConso/
--rw-r--r--   0 corentin   (501) staff       (20)     1396 2023-05-14 12:37:13.000000 FreeMobileConso-0.1.0/FreeMobileConso/__init__.py
--rw-r--r--   0 corentin   (501) staff       (20)     6173 2023-05-14 12:36:03.000000 FreeMobileConso-0.1.0/FreeMobileConso/client.py
--rw-r--r--   0 corentin   (501) staff       (20)     2033 2023-05-14 12:15:38.000000 FreeMobileConso-0.1.0/FreeMobileConso/dataClassification.py
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-14 12:38:01.416850 FreeMobileConso-0.1.0/FreeMobileConso.egg-info/
--rw-r--r--   0 corentin   (501) staff       (20)     6059 2023-05-14 12:38:01.000000 FreeMobileConso-0.1.0/FreeMobileConso.egg-info/PKG-INFO
--rw-r--r--   0 corentin   (501) staff       (20)      312 2023-05-14 12:38:01.000000 FreeMobileConso-0.1.0/FreeMobileConso.egg-info/SOURCES.txt
--rw-r--r--   0 corentin   (501) staff       (20)        1 2023-05-14 12:38:01.000000 FreeMobileConso-0.1.0/FreeMobileConso.egg-info/dependency_links.txt
--rw-r--r--   0 corentin   (501) staff       (20)       13 2023-05-14 12:38:01.000000 FreeMobileConso-0.1.0/FreeMobileConso.egg-info/requires.txt
--rw-r--r--   0 corentin   (501) staff       (20)       16 2023-05-14 12:38:01.000000 FreeMobileConso-0.1.0/FreeMobileConso.egg-info/top_level.txt
--rwxrwxrwx   0 corentin   (501) staff       (20)     1068 2022-08-01 16:04:58.000000 FreeMobileConso-0.1.0/LICENSE
--rw-r--r--   0 corentin   (501) staff       (20)     6059 2023-05-14 12:38:01.417033 FreeMobileConso-0.1.0/PKG-INFO
--rwxrwxrwx   0 corentin   (501) staff       (20)     5574 2023-05-08 18:53:17.000000 FreeMobileConso-0.1.0/README.md
--rw-r--r--   0 corentin   (501) staff       (20)       38 2023-05-14 12:38:01.417253 FreeMobileConso-0.1.0/setup.cfg
--rw-r--r--   0 corentin   (501) staff       (20)      864 2023-05-14 12:37:01.000000 FreeMobileConso-0.1.0/setup.py
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-16 17:16:37.510061 FreeMobileConso-0.1.1/
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-16 17:16:37.508925 FreeMobileConso-0.1.1/FreeMobileConso/
+-rw-r--r--   0 corentin   (501) staff       (20)     1396 2023-05-16 17:15:54.000000 FreeMobileConso-0.1.1/FreeMobileConso/__init__.py
+-rw-r--r--   0 corentin   (501) staff       (20)     6173 2023-05-14 12:36:03.000000 FreeMobileConso-0.1.1/FreeMobileConso/client.py
+-rw-r--r--   0 corentin   (501) staff       (20)     2033 2023-05-14 12:15:38.000000 FreeMobileConso-0.1.1/FreeMobileConso/dataClassification.py
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-05-16 17:16:37.509780 FreeMobileConso-0.1.1/FreeMobileConso.egg-info/
+-rw-r--r--   0 corentin   (501) staff       (20)     6054 2023-05-16 17:16:37.000000 FreeMobileConso-0.1.1/FreeMobileConso.egg-info/PKG-INFO
+-rw-r--r--   0 corentin   (501) staff       (20)      312 2023-05-16 17:16:37.000000 FreeMobileConso-0.1.1/FreeMobileConso.egg-info/SOURCES.txt
+-rw-r--r--   0 corentin   (501) staff       (20)        1 2023-05-16 17:16:37.000000 FreeMobileConso-0.1.1/FreeMobileConso.egg-info/dependency_links.txt
+-rw-r--r--   0 corentin   (501) staff       (20)       13 2023-05-16 17:16:37.000000 FreeMobileConso-0.1.1/FreeMobileConso.egg-info/requires.txt
+-rw-r--r--   0 corentin   (501) staff       (20)       16 2023-05-16 17:16:37.000000 FreeMobileConso-0.1.1/FreeMobileConso.egg-info/top_level.txt
+-rwxrwxrwx   0 corentin   (501) staff       (20)     1068 2022-08-01 16:04:58.000000 FreeMobileConso-0.1.1/LICENSE
+-rw-r--r--   0 corentin   (501) staff       (20)     6054 2023-05-16 17:16:37.509935 FreeMobileConso-0.1.1/PKG-INFO
+-rwxrwxrwx   0 corentin   (501) staff       (20)     5569 2023-05-16 17:15:01.000000 FreeMobileConso-0.1.1/README.md
+-rw-r--r--   0 corentin   (501) staff       (20)       38 2023-05-16 17:16:37.510096 FreeMobileConso-0.1.1/setup.cfg
+-rw-r--r--   0 corentin   (501) staff       (20)      864 2023-05-16 17:15:49.000000 FreeMobileConso-0.1.1/setup.py
```

### Comparing `FreeMobileConso-0.1.0/FreeMobileConso/__init__.py` & `FreeMobileConso-0.1.1/FreeMobileConso/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,12 +20,12 @@
 """
 
 
 __title__ = "FreeMobileConso"
 __author__ = "CorentinMre"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) CorentinMre"
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 
 from .dataClassification import *
 from .client import *
```

### Comparing `FreeMobileConso-0.1.0/FreeMobileConso/client.py` & `FreeMobileConso-0.1.1/FreeMobileConso/client.py`

 * *Files identical despite different names*

### Comparing `FreeMobileConso-0.1.0/FreeMobileConso/dataClassification.py` & `FreeMobileConso-0.1.1/FreeMobileConso/dataClassification.py`

 * *Files identical despite different names*

### Comparing `FreeMobileConso-0.1.0/FreeMobileConso.egg-info/PKG-INFO` & `FreeMobileConso-0.1.1/FreeMobileConso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeMobileConso
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python API for get your consommation of your Free mobile account
 Home-page: https://github.com/CorentinMre/FreeMobileConso
 Author: CorentinMre
 Author-email: corentin.marie@isen-ouest.yncrea.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,26 +14,26 @@
 
 <br>
 <p align="center"><img width="400" alt="Logo" src="https://raw.githubusercontent.com/CorentinMre/FreeMobileConso/main/images/logoV2.png"></a></p>
 
 <br/>
 
 
-<h2 style="font-family: sans-serif; font-weight: normal;" align="center">An API for get<strong> Free mobile </strong>Consommation</h2>
+<h2 style="font-family: sans-serif; font-weight: normal;" align="center">A API for get<strong> Free mobile </strong>Consumption</h2>
 
 
 <br/>
 
 
 [![pypi version](https://img.shields.io/pypi/v/FreeMobileConso.svg)](https://pypi.org/project/FreeMobileConso/)
 [![python version](https://img.shields.io/pypi/pyversions/FreeMobileConso.svg)](https://pypi.org/project/FreeMobileConso/)
 [![license](https://img.shields.io/pypi/l/FreeMobileConso.svg)](https://pypi.org/project/FreeMobileConso/)
 
 ## Description
-A python API for get your consommation of your Free mobile account
+A python API to get the consumption of your Free mobile account
 
 
 ## Dependencies
 
 - requests
 - bs4
```

### Comparing `FreeMobileConso-0.1.0/LICENSE` & `FreeMobileConso-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FreeMobileConso-0.1.0/PKG-INFO` & `FreeMobileConso-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeMobileConso
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python API for get your consommation of your Free mobile account
 Home-page: https://github.com/CorentinMre/FreeMobileConso
 Author: CorentinMre
 Author-email: corentin.marie@isen-ouest.yncrea.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,26 +14,26 @@
 
 <br>
 <p align="center"><img width="400" alt="Logo" src="https://raw.githubusercontent.com/CorentinMre/FreeMobileConso/main/images/logoV2.png"></a></p>
 
 <br/>
 
 
-<h2 style="font-family: sans-serif; font-weight: normal;" align="center">An API for get<strong> Free mobile </strong>Consommation</h2>
+<h2 style="font-family: sans-serif; font-weight: normal;" align="center">A API for get<strong> Free mobile </strong>Consumption</h2>
 
 
 <br/>
 
 
 [![pypi version](https://img.shields.io/pypi/v/FreeMobileConso.svg)](https://pypi.org/project/FreeMobileConso/)
 [![python version](https://img.shields.io/pypi/pyversions/FreeMobileConso.svg)](https://pypi.org/project/FreeMobileConso/)
 [![license](https://img.shields.io/pypi/l/FreeMobileConso.svg)](https://pypi.org/project/FreeMobileConso/)
 
 ## Description
-A python API for get your consommation of your Free mobile account
+A python API to get the consumption of your Free mobile account
 
 
 ## Dependencies
 
 - requests
 - bs4
```

### Comparing `FreeMobileConso-0.1.0/README.md` & `FreeMobileConso-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 <br>
 <p align="center"><img width="400" alt="Logo" src="https://raw.githubusercontent.com/CorentinMre/FreeMobileConso/main/images/logoV2.png"></a></p>
 
 <br/>
 
 
-<h2 style="font-family: sans-serif; font-weight: normal;" align="center">An API for get<strong> Free mobile </strong>Consommation</h2>
+<h2 style="font-family: sans-serif; font-weight: normal;" align="center">A API for get<strong> Free mobile </strong>Consumption</h2>
 
 
 <br/>
 
 
 [![pypi version](https://img.shields.io/pypi/v/FreeMobileConso.svg)](https://pypi.org/project/FreeMobileConso/)
 [![python version](https://img.shields.io/pypi/pyversions/FreeMobileConso.svg)](https://pypi.org/project/FreeMobileConso/)
 [![license](https://img.shields.io/pypi/l/FreeMobileConso.svg)](https://pypi.org/project/FreeMobileConso/)
 
 ## Description
-A python API for get your consommation of your Free mobile account
+A python API to get the consumption of your Free mobile account
 
 
 ## Dependencies
 
 - requests
 - bs4
```

### Comparing `FreeMobileConso-0.1.0/setup.py` & `FreeMobileConso-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='FreeMobileConso',
-    version='0.1.0',    
+    version='0.1.1',    
     description='A python API for get your consommation of your Free mobile account',
     long_description_content_type = "text/markdown",
     long_description=long_description,
     url='https://github.com/CorentinMre/FreeMobileConso',
     author='CorentinMre',
     author_email='corentin.marie@isen-ouest.yncrea.fr',
     license='MIT',
```

