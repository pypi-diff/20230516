# Comparing `tmp/cerc-geometry-0.1.1.tar.gz` & `tmp/cerc-geometry-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/peteryefi/Desktop/dompark/geometry/dist/.tmp-_nykkphs/cerc-geometry-0.1.1.tar", last modified: Mon May 15 23:58:34 2023, max compression
+gzip compressed data, was "/Users/peteryefi/Desktop/dompark/geometry/dist/.tmp-mrjemjyz/cerc-geometry-1.0.1.tar", last modified: Tue May 16 00:07:09 2023, max compression
```

## Comparing `cerc-geometry-0.1.1.tar` & `cerc-geometry-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-15 23:58:34.018733 cerc-geometry-0.1.1/
--rw-r--r--   0 peteryefi   (501) staff       (20)     7431 2023-05-11 00:53:33.000000 cerc-geometry-0.1.1/LICENSE.md
--rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-15 23:58:34.018055 cerc-geometry-0.1.1/PKG-INFO
--rw-r--r--   0 peteryefi   (501) staff       (20)      522 2023-05-12 17:30:08.000000 cerc-geometry-0.1.1/README.md
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-15 23:58:34.004981 cerc-geometry-0.1.1/cerc_geometry.egg-info/
--rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-15 23:58:33.000000 cerc-geometry-0.1.1/cerc_geometry.egg-info/PKG-INFO
--rw-r--r--   0 peteryefi   (501) staff       (20)      442 2023-05-15 23:58:33.000000 cerc-geometry-0.1.1/cerc_geometry.egg-info/SOURCES.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)        1 2023-05-15 23:58:33.000000 cerc-geometry-0.1.1/cerc_geometry.egg-info/dependency_links.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)       41 2023-05-15 23:58:33.000000 cerc-geometry-0.1.1/cerc_geometry.egg-info/requires.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)        4 2023-05-15 23:58:33.000000 cerc-geometry-0.1.1/cerc_geometry.egg-info/top_level.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)       99 2023-05-15 23:40:38.000000 cerc-geometry-0.1.1/pyproject.toml
--rw-r--r--   0 peteryefi   (501) staff       (20)       30 2023-05-12 21:28:55.000000 cerc-geometry-0.1.1/requirements.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)       38 2023-05-15 23:58:34.019222 cerc-geometry-0.1.1/setup.cfg
--rw-r--r--   0 peteryefi   (501) staff       (20)     1310 2023-05-15 23:55:16.000000 cerc-geometry-0.1.1/setup.py
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-15 23:58:34.008572 cerc-geometry-0.1.1/src/
--rw-r--r--   0 peteryefi   (501) staff       (20)      140 2023-05-15 23:39:05.000000 cerc-geometry-0.1.1/src/__init__.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     5388 2023-05-15 23:21:05.000000 cerc-geometry-0.1.1/src/helper.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     2168 2023-05-15 23:21:05.000000 cerc-geometry-0.1.1/src/plane.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1002 2023-05-15 23:21:05.000000 cerc-geometry-0.1.1/src/point.py
--rw-r--r--   0 peteryefi   (501) staff       (20)    14594 2023-05-15 23:21:05.000000 cerc-geometry-0.1.1/src/polygon.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     6590 2023-05-15 23:21:05.000000 cerc-geometry-0.1.1/src/polyhedron.py
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-15 23:58:34.016065 cerc-geometry-0.1.1/tests/
--rw-r--r--   0 peteryefi   (501) staff       (20)     1956 2023-05-15 23:39:05.000000 cerc-geometry-0.1.1/tests/test_helper.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      726 2023-05-15 23:39:05.000000 cerc-geometry-0.1.1/tests/test_plane.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      837 2023-05-15 23:39:05.000000 cerc-geometry-0.1.1/tests/test_point.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1503 2023-05-15 23:39:05.000000 cerc-geometry-0.1.1/tests/test_polygon.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1066 2023-05-15 23:39:05.000000 cerc-geometry-0.1.1/tests/test_polyhedron.py
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-16 00:07:09.424671 cerc-geometry-1.0.1/
+-rw-r--r--   0 peteryefi   (501) staff       (20)     7431 2023-05-11 00:53:33.000000 cerc-geometry-1.0.1/LICENSE.md
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-16 00:07:09.424296 cerc-geometry-1.0.1/PKG-INFO
+-rw-r--r--   0 peteryefi   (501) staff       (20)      522 2023-05-12 17:30:08.000000 cerc-geometry-1.0.1/README.md
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-16 00:07:09.414983 cerc-geometry-1.0.1/cerc_geometry.egg-info/
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-16 00:07:09.000000 cerc-geometry-1.0.1/cerc_geometry.egg-info/PKG-INFO
+-rw-r--r--   0 peteryefi   (501) staff       (20)      472 2023-05-16 00:07:09.000000 cerc-geometry-1.0.1/cerc_geometry.egg-info/SOURCES.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)        1 2023-05-16 00:07:09.000000 cerc-geometry-1.0.1/cerc_geometry.egg-info/dependency_links.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)       41 2023-05-16 00:07:09.000000 cerc-geometry-1.0.1/cerc_geometry.egg-info/requires.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)        9 2023-05-16 00:07:09.000000 cerc-geometry-1.0.1/cerc_geometry.egg-info/top_level.txt
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-16 00:07:09.419933 cerc-geometry-1.0.1/geometry/
+-rw-r--r--   0 peteryefi   (501) staff       (20)      140 2023-05-15 23:39:05.000000 cerc-geometry-1.0.1/geometry/__init__.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     5398 2023-05-16 00:05:51.000000 cerc-geometry-1.0.1/geometry/helper.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     2168 2023-05-15 23:21:05.000000 cerc-geometry-1.0.1/geometry/plane.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1002 2023-05-15 23:21:05.000000 cerc-geometry-1.0.1/geometry/point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)    14604 2023-05-16 00:05:51.000000 cerc-geometry-1.0.1/geometry/polygon.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     6590 2023-05-15 23:21:05.000000 cerc-geometry-1.0.1/geometry/polyhedron.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)       99 2023-05-15 23:40:38.000000 cerc-geometry-1.0.1/pyproject.toml
+-rw-r--r--   0 peteryefi   (501) staff       (20)       30 2023-05-12 21:28:55.000000 cerc-geometry-1.0.1/requirements.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)       38 2023-05-16 00:07:09.424796 cerc-geometry-1.0.1/setup.cfg
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1320 2023-05-16 00:06:45.000000 cerc-geometry-1.0.1/setup.py
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-16 00:07:09.423680 cerc-geometry-1.0.1/tests/
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1961 2023-05-16 00:05:50.000000 cerc-geometry-1.0.1/tests/test_helper.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      736 2023-05-16 00:05:50.000000 cerc-geometry-1.0.1/tests/test_plane.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      842 2023-05-16 00:05:50.000000 cerc-geometry-1.0.1/tests/test_point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1513 2023-05-16 00:05:50.000000 cerc-geometry-1.0.1/tests/test_polygon.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1076 2023-05-16 00:05:50.000000 cerc-geometry-1.0.1/tests/test_polyhedron.py
```

### Comparing `cerc-geometry-0.1.1/LICENSE.md` & `cerc-geometry-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cerc-geometry-0.1.1/PKG-INFO` & `cerc-geometry-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-geometry
-Version: 0.1.1
+Version: 1.0.1
 Summary: CERC Geometry Library with different modules to manipulate geometric objects
 Home-page: https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Author: CERC
 Author-email:  cerc@concordia.ca
 Project-URL: Repository, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Project-URL: Bug Tracker, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cerc-geometry-0.1.1/README.md` & `cerc-geometry-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cerc-geometry-0.1.1/cerc_geometry.egg-info/PKG-INFO` & `cerc-geometry-1.0.1/cerc_geometry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-geometry
