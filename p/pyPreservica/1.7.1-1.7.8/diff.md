# Comparing `tmp/pyPreservica-1.7.1.tar.gz` & `tmp/pyPreservica-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPreservica-1.7.1.tar", last modified: Wed May  3 11:04:45 2023, max compression
+gzip compressed data, was "pyPreservica-1.7.8.tar", last modified: Tue May 16 13:55:41 2023, max compression
```

## Comparing `pyPreservica-1.7.1.tar` & `pyPreservica-1.7.8.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 11:04:45.537330 pyPreservica-1.7.1/
--rw-rw-rw-   0        0        0    11558 2020-08-17 10:38:19.000000 pyPreservica-1.7.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2581 2023-05-03 11:04:45.536330 pyPreservica-1.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     1602 2022-03-16 17:04:00.000000 pyPreservica-1.7.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 11:04:45.491828 pyPreservica-1.7.1/pyPreservica/
--rw-rw-rw-   0        0        0     1021 2023-05-03 11:03:51.000000 pyPreservica-1.7.1/pyPreservica/__init__.py
--rw-rw-rw-   0        0        0    37685 2023-05-03 10:58:47.000000 pyPreservica-1.7.1/pyPreservica/adminAPI.py
--rw-rw-rw-   0        0        0    32269 2023-05-03 10:51:09.000000 pyPreservica-1.7.1/pyPreservica/common.py
--rw-rw-rw-   0        0        0    16189 2023-03-01 16:04:47.000000 pyPreservica-1.7.1/pyPreservica/contentAPI.py
--rw-rw-rw-   0        0        0   105659 2023-03-01 16:04:03.000000 pyPreservica-1.7.1/pyPreservica/entityAPI.py
--rw-rw-rw-   0        0        0     6260 2023-03-01 16:11:00.000000 pyPreservica-1.7.1/pyPreservica/monitorAPI.py
--rw-rw-rw-   0        0        0     4875 2022-04-21 08:22:10.000000 pyPreservica-1.7.1/pyPreservica/opex.py
--rw-rw-rw-   0        0        0    10522 2021-11-17 14:16:50.000000 pyPreservica-1.7.1/pyPreservica/parAPI.py
--rw-rw-rw-   0        0        0    23541 2023-04-17 14:03:38.000000 pyPreservica-1.7.1/pyPreservica/retentionAPI.py
--rw-rw-rw-   0        0        0    92270 2023-03-21 17:44:59.000000 pyPreservica-1.7.1/pyPreservica/uploadAPI.py
--rw-rw-rw-   0        0        0     2179 2023-05-02 15:51:54.000000 pyPreservica-1.7.1/pyPreservica/webHooksAPI.py
--rw-rw-rw-   0        0        0    17812 2023-03-01 16:08:31.000000 pyPreservica-1.7.1/pyPreservica/workflowAPI.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:04:45.530403 pyPreservica-1.7.1/pyPreservica.egg-info/
--rw-rw-rw-   0        0        0     2581 2023-05-03 11:04:43.000000 pyPreservica-1.7.1/pyPreservica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2023-05-03 11:04:43.000000 pyPreservica-1.7.1/pyPreservica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 11:04:43.000000 pyPreservica-1.7.1/pyPreservica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-05-03 11:04:43.000000 pyPreservica-1.7.1/pyPreservica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-03 11:04:43.000000 pyPreservica-1.7.1/pyPreservica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 11:04:45.540275 pyPreservica-1.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1645 2023-05-03 11:03:51.000000 pyPreservica-1.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:55:41.164294 pyPreservica-1.7.8/
+-rw-rw-rw-   0        0        0    11558 2020-08-17 10:38:19.000000 pyPreservica-1.7.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     2581 2023-05-16 13:55:41.162182 pyPreservica-1.7.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1602 2022-03-16 17:04:00.000000 pyPreservica-1.7.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 13:55:41.111426 pyPreservica-1.7.8/pyPreservica/
+-rw-rw-rw-   0        0        0     1037 2023-05-16 13:21:35.000000 pyPreservica-1.7.8/pyPreservica/__init__.py
+-rw-rw-rw-   0        0        0    37685 2023-05-03 10:58:47.000000 pyPreservica-1.7.8/pyPreservica/adminAPI.py
+-rw-rw-rw-   0        0        0    32269 2023-05-03 10:51:09.000000 pyPreservica-1.7.8/pyPreservica/common.py
+-rw-rw-rw-   0        0        0    16189 2023-03-01 16:04:47.000000 pyPreservica-1.7.8/pyPreservica/contentAPI.py
+-rw-rw-rw-   0        0        0   105659 2023-03-01 16:04:03.000000 pyPreservica-1.7.8/pyPreservica/entityAPI.py
+-rw-rw-rw-   0        0        0     6258 2023-05-16 11:37:54.000000 pyPreservica-1.7.8/pyPreservica/monitorAPI.py
+-rw-rw-rw-   0        0        0     4875 2022-04-21 08:22:10.000000 pyPreservica-1.7.8/pyPreservica/opex.py
+-rw-rw-rw-   0        0        0    10522 2021-11-17 14:16:50.000000 pyPreservica-1.7.8/pyPreservica/parAPI.py
+-rw-rw-rw-   0        0        0    23541 2023-04-17 14:03:38.000000 pyPreservica-1.7.8/pyPreservica/retentionAPI.py
+-rw-rw-rw-   0        0        0    92445 2023-05-16 11:37:54.000000 pyPreservica-1.7.8/pyPreservica/uploadAPI.py
+-rw-rw-rw-   0        0        0       99 2023-05-15 14:18:19.000000 pyPreservica-1.7.8/pyPreservica/vocabularyAPI.py
+-rw-rw-rw-   0        0        0     6383 2023-05-16 13:25:15.000000 pyPreservica-1.7.8/pyPreservica/webHooksAPI.py
+-rw-rw-rw-   0        0        0    17812 2023-03-01 16:08:31.000000 pyPreservica-1.7.8/pyPreservica/workflowAPI.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:55:41.151978 pyPreservica-1.7.8/pyPreservica.egg-info/
+-rw-rw-rw-   0        0        0     2581 2023-05-16 13:55:39.000000 pyPreservica-1.7.8/pyPreservica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-05-16 13:55:39.000000 pyPreservica-1.7.8/pyPreservica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 13:55:39.000000 pyPreservica-1.7.8/pyPreservica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-05-16 13:55:39.000000 pyPreservica-1.7.8/pyPreservica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-16 13:55:39.000000 pyPreservica-1.7.8/pyPreservica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 13:55:41.168356 pyPreservica-1.7.8/setup.cfg
+-rw-rw-rw-   0        0        0     1645 2023-05-16 12:42:45.000000 pyPreservica-1.7.8/setup.py
```

### Comparing `pyPreservica-1.7.1/LICENSE.txt` & `pyPreservica-1.7.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.1/PKG-INFO` & `pyPreservica-1.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservica
-Version: 1.7.1
+Version: 1.7.8
 Summary: Python library for the Preservica API
 Home-page: https://pypreservica.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pypreservica.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica
