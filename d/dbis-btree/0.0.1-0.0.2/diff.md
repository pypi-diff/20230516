# Comparing `tmp/dbis-btree-0.0.1.tar.gz` & `tmp/dbis-btree-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbis-btree-0.0.1.tar", last modified: Mon May 30 15:21:35 2022, max compression
+gzip compressed data, was "dbis-btree-0.0.2.tar", last modified: Mon May 30 16:45:46 2022, max compression
```

## Comparing `dbis-btree-0.0.1.tar` & `dbis-btree-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 philipph  (1000) philipph  (1000)        0 2022-05-30 15:21:35.160859 dbis-btree-0.0.1/
--rw-r--r--   0 philipph  (1000) philipph  (1000)       63 2022-05-30 15:14:51.000000 dbis-btree-0.0.1/MANIFEST.in
--rw-r--r--   0 philipph  (1000) philipph  (1000)     1433 2022-05-30 15:21:35.160859 dbis-btree-0.0.1/PKG-INFO
--rw-r--r--   0 philipph  (1000) philipph  (1000)      943 2022-05-30 15:14:51.000000 dbis-btree-0.0.1/README.md
-drwxr-xr-x   0 philipph  (1000) philipph  (1000)        0 2022-05-30 15:21:35.160859 dbis-btree-0.0.1/dbis_btree/
--rwxr-xr-x   0 philipph  (1000) philipph  (1000)    10126 2022-05-30 15:14:51.000000 dbis-btree-0.0.1/dbis_btree/BBaum.py
--rwxr-xr-x   0 philipph  (1000) philipph  (1000)    10839 2022-05-30 15:14:51.000000 dbis-btree-0.0.1/dbis_btree/BBaum_Creator.py
--rwxr-xr-x   0 philipph  (1000) philipph  (1000)    10584 2022-05-30 15:14:51.000000 dbis-btree-0.0.1/dbis_btree/BBaum_Exercise_Generator.py
--rw-r--r--   0 philipph  (1000) philipph  (1000)        0 2022-05-30 15:14:51.000000 dbis-btree-0.0.1/dbis_btree/__init__.py
--rw-r--r--   0 philipph  (1000) philipph  (1000)     2790 2022-05-30 15:14:51.000000 dbis-btree-0.0.1/dbis_btree/__main__.py
-drwxr-xr-x   0 philipph  (1000) philipph  (1000)        0 2022-05-30 15:21:35.160859 dbis-btree-0.0.1/dbis_btree.egg-info/
--rw-r--r--   0 philipph  (1000) philipph  (1000)     1433 2022-05-30 15:21:35.000000 dbis-btree-0.0.1/dbis_btree.egg-info/PKG-INFO
--rw-r--r--   0 philipph  (1000) philipph  (1000)      299 2022-05-30 15:21:35.000000 dbis-btree-0.0.1/dbis_btree.egg-info/SOURCES.txt
--rw-r--r--   0 philipph  (1000) philipph  (1000)        1 2022-05-30 15:21:35.000000 dbis-btree-0.0.1/dbis_btree.egg-info/dependency_links.txt
--rw-r--r--   0 philipph  (1000) philipph  (1000)       11 2022-05-30 15:21:35.000000 dbis-btree-0.0.1/dbis_btree.egg-info/top_level.txt
--rw-r--r--   0 philipph  (1000) philipph  (1000)       38 2022-05-30 15:21:35.160859 dbis-btree-0.0.1/setup.cfg
--rw-r--r--   0 philipph  (1000) philipph  (1000)      994 2022-05-30 15:21:31.000000 dbis-btree-0.0.1/setup.py
+drwxr-xr-x   0 larsleimbach   (501) staff       (20)        0 2022-05-30 16:45:46.805302 dbis-btree-0.0.2/
+-rw-r--r--   0 larsleimbach   (501) staff       (20)       63 2022-04-09 21:01:15.000000 dbis-btree-0.0.2/MANIFEST.in
+-rw-r--r--   0 larsleimbach   (501) staff       (20)     4183 2022-05-30 16:45:46.804870 dbis-btree-0.0.2/PKG-INFO
+-rw-r--r--   0 larsleimbach   (501) staff       (20)     2855 2022-05-30 16:40:08.000000 dbis-btree-0.0.2/README.md
+drwxr-xr-x   0 larsleimbach   (501) staff       (20)        0 2022-05-30 16:45:46.802773 dbis-btree-0.0.2/dbis_btree/
+-rwxr-xr-x   0 larsleimbach   (501) staff       (20)    10126 2022-05-30 15:44:39.000000 dbis-btree-0.0.2/dbis_btree/BBaum.py
+-rwxr-xr-x   0 larsleimbach   (501) staff       (20)    10629 2022-05-30 16:01:14.000000 dbis-btree-0.0.2/dbis_btree/BBaum_Creator.py
+-rwxr-xr-x   0 larsleimbach   (501) staff       (20)    10374 2022-05-30 16:01:27.000000 dbis-btree-0.0.2/dbis_btree/BBaum_Exercise_Generator.py
+-rw-r--r--   0 larsleimbach   (501) staff       (20)        0 2022-05-30 15:44:39.000000 dbis-btree-0.0.2/dbis_btree/__init__.py
+-rw-r--r--   0 larsleimbach   (501) staff       (20)     2790 2022-05-30 15:44:39.000000 dbis-btree-0.0.2/dbis_btree/__main__.py
+drwxr-xr-x   0 larsleimbach   (501) staff       (20)        0 2022-05-30 16:45:46.804262 dbis-btree-0.0.2/dbis_btree.egg-info/
+-rw-r--r--   0 larsleimbach   (501) staff       (20)     4183 2022-05-30 16:45:46.000000 dbis-btree-0.0.2/dbis_btree.egg-info/PKG-INFO
+-rw-r--r--   0 larsleimbach   (501) staff       (20)      299 2022-05-30 16:45:46.000000 dbis-btree-0.0.2/dbis_btree.egg-info/SOURCES.txt
+-rw-r--r--   0 larsleimbach   (501) staff       (20)        1 2022-05-30 16:45:46.000000 dbis-btree-0.0.2/dbis_btree.egg-info/dependency_links.txt
+-rw-r--r--   0 larsleimbach   (501) staff       (20)       11 2022-05-30 16:45:46.000000 dbis-btree-0.0.2/dbis_btree.egg-info/top_level.txt
+-rw-r--r--   0 larsleimbach   (501) staff       (20)       38 2022-05-30 16:45:46.805493 dbis-btree-0.0.2/setup.cfg
+-rw-r--r--   0 larsleimbach   (501) staff       (20)      994 2022-05-30 16:45:31.000000 dbis-btree-0.0.2/setup.py
```

### Comparing `dbis-btree-0.0.1/dbis_btree/BBaum.py` & `dbis-btree-0.0.2/dbis_btree/BBaum.py`

 * *Files identical despite different names*

### Comparing `dbis-btree-0.0.1/dbis_btree/BBaum_Creator.py` & `dbis-btree-0.0.2/dbis_btree/BBaum_Creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-#import sys
-#import os
-# to import from parent folder
-## sets current folder to parent folder
-#current = os.path.dirname(os.path.realpath(__file__))
-#parent = os.path.dirname(current)
-#sys.path.append(parent)
-
 from .BBaum import BTree
 import numpy as np
 from enum import Enum
 
 class TreeTypes(Enum):
     INSERT = "INSERT"
     INSERT_TRIVIAL = "INSERT_TRIVIAL"
```

### Comparing `dbis-btree-0.0.1/dbis_btree/BBaum_Exercise_Generator.py` & `dbis-btree-0.0.2/dbis_btree/BBaum_Exercise_Generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-#import sys
-#import os
-# to import from parent folder
-## sets current folder to parent folder
-#current = os.path.dirname(os.path.realpath(__file__))
-#parent = os.path.dirname(current)
-#sys.path.append(parent)
-
 from .BBaum_Creator import BTree_Creator
 from .BBaum_Creator import TreeTypes
 from .BBaum import BTree
 import numpy as np
 import random
 import warnings
```

### Comparing `dbis-btree-0.0.1/dbis_btree/__main__.py` & `dbis-btree-0.0.2/dbis_btree/__main__.py`

 * *Files identical despite different names*

### Comparing `dbis-btree-0.0.1/setup.py` & `dbis-btree-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 from setuptools import setup
 
 class Version(object):
     name="dbis_btree"
     description="RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme"
-    version='0.0.1'
+    version='0.0.2'
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent.resolve()
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
```

