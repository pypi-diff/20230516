# Comparing `tmp/platinumtools-0.0.4.tar.gz` & `tmp/platinumtools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platinumtools-0.0.4.tar", last modified: Tue May 16 18:18:17 2023, max compression
+gzip compressed data, was "platinumtools-0.0.5.tar", last modified: Tue May 16 18:19:16 2023, max compression
```

## Comparing `platinumtools-0.0.4.tar` & `platinumtools-0.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 18:18:17.936700 platinumtools-0.0.4/
--rw-rw-rw-   0        0        0     1064 2023-02-02 15:59:04.000000 platinumtools-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      863 2023-05-16 18:18:17.934156 platinumtools-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-02-15 19:33:40.000000 platinumtools-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 18:18:17.849920 platinumtools-0.0.4/platinumtools/
--rw-rw-rw-   0        0        0      424 2023-05-16 18:13:07.000000 platinumtools-0.0.4/platinumtools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 18:18:17.903665 platinumtools-0.0.4/platinumtools/aws_classes/
--rw-rw-rw-   0        0        0     1246 2023-05-16 15:56:00.000000 platinumtools-0.0.4/platinumtools/aws_classes/CommonProcesor.py
--rw-rw-rw-   0        0        0     2408 2023-05-16 18:16:53.000000 platinumtools-0.0.4/platinumtools/aws_classes/JobListener.py
--rw-rw-rw-   0        0        0       25 2023-05-16 18:12:38.000000 platinumtools-0.0.4/platinumtools/aws_classes/__init__.py
--rw-rw-rw-   0        0        0     2189 2023-04-28 16:22:33.000000 platinumtools-0.0.4/platinumtools/aws_classes/class_adapters.py
--rw-rw-rw-   0        0        0    28212 2023-05-16 17:43:48.000000 platinumtools-0.0.4/platinumtools/aws_classes/class_enhancement.py
--rw-rw-rw-   0        0        0     2296 2023-02-16 19:18:53.000000 platinumtools-0.0.4/platinumtools/aws_classes/class_guardian.py
--rw-rw-rw-   0        0        0    17917 2023-05-16 17:09:26.000000 platinumtools-0.0.4/platinumtools/aws_classes/class_helpers.py
--rw-rw-rw-   0        0        0     1789 2023-02-21 20:05:33.000000 platinumtools-0.0.4/platinumtools/aws_classes/class_scheduling.py
--rw-rw-rw-   0        0        0     7102 2023-05-15 19:54:00.000000 platinumtools-0.0.4/platinumtools/aws_classes/config_mapper.py
--rw-rw-rw-   0        0        0    19338 2023-05-15 20:14:06.000000 platinumtools-0.0.4/platinumtools/aws_classes/config_mapper_df.py
--rw-rw-rw-   0        0        0     1484 2023-05-16 17:41:51.000000 platinumtools-0.0.4/platinumtools/aws_classes/test_common_processing.py
--rw-rw-rw-   0        0        0    16832 2023-05-16 16:43:22.000000 platinumtools-0.0.4/platinumtools/dda_constants.py
--rw-rw-rw-   0        0        0     7993 2023-05-15 19:48:35.000000 platinumtools-0.0.4/platinumtools/dda_models.py
--rw-rw-rw-   0        0        0       67 2023-02-02 16:15:01.000000 platinumtools-0.0.4/platinumtools/etl_functions.py
--rw-rw-rw-   0        0        0      102 2023-02-15 19:22:28.000000 platinumtools-0.0.4/platinumtools/help.py
-drwxrwxrwx   0        0        0        0 2023-05-16 18:18:17.864478 platinumtools-0.0.4/platinumtools.egg-info/
--rw-rw-rw-   0        0        0      863 2023-05-16 18:18:17.000000 platinumtools-0.0.4/platinumtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1133 2023-05-16 18:18:17.000000 platinumtools-0.0.4/platinumtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 18:18:17.000000 platinumtools-0.0.4/platinumtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-05-16 18:18:17.000000 platinumtools-0.0.4/platinumtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 18:18:17.937704 platinumtools-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      990 2023-05-16 18:17:24.000000 platinumtools-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 18:18:17.925474 platinumtools-0.0.4/test_scenarios/
--rw-rw-rw-   0        0        0     2408 2023-05-16 18:01:42.000000 platinumtools-0.0.4/test_scenarios/JobListener.py
--rw-rw-rw-   0        0        0      261 2023-02-16 15:22:02.000000 platinumtools-0.0.4/test_scenarios/__init__.py
--rw-rw-rw-   0        0        0     9421 2023-03-02 14:45:40.000000 platinumtools-0.0.4/test_scenarios/test_adapters.py
--rw-rw-rw-   0        0        0       38 2023-02-15 19:35:06.000000 platinumtools-0.0.4/test_scenarios/test_code.py
--rw-rw-rw-   0        0        0     1484 2023-05-16 18:14:36.000000 platinumtools-0.0.4/test_scenarios/test_common_processing.py
--rw-rw-rw-   0        0        0    26927 2023-05-15 21:07:42.000000 platinumtools-0.0.4/test_scenarios/test_enhancement.py
--rw-rw-rw-   0        0        0    20223 2023-04-28 17:27:31.000000 platinumtools-0.0.4/test_scenarios/test_event_normalization.py
--rw-rw-rw-   0        0        0     1785 2023-02-16 19:15:21.000000 platinumtools-0.0.4/test_scenarios/test_guardian.py
--rw-rw-rw-   0        0        0     4591 2023-03-01 19:46:11.000000 platinumtools-0.0.4/test_scenarios/test_helpers.py
--rw-rw-rw-   0        0        0     5399 2023-03-01 19:46:11.000000 platinumtools-0.0.4/test_scenarios/test_scheduling.py
+drwxrwxrwx   0        0        0        0 2023-05-16 18:19:16.139622 platinumtools-0.0.5/
+-rw-rw-rw-   0        0        0     1064 2023-02-02 15:59:04.000000 platinumtools-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      863 2023-05-16 18:19:16.138604 platinumtools-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-02-15 19:33:40.000000 platinumtools-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 18:19:16.047841 platinumtools-0.0.5/platinumtools/
+-rw-rw-rw-   0        0        0      424 2023-05-16 18:13:07.000000 platinumtools-0.0.5/platinumtools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 18:19:16.085195 platinumtools-0.0.5/platinumtools/aws_classes/
+-rw-rw-rw-   0        0        0     1246 2023-05-16 15:56:00.000000 platinumtools-0.0.5/platinumtools/aws_classes/CommonProcesor.py
+-rw-rw-rw-   0        0        0     2408 2023-05-16 18:16:53.000000 platinumtools-0.0.5/platinumtools/aws_classes/JobListener.py
+-rw-rw-rw-   0        0        0       25 2023-05-16 18:12:38.000000 platinumtools-0.0.5/platinumtools/aws_classes/__init__.py
+-rw-rw-rw-   0        0        0     2189 2023-04-28 16:22:33.000000 platinumtools-0.0.5/platinumtools/aws_classes/class_adapters.py
+-rw-rw-rw-   0        0        0    28212 2023-05-16 17:43:48.000000 platinumtools-0.0.5/platinumtools/aws_classes/class_enhancement.py
+-rw-rw-rw-   0        0        0     2296 2023-02-16 19:18:53.000000 platinumtools-0.0.5/platinumtools/aws_classes/class_guardian.py
+-rw-rw-rw-   0        0        0    17917 2023-05-16 17:09:26.000000 platinumtools-0.0.5/platinumtools/aws_classes/class_helpers.py
+-rw-rw-rw-   0        0        0     1789 2023-02-21 20:05:33.000000 platinumtools-0.0.5/platinumtools/aws_classes/class_scheduling.py
+-rw-rw-rw-   0        0        0     7102 2023-05-15 19:54:00.000000 platinumtools-0.0.5/platinumtools/aws_classes/config_mapper.py
+-rw-rw-rw-   0        0        0    19338 2023-05-15 20:14:06.000000 platinumtools-0.0.5/platinumtools/aws_classes/config_mapper_df.py
+-rw-rw-rw-   0        0        0     1484 2023-05-16 17:41:51.000000 platinumtools-0.0.5/platinumtools/aws_classes/test_common_processing.py
+-rw-rw-rw-   0        0        0    16832 2023-05-16 16:43:22.000000 platinumtools-0.0.5/platinumtools/dda_constants.py
+-rw-rw-rw-   0        0        0     7993 2023-05-15 19:48:35.000000 platinumtools-0.0.5/platinumtools/dda_models.py
+-rw-rw-rw-   0        0        0       67 2023-02-02 16:15:01.000000 platinumtools-0.0.5/platinumtools/etl_functions.py
+-rw-rw-rw-   0        0        0      102 2023-02-15 19:22:28.000000 platinumtools-0.0.5/platinumtools/help.py
+drwxrwxrwx   0        0        0        0 2023-05-16 18:19:16.057123 platinumtools-0.0.5/platinumtools.egg-info/
+-rw-rw-rw-   0        0        0      863 2023-05-16 18:19:15.000000 platinumtools-0.0.5/platinumtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1133 2023-05-16 18:19:15.000000 platinumtools-0.0.5/platinumtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 18:19:15.000000 platinumtools-0.0.5/platinumtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-05-16 18:19:15.000000 platinumtools-0.0.5/platinumtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 18:19:16.141840 platinumtools-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      990 2023-05-16 18:18:44.000000 platinumtools-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 18:19:16.135847 platinumtools-0.0.5/test_scenarios/
+-rw-rw-rw-   0        0        0     2408 2023-05-16 18:01:42.000000 platinumtools-0.0.5/test_scenarios/JobListener.py
+-rw-rw-rw-   0        0        0      261 2023-02-16 15:22:02.000000 platinumtools-0.0.5/test_scenarios/__init__.py
+-rw-rw-rw-   0        0        0     9421 2023-03-02 14:45:40.000000 platinumtools-0.0.5/test_scenarios/test_adapters.py
+-rw-rw-rw-   0        0        0       38 2023-02-15 19:35:06.000000 platinumtools-0.0.5/test_scenarios/test_code.py
+-rw-rw-rw-   0        0        0     1484 2023-05-16 18:14:36.000000 platinumtools-0.0.5/test_scenarios/test_common_processing.py
+-rw-rw-rw-   0        0        0    26927 2023-05-15 21:07:42.000000 platinumtools-0.0.5/test_scenarios/test_enhancement.py
+-rw-rw-rw-   0        0        0    20223 2023-04-28 17:27:31.000000 platinumtools-0.0.5/test_scenarios/test_event_normalization.py
+-rw-rw-rw-   0        0        0     1785 2023-02-16 19:15:21.000000 platinumtools-0.0.5/test_scenarios/test_guardian.py
+-rw-rw-rw-   0        0        0     4591 2023-03-01 19:46:11.000000 platinumtools-0.0.5/test_scenarios/test_helpers.py
+-rw-rw-rw-   0        0        0     5399 2023-03-01 19:46:11.000000 platinumtools-0.0.5/test_scenarios/test_scheduling.py
```

### Comparing `platinumtools-0.0.4/LICENSE` & `platinumtools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `platinumtools-0.0.4/PKG-INFO` & `platinumtools-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platinumtools
-Version: 0.0.4
+Version: 0.0.5
 Summary: DDAPP Modules
 Author: Anon Dev
 License: UNKNOWN
 Keywords: python,utilities
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `platinumtools-0.0.4/platinumtools/aws_classes/CommonProcesor.py` & `platinumtools-0.0.5/platinumtools/aws_classes/CommonProcesor.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.0.4/platinumtools/aws_classes/JobListener.py` & `platinumtools-0.0.5/platinumtools/aws_classes/JobListener.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.0.4/platinumtools/aws_classes/class_adapters.py` & `platinumtools-0.0.5/platinumtools/aws_classes/class_adapters.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.0.4/platinumtools/aws_classes/class_enhancement.py` & `platinumtools-0.0.5/platinumtools/aws_classes/class_enhancement.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.0.4/platinumtools/aws_classes/class_guardian.py` & `platinumtools-0.0.5/platinumtools/aws_classes/class_guardian.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.0.4/platinumtools/aws_classes/class_helpers.py` & `platinumtools-0.0.5/platinumtools/aws_classes/class_helpers.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.0.4/platinumtools/aws_classes/class_scheduling.py` & `platinumtools-0.0.5/platinumtools/aws_classes/class_scheduling.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.0.4/platinumtools/aws_classes/config_mapper.py` & `platinumtools-0.0.5/platinumtools/aws_classes/config_mapper.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.0.4/platinumtools/aws_classes/config_mapper_df.py` & `platinumtools-0.0.5/platinumtools/aws_classes/config_mapper_df.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.0.4/platinumtools/aws_classes/test_common_processing.py` & `platinumtools-0.0.5/platinumtools/aws_classes/test_common_processing.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.0.4/platinumtools/dda_constants.py` & `platinumtools-0.0.5/platinumtools/dda_constants.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.0.4/platinumtools/dda_models.py` & `platinumtools-0.0.5/platinumtools/dda_models.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.0.4/platinumtools.egg-info/PKG-INFO` & `platinumtools-0.0.5/platinumtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platinumtools
-Version: 0.0.4
+Version: 0.0.5
 Summary: DDAPP Modules
 Author: Anon Dev
 License: UNKNOWN
 Keywords: python,utilities
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `platinumtools-0.0.4/platinumtools.egg-info/SOURCES.txt` & `platinumtools-0.0.5/platinumtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `platinumtools-0.0.4/setup.py` & `platinumtools-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'DDAPP Modules'
 LONG_DESCRIPTION = 'Common Constants, classes and methods for ETL and other python projects'
 
 # Setting up
 #nenewang08
 setup(
     name="platinumtools",
```

### Comparing `platinumtools-0.0.4/test_scenarios/JobListener.py` & `platinumtools-0.0.5/test_scenarios/JobListener.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.0.4/test_scenarios/test_adapters.py` & `platinumtools-0.0.5/test_scenarios/test_adapters.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.0.4/test_scenarios/test_common_processing.py` & `platinumtools-0.0.5/test_scenarios/test_common_processing.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.0.4/test_scenarios/test_enhancement.py` & `platinumtools-0.0.5/test_scenarios/test_enhancement.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.0.4/test_scenarios/test_event_normalization.py` & `platinumtools-0.0.5/test_scenarios/test_event_normalization.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.0.4/test_scenarios/test_guardian.py` & `platinumtools-0.0.5/test_scenarios/test_guardian.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.0.4/test_scenarios/test_helpers.py` & `platinumtools-0.0.5/test_scenarios/test_helpers.py`

 * *Files identical despite different names*

### Comparing `platinumtools-0.0.4/test_scenarios/test_scheduling.py` & `platinumtools-0.0.5/test_scenarios/test_scheduling.py`

 * *Files identical despite different names*