```

### Comparing `pyPreservica-1.7.1/README.md` & `pyPreservica-1.7.8/README.md`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.1/pyPreservica/__init__.py` & `pyPreservica-1.7.8/pyPreservica/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from .uploadAPI import UploadAPI, simple_asset_package, complex_asset_package, cvs_to_xsd, cvs_to_xml, \
                     cvs_to_cmis_xslt, csv_to_search_xml, generic_asset_package, upload_config, multi_asset_package
 from .workflowAPI import WorkflowAPI, WorkflowContext, WorkflowInstance
 from .retentionAPI import RetentionAPI, RetentionAssignment, RetentionPolicy
 from .parAPI import PreservationActionRegistry
 from .adminAPI import AdminAPI
 from .monitorAPI import MonitorAPI, MonitorCategory, MonitorStatus, MessageStatus
-from .webHooksAPI import WebHooksAPI, TriggerType
+from .webHooksAPI import WebHooksAPI, TriggerType, WebHookHandler
 
 
 __author__ = "James Carr (drjamescarr@gmail.com)"
 
 # Version of the Preservica API package
-__version__ = "1.7.1"
+__version__ = "1.7.8"
 
 __license__ = "Apache License Version 2.0"
```

### Comparing `pyPreservica-1.7.1/pyPreservica/adminAPI.py` & `pyPreservica-1.7.8/pyPreservica/adminAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.1/pyPreservica/common.py` & `pyPreservica-1.7.8/pyPreservica/common.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.1/pyPreservica/contentAPI.py` & `pyPreservica-1.7.8/pyPreservica/contentAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.1/pyPreservica/entityAPI.py` & `pyPreservica-1.7.8/pyPreservica/entityAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.1/pyPreservica/monitorAPI.py` & `pyPreservica-1.7.8/pyPreservica/monitorAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 """
 pyPreservica MonitorAPI module definition
 
 A client library for the Preservica Repository Monitor API
 https://us.preservica.com/api/processmonitor/documentation.html
 
 author:     James Carr