-Version: 0.1.1
+Version: 1.0.1
 Summary: CERC Geometry Library with different modules to manipulate geometric objects
 Home-page: https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Author: CERC
 Author-email:  cerc@concordia.ca
 Project-URL: Repository, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Project-URL: Bug Tracker, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cerc-geometry-0.1.1/setup.py` & `cerc-geometry-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     for requirement
     in pkg_resources.parse_requirements(r)
   ]
 install_requires.append('setuptools')
 
 setuptools.setup(
   name="cerc-geometry",
-  version="0.1.1",
+  version="1.0.1",
   author="CERC",
   author_email=" cerc@concordia.ca",
   description="CERC Geometry Library with different modules to manipulate geometric objects",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry",
   project_urls={
@@ -28,14 +28,14 @@
   },
   classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)",
     "Operating System :: OS Independent",
   ],
   data_files=[
-    ('src', glob.glob('requirements.txt')),
+    ('geometry', glob.glob('requirements.txt')),
   ],
-  packages=['src'],
+  packages=['geometry'],
   setup_requires=install_requires,
   install_requires=install_requires,
   python_requires=">=3.6"
 )
```

### Comparing `cerc-geometry-0.1.1/src/helper.py` & `cerc-geometry-1.0.1/geometry/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-Geometry class contains different src functions for manipulating
-2D and 3D src objects
+Geometry class contains different geometry functions for manipulating
+2D and 3D geometry objects
 SPDX - License - Identifier: LGPL - 3.0 - or -later
 Copyright © 2023 Concordia CERC group
 """
 import numpy as np
 from typing import List
 import sys
 import math
```

### Comparing `cerc-geometry-0.1.1/src/plane.py` & `cerc-geometry-1.0.1/geometry/plane.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-0.1.1/src/point.py` & `cerc-geometry-1.0.1/geometry/point.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-0.1.1/src/polygon.py` & `cerc-geometry-1.0.1/geometry/polygon.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from typing import List
 import numpy as np
 from trimesh import Trimesh
 import trimesh.intersections
 import trimesh.creation
 import trimesh.geometry
 from shapely.geometry.polygon import Polygon as shapley_polygon
-from src.point import Point
-from src.plane import Plane
+from geometry.point import Point
+from geometry.plane import Plane
 
 EPSILON = 0.0000001
 
 
 class Polygon:
   """
   Polygon class
