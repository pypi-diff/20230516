# Comparing `tmp/flytekitplugins-kfmpi-1.6.1.tar.gz` & `tmp/flytekitplugins-kfmpi-1.6.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-kfmpi-1.6.1.tar", last modified: Tue May 16 00:12:33 2023, max compression
+gzip compressed data, was "flytekitplugins-kfmpi-1.6.1b0.tar", last modified: Mon May 15 22:07:06 2023, max compression
```

## Comparing `flytekitplugins-kfmpi-1.6.1.tar` & `flytekitplugins-kfmpi-1.6.1b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:12:33.214360 flytekitplugins-kfmpi-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-16 00:12:33.214360 flytekitplugins-kfmpi-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-16 00:12:01.000000 flytekitplugins-kfmpi-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:12:33.214360 flytekitplugins-kfmpi-1.6.1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:12:33.214360 flytekitplugins-kfmpi-1.6.1/flytekitplugins/kfmpi/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-16 00:12:01.000000 flytekitplugins-kfmpi-1.6.1/flytekitplugins/kfmpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-16 00:12:01.000000 flytekitplugins-kfmpi-1.6.1/flytekitplugins/kfmpi/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:12:33.214360 flytekitplugins-kfmpi-1.6.1/flytekitplugins_kfmpi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-16 00:12:33.000000 flytekitplugins-kfmpi-1.6.1/flytekitplugins_kfmpi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-16 00:12:33.000000 flytekitplugins-kfmpi-1.6.1/flytekitplugins_kfmpi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:12:33.000000 flytekitplugins-kfmpi-1.6.1/flytekitplugins_kfmpi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 00:12:33.000000 flytekitplugins-kfmpi-1.6.1/flytekitplugins_kfmpi.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-16 00:12:33.000000 flytekitplugins-kfmpi-1.6.1/flytekitplugins_kfmpi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 00:12:33.000000 flytekitplugins-kfmpi-1.6.1/flytekitplugins_kfmpi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 00:12:33.214360 flytekitplugins-kfmpi-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-16 00:12:27.000000 flytekitplugins-kfmpi-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:06.275810 flytekitplugins-kfmpi-1.6.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-15 22:07:06.271810 flytekitplugins-kfmpi-1.6.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-15 22:06:44.000000 flytekitplugins-kfmpi-1.6.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:06.271810 flytekitplugins-kfmpi-1.6.1b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:06.271810 flytekitplugins-kfmpi-1.6.1b0/flytekitplugins/kfmpi/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-15 22:06:44.000000 flytekitplugins-kfmpi-1.6.1b0/flytekitplugins/kfmpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-15 22:06:44.000000 flytekitplugins-kfmpi-1.6.1b0/flytekitplugins/kfmpi/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:06.271810 flytekitplugins-kfmpi-1.6.1b0/flytekitplugins_kfmpi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-15 22:07:06.000000 flytekitplugins-kfmpi-1.6.1b0/flytekitplugins_kfmpi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-15 22:07:06.000000 flytekitplugins-kfmpi-1.6.1b0/flytekitplugins_kfmpi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:07:06.000000 flytekitplugins-kfmpi-1.6.1b0/flytekitplugins_kfmpi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:06.000000 flytekitplugins-kfmpi-1.6.1b0/flytekitplugins_kfmpi.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-15 22:07:06.000000 flytekitplugins-kfmpi-1.6.1b0/flytekitplugins_kfmpi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:06.000000 flytekitplugins-kfmpi-1.6.1b0/flytekitplugins_kfmpi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:07:06.275810 flytekitplugins-kfmpi-1.6.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-15 22:07:00.000000 flytekitplugins-kfmpi-1.6.1b0/setup.py
```

### Comparing `flytekitplugins-kfmpi-1.6.1/PKG-INFO` & `flytekitplugins-kfmpi-1.6.1b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfmpi
-Version: 1.6.1
+Version: 1.6.1b0
 Summary: K8s based MPI plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfmpi-1.6.1/flytekitplugins/kfmpi/task.py` & `flytekitplugins-kfmpi-1.6.1b0/flytekitplugins/kfmpi/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-kfmpi-1.6.1/flytekitplugins_kfmpi.egg-info/PKG-INFO` & `flytekitplugins-kfmpi-1.6.1b0/flytekitplugins_kfmpi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfmpi
-Version: 1.6.1
+Version: 1.6.1b0
 Summary: K8s based MPI plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfmpi-1.6.1/setup.py` & `flytekitplugins-kfmpi-1.6.1b0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "kfmpi"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "flyteidl>=0.21.4"]
 
-__version__ = "1.6.1"
+__version__ = "1.6.1b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="K8s based MPI plugin for flytekit",
```

