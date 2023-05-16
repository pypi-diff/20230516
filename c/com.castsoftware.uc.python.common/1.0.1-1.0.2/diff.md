# Comparing `tmp/com.castsoftware.uc.python.common-1.0.1.tar.gz` & `tmp/com.castsoftware.uc.python.common-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.python.common-1.0.1.tar", last modified: Mon May 15 20:35:58 2023, max compression
+gzip compressed data, was "com.castsoftware.uc.python.common-1.0.2.tar", last modified: Tue May 16 01:56:27 2023, max compression
```

## Comparing `com.castsoftware.uc.python.common-1.0.1.tar` & `com.castsoftware.uc.python.common-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 20:35:58.180499 com.castsoftware.uc.python.common-1.0.1/
--rw-rw-rw-   0        0        0    35823 2021-04-05 17:40:19.000000 com.castsoftware.uc.python.common-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      712 2023-05-15 20:35:58.171457 com.castsoftware.uc.python.common-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      103 2021-06-01 15:37:40.000000 com.castsoftware.uc.python.common-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 20:35:58.086056 com.castsoftware.uc.python.common-1.0.1/cast_common/
--rw-rw-rw-   0        0        0     2036 2023-05-15 13:45:17.000000 com.castsoftware.uc.python.common-1.0.1/cast_common/abstractClass.py
--rw-rw-rw-   0        0        0    11799 2023-05-15 13:45:17.000000 com.castsoftware.uc.python.common-1.0.1/cast_common/aipRestCall.py
--rw-rw-rw-   0        0        0     5466 2023-05-15 14:43:46.000000 com.castsoftware.uc.python.common-1.0.1/cast_common/hlRestCall.py
--rw-rw-rw-   0        0        0     1688 2023-05-15 16:57:58.000000 com.castsoftware.uc.python.common-1.0.1/cast_common/logger.py
--rw-rw-rw-   0        0        0     3811 2023-05-15 13:45:17.000000 com.castsoftware.uc.python.common-1.0.1/cast_common/restAPI.py
--rw-rw-rw-   0        0        0     6957 2023-05-15 14:43:46.000000 com.castsoftware.uc.python.common-1.0.1/cast_common/util.py
-drwxrwxrwx   0        0        0        0 2023-05-15 20:35:58.155969 com.castsoftware.uc.python.common-1.0.1/com.castsoftware.uc.python.common.egg-info/
--rw-rw-rw-   0        0        0      712 2023-05-15 20:35:57.000000 com.castsoftware.uc.python.common-1.0.1/com.castsoftware.uc.python.common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2023-05-15 20:35:57.000000 com.castsoftware.uc.python.common-1.0.1/com.castsoftware.uc.python.common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 20:35:57.000000 com.castsoftware.uc.python.common-1.0.1/com.castsoftware.uc.python.common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-15 20:35:57.000000 com.castsoftware.uc.python.common-1.0.1/com.castsoftware.uc.python.common.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-15 20:35:57.000000 com.castsoftware.uc.python.common-1.0.1/com.castsoftware.uc.python.common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      628 2023-05-15 20:35:23.000000 com.castsoftware.uc.python.common-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-15 20:35:58.181511 com.castsoftware.uc.python.common-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 01:56:27.314836 com.castsoftware.uc.python.common-1.0.2/
+-rw-rw-rw-   0        0        0    35823 2021-04-05 17:40:19.000000 com.castsoftware.uc.python.common-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      712 2023-05-16 01:56:27.305525 com.castsoftware.uc.python.common-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2021-06-01 15:37:40.000000 com.castsoftware.uc.python.common-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 01:56:27.215071 com.castsoftware.uc.python.common-1.0.2/cast_common/
+-rw-rw-rw-   0        0        0     2036 2023-05-15 13:45:17.000000 com.castsoftware.uc.python.common-1.0.2/cast_common/abstractClass.py
+-rw-rw-rw-   0        0        0    11799 2023-05-15 13:45:17.000000 com.castsoftware.uc.python.common-1.0.2/cast_common/aipRestCall.py
+-rw-rw-rw-   0        0        0     5466 2023-05-15 14:43:46.000000 com.castsoftware.uc.python.common-1.0.2/cast_common/hlRestCall.py
+-rw-rw-rw-   0        0        0     1688 2023-05-15 16:57:58.000000 com.castsoftware.uc.python.common-1.0.2/cast_common/logger.py
+-rw-rw-rw-   0        0        0     3811 2023-05-15 13:45:17.000000 com.castsoftware.uc.python.common-1.0.2/cast_common/restAPI.py
+-rw-rw-rw-   0        0        0     6930 2023-05-16 01:55:48.000000 com.castsoftware.uc.python.common-1.0.2/cast_common/util.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:56:27.286493 com.castsoftware.uc.python.common-1.0.2/com.castsoftware.uc.python.common.egg-info/
+-rw-rw-rw-   0        0        0      712 2023-05-16 01:56:26.000000 com.castsoftware.uc.python.common-1.0.2/com.castsoftware.uc.python.common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-05-16 01:56:27.000000 com.castsoftware.uc.python.common-1.0.2/com.castsoftware.uc.python.common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 01:56:26.000000 com.castsoftware.uc.python.common-1.0.2/com.castsoftware.uc.python.common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-16 01:56:26.000000 com.castsoftware.uc.python.common-1.0.2/com.castsoftware.uc.python.common.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-16 01:56:27.000000 com.castsoftware.uc.python.common-1.0.2/com.castsoftware.uc.python.common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      628 2023-05-16 01:56:03.000000 com.castsoftware.uc.python.common-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 01:56:27.315960 com.castsoftware.uc.python.common-1.0.2/setup.cfg
```

### Comparing `com.castsoftware.uc.python.common-1.0.1/LICENSE` & `com.castsoftware.uc.python.common-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.1/PKG-INFO` & `com.castsoftware.uc.python.common-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.python.common
-Version: 1.0.1
+Version: 1.0.2
 Summary: A set of common classes and methods for use with python projects
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.python.common
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.python.common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `com.castsoftware.uc.python.common-1.0.1/cast_common/abstractClass.py` & `com.castsoftware.uc.python.common-1.0.2/cast_common/abstractClass.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.1/cast_common/aipRestCall.py` & `com.castsoftware.uc.python.common-1.0.2/cast_common/aipRestCall.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.1/cast_common/hlRestCall.py` & `com.castsoftware.uc.python.common-1.0.2/cast_common/hlRestCall.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.1/cast_common/logger.py` & `com.castsoftware.uc.python.common-1.0.2/cast_common/logger.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.1/cast_common/restAPI.py` & `com.castsoftware.uc.python.common-1.0.2/cast_common/restAPI.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.1/cast_common/util.py` & `com.castsoftware.uc.python.common-1.0.2/cast_common/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from pandas import DataFrame,json_normalize,concat,ExcelWriter
 from os import mkdir
 from os.path import exists,abspath,join
 from subprocess import Popen,PIPE,STDOUT
-from logger import Logger
 import sys
 
 
 def get_between(txt,tag_start,tag_end,start_at=0):
     text = txt[start_at:]
     
     start = text[start_at:].find(f"{tag_start}")+len(f"{tag_start}")
```

### Comparing `com.castsoftware.uc.python.common-1.0.1/com.castsoftware.uc.python.common.egg-info/PKG-INFO` & `com.castsoftware.uc.python.common-1.0.2/com.castsoftware.uc.python.common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.python.common
-Version: 1.0.1
+Version: 1.0.2
 Summary: A set of common classes and methods for use with python projects
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.python.common
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.python.common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `com.castsoftware.uc.python.common-1.0.1/pyproject.toml` & `com.castsoftware.uc.python.common-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name='com.castsoftware.uc.python.common'
 description="A set of common classes and methods for use with python projects"
 
-version='1.0.1' #prod version
+version='1.0.2' #prod version
 
 dependencies = ['pandas','requests']
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
```