```

### Comparing `cerc-geometry-0.1.1/src/polyhedron.py` & `cerc-geometry-1.0.1/geometry/polyhedron.py`

 * *Files identical despite different names*

### Comparing `cerc-geometry-0.1.1/tests/test_helper.py` & `cerc-geometry-1.0.1/tests/test_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src import Helper
+from geometry import Helper
 from unittest import TestCase
 import numpy as np
 
 
 class TestHelper(TestCase):
   
   def setUp(self) -> None:
```

### Comparing `cerc-geometry-0.1.1/tests/test_plane.py` & `cerc-geometry-1.0.1/tests/test_plane.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from src import Plane
-from src import Point
+from geometry import Plane
+from geometry import Point
 from unittest import TestCase
 import numpy as np
 
 
 class TestPlane(TestCase):
   
   def setUp(self) -> None:
```

### Comparing `cerc-geometry-0.1.1/tests/test_point.py` & `cerc-geometry-1.0.1/tests/test_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from unittest import TestCase
-from src import Point
+from geometry import Point
 import numpy as np
 
 
 class TestPoint(TestCase):
   
   def test_positive_distance_to_point(self):
     point = Point(np.array([10, 5]))
```

### Comparing `cerc-geometry-0.1.1/tests/test_polygon.py` & `cerc-geometry-1.0.1/tests/test_polygon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from unittest import TestCase
-from src import Point
-from src import Polygon
+from geometry import Point
+from geometry import Polygon
 import numpy as np
 
 
 class TestPolygon(TestCase):
   
   def setUp(self) -> None:
     self._coordinates = [[-1.3125511246773556, 7.224814483190954], [-1.3131144073658163, 7.225133803311778],
```

### Comparing `cerc-geometry-0.1.1/tests/test_polyhedron.py` & `cerc-geometry-1.0.1/tests/test_polyhedron.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from unittest import TestCase
-from src import Polyhedron
-from src import Polygon
+from geometry import Polyhedron
+from geometry import Polygon
 import numpy as np
 
 
 class TestPolyhedron(TestCase):
   
   def setUp(self) -> None:
     self._coordinates = [[-1.3125511246773556, 7.224814483190954], [-1.3131144073658163, 7.225133803311778],
```

