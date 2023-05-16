# Comparing `tmp/drb-metadata-1.1.2.tar.gz` & `tmp/drb-metadata-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-metadata-1.1.2.tar", last modified: Thu Mar  9 15:06:04 2023, max compression
+gzip compressed data, was "drb-metadata-1.2.0.tar", last modified: Tue May 16 14:07:26 2023, max compression
```

## Comparing `drb-metadata-1.1.2.tar` & `drb-metadata-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 15:06:04.578428 drb-metadata-1.1.2/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-18 13:36:15.000000 drb-metadata-1.1.2/LICENCE.txt
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-01-03 12:49:37.000000 drb-metadata-1.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1818 2023-03-09 15:06:04.578428 drb-metadata-1.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1400 2023-02-01 15:59:39.000000 drb-metadata-1.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 15:06:04.570428 drb-metadata-1.1.2/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 15:06:04.582428 drb-metadata-1.1.2/drb/metadata/
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-01-03 14:11:31.000000 drb-metadata-1.1.2/drb/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-03-09 15:06:04.582428 drb-metadata-1.1.2/drb/metadata/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     5280 2023-02-02 14:24:12.000000 drb-metadata-1.1.2/drb/metadata/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)      759 2023-02-01 15:59:39.000000 drb-metadata-1.1.2/drb/metadata/schema.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 15:06:04.578428 drb-metadata-1.1.2/drb_metadata.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1818 2023-03-09 15:06:04.000000 drb-metadata-1.1.2/drb_metadata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      434 2023-03-09 15:06:04.000000 drb-metadata-1.1.2/drb_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-09 15:06:04.000000 drb-metadata-1.1.2/drb_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-09 15:06:04.000000 drb-metadata-1.1.2/drb_metadata.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       50 2023-03-09 15:06:04.000000 drb-metadata-1.1.2/drb_metadata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-09 15:06:04.000000 drb-metadata-1.1.2/drb_metadata.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-02-01 15:59:39.000000 drb-metadata-1.1.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-02-02 14:06:36.000000 drb-metadata-1.1.2/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-03-09 15:06:04.582428 drb-metadata-1.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-02-01 15:59:39.000000 drb-metadata-1.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 15:06:04.578428 drb-metadata-1.1.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-01-03 12:49:37.000000 drb-metadata-1.1.2/tests/test_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    81180 2022-06-08 11:25:56.000000 drb-metadata-1.1.2/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:07:26.701710 drb-metadata-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-05-16 13:05:50.000000 drb-metadata-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-05-16 13:05:50.000000 drb-metadata-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-05-16 14:07:26.701710 drb-metadata-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1400 2023-05-16 13:05:50.000000 drb-metadata-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:07:26.685710 drb-metadata-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:07:26.705710 drb-metadata-1.2.0/drb/metadata/
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-05-16 13:05:50.000000 drb-metadata-1.2.0/drb/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-16 14:07:26.705710 drb-metadata-1.2.0/drb/metadata/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     5308 2023-05-16 13:19:20.000000 drb-metadata-1.2.0/drb/metadata/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)      759 2023-05-16 13:05:50.000000 drb-metadata-1.2.0/drb/metadata/schema.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:07:26.701710 drb-metadata-1.2.0/drb_metadata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-05-16 14:07:26.000000 drb-metadata-1.2.0/drb_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      434 2023-05-16 14:07:26.000000 drb-metadata-1.2.0/drb_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 14:07:26.000000 drb-metadata-1.2.0/drb_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 14:07:26.000000 drb-metadata-1.2.0/drb_metadata.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       50 2023-05-16 14:07:26.000000 drb-metadata-1.2.0/drb_metadata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-16 14:07:26.000000 drb-metadata-1.2.0/drb_metadata.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-16 13:05:50.000000 drb-metadata-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-05-16 13:05:50.000000 drb-metadata-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-05-16 14:07:26.701710 drb-metadata-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-16 13:05:50.000000 drb-metadata-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 14:07:26.701710 drb-metadata-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-05-16 13:05:50.000000 drb-metadata-1.2.0/tests/test_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    81180 2023-05-16 13:05:50.000000 drb-metadata-1.2.0/versioneer.py
```

### Comparing `drb-metadata-1.1.2/LICENCE.txt` & `drb-metadata-1.2.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `drb-metadata-1.1.2/PKG-INFO` & `drb-metadata-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-metadata
-Version: 1.1.2
+Version: 1.2.0
 Summary: DRB Metadata Extractor
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `drb-metadata-1.1.2/README.md` & `drb-metadata-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drb-metadata-1.1.2/drb/metadata/metadata.py` & `drb-metadata-1.2.0/drb/metadata/metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 from types import ModuleType
 from typing import Any, Dict, List, Tuple
 from uuid import UUID
 from drb.core.node import DrbNode
