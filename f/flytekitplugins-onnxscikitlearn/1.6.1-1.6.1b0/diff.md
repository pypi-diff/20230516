# Comparing `tmp/flytekitplugins-onnxscikitlearn-1.6.1.tar.gz` & `tmp/flytekitplugins-onnxscikitlearn-1.6.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-onnxscikitlearn-1.6.1.tar", last modified: Tue May 16 00:12:35 2023, max compression
+gzip compressed data, was "flytekitplugins-onnxscikitlearn-1.6.1b0.tar", last modified: Mon May 15 22:07:08 2023, max compression
```

## Comparing `flytekitplugins-onnxscikitlearn-1.6.1.tar` & `flytekitplugins-onnxscikitlearn-1.6.1b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:12:35.330352 flytekitplugins-onnxscikitlearn-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-16 00:12:35.330352 flytekitplugins-onnxscikitlearn-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-16 00:12:01.000000 flytekitplugins-onnxscikitlearn-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:12:35.326352 flytekitplugins-onnxscikitlearn-1.6.1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:12:35.330352 flytekitplugins-onnxscikitlearn-1.6.1/flytekitplugins/onnxscikitlearn/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-16 00:12:01.000000 flytekitplugins-onnxscikitlearn-1.6.1/flytekitplugins/onnxscikitlearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-16 00:12:01.000000 flytekitplugins-onnxscikitlearn-1.6.1/flytekitplugins/onnxscikitlearn/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:12:35.330352 flytekitplugins-onnxscikitlearn-1.6.1/flytekitplugins_onnxscikitlearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-16 00:12:35.000000 flytekitplugins-onnxscikitlearn-1.6.1/flytekitplugins_onnxscikitlearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-16 00:12:35.000000 flytekitplugins-onnxscikitlearn-1.6.1/flytekitplugins_onnxscikitlearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:12:35.000000 flytekitplugins-onnxscikitlearn-1.6.1/flytekitplugins_onnxscikitlearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 00:12:35.000000 flytekitplugins-onnxscikitlearn-1.6.1/flytekitplugins_onnxscikitlearn.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 00:12:35.000000 flytekitplugins-onnxscikitlearn-1.6.1/flytekitplugins_onnxscikitlearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 00:12:35.000000 flytekitplugins-onnxscikitlearn-1.6.1/flytekitplugins_onnxscikitlearn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 00:12:35.330352 flytekitplugins-onnxscikitlearn-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-16 00:12:27.000000 flytekitplugins-onnxscikitlearn-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:08.379798 flytekitplugins-onnxscikitlearn-1.6.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-15 22:07:08.379798 flytekitplugins-onnxscikitlearn-1.6.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-15 22:06:44.000000 flytekitplugins-onnxscikitlearn-1.6.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:08.375798 flytekitplugins-onnxscikitlearn-1.6.1b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:08.379798 flytekitplugins-onnxscikitlearn-1.6.1b0/flytekitplugins/onnxscikitlearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-15 22:06:44.000000 flytekitplugins-onnxscikitlearn-1.6.1b0/flytekitplugins/onnxscikitlearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-15 22:06:44.000000 flytekitplugins-onnxscikitlearn-1.6.1b0/flytekitplugins/onnxscikitlearn/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:08.379798 flytekitplugins-onnxscikitlearn-1.6.1b0/flytekitplugins_onnxscikitlearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-15 22:07:08.000000 flytekitplugins-onnxscikitlearn-1.6.1b0/flytekitplugins_onnxscikitlearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-15 22:07:08.000000 flytekitplugins-onnxscikitlearn-1.6.1b0/flytekitplugins_onnxscikitlearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:07:08.000000 flytekitplugins-onnxscikitlearn-1.6.1b0/flytekitplugins_onnxscikitlearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:08.000000 flytekitplugins-onnxscikitlearn-1.6.1b0/flytekitplugins_onnxscikitlearn.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 22:07:08.000000 flytekitplugins-onnxscikitlearn-1.6.1b0/flytekitplugins_onnxscikitlearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:08.000000 flytekitplugins-onnxscikitlearn-1.6.1b0/flytekitplugins_onnxscikitlearn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:07:08.379798 flytekitplugins-onnxscikitlearn-1.6.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-15 22:07:00.000000 flytekitplugins-onnxscikitlearn-1.6.1b0/setup.py
```

### Comparing `flytekitplugins-onnxscikitlearn-1.6.1/PKG-INFO` & `flytekitplugins-onnxscikitlearn-1.6.1b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-onnxscikitlearn
-Version: 1.6.1
+Version: 1.6.1b0
 Summary: ONNX ScikitLearn Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-onnxscikitlearn-1.6.1/flytekitplugins/onnxscikitlearn/schema.py` & `flytekitplugins-onnxscikitlearn-1.6.1b0/flytekitplugins/onnxscikitlearn/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-onnxscikitlearn-1.6.1/flytekitplugins_onnxscikitlearn.egg-info/PKG-INFO` & `flytekitplugins-onnxscikitlearn-1.6.1b0/flytekitplugins_onnxscikitlearn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-onnxscikitlearn
-Version: 1.6.1
+Version: 1.6.1b0
 Summary: ONNX ScikitLearn Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-onnxscikitlearn-1.6.1/setup.py` & `flytekitplugins-onnxscikitlearn-1.6.1b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "onnxscikitlearn"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit<1.3.0b2,<2.0.0", "skl2onnx>=1.10.3"]
 
-__version__ = "1.6.1"
+__version__ = "1.6.1b0"
 
 setup(
     name=f"flytekitplugins-{PLUGIN_NAME}",
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="ONNX ScikitLearn Plugin for Flytekit",
```

