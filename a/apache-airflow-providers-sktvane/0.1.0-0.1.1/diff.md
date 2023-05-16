# Comparing `tmp/apache-airflow-providers-sktvane-0.1.0.tar.gz` & `tmp/apache-airflow-providers-sktvane-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-sktvane-0.1.0.tar", last modified: Mon May 15 08:28:13 2023, max compression
+gzip compressed data, was "apache-airflow-providers-sktvane-0.1.1.tar", last modified: Tue May 16 01:18:04 2023, max compression
```

## Comparing `apache-airflow-providers-sktvane-0.1.0.tar` & `apache-airflow-providers-sktvane-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:13.973227 apache-airflow-providers-sktvane-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-15 08:28:13.973227 apache-airflow-providers-sktvane-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:13.969227 apache-airflow-providers-sktvane-0.1.0/airflow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:13.969227 apache-airflow-providers-sktvane-0.1.0/airflow/providers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:13.969227 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:13.973227 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/macros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/macros/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/macros/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/macros/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/macros/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:13.973227 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/operators/nes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:13.973227 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/sensors/gcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:13.973227 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:28:13.973227 apache-airflow-providers-sktvane-0.1.0/apache_airflow_providers_sktvane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-15 08:28:13.000000 apache-airflow-providers-sktvane-0.1.0/apache_airflow_providers_sktvane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-15 08:28:13.000000 apache-airflow-providers-sktvane-0.1.0/apache_airflow_providers_sktvane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 08:28:13.000000 apache-airflow-providers-sktvane-0.1.0/apache_airflow_providers_sktvane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-15 08:28:13.000000 apache-airflow-providers-sktvane-0.1.0/apache_airflow_providers_sktvane.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 08:28:13.000000 apache-airflow-providers-sktvane-0.1.0/apache_airflow_providers_sktvane.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-15 08:28:13.977227 apache-airflow-providers-sktvane-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-15 08:28:07.000000 apache-airflow-providers-sktvane-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:04.431607 apache-airflow-providers-sktvane-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-16 01:18:04.431607 apache-airflow-providers-sktvane-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:04.423607 apache-airflow-providers-sktvane-0.1.1/airflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:04.423607 apache-airflow-providers-sktvane-0.1.1/airflow/providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:04.423607 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:04.427607 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/macros/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/macros/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/macros/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/macros/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:04.427607 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/operators/nes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:04.427607 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/sensors/gcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:04.427607 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:18:04.431607 apache-airflow-providers-sktvane-0.1.1/apache_airflow_providers_sktvane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-16 01:18:04.000000 apache-airflow-providers-sktvane-0.1.1/apache_airflow_providers_sktvane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-16 01:18:04.000000 apache-airflow-providers-sktvane-0.1.1/apache_airflow_providers_sktvane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 01:18:04.000000 apache-airflow-providers-sktvane-0.1.1/apache_airflow_providers_sktvane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 01:18:04.000000 apache-airflow-providers-sktvane-0.1.1/apache_airflow_providers_sktvane.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 01:18:04.000000 apache-airflow-providers-sktvane-0.1.1/apache_airflow_providers_sktvane.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 01:18:04.431607 apache-airflow-providers-sktvane-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-16 01:17:58.000000 apache-airflow-providers-sktvane-0.1.1/setup.py
```

### Comparing `apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/macros/date.py` & `apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/macros/date.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/macros/gcp.py` & `apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/macros/gcp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/macros/slack.py` & `apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/macros/slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/operators/nes.py` & `apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/operators/nes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.0/airflow/providers/sktvane/sensors/gcp.py` & `apache-airflow-providers-sktvane-0.1.1/airflow/providers/sktvane/sensors/gcp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.0/apache_airflow_providers_sktvane.egg-info/SOURCES.txt` & `apache-airflow-providers-sktvane-0.1.1/apache_airflow_providers_sktvane.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.1.0/setup.py` & `apache-airflow-providers-sktvane-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="apache-airflow-providers-sktvane",
-    version="0.1.0",
+    version="0.1.1",
     author="aidp",
     author_email="aidp@sktai.io",
     description="Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["airflow", "sktvane"],
     license="MIT",
```

