# Comparing `tmp/cwapi3d-1.3.9.tar.gz` & `tmp/cwapi3d-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwapi3d-1.3.9.tar", last modified: Wed Jun 29 14:19:01 2022, max compression
+gzip compressed data, was "cwapi3d-2.0.1.tar", last modified: Tue May 16 15:47:06 2023, max compression
```

## Comparing `cwapi3d-1.3.9.tar` & `cwapi3d-2.0.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 14:19:01.259281 cwapi3d-1.3.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-06-29 14:18:47.000000 cwapi3d-1.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-06-29 14:19:01.259281 cwapi3d-1.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-06-29 14:18:47.000000 cwapi3d-1.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-06-29 14:18:47.000000 cwapi3d-1.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-06-29 14:19:01.259281 cwapi3d-1.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1547 2022-06-29 14:18:47.000000 cwapi3d-1.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 14:19:01.255281 cwapi3d-1.3.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 14:19:01.259281 cwapi3d-1.3.9/src/attribute_controller/
--rw-r--r--   0 runner    (1001) docker     (121)    22772 2022-06-29 14:18:47.000000 cwapi3d-1.3.9/src/attribute_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 14:19:01.259281 cwapi3d-1.3.9/src/bim_controller/
--rw-r--r--   0 runner    (1001) docker     (121)     4295 2022-06-29 14:18:47.000000 cwapi3d-1.3.9/src/bim_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 14:19:01.259281 cwapi3d-1.3.9/src/cadwork/
--rw-r--r--   0 runner    (1001) docker     (121)    37963 2022-06-29 14:18:47.000000 cwapi3d-1.3.9/src/cadwork/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 14:19:01.259281 cwapi3d-1.3.9/src/connector_axis_controller/
--rw-r--r--   0 runner    (1001) docker     (121)     6105 2022-06-29 14:18:47.000000 cwapi3d-1.3.9/src/connector_axis_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 14:19:01.259281 cwapi3d-1.3.9/src/cwapi3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-06-29 14:19:00.000000 cwapi3d-1.3.9/src/cwapi3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-06-29 14:19:01.000000 cwapi3d-1.3.9/src/cwapi3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-29 14:19:00.000000 cwapi3d-1.3.9/src/cwapi3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-06-29 14:19:01.000000 cwapi3d-1.3.9/src/cwapi3d.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 14:19:01.259281 cwapi3d-1.3.9/src/element_controller/
--rw-r--r--   0 runner    (1001) docker     (121)    31206 2022-06-29 14:18:47.000000 cwapi3d-1.3.9/src/element_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 14:19:01.259281 cwapi3d-1.3.9/src/endtype_controller/
--rw-r--r--   0 runner    (1001) docker     (121)     3484 2022-06-29 14:18:47.000000 cwapi3d-1.3.9/src/endtype_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 14:19:01.259281 cwapi3d-1.3.9/src/file_controller/
--rw-r--r--   0 runner    (1001) docker     (121)     5146 2022-06-29 14:18:47.000000 cwapi3d-1.3.9/src/file_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 14:19:01.259281 cwapi3d-1.3.9/src/geometry_controller/
--rw-r--r--   0 runner    (1001) docker     (121)    18414 2022-06-29 14:18:47.000000 cwapi3d-1.3.9/src/geometry_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 14:19:01.259281 cwapi3d-1.3.9/src/list_controller/
--rw-r--r--   0 runner    (1001) docker     (121)     2693 2022-06-29 14:18:47.000000 cwapi3d-1.3.9/src/list_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 14:19:01.259281 cwapi3d-1.3.9/src/machine_controller/
--rw-r--r--   0 runner    (1001) docker     (121)     1307 2022-06-29 14:18:47.000000 cwapi3d-1.3.9/src/machine_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 14:19:01.259281 cwapi3d-1.3.9/src/material_controller/
--rw-r--r--   0 runner    (1001) docker     (121)     7847 2022-06-29 14:18:47.000000 cwapi3d-1.3.9/src/material_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 14:19:01.259281 cwapi3d-1.3.9/src/menu_controller/
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-06-29 14:18:47.000000 cwapi3d-1.3.9/src/menu_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 14:19:01.259281 cwapi3d-1.3.9/src/roof_controller/
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-06-29 14:18:47.000000 cwapi3d-1.3.9/src/roof_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 14:19:01.259281 cwapi3d-1.3.9/src/scene_controller/
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-06-29 14:18:47.000000 cwapi3d-1.3.9/src/scene_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 14:19:01.259281 cwapi3d-1.3.9/src/shop_drawing_controller/
--rw-r--r--   0 runner    (1001) docker     (121)     2704 2022-06-29 14:18:47.000000 cwapi3d-1.3.9/src/shop_drawing_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 14:19:01.259281 cwapi3d-1.3.9/src/utility_controller/
--rw-r--r--   0 runner    (1001) docker     (121)    12508 2022-06-29 14:18:47.000000 cwapi3d-1.3.9/src/utility_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-29 14:19:01.259281 cwapi3d-1.3.9/src/visualization_controller/
--rw-r--r--   0 runner    (1001) docker     (121)     4721 2022-06-29 14:18:47.000000 cwapi3d-1.3.9/src/visualization_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.831681 cwapi3d-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/attribute_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)    23816 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/attribute_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/bim_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/bim_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/cadwork/
+-rw-r--r--   0 runner    (1001) docker     (123)    86279 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/cadwork/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/connector_axis_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/connector_axis_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/cwapi3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-16 15:47:06.000000 cwapi3d-2.0.1/src/cwapi3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-16 15:47:06.000000 cwapi3d-2.0.1/src/cwapi3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 15:47:06.000000 cwapi3d-2.0.1/src/cwapi3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-16 15:47:06.000000 cwapi3d-2.0.1/src/cwapi3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/element_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)    33675 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/element_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/endtype_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/endtype_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/file_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/file_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/geometry_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/geometry_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/list_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/list_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/machine_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/machine_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/material_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/material_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/menu_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/menu_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/roof_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/roof_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/scene_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/scene_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/shop_drawing_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/shop_drawing_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/utility_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/utility_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:47:06.835682 cwapi3d-2.0.1/src/visualization_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-16 15:46:54.000000 cwapi3d-2.0.1/src/visualization_controller/__init__.pyi
```

### Comparing `cwapi3d-1.3.9/LICENSE` & `cwapi3d-2.0.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Cadwork Informatique Inc.
+Copyright (c) 2022 Cadwork Informatique Inc.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `cwapi3d-1.3.9/PKG-INFO` & `cwapi3d-2.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwapi3d
-Version: 1.3.9
+Version: 2.0.1
 Summary: Python bindings for CwAPI3D
 Home-page: https://github.com/cwapi3d/cwapi3dpython
 Author: Cadwork
 Author-email: it@cadwork.ca
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
```

