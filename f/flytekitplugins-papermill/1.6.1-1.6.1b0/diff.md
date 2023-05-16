# Comparing `tmp/flytekitplugins-papermill-1.6.1.tar.gz` & `tmp/flytekitplugins-papermill-1.6.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-papermill-1.6.1.tar", last modified: Tue May 16 00:12:36 2023, max compression
+gzip compressed data, was "flytekitplugins-papermill-1.6.1b0.tar", last modified: Mon May 15 22:07:09 2023, max compression
```

## Comparing `flytekitplugins-papermill-1.6.1.tar` & `flytekitplugins-papermill-1.6.1b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:12:36.034349 flytekitplugins-papermill-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-16 00:12:36.034349 flytekitplugins-papermill-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-16 00:12:01.000000 flytekitplugins-papermill-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:12:36.034349 flytekitplugins-papermill-1.6.1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:12:36.034349 flytekitplugins-papermill-1.6.1/flytekitplugins/papermill/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-16 00:12:01.000000 flytekitplugins-papermill-1.6.1/flytekitplugins/papermill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15374 2023-05-16 00:12:01.000000 flytekitplugins-papermill-1.6.1/flytekitplugins/papermill/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:12:36.034349 flytekitplugins-papermill-1.6.1/flytekitplugins_papermill.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-16 00:12:36.000000 flytekitplugins-papermill-1.6.1/flytekitplugins_papermill.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-16 00:12:36.000000 flytekitplugins-papermill-1.6.1/flytekitplugins_papermill.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:12:36.000000 flytekitplugins-papermill-1.6.1/flytekitplugins_papermill.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 00:12:36.000000 flytekitplugins-papermill-1.6.1/flytekitplugins_papermill.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-16 00:12:36.000000 flytekitplugins-papermill-1.6.1/flytekitplugins_papermill.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 00:12:36.000000 flytekitplugins-papermill-1.6.1/flytekitplugins_papermill.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 00:12:36.034349 flytekitplugins-papermill-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-16 00:12:27.000000 flytekitplugins-papermill-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:09.075792 flytekitplugins-papermill-1.6.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-15 22:07:09.075792 flytekitplugins-papermill-1.6.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-15 22:06:44.000000 flytekitplugins-papermill-1.6.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:09.071792 flytekitplugins-papermill-1.6.1b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:09.071792 flytekitplugins-papermill-1.6.1b0/flytekitplugins/papermill/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-15 22:06:44.000000 flytekitplugins-papermill-1.6.1b0/flytekitplugins/papermill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15374 2023-05-15 22:06:44.000000 flytekitplugins-papermill-1.6.1b0/flytekitplugins/papermill/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:09.075792 flytekitplugins-papermill-1.6.1b0/flytekitplugins_papermill.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-15 22:07:09.000000 flytekitplugins-papermill-1.6.1b0/flytekitplugins_papermill.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-15 22:07:09.000000 flytekitplugins-papermill-1.6.1b0/flytekitplugins_papermill.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:07:09.000000 flytekitplugins-papermill-1.6.1b0/flytekitplugins_papermill.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:09.000000 flytekitplugins-papermill-1.6.1b0/flytekitplugins_papermill.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-15 22:07:09.000000 flytekitplugins-papermill-1.6.1b0/flytekitplugins_papermill.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:09.000000 flytekitplugins-papermill-1.6.1b0/flytekitplugins_papermill.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:07:09.075792 flytekitplugins-papermill-1.6.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-15 22:07:00.000000 flytekitplugins-papermill-1.6.1b0/setup.py
```

### Comparing `flytekitplugins-papermill-1.6.1/PKG-INFO` & `flytekitplugins-papermill-1.6.1b0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-papermill
-Version: 1.6.1
+Version: 1.6.1b0
 Summary: This is the flytekit papermill plugin
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-papermill-1.6.1/README.md` & `flytekitplugins-papermill-1.6.1b0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-papermill-1.6.1/flytekitplugins/papermill/task.py` & `flytekitplugins-papermill-1.6.1b0/flytekitplugins/papermill/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-papermill-1.6.1/flytekitplugins_papermill.egg-info/PKG-INFO` & `flytekitplugins-papermill-1.6.1b0/flytekitplugins_papermill.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-papermill
-Version: 1.6.1
+Version: 1.6.1b0
 Summary: This is the flytekit papermill plugin
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-papermill-1.6.1/setup.py` & `flytekitplugins-papermill-1.6.1b0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 plugin_requires = [
     "flytekit>=1.3.0b2,<2.0.0",
     "papermill>=1.2.0",
     "nbconvert>=6.0.7",
     "ipykernel>=5.0.0",
 ]
 
-__version__ = "1.6.1"
+__version__ = "1.6.1b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This is the flytekit papermill plugin",
```

