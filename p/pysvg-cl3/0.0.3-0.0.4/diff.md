# Comparing `tmp/pysvg-cl3-0.0.3.tar.gz` & `tmp/pysvg-cl3-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysvg-cl3-0.0.3.tar", last modified: Tue May 16 15:16:23 2023, max compression
+gzip compressed data, was "pysvg-cl3-0.0.4.tar", last modified: Tue May 16 18:02:08 2023, max compression
```

## Comparing `pysvg-cl3-0.0.3.tar` & `pysvg-cl3-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-16 15:16:23.828563 pysvg-cl3-0.0.3/
--rw-r--r--   0 lacasta    (503) staff       (20)    35087 2023-05-16 14:25:20.000000 pysvg-cl3-0.0.3/LICENSE
--rw-r--r--   0 lacasta    (503) staff       (20)      556 2023-05-16 15:16:23.828295 pysvg-cl3-0.0.3/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      102 2023-05-16 14:16:46.000000 pysvg-cl3-0.0.3/README.md
--rw-r--r--   0 lacasta    (503) staff       (20)      611 2023-05-16 15:13:22.000000 pysvg-cl3-0.0.3/pyproject.toml
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-16 15:16:23.826364 pysvg-cl3-0.0.3/pysvg_cl3/
--rw-r--r--   0 lacasta    (503) staff       (20)     9045 2023-05-16 14:03:41.000000 pysvg-cl3-0.0.3/pysvg_cl3/DXFPainter.py
--rw-r--r--   0 lacasta    (503) staff       (20)     5026 2023-05-16 14:03:21.000000 pysvg-cl3-0.0.3/pysvg_cl3/GDSPainter.py
--rw-r--r--   0 lacasta    (503) staff       (20)     8475 2023-05-16 14:04:09.000000 pysvg-cl3-0.0.3/pysvg_cl3/Painter.py
--rw-r--r--   0 lacasta    (503) staff       (20)     4572 2020-11-28 10:22:00.000000 pysvg-cl3-0.0.3/pysvg_cl3/Path.py
--rw-r--r--   0 lacasta    (503) staff       (20)       21 2023-05-16 15:16:17.000000 pysvg-cl3-0.0.3/pysvg_cl3/__init__.py
--rw-r--r--   0 lacasta    (503) staff       (20)    28025 2023-05-16 14:03:57.000000 pysvg-cl3-0.0.3/pysvg_cl3/matrix.py
--rw-r--r--   0 lacasta    (503) staff       (20)    69301 2023-05-16 14:08:08.000000 pysvg-cl3-0.0.3/pysvg_cl3/svg.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-16 15:16:23.827877 pysvg-cl3-0.0.3/pysvg_cl3.egg-info/
--rw-r--r--   0 lacasta    (503) staff       (20)      556 2023-05-16 15:16:23.000000 pysvg-cl3-0.0.3/pysvg_cl3.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      342 2023-05-16 15:16:23.000000 pysvg-cl3-0.0.3/pysvg_cl3.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-05-16 15:16:23.000000 pysvg-cl3-0.0.3/pysvg_cl3.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       26 2023-05-16 15:16:23.000000 pysvg-cl3-0.0.3/pysvg_cl3.egg-info/requires.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       10 2023-05-16 15:16:23.000000 pysvg-cl3-0.0.3/pysvg_cl3.egg-info/top_level.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-05-16 15:16:23.828639 pysvg-cl3-0.0.3/setup.cfg
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-16 18:02:08.545488 pysvg-cl3-0.0.4/
+-rw-r--r--   0 lacasta    (503) staff       (20)    35087 2023-05-16 14:25:20.000000 pysvg-cl3-0.0.4/LICENSE
+-rw-r--r--   0 lacasta    (503) staff       (20)      556 2023-05-16 18:02:08.545215 pysvg-cl3-0.0.4/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      102 2023-05-16 14:16:46.000000 pysvg-cl3-0.0.4/README.md
+-rw-r--r--   0 lacasta    (503) staff       (20)      611 2023-05-16 18:01:48.000000 pysvg-cl3-0.0.4/pyproject.toml
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-16 18:02:08.542669 pysvg-cl3-0.0.4/pysvg_cl3/
+-rw-r--r--   0 lacasta    (503) staff       (20)     9075 2023-05-16 16:54:45.000000 pysvg-cl3-0.0.4/pysvg_cl3/DXFPainter.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     5056 2023-05-16 16:55:01.000000 pysvg-cl3-0.0.4/pysvg_cl3/GDSPainter.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     8485 2023-05-16 16:55:22.000000 pysvg-cl3-0.0.4/pysvg_cl3/Painter.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     4582 2023-05-16 16:54:17.000000 pysvg-cl3-0.0.4/pysvg_cl3/Path.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     4626 2023-05-16 16:55:39.000000 pysvg-cl3-0.0.4/pysvg_cl3/SVGPainter.py
+-rw-r--r--   0 lacasta    (503) staff       (20)       21 2023-05-16 18:02:02.000000 pysvg-cl3-0.0.4/pysvg_cl3/__init__.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    28025 2023-05-16 14:03:57.000000 pysvg-cl3-0.0.4/pysvg_cl3/matrix.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    69321 2023-05-16 16:54:07.000000 pysvg-cl3-0.0.4/pysvg_cl3/svg.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-16 18:02:08.544863 pysvg-cl3-0.0.4/pysvg_cl3.egg-info/
+-rw-r--r--   0 lacasta    (503) staff       (20)      556 2023-05-16 18:02:08.000000 pysvg-cl3-0.0.4/pysvg_cl3.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      366 2023-05-16 18:02:08.000000 pysvg-cl3-0.0.4/pysvg_cl3.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-05-16 18:02:08.000000 pysvg-cl3-0.0.4/pysvg_cl3.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       26 2023-05-16 18:02:08.000000 pysvg-cl3-0.0.4/pysvg_cl3.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       10 2023-05-16 18:02:08.000000 pysvg-cl3-0.0.4/pysvg_cl3.egg-info/top_level.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-05-16 18:02:08.545565 pysvg-cl3-0.0.4/setup.cfg
```

### Comparing `pysvg-cl3-0.0.3/LICENSE` & `pysvg-cl3-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pysvg-cl3-0.0.3/PKG-INFO` & `pysvg-cl3-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysvg-cl3
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python class to build SVG and 'paint' them as DXF or GDS.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pysvg-cl3-0.0.3/pyproject.toml` & `pysvg-cl3-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysvg-cl3"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@cern.ch" },
 ]
 description = "A python class to build SVG and 'paint' them as DXF or GDS."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `pysvg-cl3-0.0.3/pysvg_cl3/DXFPainter.py` & `pysvg-cl3-0.0.4/pysvg_cl3/DXFPainter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Draws in a DXF file."""
 import math
 
 import ezdxf
 
-from matrix import Point
-from Painter import Layout
-from Painter import Painter
+from pysvg_cl3.matrix import Point
+from pysvg_cl3.Painter import Layout
+from pysvg_cl3.Painter import Painter
 
 
 class DXFUnits(object):
     """Stores conversions among units.
 
     Base Unit is mm=1, however, to avoid rounding errors we use um=1 and scale
     at the very end.
```

