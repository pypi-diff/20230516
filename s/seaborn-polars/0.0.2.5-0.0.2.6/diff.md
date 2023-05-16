# Comparing `tmp/seaborn_polars-0.0.2.5.tar.gz` & `tmp/seaborn_polars-0.0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaborn_polars-0.0.2.5.tar", last modified: Tue May 16 03:07:44 2023, max compression
+gzip compressed data, was "seaborn_polars-0.0.2.6.tar", last modified: Tue May 16 03:15:19 2023, max compression
```

## Comparing `seaborn_polars-0.0.2.5.tar` & `seaborn_polars-0.0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 pav       (1000) pav       (1000)        0 2023-05-16 03:07:44.213090 seaborn_polars-0.0.2.5/
--rw-r--r--   0 pav       (1000) pav       (1000)    11357 2023-05-16 02:07:12.000000 seaborn_polars-0.0.2.5/LICENSE
--rw-r--r--   0 pav       (1000) pav       (1000)     1417 2023-05-16 03:07:44.212090 seaborn_polars-0.0.2.5/PKG-INFO
--rw-r--r--   0 pav       (1000) pav       (1000)     1003 2023-05-16 02:23:33.000000 seaborn_polars-0.0.2.5/README.md
--rw-r--r--   0 pav       (1000) pav       (1000)       29 2023-05-16 02:26:53.000000 seaborn_polars-0.0.2.5/pyproject.toml
-drwxr-xr-x   0 pav       (1000) pav       (1000)        0 2023-05-16 03:07:44.211090 seaborn_polars-0.0.2.5/seaborn_polars/
-drwxr-xr-x   0 pav       (1000) pav       (1000)        0 2023-05-16 03:07:44.212090 seaborn_polars-0.0.2.5/seaborn_polars/src/
-drwxr-xr-x   0 pav       (1000) pav       (1000)        0 2023-05-16 03:07:44.212090 seaborn_polars-0.0.2.5/seaborn_polars/src/seaborn_polars.egg-info/
--rw-r--r--   0 pav       (1000) pav       (1000)     1417 2023-05-16 03:07:44.000000 seaborn_polars-0.0.2.5/seaborn_polars/src/seaborn_polars.egg-info/PKG-INFO
--rw-r--r--   0 pav       (1000) pav       (1000)      306 2023-05-16 03:07:44.000000 seaborn_polars-0.0.2.5/seaborn_polars/src/seaborn_polars.egg-info/SOURCES.txt
--rw-r--r--   0 pav       (1000) pav       (1000)        1 2023-05-16 03:07:44.000000 seaborn_polars-0.0.2.5/seaborn_polars/src/seaborn_polars.egg-info/dependency_links.txt
--rw-r--r--   0 pav       (1000) pav       (1000)       15 2023-05-16 03:07:44.000000 seaborn_polars-0.0.2.5/seaborn_polars/src/seaborn_polars.egg-info/top_level.txt
--rw-r--r--   0 pav       (1000) pav       (1000)     3133 2023-05-16 02:07:12.000000 seaborn_polars-0.0.2.5/seaborn_polars/src/seaborn_polars.py
--rw-r--r--   0 pav       (1000) pav       (1000)       38 2023-05-16 03:07:44.213090 seaborn_polars-0.0.2.5/setup.cfg
--rw-r--r--   0 pav       (1000) pav       (1000)     1279 2023-05-16 03:07:20.000000 seaborn_polars-0.0.2.5/setup.py
+drwxr-xr-x   0 pav       (1000) pav       (1000)        0 2023-05-16 03:15:19.653214 seaborn_polars-0.0.2.6/
+-rw-r--r--   0 pav       (1000) pav       (1000)    11357 2023-05-16 02:07:12.000000 seaborn_polars-0.0.2.6/LICENSE
+-rw-r--r--   0 pav       (1000) pav       (1000)     1453 2023-05-16 03:15:19.653214 seaborn_polars-0.0.2.6/PKG-INFO
+-rw-r--r--   0 pav       (1000) pav       (1000)     1039 2023-05-16 03:14:58.000000 seaborn_polars-0.0.2.6/README.md
+-rw-r--r--   0 pav       (1000) pav       (1000)       29 2023-05-16 02:26:53.000000 seaborn_polars-0.0.2.6/pyproject.toml
+drwxr-xr-x   0 pav       (1000) pav       (1000)        0 2023-05-16 03:15:19.652214 seaborn_polars-0.0.2.6/seaborn_polars/
+drwxr-xr-x   0 pav       (1000) pav       (1000)        0 2023-05-16 03:15:19.652214 seaborn_polars-0.0.2.6/seaborn_polars/src/
+drwxr-xr-x   0 pav       (1000) pav       (1000)        0 2023-05-16 03:15:19.653214 seaborn_polars-0.0.2.6/seaborn_polars/src/seaborn_polars.egg-info/
+-rw-r--r--   0 pav       (1000) pav       (1000)     1453 2023-05-16 03:15:19.000000 seaborn_polars-0.0.2.6/seaborn_polars/src/seaborn_polars.egg-info/PKG-INFO
+-rw-r--r--   0 pav       (1000) pav       (1000)      306 2023-05-16 03:15:19.000000 seaborn_polars-0.0.2.6/seaborn_polars/src/seaborn_polars.egg-info/SOURCES.txt
+-rw-r--r--   0 pav       (1000) pav       (1000)        1 2023-05-16 03:15:19.000000 seaborn_polars-0.0.2.6/seaborn_polars/src/seaborn_polars.egg-info/dependency_links.txt
+-rw-r--r--   0 pav       (1000) pav       (1000)       15 2023-05-16 03:15:19.000000 seaborn_polars-0.0.2.6/seaborn_polars/src/seaborn_polars.egg-info/top_level.txt
+-rw-r--r--   0 pav       (1000) pav       (1000)     3133 2023-05-16 02:07:12.000000 seaborn_polars-0.0.2.6/seaborn_polars/src/seaborn_polars.py
+-rw-r--r--   0 pav       (1000) pav       (1000)       38 2023-05-16 03:15:19.653214 seaborn_polars-0.0.2.6/setup.cfg
+-rw-r--r--   0 pav       (1000) pav       (1000)     1279 2023-05-16 03:14:41.000000 seaborn_polars-0.0.2.6/setup.py
```

### Comparing `seaborn_polars-0.0.2.5/LICENSE` & `seaborn_polars-0.0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `seaborn_polars-0.0.2.5/PKG-INFO` & `seaborn_polars-0.0.2.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaborn_polars
-Version: 0.0.2.5
+Version: 0.0.2.6
 Summary: Wrapper for plotting with seaborn using Polars dataframes and lazyframes
 Author: Pavel Cherepanskiy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -17,15 +17,15 @@
 Python 3.8+
 
 Seaborn, Polars, Pandas, Numpy, Pyarrow
 
 # Installation
 Use regular pip install:
 ```