```

### Comparing `pyPreservica-1.7.1/pyPreservica/opex.py` & `pyPreservica-1.7.8/pyPreservica/opex.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.1/pyPreservica/parAPI.py` & `pyPreservica-1.7.8/pyPreservica/parAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.1/pyPreservica/retentionAPI.py` & `pyPreservica-1.7.8/pyPreservica/retentionAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.1/pyPreservica/uploadAPI.py` & `pyPreservica-1.7.8/pyPreservica/uploadAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+"""
+pyPreservica UploadAPI module definition
+
+A client library for the Preservica Repository Upload API
+
+author:     James Carr
+licence:    Apache License 2.0
+
+"""
+
 import csv
 import shutil
 import tempfile
 import uuid
 import xml
 from datetime import datetime
 from time import sleep
```

### Comparing `pyPreservica-1.7.1/pyPreservica/workflowAPI.py` & `pyPreservica-1.7.8/pyPreservica/workflowAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.1/pyPreservica.egg-info/PKG-INFO` & `pyPreservica-1.7.8/pyPreservica.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservica
-Version: 1.7.1
+Version: 1.7.8
 Summary: Python library for the Preservica API
 Home-page: https://pypreservica.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pypreservica.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica
```

### Comparing `pyPreservica-1.7.1/pyPreservica.egg-info/SOURCES.txt` & `pyPreservica-1.7.8/pyPreservica.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 pyPreservica/contentAPI.py
 pyPreservica/entityAPI.py
 pyPreservica/monitorAPI.py
 pyPreservica/opex.py
 pyPreservica/parAPI.py
 pyPreservica/retentionAPI.py
 pyPreservica/uploadAPI.py
+pyPreservica/vocabularyAPI.py
 pyPreservica/webHooksAPI.py
 pyPreservica/workflowAPI.py
 pyPreservica.egg-info/PKG-INFO
 pyPreservica.egg-info/SOURCES.txt
 pyPreservica.egg-info/dependency_links.txt
 pyPreservica.egg-info/requires.txt
 pyPreservica.egg-info/top_level.txt
```

### Comparing `pyPreservica-1.7.1/setup.py` & `pyPreservica-1.7.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     os.system('twine upload dist/*')
     sys.exit()
 
 
 # This call to setup() does all the work
 setup(
     name=PKG,
-    version="1.7.1",
+    version="1.7.8",
     description="Python library for the Preservica API",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://pypreservica.readthedocs.io/",
     author="James Carr",
     author_email="drjamescarr@gmail.com",
     license="Apache License 2.0",
```

