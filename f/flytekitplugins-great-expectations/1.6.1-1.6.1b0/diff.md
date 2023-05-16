# Comparing `tmp/flytekitplugins-great_expectations-1.6.1.tar.gz` & `tmp/flytekitplugins-great_expectations-1.6.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-great_expectations-1.6.1.tar", last modified: Tue May 16 00:12:31 2023, max compression
+gzip compressed data, was "flytekitplugins-great_expectations-1.6.1b0.tar", last modified: Mon May 15 22:07:04 2023, max compression
```

## Comparing `flytekitplugins-great_expectations-1.6.1.tar` & `flytekitplugins-great_expectations-1.6.1b0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:12:31.806365 flytekitplugins-great_expectations-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-16 00:12:31.806365 flytekitplugins-great_expectations-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-16 00:12:01.000000 flytekitplugins-great_expectations-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:12:31.806365 flytekitplugins-great_expectations-1.6.1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:12:31.806365 flytekitplugins-great_expectations-1.6.1/flytekitplugins/great_expectations/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-16 00:12:01.000000 flytekitplugins-great_expectations-1.6.1/flytekitplugins/great_expectations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-05-16 00:12:01.000000 flytekitplugins-great_expectations-1.6.1/flytekitplugins/great_expectations/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-05-16 00:12:01.000000 flytekitplugins-great_expectations-1.6.1/flytekitplugins/great_expectations/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:12:31.806365 flytekitplugins-great_expectations-1.6.1/flytekitplugins_great_expectations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-16 00:12:31.000000 flytekitplugins-great_expectations-1.6.1/flytekitplugins_great_expectations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-16 00:12:31.000000 flytekitplugins-great_expectations-1.6.1/flytekitplugins_great_expectations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:12:31.000000 flytekitplugins-great_expectations-1.6.1/flytekitplugins_great_expectations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 00:12:31.000000 flytekitplugins-great_expectations-1.6.1/flytekitplugins_great_expectations.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-16 00:12:31.000000 flytekitplugins-great_expectations-1.6.1/flytekitplugins_great_expectations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 00:12:31.000000 flytekitplugins-great_expectations-1.6.1/flytekitplugins_great_expectations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 00:12:31.806365 flytekitplugins-great_expectations-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-16 00:12:27.000000 flytekitplugins-great_expectations-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:04.851819 flytekitplugins-great_expectations-1.6.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-15 22:07:04.851819 flytekitplugins-great_expectations-1.6.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-15 22:06:44.000000 flytekitplugins-great_expectations-1.6.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:04.851819 flytekitplugins-great_expectations-1.6.1b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:04.851819 flytekitplugins-great_expectations-1.6.1b0/flytekitplugins/great_expectations/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-15 22:06:44.000000 flytekitplugins-great_expectations-1.6.1b0/flytekitplugins/great_expectations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-05-15 22:06:44.000000 flytekitplugins-great_expectations-1.6.1b0/flytekitplugins/great_expectations/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-05-15 22:06:44.000000 flytekitplugins-great_expectations-1.6.1b0/flytekitplugins/great_expectations/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:04.851819 flytekitplugins-great_expectations-1.6.1b0/flytekitplugins_great_expectations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-15 22:07:04.000000 flytekitplugins-great_expectations-1.6.1b0/flytekitplugins_great_expectations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-15 22:07:04.000000 flytekitplugins-great_expectations-1.6.1b0/flytekitplugins_great_expectations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:07:04.000000 flytekitplugins-great_expectations-1.6.1b0/flytekitplugins_great_expectations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:04.000000 flytekitplugins-great_expectations-1.6.1b0/flytekitplugins_great_expectations.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 22:07:04.000000 flytekitplugins-great_expectations-1.6.1b0/flytekitplugins_great_expectations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:04.000000 flytekitplugins-great_expectations-1.6.1b0/flytekitplugins_great_expectations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:07:04.851819 flytekitplugins-great_expectations-1.6.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-15 22:07:00.000000 flytekitplugins-great_expectations-1.6.1b0/setup.py
```

### Comparing `flytekitplugins-great_expectations-1.6.1/PKG-INFO` & `flytekitplugins-great_expectations-1.6.1b0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-great_expectations
-Version: 1.6.1
+Version: 1.6.1b0
 Summary: Great Expectations Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-great_expectations-1.6.1/README.md` & `flytekitplugins-great_expectations-1.6.1b0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-great_expectations-1.6.1/flytekitplugins/great_expectations/schema.py` & `flytekitplugins-great_expectations-1.6.1b0/flytekitplugins/great_expectations/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-great_expectations-1.6.1/flytekitplugins/great_expectations/task.py` & `flytekitplugins-great_expectations-1.6.1b0/flytekitplugins/great_expectations/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-great_expectations-1.6.1/flytekitplugins_great_expectations.egg-info/PKG-INFO` & `flytekitplugins-great_expectations-1.6.1b0/flytekitplugins_great_expectations.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-great-expectations
-Version: 1.6.1
+Version: 1.6.1b0
 Summary: Great Expectations Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-great_expectations-1.6.1/setup.py` & `flytekitplugins-great_expectations-1.6.1b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "great_expectations"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "great-expectations>=0.13.30", "sqlalchemy>=1.4.23,<2.0.0"]
 
-__version__ = "1.6.1"
+__version__ = "1.6.1b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="Great Expectations Plugin for Flytekit",
```