-pip install seaborn_polars
+pip install seaborn_polars pandas numpy polars seaborn pyarrow
 ```
 Alternatively, clone this repository.
 
 # Usage
 The package is a wrapper around seaborn plotting functions allowing to use Polars DataFrames and LazyFrames with the same syntax as when using Pandas DataFrames.
 ```
 import polars as pl
```

### Comparing `seaborn_polars-0.0.2.5/README.md` & `seaborn_polars-0.0.2.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Python 3.8+
 
 Seaborn, Polars, Pandas, Numpy, Pyarrow
 
 # Installation
 Use regular pip install:
 ```
-pip install seaborn_polars
+pip install seaborn_polars pandas numpy polars seaborn pyarrow
 ```
 Alternatively, clone this repository.
 
 # Usage
 The package is a wrapper around seaborn plotting functions allowing to use Polars DataFrames and LazyFrames with the same syntax as when using Pandas DataFrames.
 ```
 import polars as pl
```

### Comparing `seaborn_polars-0.0.2.5/seaborn_polars/src/seaborn_polars.egg-info/PKG-INFO` & `seaborn_polars-0.0.2.6/seaborn_polars/src/seaborn_polars.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaborn-polars
-Version: 0.0.2.5
+Version: 0.0.2.6
 Summary: Wrapper for plotting with seaborn using Polars dataframes and lazyframes
 Author: Pavel Cherepanskiy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -17,15 +17,15 @@
 Python 3.8+
 
 Seaborn, Polars, Pandas, Numpy, Pyarrow
 
 # Installation
 Use regular pip install:
 ```
-pip install seaborn_polars
+pip install seaborn_polars pandas numpy polars seaborn pyarrow
 ```
 Alternatively, clone this repository.
 
 # Usage
 The package is a wrapper around seaborn plotting functions allowing to use Polars DataFrames and LazyFrames with the same syntax as when using Pandas DataFrames.
 ```
 import polars as pl
```

### Comparing `seaborn_polars-0.0.2.5/seaborn_polars/src/seaborn_polars.py` & `seaborn_polars-0.0.2.6/seaborn_polars/src/seaborn_polars.py`

 * *Files identical despite different names*

### Comparing `seaborn_polars-0.0.2.5/setup.py` & `seaborn_polars-0.0.2.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seaborn_polars",                           # This is the name of the package
-    version="0.0.2.5",                                 # The initial release version
+    version="0.0.2.6",                                 # The initial release version
     author="Pavel Cherepanskiy",                     # Full name of the author
     description="Wrapper for plotting with seaborn using Polars dataframes and lazyframes",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

