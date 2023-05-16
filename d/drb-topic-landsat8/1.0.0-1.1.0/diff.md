# Comparing `tmp/drb-topic-landsat8-1.0.0.tar.gz` & `tmp/drb-topic-landsat8-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-topic-landsat8-1.0.0.tar", last modified: Fri Feb 24 08:48:06 2023, max compression
+gzip compressed data, was "drb-topic-landsat8-1.1.0.tar", last modified: Tue May 16 15:37:13 2023, max compression
```

## Comparing `drb-topic-landsat8-1.0.0.tar` & `drb-topic-landsat8-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 08:48:06.496641 drb-topic-landsat8-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-02-16 14:03:10.000000 drb-topic-landsat8-1.0.0/LICENCE.txt
--rw-r--r--   0 root         (0) root         (0)     1098 2023-02-24 08:48:06.496641 drb-topic-landsat8-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      712 2023-02-21 10:36:54.000000 drb-topic-landsat8-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 08:48:06.488641 drb-topic-landsat8-1.0.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 08:48:06.488641 drb-topic-landsat8-1.0.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 08:48:06.500641 drb-topic-landsat8-1.0.0/drb/topics/landsat8/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-02-16 14:03:10.000000 drb-topic-landsat8-1.0.0/drb/topics/landsat8/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-02-24 08:48:06.500641 drb-topic-landsat8-1.0.0/drb/topics/landsat8/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     1306 2023-02-21 10:36:54.000000 drb-topic-landsat8-1.0.0/drb/topics/landsat8/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 08:48:06.496641 drb-topic-landsat8-1.0.0/drb/topics/landsat8/libs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 15:58:16.000000 drb-topic-landsat8-1.0.0/drb/topics/landsat8/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 08:48:06.496641 drb-topic-landsat8-1.0.0/drb_topic_landsat8.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1098 2023-02-24 08:48:06.000000 drb-topic-landsat8-1.0.0/drb_topic_landsat8.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      565 2023-02-24 08:48:06.000000 drb-topic-landsat8-1.0.0/drb_topic_landsat8.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-24 08:48:06.000000 drb-topic-landsat8-1.0.0/drb_topic_landsat8.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       93 2023-02-24 08:48:06.000000 drb-topic-landsat8-1.0.0/drb_topic_landsat8.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-24 08:48:06.000000 drb-topic-landsat8-1.0.0/drb_topic_landsat8.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       77 2023-02-24 08:48:06.000000 drb-topic-landsat8-1.0.0/drb_topic_landsat8.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-02-24 08:48:06.000000 drb-topic-landsat8-1.0.0/drb_topic_landsat8.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-02-16 14:03:10.000000 drb-topic-landsat8-1.0.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-02-23 15:58:16.000000 drb-topic-landsat8-1.0.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      982 2023-02-24 08:48:06.500641 drb-topic-landsat8-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-02-16 14:03:10.000000 drb-topic-landsat8-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-24 08:48:06.496641 drb-topic-landsat8-1.0.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3509 2023-02-21 10:36:54.000000 drb-topic-landsat8-1.0.0/tests/test_landsat8_topic.py
--rw-rw-rw-   0 root         (0) root         (0)     1357 2023-02-21 10:36:54.000000 drb-topic-landsat8-1.0.0/tests/test_mtl_data.py
--rw-rw-rw-   0 root         (0) root         (0)    83607 2023-02-16 14:03:10.000000 drb-topic-landsat8-1.0.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:37:13.461457 drb-topic-landsat8-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-02-16 14:03:10.000000 drb-topic-landsat8-1.1.0/LICENCE.txt
+-rw-r--r--   0 root         (0) root         (0)     1098 2023-05-16 15:37:13.461457 drb-topic-landsat8-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-02-21 10:36:54.000000 drb-topic-landsat8-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:37:13.445457 drb-topic-landsat8-1.1.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:37:13.445457 drb-topic-landsat8-1.1.0/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:37:13.461457 drb-topic-landsat8-1.1.0/drb/topics/landsat8/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-02-16 14:03:10.000000 drb-topic-landsat8-1.1.0/drb/topics/landsat8/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-16 15:37:13.461457 drb-topic-landsat8-1.1.0/drb/topics/landsat8/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1306 2023-05-16 15:36:15.000000 drb-topic-landsat8-1.1.0/drb/topics/landsat8/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:37:13.453457 drb-topic-landsat8-1.1.0/drb/topics/landsat8/libs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-23 15:58:16.000000 drb-topic-landsat8-1.1.0/drb/topics/landsat8/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:37:13.457457 drb-topic-landsat8-1.1.0/drb_topic_landsat8.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1098 2023-05-16 15:37:13.000000 drb-topic-landsat8-1.1.0/drb_topic_landsat8.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      565 2023-05-16 15:37:13.000000 drb-topic-landsat8-1.1.0/drb_topic_landsat8.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:37:13.000000 drb-topic-landsat8-1.1.0/drb_topic_landsat8.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-16 15:37:13.000000 drb-topic-landsat8-1.1.0/drb_topic_landsat8.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:37:13.000000 drb-topic-landsat8-1.1.0/drb_topic_landsat8.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-16 15:37:13.000000 drb-topic-landsat8-1.1.0/drb_topic_landsat8.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-16 15:37:13.000000 drb-topic-landsat8-1.1.0/drb_topic_landsat8.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-02-16 14:03:10.000000 drb-topic-landsat8-1.1.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-05-16 14:20:26.000000 drb-topic-landsat8-1.1.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      982 2023-05-16 15:37:13.461457 drb-topic-landsat8-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-02-16 14:03:10.000000 drb-topic-landsat8-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:37:13.461457 drb-topic-landsat8-1.1.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3503 2023-05-16 14:32:35.000000 drb-topic-landsat8-1.1.0/tests/test_landsat8_topic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1388 2023-05-16 14:28:11.000000 drb-topic-landsat8-1.1.0/tests/test_mtl_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    83607 2023-02-16 14:03:10.000000 drb-topic-landsat8-1.1.0/versioneer.py
```

### Comparing `drb-topic-landsat8-1.0.0/LICENCE.txt` & `drb-topic-landsat8-1.1.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `drb-topic-landsat8-1.0.0/PKG-INFO` & `drb-topic-landsat8-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-topic-landsat8
-Version: 1.0.0
+Version: 1.1.0
 Summary: DRB Landsat 8 Topic
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
```

