# Comparing `tmp/flytekitplugins-mlflow-1.6.0b4.tar.gz` & `tmp/flytekitplugins-mlflow-1.6.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-mlflow-1.6.0b4.tar", last modified: Tue May  9 00:42:37 2023, max compression
+gzip compressed data, was "flytekitplugins-mlflow-1.6.1b0.tar", last modified: Mon May 15 22:07:07 2023, max compression
```

## Comparing `flytekitplugins-mlflow-1.6.0b4.tar` & `flytekitplugins-mlflow-1.6.1b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:37.120769 flytekitplugins-mlflow-1.6.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-09 00:42:37.120769 flytekitplugins-mlflow-1.6.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-09 00:42:15.000000 flytekitplugins-mlflow-1.6.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:37.120769 flytekitplugins-mlflow-1.6.0b4/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:37.120769 flytekitplugins-mlflow-1.6.0b4/flytekitplugins/mlflow/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-09 00:42:15.000000 flytekitplugins-mlflow-1.6.0b4/flytekitplugins/mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-09 00:42:15.000000 flytekitplugins-mlflow-1.6.0b4/flytekitplugins/mlflow/tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:37.120769 flytekitplugins-mlflow-1.6.0b4/flytekitplugins_mlflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-09 00:42:37.000000 flytekitplugins-mlflow-1.6.0b4/flytekitplugins_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-09 00:42:37.000000 flytekitplugins-mlflow-1.6.0b4/flytekitplugins_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:42:37.000000 flytekitplugins-mlflow-1.6.0b4/flytekitplugins_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:37.000000 flytekitplugins-mlflow-1.6.0b4/flytekitplugins_mlflow.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-09 00:42:37.000000 flytekitplugins-mlflow-1.6.0b4/flytekitplugins_mlflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:37.000000 flytekitplugins-mlflow-1.6.0b4/flytekitplugins_mlflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:42:37.120769 flytekitplugins-mlflow-1.6.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-09 00:42:30.000000 flytekitplugins-mlflow-1.6.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:07.331804 flytekitplugins-mlflow-1.6.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-15 22:07:07.331804 flytekitplugins-mlflow-1.6.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-15 22:06:44.000000 flytekitplugins-mlflow-1.6.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:07.331804 flytekitplugins-mlflow-1.6.1b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:07.331804 flytekitplugins-mlflow-1.6.1b0/flytekitplugins/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-15 22:06:44.000000 flytekitplugins-mlflow-1.6.1b0/flytekitplugins/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-15 22:06:44.000000 flytekitplugins-mlflow-1.6.1b0/flytekitplugins/mlflow/tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:07.331804 flytekitplugins-mlflow-1.6.1b0/flytekitplugins_mlflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-15 22:07:07.000000 flytekitplugins-mlflow-1.6.1b0/flytekitplugins_mlflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-15 22:07:07.000000 flytekitplugins-mlflow-1.6.1b0/flytekitplugins_mlflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:07:07.000000 flytekitplugins-mlflow-1.6.1b0/flytekitplugins_mlflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:07.000000 flytekitplugins-mlflow-1.6.1b0/flytekitplugins_mlflow.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-15 22:07:07.000000 flytekitplugins-mlflow-1.6.1b0/flytekitplugins_mlflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:07.000000 flytekitplugins-mlflow-1.6.1b0/flytekitplugins_mlflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:07:07.331804 flytekitplugins-mlflow-1.6.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-15 22:07:00.000000 flytekitplugins-mlflow-1.6.1b0/setup.py
```

### Comparing `flytekitplugins-mlflow-1.6.0b4/PKG-INFO` & `flytekitplugins-mlflow-1.6.1b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-mlflow
-Version: 1.6.0b4
+Version: 1.6.1b0
 Summary: This package enables seamless use of MLFlow within Flyte
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-mlflow-1.6.0b4/README.md` & `flytekitplugins-mlflow-1.6.1b0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-mlflow-1.6.0b4/flytekitplugins/mlflow/tracking.py` & `flytekitplugins-mlflow-1.6.1b0/flytekitplugins/mlflow/tracking.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-mlflow-1.6.0b4/flytekitplugins_mlflow.egg-info/PKG-INFO` & `flytekitplugins-mlflow-1.6.1b0/flytekitplugins_mlflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-mlflow
-Version: 1.6.0b4
+Version: 1.6.1b0
 Summary: This package enables seamless use of MLFlow within Flyte
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-mlflow-1.6.0b4/setup.py` & `flytekitplugins-mlflow-1.6.1b0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "mlflow"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.1.0,<2.0.0", "plotly", "mlflow"]
 
-__version__ = "1.6.0b4"
+__version__ = "1.6.1b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package enables seamless use of MLFlow within Flyte",
```

