# Comparing `tmp/kolyaklimkLab3-0.2.0.tar.gz` & `tmp/kolyaklimkLab3-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolyaklimkLab3-0.2.0.tar", last modified: Tue May 16 07:46:13 2023, max compression
+gzip compressed data, was "kolyaklimkLab3-0.4.0.tar", last modified: Tue May 16 07:51:25 2023, max compression
```

## Comparing `kolyaklimkLab3-0.2.0.tar` & `kolyaklimkLab3-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,12 @@
-drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 07:46:13.536316 kolyaklimkLab3-0.2.0/
-drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 07:46:13.536316 kolyaklimkLab3-0.2.0/Lab3/
-drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 07:46:13.536316 kolyaklimkLab3-0.2.0/Lab3/MyParser/
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)     1510 2023-05-15 22:04:44.000000 kolyaklimkLab3-0.2.0/Lab3/MyParser/Constants.py
-drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 07:46:13.536316 kolyaklimkLab3-0.2.0/Lab3/MyParser/JsonParser/
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      682 2023-05-15 21:19:59.000000 kolyaklimkLab3-0.2.0/Lab3/MyParser/JsonParser/Constants.py
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)     2762 2023-05-16 06:42:22.000000 kolyaklimkLab3-0.2.0/Lab3/MyParser/JsonParser/Json.py
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      182 2023-05-16 06:47:12.000000 kolyaklimkLab3-0.2.0/Lab3/MyParser/JsonParser/__init__.py
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)     7359 2023-05-16 06:42:22.000000 kolyaklimkLab3-0.2.0/Lab3/MyParser/Parser.py
-drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 07:46:13.536316 kolyaklimkLab3-0.2.0/Lab3/MyParser/XmlParser/
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      857 2023-05-15 21:40:36.000000 kolyaklimkLab3-0.2.0/Lab3/MyParser/XmlParser/Constants.py
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)     3044 2023-05-16 06:44:51.000000 kolyaklimkLab3-0.2.0/Lab3/MyParser/XmlParser/Xml.py
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      152 2023-05-16 06:44:51.000000 kolyaklimkLab3-0.2.0/Lab3/MyParser/XmlParser/__init__.py
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      379 2023-05-16 06:45:27.000000 kolyaklimkLab3-0.2.0/Lab3/MyParser/__init__.py
-drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 07:46:13.536316 kolyaklimkLab3-0.2.0/Lab3/MySerializer/
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      446 2023-05-16 06:47:40.000000 kolyaklimkLab3-0.2.0/Lab3/MySerializer/Factory.py
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      418 2023-05-15 21:35:45.000000 kolyaklimkLab3-0.2.0/Lab3/MySerializer/Serializer.py
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      114 2023-05-16 06:44:06.000000 kolyaklimkLab3-0.2.0/Lab3/MySerializer/__init__.py
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 07:00:46.000000 kolyaklimkLab3-0.2.0/Lab3/__init__.py
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      582 2023-05-16 07:46:13.536316 kolyaklimkLab3-0.2.0/PKG-INFO
-drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 07:46:13.536316 kolyaklimkLab3-0.2.0/kolyaklimkLab3.egg-info/
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      582 2023-05-16 07:46:13.000000 kolyaklimkLab3-0.2.0/kolyaklimkLab3.egg-info/PKG-INFO
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      594 2023-05-16 07:46:13.000000 kolyaklimkLab3-0.2.0/kolyaklimkLab3.egg-info/SOURCES.txt
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)        1 2023-05-16 07:46:13.000000 kolyaklimkLab3-0.2.0/kolyaklimkLab3.egg-info/dependency_links.txt
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)        6 2023-05-16 07:46:13.000000 kolyaklimkLab3-0.2.0/kolyaklimkLab3.egg-info/requires.txt
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)        5 2023-05-16 07:46:13.000000 kolyaklimkLab3-0.2.0/kolyaklimkLab3.egg-info/top_level.txt
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)       38 2023-05-16 07:46:13.536316 kolyaklimkLab3-0.2.0/setup.cfg
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      900 2023-05-16 07:46:10.000000 kolyaklimkLab3-0.2.0/setup.py
+drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 07:51:25.092361 kolyaklimkLab3-0.4.0/
+drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 07:51:25.092361 kolyaklimkLab3-0.4.0/Lab3/
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)       56 2023-05-16 07:50:54.000000 kolyaklimkLab3-0.4.0/Lab3/__init__.py
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      582 2023-05-16 07:51:25.092361 kolyaklimkLab3-0.4.0/PKG-INFO
+drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 07:51:25.092361 kolyaklimkLab3-0.4.0/kolyaklimkLab3.egg-info/
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      582 2023-05-16 07:51:25.000000 kolyaklimkLab3-0.4.0/kolyaklimkLab3.egg-info/PKG-INFO
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      214 2023-05-16 07:51:25.000000 kolyaklimkLab3-0.4.0/kolyaklimkLab3.egg-info/SOURCES.txt
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)        1 2023-05-16 07:51:25.000000 kolyaklimkLab3-0.4.0/kolyaklimkLab3.egg-info/dependency_links.txt
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)        6 2023-05-16 07:51:25.000000 kolyaklimkLab3-0.4.0/kolyaklimkLab3.egg-info/requires.txt
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)        5 2023-05-16 07:51:25.000000 kolyaklimkLab3-0.4.0/kolyaklimkLab3.egg-info/top_level.txt
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)       38 2023-05-16 07:51:25.092361 kolyaklimkLab3-0.4.0/setup.cfg
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      893 2023-05-16 07:51:14.000000 kolyaklimkLab3-0.4.0/setup.py
```

### Comparing `kolyaklimkLab3-0.2.0/PKG-INFO` & `kolyaklimkLab3-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolyaklimkLab3
-Version: 0.2.0
+Version: 0.4.0
 Summary: # Serializerib
 Author: kolyaklimk
 Author-email: kolyaklimk@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `kolyaklimkLab3-0.2.0/kolyaklimkLab3.egg-info/PKG-INFO` & `kolyaklimkLab3-0.4.0/kolyaklimkLab3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolyaklimkLab3
-Version: 0.2.0
+Version: 0.4.0
 Summary: # Serializerib
 Author: kolyaklimk
 Author-email: kolyaklimk@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `kolyaklimkLab3-0.2.0/setup.py` & `kolyaklimkLab3-0.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from codecs import open
 from os import path
 
 import Lab3
 
 setup(
     name="kolyaklimkLab3",
-    version="0.2.0",
+    version="0.4.0",
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
-    packages=find_packages(),
+    packages=["Lab3"],
     include_package_data=True,
     install_requires=["regex"]
 )
```