### Comparing `drb-topic-landsat8-1.0.0/README.md` & `drb-topic-landsat8-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `drb-topic-landsat8-1.0.0/drb/topics/landsat8/cortex.yml` & `drb-topic-landsat8-1.1.0/drb/topics/landsat8/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-landsat8-1.0.0/drb_topic_landsat8.egg-info/PKG-INFO` & `drb-topic-landsat8-1.1.0/drb_topic_landsat8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-topic-landsat8
-Version: 1.0.0
+Version: 1.1.0
 Summary: DRB Landsat 8 Topic
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
```

### Comparing `drb-topic-landsat8-1.0.0/drb_topic_landsat8.egg-info/SOURCES.txt` & `drb-topic-landsat8-1.1.0/drb_topic_landsat8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drb-topic-landsat8-1.0.0/setup.cfg` & `drb-topic-landsat8-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `drb-topic-landsat8-1.0.0/tests/test_landsat8_topic.py` & `drb-topic-landsat8-1.1.0/tests/test_landsat8_topic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import shutil
 
-from drb.core.item_class import ItemClassLoader
 import unittest
 import uuid
 import os
 import tempfile
 import tarfile
 import drb.topics.resolver as resolver
+from drb.topics.dao import ManagerDao
 
 
 class TestLandsat8Topic(unittest.TestCase):
     # from GAEL Systems dataset ref
     data = {
             "LC81820462016026LBG00.tar.gz",
             "LC81830602017019LBG00.tar.gz",
@@ -54,35 +54,35 @@
         path = os.path.join(tempfile.gettempdir(), name)
         mode = "w|gz" if name.lower().endswith('gz') else "w|"
         tar = tarfile.open(path, mode)
         tar.close()
         return path
 
     def test_topic_loading(self):
-        topic_loader = ItemClassLoader()
+        topic_loader = ManagerDao()
         for key in self.topic_labels.keys():
-            topic = topic_loader.get_item_class(key)
+            topic = topic_loader.get_drb_topic(key)
             self.assertEqual(self.topic_labels[key], topic.label)
 
     def test_topic_resolution(self):
-        topics = ItemClassLoader()
+        topics = ManagerDao()
 
         # Landsat-8 product before 2017
-        ex_topic = topics.get_item_class(
+        ex_topic = topics.get_drb_topic(
             uuid.UUID('d6ec274f-d84a-499d-923a-5116c1b96655'))
         for n in filter(lambda x: x[2] == '8', self.data):
             ac_topic, node = resolver.resolve(os.path.join(self.data_dir, n))
-            self.assertEqual(ex_topic, ac_topic)
+            self.assertEqual(ex_topic.id, ac_topic.id)
 
         # Collection 1
-        ex_topic = topics.get_item_class(
+        ex_topic = topics.get_drb_topic(
             uuid.UUID('10e14810-3060-4f55-99e7-3a84e2947343'))
         for n in filter(lambda x: len(x) > 37 and x[35:37] == '01', self.data):
             ac_topic, node = resolver.resolve(os.path.join(self.data_dir, n))
-            self.assertEqual(ex_topic, ac_topic)
+            self.assertEqual(ex_topic.id, ac_topic.id)
 
         # Collection 2
-        ex_topic = topics.get_item_class(
+        ex_topic = topics.get_drb_topic(
             uuid.UUID('460f7ffa-3ebb-4122-8ce3-53d54432727b'))
         for n in filter(lambda x: len(x) > 37 and x[35:37] == '02', self.data):
             ac_topic, node = resolver.resolve(os.path.join(self.data_dir, n))
-            self.assertEqual(ex_topic, ac_topic)
+            self.assertEqual(ex_topic.id, ac_topic.id)
```

### Comparing `drb-topic-landsat8-1.0.0/tests/test_mtl_data.py` & `drb-topic-landsat8-1.1.0/tests/test_mtl_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,17 +17,18 @@
         if self.current_node is not None:
             self.current_node.close()
 
     def test_resolve_mtl_file(self):
         topic, self.current_node = resolver.resolve(self.path)
         self.assertEqual(uuid.UUID("b299117e-123b-482e-869f-ddb085677952"),
                          topic.id)
-        java_node_factory = self.factories.get_factory('java')
+        factory_name = 'java'
+        java_node_factory = self.factories.get_factory(factory_name)
         self.assertIsNotNone(java_node_factory)
-        self.assertEqual(java_node_factory, topic.factory)
+        self.assertEqual(factory_name, topic.factory)
 
     def test_browse_mtl_file(self):
         self.current_node = DrbJavaFactory().create(self.path)
         node = self.current_node["l1MetadataFile"]
 
         expected = "L1TP"
         actual = node["productMetadata"]["dataType"].value
```

### Comparing `drb-topic-landsat8-1.0.0/versioneer.py` & `drb-topic-landsat8-1.1.0/versioneer.py`

 * *Files identical despite different names*

