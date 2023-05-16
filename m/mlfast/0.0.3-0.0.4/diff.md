# Comparing `tmp/mlfast-0.0.3.tar.gz` & `tmp/mlfast-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlfast-0.0.3.tar", last modified: Tue May  9 17:55:47 2023, max compression
+gzip compressed data, was "mlfast-0.0.4.tar", last modified: Tue May 16 20:48:20 2023, max compression
```

## Comparing `mlfast-0.0.3.tar` & `mlfast-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:55:47.053438 mlfast-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-09 17:54:47.000000 mlfast-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-09 17:55:47.053438 mlfast-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-09 17:54:47.000000 mlfast-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-09 17:54:47.000000 mlfast-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-09 17:55:47.053438 mlfast-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-09 17:54:47.000000 mlfast-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:55:47.053438 mlfast-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:55:47.053438 mlfast-0.0.3/src/mlfast/
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-09 17:54:47.000000 mlfast-0.0.3/src/mlfast/Classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-09 17:54:47.000000 mlfast-0.0.3/src/mlfast/Regression.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 17:54:47.000000 mlfast-0.0.3/src/mlfast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-09 17:54:47.000000 mlfast-0.0.3/src/mlfast/custom_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-09 17:54:47.000000 mlfast-0.0.3/src/mlfast/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:55:47.053438 mlfast-0.0.3/src/mlfast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-09 17:55:47.000000 mlfast-0.0.3/src/mlfast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-09 17:55:47.000000 mlfast-0.0.3/src/mlfast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 17:55:47.000000 mlfast-0.0.3/src/mlfast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 17:55:47.000000 mlfast-0.0.3/src/mlfast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 17:55:47.000000 mlfast-0.0.3/src/mlfast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:48:20.049194 mlfast-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-16 20:47:18.000000 mlfast-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-16 20:48:20.049194 mlfast-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-16 20:47:18.000000 mlfast-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-16 20:47:18.000000 mlfast-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-16 20:48:20.049194 mlfast-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-16 20:47:18.000000 mlfast-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:48:20.045194 mlfast-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:48:20.049194 mlfast-0.0.4/src/mlfast/
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-16 20:47:18.000000 mlfast-0.0.4/src/mlfast/Classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-16 20:47:18.000000 mlfast-0.0.4/src/mlfast/Regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-16 20:47:18.000000 mlfast-0.0.4/src/mlfast/Text_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-16 20:47:18.000000 mlfast-0.0.4/src/mlfast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-16 20:47:18.000000 mlfast-0.0.4/src/mlfast/custom_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-16 20:47:18.000000 mlfast-0.0.4/src/mlfast/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:48:20.049194 mlfast-0.0.4/src/mlfast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-16 20:48:20.000000 mlfast-0.0.4/src/mlfast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-16 20:48:20.000000 mlfast-0.0.4/src/mlfast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:48:20.000000 mlfast-0.0.4/src/mlfast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-16 20:48:20.000000 mlfast-0.0.4/src/mlfast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 20:48:20.000000 mlfast-0.0.4/src/mlfast.egg-info/top_level.txt
```

### Comparing `mlfast-0.0.3/LICENSE` & `mlfast-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mlfast-0.0.3/PKG-INFO` & `mlfast-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlfast
-Version: 0.0.3
+Version: 0.0.4
 Summary: its a python machine learning package
 Home-page: https://github.com/Abdul-Jaweed/mlfast
 Author: Abdul-Jaweed
 Author-email: jdgaming7320@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Abdul-Jaweed/mlfast/issues
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mlfast-0.0.3/README.md` & `mlfast-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mlfast-0.0.3/setup.cfg` & `mlfast-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `mlfast-0.0.3/setup.py` & `mlfast-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 REPO_NAME = "mlfast"
 AUTHOR_USER_NAME = "Abdul-Jaweed"
 SRC_REPO = "mlfast"
 AUTHOR_EMAIL = "jdgaming7320@gmail.com"
 
 setuptools.setup(
```

### Comparing `mlfast-0.0.3/src/mlfast/Classification.py` & `mlfast-0.0.4/src/mlfast/Classification.py`

 * *Files identical despite different names*

### Comparing `mlfast-0.0.3/src/mlfast/Regression.py` & `mlfast-0.0.4/src/mlfast/Regression.py`

 * *Files identical despite different names*

### Comparing `mlfast-0.0.3/src/mlfast.egg-info/PKG-INFO` & `mlfast-0.0.4/src/mlfast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlfast
-Version: 0.0.3
+Version: 0.0.4
 Summary: its a python machine learning package
 Home-page: https://github.com/Abdul-Jaweed/mlfast
 Author: Abdul-Jaweed
 Author-email: jdgaming7320@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Abdul-Jaweed/mlfast/issues
 Classifier: Programming Language :: Python :: 3.7
```

