# Comparing `tmp/ddaplib-0.0.2.tar.gz` & `tmp/ddaplib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddaplib-0.0.2.tar", last modified: Thu Feb 16 15:15:08 2023, max compression
+gzip compressed data, was "ddaplib-0.0.3.tar", last modified: Tue May 16 18:09:06 2023, max compression
```

## Comparing `ddaplib-0.0.2.tar` & `ddaplib-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-02-16 15:15:08.640739 ddaplib-0.0.2/
--rw-rw-rw-   0        0        0     1064 2023-02-02 15:59:04.000000 ddaplib-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      857 2023-02-16 15:15:08.638733 ddaplib-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-02-15 19:33:40.000000 ddaplib-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-02-16 15:15:08.622673 ddaplib-0.0.2/ddaplib.egg-info/
--rw-rw-rw-   0        0        0      857 2023-02-16 15:15:07.000000 ddaplib-0.0.2/ddaplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-02-16 15:15:08.000000 ddaplib-0.0.2/ddaplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-16 15:15:07.000000 ddaplib-0.0.2/ddaplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-02-16 15:15:07.000000 ddaplib-0.0.2/ddaplib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-16 15:15:08.633688 ddaplib-0.0.2/platinumtools/
--rw-rw-rw-   0        0        0      256 2023-02-16 14:25:38.000000 ddaplib-0.0.2/platinumtools/__init__.py
--rw-rw-rw-   0        0        0     5600 2023-02-15 19:36:39.000000 ddaplib-0.0.2/platinumtools/dda_constants.py
--rw-rw-rw-   0        0        0       67 2023-02-02 16:15:01.000000 ddaplib-0.0.2/platinumtools/etl_functions.py
--rw-rw-rw-   0        0        0      102 2023-02-15 19:22:28.000000 ddaplib-0.0.2/platinumtools/help.py
--rw-rw-rw-   0        0        0       42 2023-02-16 15:15:08.640739 ddaplib-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      984 2023-02-16 15:14:49.000000 ddaplib-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 18:09:06.610284 ddaplib-0.0.3/
+-rw-rw-rw-   0        0        0     1064 2023-02-02 15:59:04.000000 ddaplib-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      857 2023-05-16 18:09:06.609277 ddaplib-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-02-15 19:33:40.000000 ddaplib-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 18:09:06.576322 ddaplib-0.0.3/ddaplib.egg-info/
+-rw-rw-rw-   0        0        0      857 2023-05-16 18:09:05.000000 ddaplib-0.0.3/ddaplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      621 2023-05-16 18:09:06.000000 ddaplib-0.0.3/ddaplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 18:09:05.000000 ddaplib-0.0.3/ddaplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-05-16 18:09:06.000000 ddaplib-0.0.3/ddaplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 18:09:06.580594 ddaplib-0.0.3/platinumtools/
+-rw-rw-rw-   0        0        0      256 2023-02-16 14:25:38.000000 ddaplib-0.0.3/platinumtools/__init__.py
+-rw-rw-rw-   0        0        0    16832 2023-05-16 16:43:22.000000 ddaplib-0.0.3/platinumtools/dda_constants.py
+-rw-rw-rw-   0        0        0     7993 2023-05-15 19:48:35.000000 ddaplib-0.0.3/platinumtools/dda_models.py
+-rw-rw-rw-   0        0        0       67 2023-02-02 16:15:01.000000 ddaplib-0.0.3/platinumtools/etl_functions.py
+-rw-rw-rw-   0        0        0      102 2023-02-15 19:22:28.000000 ddaplib-0.0.3/platinumtools/help.py
+-rw-rw-rw-   0        0        0       42 2023-05-16 18:09:06.611363 ddaplib-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      984 2023-05-16 18:07:16.000000 ddaplib-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 18:09:06.606822 ddaplib-0.0.3/test_scenarios/
+-rw-rw-rw-   0        0        0     2408 2023-05-16 18:01:42.000000 ddaplib-0.0.3/test_scenarios/JobListener.py
+-rw-rw-rw-   0        0        0      261 2023-02-16 15:22:02.000000 ddaplib-0.0.3/test_scenarios/__init__.py
+-rw-rw-rw-   0        0        0     9421 2023-03-02 14:45:40.000000 ddaplib-0.0.3/test_scenarios/test_adapters.py
+-rw-rw-rw-   0        0        0       38 2023-02-15 19:35:06.000000 ddaplib-0.0.3/test_scenarios/test_code.py
+-rw-rw-rw-   0        0        0     1484 2023-05-16 17:41:51.000000 ddaplib-0.0.3/test_scenarios/test_common_processing.py
+-rw-rw-rw-   0        0        0    26927 2023-05-15 21:07:42.000000 ddaplib-0.0.3/test_scenarios/test_enhancement.py
+-rw-rw-rw-   0        0        0    20223 2023-04-28 17:27:31.000000 ddaplib-0.0.3/test_scenarios/test_event_normalization.py
+-rw-rw-rw-   0        0        0     1785 2023-02-16 19:15:21.000000 ddaplib-0.0.3/test_scenarios/test_guardian.py
+-rw-rw-rw-   0        0        0     4591 2023-03-01 19:46:11.000000 ddaplib-0.0.3/test_scenarios/test_helpers.py
+-rw-rw-rw-   0        0        0     5399 2023-03-01 19:46:11.000000 ddaplib-0.0.3/test_scenarios/test_scheduling.py
```

### Comparing `ddaplib-0.0.2/LICENSE` & `ddaplib-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ddaplib-0.0.2/PKG-INFO` & `ddaplib-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddaplib
-Version: 0.0.2
+Version: 0.0.3
 Summary: DDAPP Modules
 Author: Anon Dev
 License: UNKNOWN
 Keywords: python,utilities
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `ddaplib-0.0.2/ddaplib.egg-info/PKG-INFO` & `ddaplib-0.0.3/ddaplib.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddaplib
-Version: 0.0.2
+Version: 0.0.3
 Summary: DDAPP Modules
 Author: Anon Dev
 License: UNKNOWN
 Keywords: python,utilities
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `ddaplib-0.0.2/setup.py` & `ddaplib-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'DDAPP Modules'
 LONG_DESCRIPTION = 'Common Constants, classes and methods for ETL and other python projects'
 
 # Setting up
 #nenewang08
 setup(
     name="ddaplib",
```