### Comparing `cwapi3d-1.3.9/README.md` & `cwapi3d-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cwapi3d-1.3.9/setup.py` & `cwapi3d-2.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='cwapi3d',
-    version='1.3.9',
+    version='2.0.1',
     author='Cadwork',
     author_email='it@cadwork.ca',
     description='Python bindings for CwAPI3D',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/cwapi3d/cwapi3dpython',
     classifiers=[
```

### Comparing `cwapi3d-1.3.9/src/cwapi3d.egg-info/PKG-INFO` & `cwapi3d-2.0.1/src/cwapi3d.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwapi3d
-Version: 1.3.9
+Version: 2.0.1
 Summary: Python bindings for CwAPI3D
 Home-page: https://github.com/cwapi3d/cwapi3dpython
 Author: Cadwork
 Author-email: it@cadwork.ca
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
```

### Comparing `cwapi3d-1.3.9/src/cwapi3d.egg-info/SOURCES.txt` & `cwapi3d-2.0.1/src/cwapi3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cwapi3d-1.3.9/src/element_controller/__init__.pyi` & `cwapi3d-2.0.1/src/element_controller/__init__.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,200 +1,211 @@
 from typing import List
-from cadwork import (element_module_properties, 
-                         point_3d,
-                         element_module_detail)
+from cadwork import (element_module_properties,
+                     point_3d,
+                     element_module_detail)
 
 
-
-    
 def get_all_identifiable_element_ids() -> List[int]:
     """get all identifiable element IDs (visible and unvisible)
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Returns:
         List[int]: element_id list
     """
-    
+
+
 def get_visible_identifiable_element_ids() -> List[int]:
     """get all visible identifiable elemnt ids
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Returns:
         List[int]: element_id list
     """
-    
+
+
 def get_invisible_identifiable_element_ids() -> List[int]:
     """Get invisible cadwork element IDs
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Returns:
         List[int]: element_id list
     """
-    
+
+
 def get_active_identifiable_element_ids() -> List[int]:
     """Get active cadwork element IDs
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Returns:
         List[int]: element_id list
     """
 
+
 def get_inactive_all_identifiable_element_ids() -> List[int]:
     """Get inactive cadwork element IDs
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Returns:
         List[int]: element_id list
     """
-    
+
+
 def get_inactive_visible_identifiable_element_ids() -> List[int]:
     """Get inactive visible cadwork element IDs
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Returns:
         List[int]: element_id list
     """
-    
+
+
 def delete_elements(elements: List[int]) -> None:
     """Delete elements 
 
     Args:
         elements (List[int]): element IDs
     """
-    
+
+
 def join_elements(elements: List[int]) -> None:
     """join elements (group)
 
     Args:
         elements (List[int]): element IDs
     """
-    
+
+
 def join_top_level_elements(elements: List[int]) -> None:
     """join elements on highest leve. Previously joined elements are dissolved and joined at the top level.
 
     Args:
         elements (List[int]): element IDs
     """
-    
+
+
 def create_rectangular_beam_points(width: float, height: float, p1: point_3d, p2: point_3d, p3: point_3d) -> int:
     """create a rectangular beam. The direction (local x axis) and length of the beam is defined via p1 and p2. 
     The parameter p3 is used to set the local z vector (height) of the beams coordinate system. 
 
     Args:
         width (float): beam width
         height (float): beam height
         p1 (point_3d): start point
         p2 (point_3d): end point
         p3 (point_3d): height point
 
     Returns:
         int: element ID
     """
-    
+
+
 def create_circular_beam_points(diameter: float, p1: point_3d, p2: point_3d, p3: point_3d) -> int:
     """create a circular beam. The direction (local x axis) and length of the beam is defined via p1 and p2. 
    The parameter p3 is used to set the local z vector (height) of the beams coordinate system. 
 
     Args:
         diameter (float): circle diameter
         p1 (point_3d): start point
         p2 (point_3d): end point
         p3 (point_3d): height point
 
     Returns:
         int: element ID
     """
-    
+
+
 def create_square_beam_points(width: float, p1: point_3d, p2: point_3d, p3: point_3d) -> int:
     """create a square beam. The direction (local x axis) and length of the beam is defined via p1 and p2. 
     The parameter p3 is used to set the local z vector (height) of the beams coordinate system. 
 
     Args:
         width (float): beam width
         p1 (point_3d): start point
         p2 (point_3d): end point
         p3 (point_3d): height point
 
     Returns:
         int: element ID
     """
-    
-def create_rectangular_beam_vectors(length: float, width: float, height: float, p1: point_3d, xl: point_3d, zl: point_3d) -> int:
+
+
+def create_rectangular_beam_vectors(width: float, height: float, length: float, p1: point_3d, xl: point_3d, zl: point_3d) -> int:
     """create a rectangular beam from vectors. The start point of the element is defined by p1. Then the direction (local x axis) is definied by p2 (e.g. point_3d(1.,0.,0.)).
     The local z vector is defined via p3 (e.g. point_3d(0.,1.,0.)). 
 
+    Examples:
+        >>> beam = ec.create_rectangular_beam_vectors(120.0, 240.0, 2800.0, cadwork.point_3d(0.,0.,0.), cadwork.point_3d(1.,0.,0.), cadwork.point_3d(0.,0.,1.))
+
     Args:
         length (float): length of beam axis
         width (float): beam width
         height (float): beam height
         p1 (point_3d): start point 
         xl (point_3d): local x vector
         zl (point_3d): local z vector
 
     Returns:
         int: element ID
     """
-    
+
+
 def create_circular_beam_vectors(diameter: float, length: float, p1: point_3d, xl: point_3d, zl: point_3d) -> int:
     """create a circular beam from vectors. The start point of the element is defined by p1. Then the direction (local x axis) is definied by xl (e.g. point_3d(1.,0.,0.)).
     The local z vector is defined via zl (e.g. point_3d(0.,1.,0.)).
 
     Args:
         diameter (float): circle diameter
         length (float): beam/axis length
         p1 (point_3d): start point
         xl (point_3d): local x vector
         zl (point_3d): local z vector
 
     Returns:
         int: element ID
     """
-    
+
+
 def create_square_beam_vectors(width: float, length: float, p1: point_3d, xl: point_3d, zl: point_3d) -> int:
     """create a square beam from vectors. The start point of the element is defined by p1. Then the direction (local x axis) is definied by xl (e.g. point_3d(1.,0.,0.)).
     The local z vector is defined via zl (e.g. point_3d(0.,1.,0.)).
 
     Args:
         width (float): beam width
         length (float): beam/axis length
         p1 (point_3d): start point
         xl (point_3d): local x vector
         zl (point_3d): local z vector
 
     Returns:
         int: element ID
     """
-    
+
+
 def create_rectangular_panel_points(width: float, thickness: float, p1: point_3d, p2: point_3d, p3: point_3d) -> int:
     """create a rectangular panel. The direction (local x axis) and length of the panel is defined via p1 and p2. 
     The parameter (p3) is used to set the local z vector (thickness) of the beams coordinate system.
 
     Args:
         width (float): beam width
         thickness (float): beam thickness
         p1 (point_3d): start point
         p2 (point_3d): end point
         p3 (point_3d): height point
 
     Returns:
         int: element ID
     """
-    
+
+
 def create_rectangular_panel_vectors(width: float, thickness: float, length: float, p1: point_3d, xl: point_3d, zl: point_3d) -> int:
     """create a rectangular panel from vectors. The start point of the element is defined by p1. Then the direction (local x axis) is definied by p2 (e.g. point_3d(1.,0.,0.)).
     The local z vector is defined via p3 (e.g. point_3d(0.,1.,0.)). 
 
     Args:
         width (float): panel width
         thickness (float): panel thickness
@@ -202,885 +213,1090 @@
         p1 (point_3d): start point
         xl (point_3d): local x vector
         zl (point_3d): local z vector
 
     Returns:
         int: element ID
     """
-    
+
+
 def create_drilling_points(diameter: float, p1: point_3d, p2: point_3d) -> int:
     """Create a drilling from two points. 
 
     Args:
         diameter (float): drilling diameter
         p1 (point_3d): start point
         p2 (point_3d): end point
 
     Returns:
         int: element ID
     """
-    
-def create_drilling_vectors(diameter: float, length: float, p1: point_3d, xl:point_3d) -> int:
+
+
+def create_drilling_vectors(diameter: float, length: float, p1: point_3d, xl: point_3d) -> int:
     """Create a drilling from a point and a direction vector. 
 
     Args:
         diameter (float): drilling diameter
         length (float): drilling length
         p1 (point_3d): start point
         xl (point_3d): vector direction
 
     Returns:
         int: [description]
     """
-    
+
+
 def create_line_points(p1: point_3d, p2: point_3d) -> int:
     """crete a line
 
     Args:
         p1 (point_3d): start point
         p2 (point_3d): end point
 
     Returns:
         int: element ID
     """
-    
+
+
 def create_line_vectors(length: float, p1: point_3d, xl: point_3d) -> int:
     """crete a line
 
     Args:
         length (float): line length
         p1 (point_3d): start point
         xl (point_3d): vector direction
 
     Returns:
         int: elmement id
     """
-    
+
+
 def create_node(p1: point_3d) -> int:
     """create a node
 
     Args:
         p1 (point_3d): point
 
     Returns:
         int: element ID
     """
-    
+
+
 def solder_elements(elements: List[int]) -> List[int]:
     """solder elements, if they are in contact. 
 
     Args:
         elements (List[int]): element IDs
 
     Returns:
         List[int]: element ID
     """
-    
+
+
 def convert_beam_to_panel(elements: List[int]) -> None:
     """convert beam(s) to panel(s)
 
     Args:
         elements (List[int]): element IDs
     """
-    
+
+
 def convert_panel_to_beam(elements: List[int]) -> None:
     """convert panel(s) to beam(s)
 
     Args:
         elements (List[int]): element IDs
     """
+
+
 def delete_all_element_end_types(elements: List[int]) -> None:
     """delete end types
 
     Args:
         elements (List[int]): element IDs
     """
+
+
 def delete_all_element_processes(elements: List[int]) -> None:
     """delete element processes
 
     Args:
         elements (List[int]): element IDs
     """
+
+
 def move_element(elements: List[int], vector: point_3d) -> None:
     """move element by a vector
 
     Args:
         elements (List[int]): element IDs
         vector (point_3d): vector
     """
+
+
 def create_polygon_beam(points: List[point_3d], thickness: float, xl: point_3d, zl: point_3d) -> int:
     """create a polygon beam. Define the polygon outline in a vertex list.  
-    
+
     Args:
         points (List[point_3d]): vertex list
         thickness (float): beam thickness
         xl (point_3d): vector (length dir)
         zl (point_3d): vector (height dir)
 
     Returns:
         int: element ID
     """
+
+
 def create_text_object(text: str, position: point_3d, xl: point_3d, zl: point_3d, size: float) -> int:
     """create text object
 
     Args:
         text (str): your text
         position (point_3d): location
         xl (point_3d): length dir
         zl (point_3d): height dir
         size (float): font size
 
     Returns:
         int: element ID
     """
+
+
 def copy_elements(elements: List[int], vector: point_3d) -> List[int]:
     """copy elements
 
     Args:
         elements (List[int]): element IDs
         vector (point_3d): copy vector
 
     Returns:
         List[int]: element IDs
     """
+
+
 def rotate_elements(elements: List[int], origin: point_3d, rotation_axis: point_3d, rotation_angle: float) -> None:
     """rotate elements
 
     Args:
         elements (List[int]): element IDs
         origin (point_3d): element origin (p1)
         rotation_axis (point_3d): vector axis
         rotation_angle (float): radians
     """
+
+
 def subtract_elements(hard_elements: List[int], soft_elements: List[int]) -> List[int]:
     """Subtract elements. The first element is hard, the second soft.
 
     Args:
         hard_elements (List[int]): subtract with
         soft_elements (List[int]): subtract from
 
     Returns:
         List[int]: element IDs
     """
+
+
+def subtract_elements_with_undo(hard_elements: List[int], soft_elements: List[int], with_undo: bool) -> List[int]:
+    """Subtract elements with undo. The first element is hard, the second soft.
+
+    Args:
+        hard_elements (List[int]): subtract with
+        soft_elements (List[int]): subtract from
+        with_undo (bool): with undo
+
+    Returns:
+        List[int]: element IDs
+    """
+
+
 def check_element_id(element: int) -> bool:
     """check element ID
 
     Args:
         element (int): element ID
 
     Returns:
         bool: True/False
     """
+
+
 def start_element_module_calculation(elements: List[int]) -> None:
     """start the elemend module calculation. Inputarguments are cover elements. 
 
     Args:
         elements (List[int]): element IDs (cover(s) architectural elementtypes)
     """
+
+
 def set_element_detail_path(path: str) -> None:
     """set element detail path
 
     Args:
         path (str): path to elementmodule directory
     """
+
+
 def get_element_detail_path() -> str:
     """get the path from active elmeentmodule
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Returns:
         str: path
     """
+
+
 def get_element_cadwork_guid(element: int) -> str:
     """get cadwork element guid
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         element (int): element ID
 
     Returns:
         str: guid
     """
+
+
 def get_element_from_cadwork_guid(guid: str) -> int:
     """get element from cadwork guid
 
     Args:
         guid (str): cadwork guid
 
     Returns:
         int: element ID
     """
+
+
 def add_elements_to_undo(elements: List[int], number: int) -> None:
     """add elements to undo
 
     Args:
         elements (List[int]): element IDs
         number (int): enum(1:add, 2:modify)
     """
+
+
 def make_undo() -> None:
     """make undo
     """
+
+
 def make_redo() -> None:
     """make redo
     """
+
+
 def split_elements(elements: List[int]) -> None:
     """split joined elmements
 
     Args:
         elements (List[int]): element IDs
     """
+
+
 def set_line_to_marking_line(elements: List[int]) -> None:
     """modify a line to a marking line
 
     Args:
         elements (List[int]): element IDs
     """
+
+
 def set_line_to_normal_line(elements: List[int]) -> None:
     """set line to normal line
 
     Args:
         elements (List[int]): element IDs
     """
-def create_auto_export_solid_from_standard(elements: List[int], name:str, standard_element_name:str) -> int:
+
+
+def create_auto_export_solid_from_standard(elements: List[int], name: str, standard_element_name: str) -> int:
     """create automatic export solid from a standard export solid
 
     Args:
         elements (List[int]): element IDs
         name (str): new name for export solid
         standard_element_name (str): name of standard export solid
 
     Returns:
         int: element ID
     """
+
+
 def set_element_module_properties_for_elements(elements: List[int], properties: element_module_properties) -> None:
     """set element module properties for elements
-    
+
     Examples:
         >>> import cadwork as cw
         >>> import element_controller as ec
         >>> element_properties = ec.get_element_module_properties_for_element(540915) # 540915 = some element ID
         >>> cw.element_module_properties.set_bottom_plate(element_properties, True)
         >>> cw.element_module_properties.set_solder_in_axis_direction(element_properties, True)
         >>> cw.element_module_properties.set_main_element(element_properties, True)
         >>> cw.element_module_properties.set_strecht_according_thickness_axis(element_properties, True)
         >>> ec.set_element_module_properties_for_elements([540915],element_properties)
         None
-        
 
     Args:
         elements (List[int]): element IDs
         properties (element_module_properties): elment module properties
     """
+
+
 def get_element_module_properties_for_element(element: int) -> element_module_properties:
     """get element module properties for element
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         element (int): element ID
 
     Returns:
         element_module_properties: elmement module properties
     """
+
+
 def get_element_type_description(element: int) -> str:
     """get the description of the cadwork element type
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         element (int): element ID
 
     Returns:
         str: element type (e.g. beam)
     """
+
+
 def create_text_object_with_font(text: str, position: point_3d, xl: point_3d, zl: point_3d, size: float, font: str) -> int:
     """create text object with font
 
     Args:
         text (str): your text
         position (point_3d): location
         xl (point_3d): length dir
         zl (point_3d): height dir
         size (float): font size
         font (str): font type (e.g. , "Times New Roman")
 
     Returns:
         int: element ID
     """
+
+
 def get_opening_variant_ids(elements: List[int], opening_type: int) -> List[int]:
     """get opening variant ids
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         elements (List[int]): element IDs
         opening_type (int): number of opening type (enum)
 
     Returns:
         List[int]: element IDs
     """
+
+
 def get_parent_container_id(element: int) -> int:
     """get parent container id
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         element (int): element ID
 
     Returns:
         int: element ID
     """
+
+
 def get_export_solid_content_elements(element: int) -> List[int]:
     """get export solid content elements
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
-        element (int): element ID
+        element (int): element ID of export solid
     Returns:
         List[int]: element IDs
     """
+
+
 def get_container_content_elements(element: int) -> List[int]:
     """get container content elements
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         element (int): element ID
     Returns:
         List[int]: element IDs
     """
+
+
 def apply_transformation_coordinate(elments: List[int], old_point: point_3d, old_xl: point_3d, old_yl: point_3d, new_point: point_3d, new_xl: point_3d, new_yl: point_3d) -> None:
     """apply transformation coordinate to transform elements in 3D space
 
     Args:
         elments (List[int]): element IDs to transform
         old_point (point_3d): location origin
         old_xl (point_3d): origin x dir (vector)
         old_yl (point_3d): origin y dir (vector)
         new_point (point_3d): new location
         new_xl (point_3d): new x dir (vector)
         new_yl (point_3d): new y dir (vector)
     """
+
+
 def delete_elements_with_undo(elements: List[int]) -> None:
     """delete elements and store the in undo
 
     Args:
         elements (List[int]): element IDs
     """
+
+
 def add_created_elements_to_undo(elements: List[int]) -> None:
     """add created elementes to undo storeage
 
     Args:
         elements (List[int]): element IDs
     """
+
+
 def add_modified_elements_to_undo(elements: List[int]) -> None:
     """add modified elementes to undo storeage
 
     Args:
         elements (List[int]): element IDs
     """
+
+
 def recreate_elements(elements: List[int]) -> None:
     """recreate elements
 
     Args:
         elements (List[int]): element IDs
     """
-def check_if_elements_are_in_collision(first_element:int, second_element:int) -> bool:
+
+
+def check_if_elements_are_in_collision(first_element: int, second_element: int) -> bool:
     """collision detection
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         element (int): first element ID
         element (int): second element ID
 
     Returns:
         bool: true/false
     """
-def check_if_elements_are_in_contact(first_element:int, second_element:int) -> bool:
+
+
+def check_if_elements_are_in_contact(first_element: int, second_element: int) -> bool:
     """check if element faces are in contact
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         element (int): first element ID
         element (int): second element ID
 
     Returns:
         bool: true/false
     """
+
+
 def create_multi_wall(elements: List[int]) -> None:
     """create multi wall
 
     Args:
         elements (List[int]): element IDs
     """
+
+
 def get_user_element_ids() -> List[int]:
     """prompt that user select element IDs in 3D
 
     Returns:
         List[int]: elmement ids from selection
     """
-def get_element_contact_vertices(first_element:int, second_element:int) -> List[point_3d]:
+
+
+def get_element_contact_vertices(first_element: int, second_element: int) -> List[point_3d]:
     """get element contact vertices
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         element (int): first element ID
         element (int): second element ID
 
     Returns:
         List[point_3d]: vertices list
     """
-def get_nesting_parent_id(element:int) -> int:
+
+
+def get_nesting_parent_id(element: int) -> int:
     """get nesting parent id
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         element (int): element ID
 
     Returns:
         int: element ID
     """
+
+
 def get_user_element_ids_with_existing(elements: List[int]) -> List[int]:
     """
     """
+
+
 def clear_errors() -> None:
     """
     """
+
+
 def glide_elements(elements: List[int], glide_point: point_3d) -> None:
     """glide elements
 
     Args:
         elements (List[int]): element IDs
         glide_point (point_3d): a glide point
     """
-def get_element_contact_facets(first_element:int, second_element:int) -> List[List[point_3d]]:
+
+
+def get_element_contact_facets(first_element: int, second_element: int) -> List[List[point_3d]]:
     """get element contact faces
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         element (int): element ID
         element (int): element ID
 
     Returns:
         List[List[point_3d]]: contact face vertice list
     """
-def get_element_raw_interface_vertices(first_element:int, second_element:int) -> List[point_3d]:
+
+
+def get_element_raw_interface_vertices(first_element: int, second_element: int) -> List[point_3d]:
     """get element raw interface vertices
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         element (int): element ID
         element (int): element ID
 
     Returns:
         List[point_3d]: vertice list
     """
-def cut_elements_with_miter(first_element:int, second_element:int) -> bool:
+
+
+def cut_elements_with_miter(first_element: int, second_element: int) -> bool:
     """cut elements with miter. The miter is "cut" on loxal x-axis. 
 
     Args:
         element (int): element ID
         element (int): element ID
 
     Returns:
         bool: true/false
     """
+
+
 def cut_element_with_plane(element: int, cut_plane_normal_vector: point_3d, distance_from_global_origin: float) -> bool:
     """cut an elment with a plane
 
     Args:
         element (int): element ID
         cut_plane_normal_vector (point_3d): plane normal vector
         distance_from_global_origin (float): distance from origin to plane
 
     Returns:
         bool: true/false
     """
+
+
 def create_circular_mep(diameter: float, points: List[point_3d]) -> int:
     """create a circular mep
 
     Args:
         diameter (float): diameter
         points (List[point_3d]): vertice list
 
     Returns:
         int: element ID
     """
+
+
 def create_rectangular_mep(width: float, depth: float, points: List[point_3d]) -> int:
     """create rectangular mep. The mep is orientied by an active element face.
 
     Args:
         width (float): mep width
         depth (float): mep depth
         points (List[point_3d]): vertice list
 
     Returns:
         int: element ID
     """
+
+
 def slice_element_with_plane(element: int, cut_plane_normal_vector: point_3d, distance_from_global_origin: float) -> bool:
     """slice an elment with a plane
 
     Args:
         element (int): element ID
         cut_plane_normal_vector (point_3d): plane normal vector
         distance_from_global_origin (float): distance from origin to plane
 
     Returns:
         bool: true/false
     """
+
+
 def create_auto_container_from_standard(elements: List[int], output_name: str, standard_element_name: str) -> int:
     """create an automatic container from a standard container
 
     Args:
         elements (List[int]): element ID
         output_name (str): container name
         standard_element_name (str): default container name
 
     Returns:
         int: element ID
     """
+
+
 def create_auto_export_solid_from_standard_with_reference(elements: List[int], output_name: str, standard_element_name: str, reference_id: int) -> int:
     """create auto export solid from standard. The orientation is determined according to an element. 
 
     Args:
         elements (List[int]): element IDs
         output_name (str): export solid name
         standard_element_name (str): standard element name
         reference_id (int): element ID (reference - orientation)
 
     Returns:
         int: element ID
     """
+
+
 def create_auto_container_from_standard_with_reference(elements: List[int], output_name: str, standard_element_name: str, reference_id: int) -> int:
     """create auto container from standard. The orientation is determined according to an element. 
 
     Args:
         elements (List[int]): element IDs
         output_name (str): export solid name
         standard_element_name (str): standard element name
         reference_id (int): element ID (reference - orientation)
 
     Returns:
         int: element ID
     """
+
+
 def slice_elements_with_plane_and_get_new_elements(element: int, cut_plane_normal_vector: point_3d, distance_from_global_origin: point_3d) -> List[int]:
     """slice elments in two with a cutting plane.
 
     Args:
         element (int): element ID
         cut_plane_normal_vector (point_3d): plane normal vector
         distance_from_global_origin (float): distance from origin to plane
 
     Returns:
         bool: true/false
     """
+
+
 def create_surface(points: List[point_3d]) -> int:
     """create a surface
 
     Args:
         points (List[point_3d]): vertex list
 
     Returns:
         int: element ID
     """
+
+
 def convert_circular_beam_to_drilling(elements: List[int]) -> None:
     """convert circular beam to drilling 
 
     Args:
         elements (List[int]): element ID
     """
+
+
 def get_standard_export_solid_list() -> List[str]:
     """get list of standard export solid names
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Returns:
         List[str]: names
     """
+
+
 def get_standard_container_list() -> List[str]:
     """get list of standard container names
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Returns:
         List[str]: names
     """
+
+
 def stretch_start_facet(elements: List[int], stretch_vector: point_3d) -> None:
     """stretch start facet of element(s)
 
     Args:
         elements (List[int]): element ID
         stretch_vector (point_3d): vector
     """
+
+
 def stretch_end_facet(elements: List[int], stretch_vector: point_3d) -> None:
     """stretch end facet of element(s)
 
     Args:
         elements (List[int]): element ID
         stretch_vector (point_3d): vector
     """
+
+
 def get_variant_sibling_element_ids(element: int) -> List[int]:
     """get variant sibling element IDs
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         element (int): element ID
 
     Returns:
         List[int]: element IDs
     """
+
+
 def set_export_solid_contents(solid_id: int, elements: List[int]) -> None:
     """set export solid contents
 
     Args:
-        solid_id (int): element ID
-        elements (List[int]): element IDs
+        solid_id (int): element ID of export solid
+        elements (List[int]): element IDs to assign
     """
+
+
 def set_container_contents(container_id: int, elements: List[int]) -> None:
     """set container contents
 
     Args:
         solid_id (int): element ID
         elements (List[int]): element IDs
     """
+
+
 def set_parent_opening_variants_opening_angle(elements: List[int], angle: float) -> None:
     """set parent opening variants opening angle
 
     Args:
         elements (List[int]): element IDs
         angle (float): radians
     """
+
+
 def mirror_move_elements(elements: List[int], plane_definition: point_3d, plane_distance: float) -> None:
     """mirror elements (no copy)
 
     Args:
         elements (List[int]): element IDs
         plane_definition (point_3d): mirror plane
         plane_distance (float): perp. distance from origin to plane
     """
+
+
 def mirror_copy_elements(elements: List[int], plane_definition: point_3d, plane_distance: float) -> List[int]:
     """mirror elements (copy)
 
     Args:
         elements (List[int]): element IDs
         plane_definition (point_3d): mirror plane
         plane_distance (float): perp. distance from origin to plane
 
     Returns:
         List[int]: element IDs
     """
 
-def check_if_point_is_on_element(point:point_3d, element:int) -> bool:
+
+def check_if_point_is_on_element(point: point_3d, element: int) -> bool:
     """Checks if a point is on a element
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         point (point_3d): a cadwork point
         element (int): element ID
 
     Returns:
         bool: if point 
     """
 
-def check_if_point_is_in_element(point:point_3d, element:int) -> bool:
+
+def check_if_point_is_in_element(point: point_3d, element: int) -> bool:
     """Check if point is in element
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         point (point_3d): a cadwork point
         element (int): element ID
 
     Returns:
         bool: if point 
     """
-def get_bounding_box_vertices_local(element:int, elements:List[int]) -> List[point_3d]:
+
+
+def get_bounding_box_vertices_local(element: int, elements: List[int]) -> List[point_3d]:
     """create a bounding box that is aligned to a reference element. 
     The bounding box includes all elements contained in the list.
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         element (int): element ID reference element
         elements (List[int]): element IDs
 
     Returns:
         List[point_3d]: bbx vertices
     """
-def get_bounding_box_vertices_global(elements:List[int]) -> List[point_3d]:
+
+
+def get_bounding_box_vertices_global(elements: List[int]) -> List[point_3d]:
     """create a bounding box that is aligned to the global coordinate system.
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         elements (List[int]): element IDs
 
     Returns:
         List[point_3d]: bbx vertices
     """
-def create_bounding_box_local(element:int, elements:List[int]) -> int:
+
+
+def create_bounding_box_local(element: int, elements: List[int]) -> int:
     """create a bounding box that is aligned to a reference element. 
     The bounding box includes all elements contained in the list.
 
     Args:
         element (int): element ID reference element
         elements (List[int]): element IDs
 
     Returns:
         int: element ID bounding box
     """
+
+
 def create_bounding_box_global(elements: List[int]) -> int:
     """create a bounding box that is aligned to the global coordinate system.
 
     Args:
         elements (List[int]): element IDs
 
     Returns:
         int: element ID bounding box
     """
-def extrude_surface_to_auxiliary_vector(element:int, vector:point_3d) -> int:
+
+
+def extrude_surface_to_auxiliary_vector(element: int, vector: point_3d) -> int:
     """Extrude a surface to a auxiliary element. 
 
     Args:
         element (int): element ID
         vector (point_3d): vector e.g. point_3d(0,0,1200)
 
     Returns:
         int: element ID
     """
-def extrude_surface_to_beam_vector(element:int, vector:point_3d) -> int:
+
+
+def extrude_surface_to_beam_vector(element: int, vector: point_3d) -> int:
     """Extrude a surface to a beam. 
 
     Args:
         element (int): element ID
         vector (point_3d): vector e.g. point_3d(0,0,1200)
 
     Returns:
         int: element ID
     """
-def extrude_surface_to_panel_vector(element:int, vector:point_3d) -> int:
+
+
+def extrude_surface_to_panel_vector(element: int, vector: point_3d) -> int:
     """Extrude a surface to a panel.
 
     Args:
         element (int): element ID
         vector (point_3d): vector e.g. point_3d(0,0,1200)
 
     Returns:
         int: element ID
     """
-def activate_parts_without_situation()->List[int]:
+
+
+def activate_parts_without_situation() -> List[int]:
     """
 
     Returns:
         List[int]: element IDs
     """
-def activate_rv_without_situation()->List[int]:
+
+
+def activate_rv_without_situation() -> List[int]:
     """
 
     Returns:
         List[int]: element IDs
     """
-def parts_situation_manual(element: int, addChilds: List[int], removeChilds: List[int])->None:
+
+
+def parts_situation_manual(element: int, addChilds: List[int], removeChilds: List[int]) -> None:
     """
 
     Args:
         element (int): element ID
         addChilds (List[int]): add childs
         removeChilds (List[int]): remove childs
     """
+
+
 def auto_set_parts_situation(elements: List[int]) -> None:
     """
 
     Args:
         elementIDs (List[int]): element IDs
     """
+
+
 def auto_set_rough_volume_situation(elements: List[int]) -> None:
     """
 
     Args:
         elements (List[int]): element IDs
     """
+
+
 def rough_volume_situation_manual(element: int, addPartner: List[int], removePartner: List[int]) -> None:
     """
 
     Args:
         element (int): element ID
         addPartner (List[int]): add partner
         removePartner (List[int]): remove partner
     """
-def add_elements_to_detail(detail_group:element_module_detail, elements:List[int])->None:
+
+
+def add_elements_to_detail(elements: List[int], detail_group: int) -> None:
     """
+    detail groups:
+    0: without assigment
+
+    1: Angle; 2: Area; 3: Cross; 4: Edge; 5: End; 6: Line; 7: Open; 
+    8: T; 9: FloorArea; 10: FloorEnd; 11: FloorLine; 12: FloorOpen
 
     Args:
-        detail_group (element_module_detail): detail type
         elements (List[int]): element IDs
+        detail_group (int): a detail group
     """
+
+
 def get_all_nesting_raw_parts() -> List[int]:
     """Get all nesting raw parts.
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Returns:
         List[int]: element IDs
     """
+
+
 def get_standard_beam_list() -> List[str]:
     """Get standard beam list
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Returns:
         List[str]: standard beam names
     """
+
+
 def get_standard_panel_list() -> List[str]:
     """Get standard panel list
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Returns:
         List[str]: standard panel names
     """
+
+
 def get_reference_element(element: int) -> int:
     """Get reference element
-    
-    !!! Info
-            Available in script filled attributes
+
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         element (int): element ID
 
     Returns:
         int: element ID
-    """
+    """
+
+
+def create_linear_optimization(elements: List[int], optimization_number: int,
+                               total_length: float, start_cut: float,
+                               end_cut: float, saw_kerf: float, is_production_list: bool) -> int:
+    """create linear optimization
+
+    Args:
+        elements (List[int]): element IDs
+        optimization_number (int): number of nesting volume
+        total_length (float): total length nesting volume
+        start_cut (float): start cut
+        end_cut (float): end cut
+        saw_kerf (float): saw kerf
+        is_production_list (bool): measurements
+
+    Returns:
+        int: element ID
+    """
+
+
+def move_element_with_undo(elements: List[int], aVector: point_3d) -> None:
+    """Move elements and add 'step' to undo memory.
+
+     Examples:
+        >>> import element_controller as ec
+        >>> import geometry_controller as gc
+        >>> import cadwork
+        >>> element_ids = ec.get_active_identifiable_element_ids()
+        >>> ec.move_element_with_undo(element_ids, gc.get_yl(*element_ids) * 1500.)
+
+    Args:
+        elements (List[int]): element IDs
+        aVector (point_3d): a Target
+    """
```

### Comparing `cwapi3d-1.3.9/src/endtype_controller/__init__.pyi` & `cwapi3d-2.0.1/src/endtype_controller/__init__.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -49,53 +49,49 @@
 
     Returns:
         int: endtype id
     """
 def get_endtype_name(endtype_id: int) -> str:
     """Get endtype name
     
-    !!! Info
-            Available in script filled attributes
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         endtype_id (int): endtype ID
 
     Returns:
         str: endtype name
     """
 def get_endtype_name_end(element: int) -> str:
     """Get endtype name end
     
-    !!! Info
-            Available in script filled attributes
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         endtype_id (int): endtype ID
 
     Returns:
         str: endtype name
     """
 def get_endtype_name_facet(element: int, face_number: int) -> str:
     """Gets the endtypename of the face with a number
     
-    !!! Info
-            Available in script filled attributes
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         element (int): element ID
         face_number (int): face number
 
     Returns:
         str: endtype name facet
     """
 def get_endtype_name_start(element: int) -> str:
     """Gets the endtypename of the start face
     
-    !!! Info
-            Available in script filled attributes
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         element (int): element ID
 
     Returns:
         str: endtype name start
     """
```

### Comparing `cwapi3d-1.3.9/src/file_controller/__init__.pyi` & `cwapi3d-2.0.1/src/file_controller/__init__.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,197 +1,243 @@
 from typing import List
 
 from cadwork import point_3d
 
+
 def export_stl_file(elements: List[int], file: str) -> None:
     """ Exports an STL file
 
     Args:
         elements (List[int]): element IDs
         file (str): file path
     """
-def import_step_file(file: str, scale: float) -> List[int]: 
+
+
+def import_step_file(file: str, scale: float) -> List[int]:
     """Imports a STEP file
 
     Args:
         file (str): file path
         scale (float): file scale factor
 
     Returns:
         List[int]: element IDs
     """
-def import_step_file_with_message_option(file: str, scale: float, option: bool) -> List[int]: 
+
+
+def import_step_file_with_message_option(file: str, scale: float, option: bool) -> List[int]:
     """Imports a STEP file
 
     Args:
         file (str): file path
         scale (float): file scale factor
         option (bool): hide message
 
     Returns:
         List[int]: element IDs
     """
-def export_webgl(elements: List[int], file: str) -> None: 
-    """_summary_
+
+
+def export_webgl(elements: List[int], file: str) -> None:
+    """Exports a WebGL File
 
     Args:
-        elements (List[int]): _description_
-        file (str): _description_
+        elements (List[int]): element IDs
+        file (str): file path
     """
-def export_3d_file(elements: List[int], file: str) -> None: 
-    """Exports a WebGL file
+
+
+def export_3d_file(elements: List[int], file: str) -> None:
+    """Exports a 3d or 3dc file. Based on the extension in the file name.
+
+    Examples:
+    >>> export_3d_file(elements, "example.3dc")
+    >>> export_3d_file(elements, "example.3d")
 
     Args:
         elements (List[int]): element IDs
         file (str): file path
     """
-def import_sat_file(file: str, scale: float, option: bool) -> List[int]: 
+
+
+def import_sat_file(file: str, scale: float, option: bool) -> List[int]:
     """Imports an SAT file
 
     Args:
         file (str): file path
         scale (float): file scale factor
         option (bool): use binary mode
 
     Returns:
         List[int]: element IDs
     """
-def import_3dc_file(file: str) -> List[int]: 
+
+
+def import_3dc_file(file: str) -> List[int]:
     """Imports a 3DC file
 
     Args:
         file (str): file path
 
     Returns:
         List[int]: element IDs
     """
-def import_rhino_file(file: str, option: bool) -> List[int]: 
+
+
+def import_rhino_file(file: str, option: bool) -> List[int]:
     """Imports a Rhino file
 
     Args:
         file (str): file path
         option (bool): import without dialog
 
     Returns:
         List[int]: element IDs
     """
-def export_step_file(elements: List[int], file: str, scale: float, number: int, option: bool) -> None: 
+
+
+def export_step_file(elements: List[int], file: str, scale: float, number: int, option: bool) -> None:
     """Exports a STEP file
 
     Args:
         elements (List[int]): element IDs
         file (str): file path
         scale (float): file scale factor
         number (int): file version
         option (bool): use text mode
     """
-def import_3dz_file(file: str) -> None: 
+
+
+def import_3dz_file(file: str) -> None:
     """Imports a 3DZ file
 
     Args:
         file (str): file path
     """
-def export_obj_file(elements: List[int], file: str) -> None: 
+
+
+def export_obj_file(elements: List[int], file: str) -> None:
     """Exports a OBJ file
 
     Args:
         elements (List[int]): element IDs
         file (str): file path
     """
-def import_sat_file_silently(file: str, scale: float, option: bool) -> List[int]: 
+
+
+def import_sat_file_silently(file: str, scale: float, option: bool) -> List[int]:
     """_summary_
 
     Args:
         file (str): _description_
         scale (float): _description_
         option (bool): _description_
 
     Returns:
         List[int]: _description_
     """
-def export_fbx_file(elements: List[int], file: str, number: int) -> None: 
+
+
+def export_fbx_file(elements: List[int], file: str, number: int) -> None:
     """Export fbx file
 
     Args:
         elements (List[int]): element IDs
         file (str): file path
         number (int): fbx format  1 = "FBX binary(*.fbx) ; 2 = "FBX ascii(*.fbx)" ; 3 = "FBX encrypted(*.fbx)" ; 4 = "FBX 6.0 binary(*.fbx)" ; 5 = "FBX 6.0 ascii(*.fbx)" ; 6 = "FBX 6.0 encrypted(*.fbx)"
     """
-def import_3dc_file_with_glide(file: str) -> List[int]: 
+
+
+def import_3dc_file_with_glide(file: str) -> List[int]:
     """Imports a 3DC file with glide
 
     Args:
         file (str): file path
 
     Returns:
         List[int]: element IDs
     """
-def import_btl_file(file: str) -> None: 
+
+
+def import_btl_file(file: str) -> None:
     """Imports a BTL file
 
     Args:
         file (str): file path
     """
-def export_3dc_file(elements: List[int], file: str) -> None: 
+
+
+def export_3dc_file(elements: List[int], file: str) -> None:
     """Exports a 3D/3DC file
 
     Args:
         elements (List[int]): element IDs
         file (str): file path
     """
-def import_btl_file_for_nesting(file: str) -> None: 
+
+
+def import_btl_file_for_nesting(file: str) -> None:
     """Imports a BTL file for nesting
 
     Args:
         file (str): file path
     """
-def export_btl_file_for_nesting(file: str) -> None: 
+
+
+def export_btl_file_for_nesting(file: str) -> None:
     """Exports a BTL file for nesting
 
     Args:
         file (str): file path
     """
-def export_rhino_file(elements: List[int], file: str, version: int, user_efault_assignment: bool, write_standard_attributes: bool) -> None: 
+
+
+def export_rhino_file(elements: List[int], file: str, version: int, user_efault_assignment: bool, write_standard_attributes: bool) -> None:
     """Exports a 3dm rhino file
 
     Args:
         elements (List[int]): element IDs
         file (str): file path
         version (int): Rhino version V5.0 = 5, V6.0 = 6, V7.0 = 7
         user_efault_assignment (bool): true: default assignment is used; false: no attributes are exported
         write_standard_attributes (bool): see checkbox in assignment dialog
     """
-def export_sat_file(elements: List[int], file: str, scale: float, option: bool, number: int) -> None: 
+
+
+def export_sat_file(elements: List[int], file: str, scale: float, option: bool, number: int) -> None:
     """exports a SAT File
 
     Args:
         elements (List[int]): element IDs
         file (str): file path
         scale (float): scale factor
         option (bool): binary 
         number (int): version
     """
 
-def import_variant_file(file:str, insert_point:point_3d)-> List[int]:
+
+def import_variant_file(file: str, insert_point: point_3d) -> List[int]:
     """imports a variant by .val-File
 
     Args:
         file (str): file path
         insert_point (point_3d): insert point
 
     Returns:
         List[int]: element IDs
     """
 
-def set_blum_export_path(file:str) -> None:
+
+def set_blum_export_path(file: str) -> None:
     """Set blum export path
 
     Args:
         file (str): file path
     """
 
+
 def get_blum_export_path() -> str:
     """Get blum export path
 
     Returns:
         str: file path
     """
```

### Comparing `cwapi3d-1.3.9/src/scene_controller/__init__.pyi` & `cwapi3d-2.0.1/src/scene_controller/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,70 +1,89 @@
 from typing import List
 
 
-def add_scene(name: str) -> bool: 
+def add_scene(name: str) -> bool:
     """
 
     Args:
         name (str): scene name
 
     Returns:
         bool: result
     """
-def rename_scene(old_name: str, new_name: str) -> bool: 
+
+
+def rename_scene(old_name: str, new_name: str) -> bool:
     """
 
     Args:
         old_name (str): old scene name
         new_name (str): new scene name
 
     Returns:
         bool: result
     """
-def delete_scene(name: str) -> bool: 
+
+
+def delete_scene(name: str) -> bool:
     """
 
     Args:
         name (str): name
 
     Returns:
         bool: result
     """
-def add_elements_to_scene(name: str, elements: List[int]) -> bool: 
+
+
+def add_elements_to_scene(name: str, elements: List[int]) -> bool:
     """
 
     Args:
         name (str): name
         elements (List[int]): element IDs
 
     Returns:
         bool: result
     """
-def remove_elements_from_scene(name: str, elements: List[int]) -> bool: 
+
+
+def remove_elements_from_scene(name: str, elements: List[int]) -> bool:
     """
 
     Args:
         name (str): name
         elements (List[int]): element IDs
 
     Returns:
         bool: result
     """
-def get_elements_from_scene(name: str) -> List[int]: 
+
+
+def get_elements_from_scene(name: str) -> List[int]:
     """
 
     Args:
         name (str): name
 
     Returns:
         List[int]: element IDs
     """
-def activate_scene(name: str) -> bool: 
+
+
+def activate_scene(name: str) -> bool:
     """
 
     Args:
         name (str): name
 
     Returns:
         bool: result
     """
 
+
+def get_scene_list() -> List[str]:
+    """get list of scenes in use
+
+    Returns:
+        List[str]: scenes
+    """
```

### Comparing `cwapi3d-1.3.9/src/shop_drawing_controller/__init__.pyi` & `cwapi3d-2.0.1/src/shop_drawing_controller/__init__.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -32,34 +32,34 @@
 def export_wall_with_clipboard(clipboard: int, elements: List[int]) -> None: 
     """
 
     Args:
         clipboard (int): clipboard element
         elements (List[int]): element IDs
     """
-def export_export_solid_with_clipboard(clipboard: int, elements: List[int]) -> None: 
+def export_export_solid_with_clipboard(clipboard: int, export_solid_ids: List[int]) -> None: 
     """
 
     Args:
         clipboard (int): clipboard element
-        elements (List[int]): element IDs
+        export_solid_ids (List[int]): element IDs
     """
 def export_piece_by_piece_with_clipboard(clipboard: int, elements: List[int]) -> None: 
     """
 
     Args:
         clipboard (int): clipboard element
         elements (List[int]): element IDs
     """
-def assign_export_solid(elements: List[int], other_elements: List[int]) -> None: 
+def assign_export_solid(a_export_solid_element: List[int], elements_to_assign: List[int]) -> None: 
     """Assigns elements to an export solid
 
     Args:
-        elements (List[int]): element IDs
-        other_elements (List[int]): element IDs
+        a_export_solid_element (List[int]): element ID export solid
+        other_elements (List[int]): element IDs to assign
     """
 def export_container_with_clipboard(clipboard: int, elements: List[int]) -> None: 
     """
 
     Args:
         clipboard (int): clipboard element
         elements (List[int]): element IDs
```

### Comparing `cwapi3d-1.3.9/src/visualization_controller/__init__.pyi` & `cwapi3d-2.0.1/src/bim_controller/__init__.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,223 +1,172 @@
 from typing import List
-from cadwork import (rgb_color,
-                     visibility_state,
-                     activation_state)
+from cadwork import ifc_2x3_element_type
 
 
-def get_color(element: int) -> int: 
-    """
-    
-    !!! Info
-            Available in script filled attributes
+def get_ifc_guid(element: int) -> str: 
+    """Get readable ifc guid. Convert readable guid to IfcGuid, see -> https://github.com/IfcOpenShell/IfcOpenShell/blob/master/src/ifcopenshell-python/ifcopenshell/guid.py
 
     Args:
-        number (int): element ID
+        element (int): element ID
 
     Returns:
-        int: color number
-    """
-def set_color(element: int, color: int) -> None: 
+        str: readable guid
     """
+def set_building_and_storey(elements: List[int], building: str, storey: str) -> None: 
+    """Set bulding and storey 
+    
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
-        element (int): element ID
-        color (int): color number
-    """
-def get_opengl_color(element: int) -> rgb_color: 
+        elements (List[int]): element IDs
+        building (str): building name
+        storey (str): storey name
     """
+def get_building(element: int) -> str: 
+    """Get building name
     
-    !!! Info
-            Available in script filled attributes
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         element (int): element ID
 
     Returns:
-        rgb_color: rgb color 
+        str: building name
     """
-def set_opengl_color(element: int, color: rgb_color) -> None: 
-    """_summary_
+def get_storey(element: int) -> str: 
+    """Get Storey
+    
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
         element (int): element ID
-        color (rgb_color): rgb color
+
+    Returns:
+        str: storey name
     """
-def is_active(element: int) -> bool: 
-    """Tests if element is active
+
+def get_ifc2x3_element_type(element: int) -> ifc_2x3_element_type: 
+    """Get IFC element type. 
 
     Args:
         element (int): element ID
 
     Returns:
-        bool: result
+        ifc_2x3_element_type: ifc type 
     """
-def set_active(elements: List[int]) -> None: 
-    """Set elements active
+def set_ifc2x3_element_type(elements: List[int], ifc_2x3_element_type: ifc_2x3_element_type) -> None: 
+    """Set IFC element type.
 
     Args:
         elements (List[int]): element IDs
+        ifc_2x3_element_type (ifc_2x3_element_type): cadwork ifc element type
     """
-def set_inactive(elements: List[int]) -> None: 
-    """Set elements inactive
+def import_ifc_as_graphical_object(file: str) -> None: 
+    """Import ifc as graphical object
 
     Args:
-        elements (List[int]): element IDs
+        file (str): path to ifc file
     """
-def is_visible(element: int) -> bool: 
-    """Check if element is visible
+def import_bcf(file: str) -> None: 
+    """Import bcf file.
 
     Args:
-        element (int): element ID
-
-    Returns:
-        bool: result
+        file (str): path to bcf file
     """
-def set_visible(elements: List[int]) -> None: 
-    """Sets the element visible
+def export_bcf(file: str) -> None: 
+    """Export bcf file. 
 
     Args:
-        elements (List[int]): element IDs
+        file (str): Destination path 
     """
-def set_invisible(elements: List[int]) -> None: 
-    """Sets the element invisible
+def export_ifc(elements: List[int], file: str) -> None: 
+    """Export an ifc file. 
 
     Args:
         elements (List[int]): element IDs
+        file (str): Destination path 
     """
-def is_immutable(element: int) -> bool: 
-    """ests if the element is immutable
+
+def convert_exchange_objects(elements: List[int]) -> List[int]:
+    """Convert exchange objects to cadwork elements 
 
     Args:
-        element (int): element ID
+        elements (List[int]): element IDs
 
     Returns:
-        bool: result
+        List[int]: converted elements 
     """
-def set_immutable(elements: List[int]) -> None: 
-    """Sets the element immutable
 
-    Args:
-        elements (List[int]): element IDs
-    """
-def set_mutable(elements: List[int]) -> None: 
-    """Sets the element mutable
+def get_all_buildings() -> List[str]:
+    """Get all, in 3D, existing buildings 
+    
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
-    Args:
-        elements (List[int]): element IDs
-    """
-def show_all_elements() -> None: 
-    """Shows all elements
-    """
-def hide_all_elements() -> None: 
-    """Hide all elements
-    """
-def zoom_all_elements() -> None: 
-    """zoom all elements
-    """
-def zoom_active_elements() -> None: 
-    """zoom only active elements
-    """
-def refresh() -> None: 
-    """Refresh the drawing area
+    Returns:
+        List[str]: building names 
     """
-def set_material(elements: List[int], element: int) -> None: 
-    """Sets the element material
 
-    Args:
-        elements (List[int]): element IDs
-        element (int): element ID
-    """
-def get_material(element: int) -> int: 
-    """Gets the element material
+def get_all_storeys(building_name:str) -> List[str]:
+    """Get all Storeys from a building.
     
-    !!! Info
-            Available in script filled attributes
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
-        element (int): element ID
+        building_name (str): building name
 
     Returns:
-        int: material ID
+        List[str]: storey names 
     """
-def save_visibility_state() -> visibility_state: 
-    """Saves the visibility state
 
-    Returns:
-        visibility_state: visibility state
-    """
-def restore_visibility_state(state: visibility_state) -> None: 
-    """Restores the visibility state
+
+def get_storey_height(building_name:str, storey_name:str) -> float:
+    """Get the storey height. 
+    
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
-        state (visibility_state): visibility state
-    """
-def save_activation_state() -> activation_state: 
-    """_summary_
+        building_name (str): building name
+        storey_name (str): storey name
 
     Returns:
-        activation_state: _description_
+        float: storey elevation height
     """
-def restore_activation_state(state: activation_state) -> None: 
-    """Saves the activation state
+
+
+def import_ifc_return_exchange_objects(file_path:str) -> None:
+    """Import ifc as exchange objects
 
     Args:
-        state (activation_state): activation state
-    """
-def show_view_positive_x() -> None: 
-    """
-    """
-def show_view_negative_x() -> None: 
-    """
-    """
-def show_view_positive_y() -> None: 
-    """
-    """
-def show_view_negative_y() -> None: 
-    """
-    """
-def show_view_positive_z() -> None: 
-    """
-    """
-def show_view_negative_z() -> None: 
-    """
-    """
-def show_view_standard_axo() -> None: 
-    """
-    """
-def show_view_wireframe() -> None: 
-    """
+        file_path (str): file path
     """
-def show_view_hidden_lines() -> None: 
-    """
-    """
-def show_view_dashed_hidden_lines() -> None: 
-    """
-    """
-def show_view_shaded2() -> None: 
-    """
-    """
-def show_view_shaded1() -> None: 
-    """
-    """
-def is_selectable(element: int) -> bool: 
-    """Returns if the element is selectable
 
-    Args:
-        element (int): element ID
+def set_storey_height(building_name:str, storey_name:str, height:float) -> None:
+    """Set the storey elevation. 
 
-    Returns:
-        bool: result
+    Args:
+        building_name (str): building name
+        storey_name (str): storey name
+        height (float): storey elevation 
     """
-def set_unselectable(elements: List[int]) -> None: 
-    """Sets a list of elements unselectable
+
+def get_ifc2x3_element_type_string(ifc_2x3_element_type: ifc_2x3_element_type) -> str:
+    """Get ifc tpye as a string
+    
+    [:information_source: Available for script filled attributes](#){.mark-text}
 
     Args:
-        elements (List[int]): element IDs
+        ifc_2x3_element_type (ifc_2x3_element_type): cadwork ifc element type
+
+    Returns:
+        str: entity name
     """
-def set_selectable(elements: List[int]) -> None: 
-    """Sets a list of elements selectable
+def get_ifc2x3_element_type_display_string(ifc_2x3_element_type: ifc_2x3_element_type) -> str:
+    """Get ifc tpye display string
 
+    [:information_source: Available for script filled attributes](#){.mark-text}
+            
     Args:
-        elements (List[int]): element IDs
-    """
+        ifc_2x3_element_type (ifc_2x3_element_type): cadwork ifc element type
 
+    Returns:
+        str: entity name
+    """
```