-from drb.nodes.logical_node import DrbLogicalNode
-from drb.core.item_class import ItemClass, ItemClassLoader
 from drb.exceptions.core import DrbException
+from drb.topics.dao import ManagerDao
+from drb.topics.topic import DrbTopic
 from drb.utils.plugins import get_entry_points
 from drb.extractor import parse_extractor, Extractor
 import os
 import jsonschema
 import yaml
 import importlib
 import logging
@@ -130,32 +130,34 @@
 
     def __eq__(self, other: object) -> bool:
         return isinstance(other, DrbMetadata) and self._name == other._name
 
 
 class DrbMetadataResolver:
     __instance = None
-    __ic_loader: ItemClassLoader = None
+    __ic_loader: ManagerDao = None
     __metadata: Dict[UUID, List[DrbMetadata]] = None
 
     def __new__(cls, *args, **kwargs):
         if cls.__instance is None:
             cls.__instance = super(DrbMetadataResolver, cls).__new__(cls)
-            cls.__ic_loader = ItemClassLoader()
+            cls.__ic_loader = ManagerDao()
             cls.__metadata = _load_all_metadata()
         return cls.__instance
 
-    def _retrieve_metadata(self, ic: ItemClass) -> Dict[str, DrbMetadata]:
+    def _retrieve_metadata(self, ic: DrbTopic) -> Dict[str, DrbMetadata]:
         metadata = None
 
         # load metadata from super class
-        if ic.parent_class_id is not None:
-            parent = self.__ic_loader.get_item_class(ic.parent_class_id)
-            metadata = self._retrieve_metadata(
-                self.__ic_loader.get_item_class(parent.id))
+        if ic.subClassOf is not None:
+            metadata = {}
+            for parent_id in ic.subClassOf:
+                parent = self.__ic_loader.get_drb_topic(parent_id)
+                metadata.update(self._retrieve_metadata(
+                    self.__ic_loader.get_drb_topic(parent.id)))
 
         if metadata is None:
             metadata = {}
 
         # add specific metadata of the given class (override if necessary)
         if ic.id in self.__metadata.keys():
             for md in self.__metadata[ic.id]:
```

### Comparing `drb-metadata-1.1.2/drb/metadata/schema.yml` & `drb-metadata-1.2.0/drb/metadata/schema.yml`

 * *Files identical despite different names*

### Comparing `drb-metadata-1.1.2/drb_metadata.egg-info/PKG-INFO` & `drb-metadata-1.2.0/drb_metadata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-metadata
-Version: 1.1.2
+Version: 1.2.0
 Summary: DRB Metadata Extractor
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `drb-metadata-1.1.2/setup.cfg` & `drb-metadata-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `drb-metadata-1.1.2/tests/test_metadata.py` & `drb-metadata-1.2.0/tests/test_metadata.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from drb.nodes.logical_node import DrbLogicalNode
-from drb.metadata import DrbMetadataResolver
 import os
 import unittest
 import drb.topics.resolver as topic_resolver
+from drb.metadata import DrbMetadataResolver
 
 
 class TestMetadataResolver(unittest.TestCase):
     resource_dir = None
     resolver = None
 
     @classmethod
```

### Comparing `drb-metadata-1.1.2/versioneer.py` & `drb-metadata-1.2.0/versioneer.py`

 * *Files identical despite different names*

