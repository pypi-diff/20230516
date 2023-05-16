# Comparing `tmp/platinumtools-0.0.2.tar.gz` & `tmp/platinumtools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platinumtools-0.0.2.tar", last modified: Wed Feb 15 19:17:30 2023, max compression
+gzip compressed data, was "platinumtools-0.0.3.tar", last modified: Tue May 16 18:09:56 2023, max compression
```

## Comparing `platinumtools-0.0.2.tar` & `platinumtools-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 19:17:30.241845 platinumtools-0.0.2/
--rw-rw-rw-   0        0        0     1064 2023-02-02 15:59:04.000000 platinumtools-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      706 2023-02-15 19:17:30.240847 platinumtools-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      119 2023-02-15 19:11:07.000000 platinumtools-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-02-15 19:17:30.226958 platinumtools-0.0.2/platinumtools/
--rw-rw-rw-   0        0        0      282 2023-02-02 16:09:02.000000 platinumtools-0.0.2/platinumtools/__init__.py
--rw-rw-rw-   0        0        0     5600 2023-02-02 16:08:54.000000 platinumtools-0.0.2/platinumtools/dda_constants.py
--rw-rw-rw-   0        0        0       67 2023-02-02 16:15:01.000000 platinumtools-0.0.2/platinumtools/etl_functions.py
--rw-rw-rw-   0        0        0      115 2023-02-02 15:59:04.000000 platinumtools-0.0.2/platinumtools/hello.py
--rw-rw-rw-   0        0        0    14643 2023-02-02 15:59:04.000000 platinumtools-0.0.2/platinumtools/streaming.py
-drwxrwxrwx   0        0        0        0 2023-02-15 19:17:30.238841 platinumtools-0.0.2/platinumtools.egg-info/
--rw-rw-rw-   0        0        0      706 2023-02-15 19:17:29.000000 platinumtools-0.0.2/platinumtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-02-15 19:17:30.000000 platinumtools-0.0.2/platinumtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 19:17:29.000000 platinumtools-0.0.2/platinumtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-02-15 19:17:29.000000 platinumtools-0.0.2/platinumtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-15 19:17:30.242840 platinumtools-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1040 2023-02-15 19:16:10.000000 platinumtools-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 18:09:56.704541 platinumtools-0.0.3/
+-rw-rw-rw-   0        0        0     1064 2023-02-02 15:59:04.000000 platinumtools-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      863 2023-05-16 18:09:56.703539 platinumtools-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-02-15 19:33:40.000000 platinumtools-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 18:09:56.647661 platinumtools-0.0.3/platinumtools/
+-rw-rw-rw-   0        0        0      256 2023-02-16 14:25:38.000000 platinumtools-0.0.3/platinumtools/__init__.py
+-rw-rw-rw-   0        0        0    16832 2023-05-16 16:43:22.000000 platinumtools-0.0.3/platinumtools/dda_constants.py
+-rw-rw-rw-   0        0        0     7993 2023-05-15 19:48:35.000000 platinumtools-0.0.3/platinumtools/dda_models.py
+-rw-rw-rw-   0        0        0       67 2023-02-02 16:15:01.000000 platinumtools-0.0.3/platinumtools/etl_functions.py
+-rw-rw-rw-   0        0        0      102 2023-02-15 19:22:28.000000 platinumtools-0.0.3/platinumtools/help.py
+drwxrwxrwx   0        0        0        0 2023-05-16 18:09:56.677857 platinumtools-0.0.3/platinumtools.egg-info/
+-rw-rw-rw-   0        0        0      863 2023-05-16 18:09:55.000000 platinumtools-0.0.3/platinumtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      645 2023-05-16 18:09:56.000000 platinumtools-0.0.3/platinumtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 18:09:55.000000 platinumtools-0.0.3/platinumtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-05-16 18:09:56.000000 platinumtools-0.0.3/platinumtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 18:09:56.705596 platinumtools-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      990 2023-05-16 18:09:49.000000 platinumtools-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 18:09:56.700536 platinumtools-0.0.3/test_scenarios/
+-rw-rw-rw-   0        0        0     2408 2023-05-16 18:01:42.000000 platinumtools-0.0.3/test_scenarios/JobListener.py
+-rw-rw-rw-   0        0        0      261 2023-02-16 15:22:02.000000 platinumtools-0.0.3/test_scenarios/__init__.py
+-rw-rw-rw-   0        0        0     9421 2023-03-02 14:45:40.000000 platinumtools-0.0.3/test_scenarios/test_adapters.py
+-rw-rw-rw-   0        0        0       38 2023-02-15 19:35:06.000000 platinumtools-0.0.3/test_scenarios/test_code.py
+-rw-rw-rw-   0        0        0     1484 2023-05-16 17:41:51.000000 platinumtools-0.0.3/test_scenarios/test_common_processing.py
+-rw-rw-rw-   0        0        0    26927 2023-05-15 21:07:42.000000 platinumtools-0.0.3/test_scenarios/test_enhancement.py
+-rw-rw-rw-   0        0        0    20223 2023-04-28 17:27:31.000000 platinumtools-0.0.3/test_scenarios/test_event_normalization.py
+-rw-rw-rw-   0        0        0     1785 2023-02-16 19:15:21.000000 platinumtools-0.0.3/test_scenarios/test_guardian.py
+-rw-rw-rw-   0        0        0     4591 2023-03-01 19:46:11.000000 platinumtools-0.0.3/test_scenarios/test_helpers.py
+-rw-rw-rw-   0        0        0     5399 2023-03-01 19:46:11.000000 platinumtools-0.0.3/test_scenarios/test_scheduling.py
```

### Comparing `platinumtools-0.0.2/LICENSE` & `platinumtools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `platinumtools-0.0.2/setup.py` & `platinumtools-0.0.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
-DESCRIPTION = 'Core Platinum Components'
+VERSION = '0.0.3'
+DESCRIPTION = 'DDAPP Modules'
 LONG_DESCRIPTION = 'Common Constants, classes and methods for ETL and other python projects'
 
 # Setting up
+#nenewang08
 setup(
     name="platinumtools",
     version=VERSION,
-    author="Nelson Wang",
-    author_email="<nwang@platinumfilings.com>",
+    author="Anon Dev",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=[],
     keywords=['python', 'utilities'],
     classifiers=[
```

