# Comparing `tmp/clipping-5.1.2.tar.gz` & `tmp/clipping-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipping-5.1.2.tar", last modified: Sun Sep  4 21:46:06 2022, max compression
+gzip compressed data, was "clipping-6.0.0.tar", last modified: Mon May 15 22:03:51 2023, max compression
```

## Comparing `clipping-5.1.2.tar` & `clipping-6.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 21:46:06.609045 clipping-5.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-09-04 21:45:53.000000 clipping-5.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-09-04 21:45:53.000000 clipping-5.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9750 2022-09-04 21:46:06.609045 clipping-5.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8907 2022-09-04 21:45:53.000000 clipping-5.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 21:46:06.605045 clipping-5.1.2/clipping/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-09-04 21:45:53.000000 clipping-5.1.2/clipping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 21:46:06.609045 clipping-5.1.2/clipping/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-04 21:45:53.000000 clipping-5.1.2/clipping/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15868 2022-09-04 21:45:53.000000 clipping-5.1.2/clipping/core/bounding.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-09-04 21:45:53.000000 clipping-5.1.2/clipping/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)    15960 2022-09-04 21:45:53.000000 clipping-5.1.2/clipping/core/event.py
--rw-r--r--   0 runner    (1001) docker     (121)    20111 2022-09-04 21:45:53.000000 clipping-5.1.2/clipping/core/events_queue.py
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-09-04 21:45:53.000000 clipping-5.1.2/clipping/core/hints.py
--rw-r--r--   0 runner    (1001) docker     (121)    11009 2022-09-04 21:45:53.000000 clipping-5.1.2/clipping/core/holeless.py
--rw-r--r--   0 runner    (1001) docker     (121)    20693 2022-09-04 21:45:53.000000 clipping-5.1.2/clipping/core/holey.py
--rw-r--r--   0 runner    (1001) docker     (121)    26120 2022-09-04 21:45:53.000000 clipping-5.1.2/clipping/core/linear.py
--rw-r--r--   0 runner    (1001) docker     (121)    12122 2022-09-04 21:45:53.000000 clipping-5.1.2/clipping/core/mixed.py
--rw-r--r--   0 runner    (1001) docker     (121)     2542 2022-09-04 21:45:53.000000 clipping-5.1.2/clipping/core/operands.py
--rw-r--r--   0 runner    (1001) docker     (121)     7812 2022-09-04 21:45:53.000000 clipping-5.1.2/clipping/core/sweep_line.py
--rw-r--r--   0 runner    (1001) docker     (121)     2724 2022-09-04 21:45:53.000000 clipping-5.1.2/clipping/core/unpacking.py
--rw-r--r--   0 runner    (1001) docker     (121)     3878 2022-09-04 21:45:53.000000 clipping-5.1.2/clipping/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-09-04 21:45:53.000000 clipping-5.1.2/clipping/hints.py
--rw-r--r--   0 runner    (1001) docker     (121)   220391 2022-09-04 21:45:53.000000 clipping-5.1.2/clipping/planar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 21:46:06.609045 clipping-5.1.2/clipping.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9750 2022-09-04 21:46:06.000000 clipping-5.1.2/clipping.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-09-04 21:46:06.000000 clipping-5.1.2/clipping.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-04 21:46:06.000000 clipping-5.1.2/clipping.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-04 21:46:06.000000 clipping-5.1.2/clipping.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-04 21:46:06.000000 clipping-5.1.2/clipping.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-04 21:45:53.000000 clipping-5.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-04 21:46:06.609045 clipping-5.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1294 2022-09-04 21:45:53.000000 clipping-5.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:03:51.199402 clipping-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-15 22:03:41.000000 clipping-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:03:41.000000 clipping-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-05-15 22:03:51.199402 clipping-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-15 22:03:41.000000 clipping-6.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:03:51.195402 clipping-6.0.0/clipping/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-15 22:03:41.000000 clipping-6.0.0/clipping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:03:51.199402 clipping-6.0.0/clipping/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:03:41.000000 clipping-6.0.0/clipping/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15868 2023-05-15 22:03:41.000000 clipping-6.0.0/clipping/core/bounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 22:03:41.000000 clipping-6.0.0/clipping/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15960 2023-05-15 22:03:41.000000 clipping-6.0.0/clipping/core/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20111 2023-05-15 22:03:41.000000 clipping-6.0.0/clipping/core/events_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-15 22:03:41.000000 clipping-6.0.0/clipping/core/hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-05-15 22:03:41.000000 clipping-6.0.0/clipping/core/holeless.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20715 2023-05-15 22:03:41.000000 clipping-6.0.0/clipping/core/holey.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26120 2023-05-15 22:03:41.000000 clipping-6.0.0/clipping/core/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-05-15 22:03:41.000000 clipping-6.0.0/clipping/core/mixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-15 22:03:41.000000 clipping-6.0.0/clipping/core/operands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-15 22:03:41.000000 clipping-6.0.0/clipping/core/sweep_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-15 22:03:41.000000 clipping-6.0.0/clipping/core/unpacking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-15 22:03:41.000000 clipping-6.0.0/clipping/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-15 22:03:41.000000 clipping-6.0.0/clipping/hints.py
+-rw-r--r--   0 runner    (1001) docker     (123)   220391 2023-05-15 22:03:41.000000 clipping-6.0.0/clipping/planar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:03:51.199402 clipping-6.0.0/clipping.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-05-15 22:03:51.000000 clipping-6.0.0/clipping.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-15 22:03:51.000000 clipping-6.0.0/clipping.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:03:51.000000 clipping-6.0.0/clipping.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-15 22:03:51.000000 clipping-6.0.0/clipping.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 22:03:51.000000 clipping-6.0.0/clipping.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-15 22:03:41.000000 clipping-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:03:51.199402 clipping-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-15 22:03:41.000000 clipping-6.0.0/setup.py
```

### Comparing `clipping-5.1.2/LICENSE` & `clipping-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clipping-5.1.2/PKG-INFO` & `clipping-6.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: clipping
-Version: 5.1.2
-Summary: Multisegments, polygons & multipolygons clipping.
-Home-page: https://github.com/lycantropos/clipping/
-Download-URL: https://github.com/lycantropos/clipping/archive/master.zip
-Author: Azat Ibrakov
-Author-email: azatibrakov@gmail.com
-License: MIT License
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 clipping
 ========
 
 [![](https://github.com/lycantropos/clipping/workflows/CI/badge.svg)](https://github.com/lycantropos/clipping/actions/workflows/ci.yml "Github Actions")
 [![](https://readthedocs.org/projects/clip/badge/?version=latest)](https://clip.readthedocs.io/en/latest "Documentation")
 [![](https://codecov.io/gh/lycantropos/clipping/branch/master/graph/badge.svg)](https://codecov.io/gh/lycantropos/clipping "Codecov")
 [![](https://img.shields.io/github/license/lycantropos/clipping.svg)](https://github.com/lycantropos/clipping/blob/master/LICENSE "License")
```

### Comparing `clipping-5.1.2/clipping/core/bounding.py` & `clipping-6.0.0/clipping/core/bounding.py`

 * *Files identical despite different names*

### Comparing `clipping-5.1.2/clipping/core/event.py` & `clipping-6.0.0/clipping/core/event.py`

 * *Files identical despite different names*

### Comparing `clipping-5.1.2/clipping/core/events_queue.py` & `clipping-6.0.0/clipping/core/events_queue.py`

 * *Files identical despite different names*

### Comparing `clipping-5.1.2/clipping/core/holeless.py` & `clipping-6.0.0/clipping/core/holeless.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,19 +111,21 @@
         return result
 
     def fill_queue(self) -> None:
         events_queue = self._events_queue
         for region in self.first.regions:
             events_queue.register(
                     contour_to_oriented_edges_endpoints(region, self.context),
-                    True)
+                    True
+            )
         for region in self.second.regions:
             events_queue.register(
                     contour_to_oriented_edges_endpoints(region, self.context),
-                    False)
+                    False
+            )
 
     @abstractmethod
     def from_shaped_result(self, event: LeftEvent) -> bool:
         """Detects if event is a part of resulting shaped geometry."""
 
     def process_event(self,
                       event: Event,
```

### Comparing `clipping-5.1.2/clipping/core/holey.py` & `clipping-6.0.0/clipping/core/holey.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,15 +403,16 @@
             polygons += self.second.polygons
             polygons.sort(key=to_first_border_vertex)
             return context.multipolygon_cls(polygons)
         return unpack_polygons(self.events_to_polygons(self.sweep()), context)
 
     def from_shaped_result(self, event: LeftEvent) -> bool:
         return (event.outside
-                or not event.from_first_operand and event.is_common_region_boundary)
+                or (not event.from_first_operand
+                    and event.is_common_region_boundary))
 
 
 def _compute_relations(event: LeftEvent,
                        contour_id: int,
                        are_internal: List[bool],
                        depths: List[int],
                        holes: List[List[int]],
```

### Comparing `clipping-5.1.2/clipping/core/linear.py` & `clipping-6.0.0/clipping/core/linear.py`

 * *Files identical despite different names*

### Comparing `clipping-5.1.2/clipping/core/mixed.py` & `clipping-6.0.0/clipping/core/mixed.py`

 * *Files identical despite different names*

### Comparing `clipping-5.1.2/clipping/core/operands.py` & `clipping-6.0.0/clipping/core/operands.py`

 * *Files identical despite different names*

### Comparing `clipping-5.1.2/clipping/core/sweep_line.py` & `clipping-6.0.0/clipping/core/sweep_line.py`

 * *Files identical despite different names*

### Comparing `clipping-5.1.2/clipping/core/unpacking.py` & `clipping-6.0.0/clipping/core/unpacking.py`

 * *Files identical despite different names*

### Comparing `clipping-5.1.2/clipping/core/utils.py` & `clipping-6.0.0/clipping/core/utils.py`

 * *Files identical despite different names*

### Comparing `clipping-5.1.2/clipping/planar.py` & `clipping-6.0.0/clipping/planar.py`

 * *Files identical despite different names*

### Comparing `clipping-5.1.2/clipping.egg-info/PKG-INFO` & `clipping-6.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,49 @@
 Metadata-Version: 2.1
 Name: clipping
-Version: 5.1.2
-Summary: Multisegments, polygons & multipolygons clipping.
+Version: 6.0.0
+Summary: Geometries clipping.
 Home-page: https://github.com/lycantropos/clipping/
 Download-URL: https://github.com/lycantropos/clipping/archive/master.zip
-Author: Azat Ibrakov
-Author-email: azatibrakov@gmail.com
+Author-email: Azat Ibrakov <azatibrakov@gmail.com>
 License: MIT License
+        
+        Copyright (c) 2020 Azat Ibrakov
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: tests
 License-File: LICENSE
 
 clipping
 ========
 
 [![](https://github.com/lycantropos/clipping/workflows/CI/badge.svg)](https://github.com/lycantropos/clipping/actions/workflows/ci.yml "Github Actions")
 [![](https://readthedocs.org/projects/clip/badge/?version=latest)](https://clip.readthedocs.io/en/latest "Documentation")
```

### Comparing `clipping-5.1.2/clipping.egg-info/SOURCES.txt` & `clipping-6.0.0/clipping.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
-requirements.txt
+pyproject.toml
 setup.py
 clipping/__init__.py
 clipping/hints.py
 clipping/planar.py
 clipping.egg-info/PKG-INFO
 clipping.egg-info/SOURCES.txt
 clipping.egg-info/dependency_links.txt
```