### Comparing `pysvg-cl3-0.0.3/pysvg_cl3/GDSPainter.py` & `pysvg-cl3-0.0.4/pysvg_cl3/GDSPainter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 """ Draws in a GDS file
 """
 import math
 
 import gdspy
 
-from matrix import Point
-from Painter import Layout
-from Painter import Painter
+from pysvg_cl3.matrix import Point
+from pysvg_cl3.Painter import Layout
+from pysvg_cl3.Painter import Painter
 
 twopi = 2.0*math.pi
 
 
 class GDSUnits(object):
     """ A class which stores conversions among units.
         Base Unit is mm=1
```

### Comparing `pysvg-cl3-0.0.3/pysvg_cl3/Painter.py` & `pysvg-cl3-0.0.4/pysvg_cl3/Painter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Defines the interface of a painter."""
 
-from Path import Path
+from pysvg_cl3.Path import Path
 
 default_unit_scale = 1000.0
 
 
 def transform_units(P, scale=default_unit_scale):
     """Closure for transform and unit conversion."""
     return P.x*scale, P.y*scale
```

### Comparing `pysvg-cl3-0.0.3/pysvg_cl3/Path.py` & `pysvg-cl3-0.0.4/pysvg_cl3/Path.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from matrix import Point, Line
+from pysvg_cl3.matrix import Point, Line
 
 
 class Path(object):
     """ This class defines a collection of subpaths that define a path.
         Each subpath is a collection of points. Subpaths are started by the
         move_to method.
```

### Comparing `pysvg-cl3-0.0.3/pysvg_cl3/matrix.py` & `pysvg-cl3-0.0.4/pysvg_cl3/matrix.py`

 * *Files identical despite different names*

### Comparing `pysvg-cl3-0.0.3/pysvg_cl3/svg.py` & `pysvg-cl3-0.0.4/pysvg_cl3/svg.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import math
 import os
 import re
 import subprocess
 import uuid
 import xml.dom.minidom
 
-from matrix import Matrix
-from matrix import Point
+from pysvg_cl3.matrix import Matrix
+from pysvg_cl3.matrix import Point
 
 SVG_NS = "http://www.w3.org/2000/svg"
 XLINK_NS = "http://www.w3.org/1999/xlink"
 SODIPODY_NS = "http://sodipodi.sourceforge.net/DTD/sodipodi-0.dtd"
 INKSCAPE_NS = "http://www.inkscape.org/namespaces/inkscape"
 
 SVG_HEADER = '''<?xml version="1.0" encoding="UTF-8"?>
```

### Comparing `pysvg-cl3-0.0.3/pysvg_cl3.egg-info/PKG-INFO` & `pysvg-cl3-0.0.4/pysvg_cl3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysvg-cl3
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python class to build SVG and 'paint' them as DXF or GDS.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

