# Comparing `tmp/flytekitplugins-awsbatch-1.6.0b4.tar.gz` & `tmp/flytekitplugins-awsbatch-1.6.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-awsbatch-1.6.0b4.tar", last modified: Tue May  9 00:42:31 2023, max compression
+gzip compressed data, was "flytekitplugins-awsbatch-1.6.1b0.tar", last modified: Mon May 15 22:07:01 2023, max compression
```

## Comparing `flytekitplugins-awsbatch-1.6.0b4.tar` & `flytekitplugins-awsbatch-1.6.1b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:31.104753 flytekitplugins-awsbatch-1.6.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-09 00:42:31.104753 flytekitplugins-awsbatch-1.6.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-09 00:42:14.000000 flytekitplugins-awsbatch-1.6.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:31.100753 flytekitplugins-awsbatch-1.6.0b4/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:31.104753 flytekitplugins-awsbatch-1.6.0b4/flytekitplugins/awsbatch/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-09 00:42:14.000000 flytekitplugins-awsbatch-1.6.0b4/flytekitplugins/awsbatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-09 00:42:14.000000 flytekitplugins-awsbatch-1.6.0b4/flytekitplugins/awsbatch/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:31.104753 flytekitplugins-awsbatch-1.6.0b4/flytekitplugins_awsbatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-09 00:42:31.000000 flytekitplugins-awsbatch-1.6.0b4/flytekitplugins_awsbatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-09 00:42:31.000000 flytekitplugins-awsbatch-1.6.0b4/flytekitplugins_awsbatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:42:31.000000 flytekitplugins-awsbatch-1.6.0b4/flytekitplugins_awsbatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:31.000000 flytekitplugins-awsbatch-1.6.0b4/flytekitplugins_awsbatch.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 00:42:31.000000 flytekitplugins-awsbatch-1.6.0b4/flytekitplugins_awsbatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:31.000000 flytekitplugins-awsbatch-1.6.0b4/flytekitplugins_awsbatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:42:31.104753 flytekitplugins-awsbatch-1.6.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-09 00:42:30.000000 flytekitplugins-awsbatch-1.6.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:01.255840 flytekitplugins-awsbatch-1.6.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-15 22:07:01.255840 flytekitplugins-awsbatch-1.6.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 22:06:44.000000 flytekitplugins-awsbatch-1.6.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:01.251840 flytekitplugins-awsbatch-1.6.1b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:01.255840 flytekitplugins-awsbatch-1.6.1b0/flytekitplugins/awsbatch/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-15 22:06:44.000000 flytekitplugins-awsbatch-1.6.1b0/flytekitplugins/awsbatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-15 22:06:44.000000 flytekitplugins-awsbatch-1.6.1b0/flytekitplugins/awsbatch/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:01.255840 flytekitplugins-awsbatch-1.6.1b0/flytekitplugins_awsbatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-15 22:07:01.000000 flytekitplugins-awsbatch-1.6.1b0/flytekitplugins_awsbatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-15 22:07:01.000000 flytekitplugins-awsbatch-1.6.1b0/flytekitplugins_awsbatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:07:01.000000 flytekitplugins-awsbatch-1.6.1b0/flytekitplugins_awsbatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:01.000000 flytekitplugins-awsbatch-1.6.1b0/flytekitplugins_awsbatch.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-15 22:07:01.000000 flytekitplugins-awsbatch-1.6.1b0/flytekitplugins_awsbatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:01.000000 flytekitplugins-awsbatch-1.6.1b0/flytekitplugins_awsbatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:07:01.255840 flytekitplugins-awsbatch-1.6.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-15 22:07:00.000000 flytekitplugins-awsbatch-1.6.1b0/setup.py
```

### Comparing `flytekitplugins-awsbatch-1.6.0b4/PKG-INFO` & `flytekitplugins-awsbatch-1.6.1b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-awsbatch
-Version: 1.6.0b4
+Version: 1.6.1b0
 Summary: This package holds the AWS Batch plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-awsbatch-1.6.0b4/flytekitplugins/awsbatch/task.py` & `flytekitplugins-awsbatch-1.6.1b0/flytekitplugins/awsbatch/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-awsbatch-1.6.0b4/flytekitplugins_awsbatch.egg-info/PKG-INFO` & `flytekitplugins-awsbatch-1.6.1b0/flytekitplugins_awsbatch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-awsbatch
-Version: 1.6.0b4
+Version: 1.6.1b0
 Summary: This package holds the AWS Batch plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-awsbatch-1.6.0b4/setup.py` & `flytekitplugins-awsbatch-1.6.1b0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "awsbatch"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0"]
 
-__version__ = "1.6.0b4"
+__version__ = "1.6.1b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the AWS Batch plugins for flytekit",
```
