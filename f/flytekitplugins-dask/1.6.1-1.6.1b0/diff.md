# Comparing `tmp/flytekitplugins-dask-1.6.1.tar.gz` & `tmp/flytekitplugins-dask-1.6.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-dask-1.6.1.tar", last modified: Tue May 16 00:12:29 2023, max compression
+gzip compressed data, was "flytekitplugins-dask-1.6.1b0.tar", last modified: Mon May 15 22:07:02 2023, max compression
```

## Comparing `flytekitplugins-dask-1.6.1.tar` & `flytekitplugins-dask-1.6.1b0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:12:29.290375 flytekitplugins-dask-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-16 00:12:29.290375 flytekitplugins-dask-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-16 00:12:01.000000 flytekitplugins-dask-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:12:29.290375 flytekitplugins-dask-1.6.1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:12:29.290375 flytekitplugins-dask-1.6.1/flytekitplugins/dask/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-16 00:12:01.000000 flytekitplugins-dask-1.6.1/flytekitplugins/dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-16 00:12:01.000000 flytekitplugins-dask-1.6.1/flytekitplugins/dask/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-16 00:12:01.000000 flytekitplugins-dask-1.6.1/flytekitplugins/dask/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:12:29.290375 flytekitplugins-dask-1.6.1/flytekitplugins_dask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-16 00:12:29.000000 flytekitplugins-dask-1.6.1/flytekitplugins_dask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-16 00:12:29.000000 flytekitplugins-dask-1.6.1/flytekitplugins_dask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:12:29.000000 flytekitplugins-dask-1.6.1/flytekitplugins_dask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 00:12:29.000000 flytekitplugins-dask-1.6.1/flytekitplugins_dask.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-16 00:12:29.000000 flytekitplugins-dask-1.6.1/flytekitplugins_dask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 00:12:29.000000 flytekitplugins-dask-1.6.1/flytekitplugins_dask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 00:12:29.290375 flytekitplugins-dask-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-16 00:12:27.000000 flytekitplugins-dask-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:02.355833 flytekitplugins-dask-1.6.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-15 22:07:02.355833 flytekitplugins-dask-1.6.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-15 22:06:44.000000 flytekitplugins-dask-1.6.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:02.355833 flytekitplugins-dask-1.6.1b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:02.355833 flytekitplugins-dask-1.6.1b0/flytekitplugins/dask/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-15 22:06:44.000000 flytekitplugins-dask-1.6.1b0/flytekitplugins/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-15 22:06:44.000000 flytekitplugins-dask-1.6.1b0/flytekitplugins/dask/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-15 22:06:44.000000 flytekitplugins-dask-1.6.1b0/flytekitplugins/dask/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:02.355833 flytekitplugins-dask-1.6.1b0/flytekitplugins_dask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-15 22:07:02.000000 flytekitplugins-dask-1.6.1b0/flytekitplugins_dask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-15 22:07:02.000000 flytekitplugins-dask-1.6.1b0/flytekitplugins_dask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:07:02.000000 flytekitplugins-dask-1.6.1b0/flytekitplugins_dask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:02.000000 flytekitplugins-dask-1.6.1b0/flytekitplugins_dask.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-15 22:07:02.000000 flytekitplugins-dask-1.6.1b0/flytekitplugins_dask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:02.000000 flytekitplugins-dask-1.6.1b0/flytekitplugins_dask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:07:02.355833 flytekitplugins-dask-1.6.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-15 22:07:00.000000 flytekitplugins-dask-1.6.1b0/setup.py
```

### Comparing `flytekitplugins-dask-1.6.1/PKG-INFO` & `flytekitplugins-dask-1.6.1b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-dask
-Version: 1.6.1
+Version: 1.6.1b0
 Summary: Dask plugin for flytekit
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-dask
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-dask-1.6.1/README.md` & `flytekitplugins-dask-1.6.1b0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-dask-1.6.1/flytekitplugins/dask/models.py` & `flytekitplugins-dask-1.6.1b0/flytekitplugins/dask/models.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-dask-1.6.1/flytekitplugins/dask/task.py` & `flytekitplugins-dask-1.6.1b0/flytekitplugins/dask/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-dask-1.6.1/flytekitplugins_dask.egg-info/PKG-INFO` & `flytekitplugins-dask-1.6.1b0/flytekitplugins_dask.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-dask
-Version: 1.6.1
+Version: 1.6.1b0
 Summary: Dask plugin for flytekit
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-dask
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-dask-1.6.1/setup.py` & `flytekitplugins-dask-1.6.1b0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 plugin_requires = [
     "flyteidl>=1.3.2",
     "flytekit>=1.3.0b2,<2.0.0",
     "dask[distributed]>=2022.10.2",
 ]
 
-__version__ = "1.6.1"
+__version__ = "1.6.1b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="Dask plugin for flytekit",
```

