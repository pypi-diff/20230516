# Comparing `tmp/kolyaklimkLab3-0.4.0.tar.gz` & `tmp/kolyaklimkLab3-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolyaklimkLab3-0.4.0.tar", last modified: Tue May 16 07:51:25 2023, max compression
+gzip compressed data, was "kolyaklimkLab3-0.6.0.tar", last modified: Tue May 16 07:59:05 2023, max compression
```

## Comparing `kolyaklimkLab3-0.4.0.tar` & `kolyaklimkLab3-0.6.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 07:51:25.092361 kolyaklimkLab3-0.4.0/
-drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 07:51:25.092361 kolyaklimkLab3-0.4.0/Lab3/
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)       56 2023-05-16 07:50:54.000000 kolyaklimkLab3-0.4.0/Lab3/__init__.py
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      582 2023-05-16 07:51:25.092361 kolyaklimkLab3-0.4.0/PKG-INFO
-drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 07:51:25.092361 kolyaklimkLab3-0.4.0/kolyaklimkLab3.egg-info/
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      582 2023-05-16 07:51:25.000000 kolyaklimkLab3-0.4.0/kolyaklimkLab3.egg-info/PKG-INFO
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      214 2023-05-16 07:51:25.000000 kolyaklimkLab3-0.4.0/kolyaklimkLab3.egg-info/SOURCES.txt
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)        1 2023-05-16 07:51:25.000000 kolyaklimkLab3-0.4.0/kolyaklimkLab3.egg-info/dependency_links.txt
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)        6 2023-05-16 07:51:25.000000 kolyaklimkLab3-0.4.0/kolyaklimkLab3.egg-info/requires.txt
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)        5 2023-05-16 07:51:25.000000 kolyaklimkLab3-0.4.0/kolyaklimkLab3.egg-info/top_level.txt
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)       38 2023-05-16 07:51:25.092361 kolyaklimkLab3-0.4.0/setup.cfg
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      893 2023-05-16 07:51:14.000000 kolyaklimkLab3-0.4.0/setup.py
+drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 07:59:05.396243 kolyaklimkLab3-0.6.0/
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      582 2023-05-16 07:59:05.396243 kolyaklimkLab3-0.6.0/PKG-INFO
+drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 07:59:05.396243 kolyaklimkLab3-0.6.0/kolyaklimkLab3/
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)       76 2023-05-16 07:57:06.000000 kolyaklimkLab3-0.6.0/kolyaklimkLab3/__init__.py
+drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 07:59:05.396243 kolyaklimkLab3-0.6.0/kolyaklimkLab3.egg-info/
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      582 2023-05-16 07:59:05.000000 kolyaklimkLab3-0.6.0/kolyaklimkLab3.egg-info/PKG-INFO
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      224 2023-05-16 07:59:05.000000 kolyaklimkLab3-0.6.0/kolyaklimkLab3.egg-info/SOURCES.txt
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)        1 2023-05-16 07:59:05.000000 kolyaklimkLab3-0.6.0/kolyaklimkLab3.egg-info/dependency_links.txt
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)        6 2023-05-16 07:59:05.000000 kolyaklimkLab3-0.6.0/kolyaklimkLab3.egg-info/requires.txt
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)       15 2023-05-16 07:59:05.000000 kolyaklimkLab3-0.6.0/kolyaklimkLab3.egg-info/top_level.txt
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)       38 2023-05-16 07:59:05.396243 kolyaklimkLab3-0.6.0/setup.cfg
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      913 2023-05-16 07:57:06.000000 kolyaklimkLab3-0.6.0/setup.py
```

### Comparing `kolyaklimkLab3-0.4.0/PKG-INFO` & `kolyaklimkLab3-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolyaklimkLab3
-Version: 0.4.0
+Version: 0.6.0
 Summary: # Serializerib
 Author: kolyaklimk
 Author-email: kolyaklimk@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `kolyaklimkLab3-0.4.0/kolyaklimkLab3.egg-info/PKG-INFO` & `kolyaklimkLab3-0.6.0/kolyaklimkLab3.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolyaklimkLab3
-Version: 0.4.0
+Version: 0.6.0
 Summary: # Serializerib
 Author: kolyaklimk
 Author-email: kolyaklimk@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `kolyaklimkLab3-0.4.0/setup.py` & `kolyaklimkLab3-0.6.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 
 # To use a consistent encoding
 from codecs import open
 from os import path
 
-import Lab3
+import kolyaklimkLab3
 
 setup(
     name="kolyaklimkLab3",
-    version="0.4.0",
+    version="0.6.0",
     description=open('README.MD').read(),
     author="kolyaklimk",
     author_email="kolyaklimk@gmail.com",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
@@ -21,11 +21,11 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ],
-    packages=["Lab3"],
+    packages=["kolyaklimkLab3"],
     include_package_data=True,
     install_requires=["regex"]
 )
```

