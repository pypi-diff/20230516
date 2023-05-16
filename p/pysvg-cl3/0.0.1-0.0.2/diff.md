# Comparing `tmp/pysvg-cl3-0.0.1.tar.gz` & `tmp/pysvg-cl3-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysvg-cl3-0.0.1.tar", last modified: Tue May 16 15:00:49 2023, max compression
+gzip compressed data, was "pysvg-cl3-0.0.2.tar", last modified: Tue May 16 15:11:31 2023, max compression
```

## Comparing `pysvg-cl3-0.0.1.tar` & `pysvg-cl3-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-16 15:00:49.130164 pysvg-cl3-0.0.1/
--rw-r--r--   0 lacasta    (503) staff       (20)    35087 2023-05-16 14:25:20.000000 pysvg-cl3-0.0.1/LICENSE
--rw-r--r--   0 lacasta    (503) staff       (20)      556 2023-05-16 15:00:49.129713 pysvg-cl3-0.0.1/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      102 2023-05-16 14:16:46.000000 pysvg-cl3-0.0.1/README.md
--rw-r--r--   0 lacasta    (503) staff       (20)      611 2023-05-16 14:59:56.000000 pysvg-cl3-0.0.1/pyproject.toml
--rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-05-16 15:00:49.130256 pysvg-cl3-0.0.1/setup.cfg
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-16 15:00:49.126422 pysvg-cl3-0.0.1/src/
--rw-r--r--   0 lacasta    (503) staff       (20)     9045 2023-05-16 14:03:41.000000 pysvg-cl3-0.0.1/src/DXFPainter.py
--rw-r--r--   0 lacasta    (503) staff       (20)     5026 2023-05-16 14:03:21.000000 pysvg-cl3-0.0.1/src/GDSPainter.py
--rw-r--r--   0 lacasta    (503) staff       (20)     8475 2023-05-16 14:04:09.000000 pysvg-cl3-0.0.1/src/Painter.py
--rw-r--r--   0 lacasta    (503) staff       (20)     4572 2020-11-28 10:22:00.000000 pysvg-cl3-0.0.1/src/Path.py
--rw-r--r--   0 lacasta    (503) staff       (20)    28025 2023-05-16 14:03:57.000000 pysvg-cl3-0.0.1/src/matrix.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-16 15:00:49.129030 pysvg-cl3-0.0.1/src/pysvg_cl3.egg-info/
--rw-r--r--   0 lacasta    (503) staff       (20)      556 2023-05-16 15:00:49.000000 pysvg-cl3-0.0.1/src/pysvg_cl3.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      304 2023-05-16 15:00:49.000000 pysvg-cl3-0.0.1/src/pysvg_cl3.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-05-16 15:00:49.000000 pysvg-cl3-0.0.1/src/pysvg_cl3.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       26 2023-05-16 15:00:49.000000 pysvg-cl3-0.0.1/src/pysvg_cl3.egg-info/requires.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       46 2023-05-16 15:00:49.000000 pysvg-cl3-0.0.1/src/pysvg_cl3.egg-info/top_level.txt
--rw-r--r--   0 lacasta    (503) staff       (20)    69301 2023-05-16 14:08:08.000000 pysvg-cl3-0.0.1/src/svg.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-16 15:11:31.481748 pysvg-cl3-0.0.2/
+-rw-r--r--   0 lacasta    (503) staff       (20)    35087 2023-05-16 14:25:20.000000 pysvg-cl3-0.0.2/LICENSE
+-rw-r--r--   0 lacasta    (503) staff       (20)      556 2023-05-16 15:11:31.481301 pysvg-cl3-0.0.2/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      102 2023-05-16 14:16:46.000000 pysvg-cl3-0.0.2/README.md
+-rw-r--r--   0 lacasta    (503) staff       (20)      611 2023-05-16 15:11:21.000000 pysvg-cl3-0.0.2/pyproject.toml
+-rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-05-16 15:11:31.481863 pysvg-cl3-0.0.2/setup.cfg
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-16 15:11:31.477505 pysvg-cl3-0.0.2/src/
+-rw-r--r--   0 lacasta    (503) staff       (20)     9045 2023-05-16 14:03:41.000000 pysvg-cl3-0.0.2/src/DXFPainter.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     5026 2023-05-16 14:03:21.000000 pysvg-cl3-0.0.2/src/GDSPainter.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     8475 2023-05-16 14:04:09.000000 pysvg-cl3-0.0.2/src/Painter.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     4572 2020-11-28 10:22:00.000000 pysvg-cl3-0.0.2/src/Path.py
+-rw-r--r--   0 lacasta    (503) staff       (20)       21 2023-05-16 15:11:26.000000 pysvg-cl3-0.0.2/src/__init__.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    28025 2023-05-16 14:03:57.000000 pysvg-cl3-0.0.2/src/matrix.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-16 15:11:31.479944 pysvg-cl3-0.0.2/src/pysvg_cl3.egg-info/
+-rw-r--r--   0 lacasta    (503) staff       (20)      556 2023-05-16 15:11:31.000000 pysvg-cl3-0.0.2/src/pysvg_cl3.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      320 2023-05-16 15:11:31.000000 pysvg-cl3-0.0.2/src/pysvg_cl3.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-05-16 15:11:31.000000 pysvg-cl3-0.0.2/src/pysvg_cl3.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       26 2023-05-16 15:11:31.000000 pysvg-cl3-0.0.2/src/pysvg_cl3.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       55 2023-05-16 15:11:31.000000 pysvg-cl3-0.0.2/src/pysvg_cl3.egg-info/top_level.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)    69301 2023-05-16 14:08:08.000000 pysvg-cl3-0.0.2/src/svg.py
```

### Comparing `pysvg-cl3-0.0.1/LICENSE` & `pysvg-cl3-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysvg-cl3-0.0.1/PKG-INFO` & `pysvg-cl3-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysvg-cl3
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python class to build SVG and 'paint' them as DXF or GDS.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pysvg-cl3-0.0.1/pyproject.toml` & `pysvg-cl3-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysvg-cl3"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@cern.ch" },
 ]
 description = "A python class to build SVG and 'paint' them as DXF or GDS."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `pysvg-cl3-0.0.1/src/DXFPainter.py` & `pysvg-cl3-0.0.2/src/DXFPainter.py`

 * *Files identical despite different names*

### Comparing `pysvg-cl3-0.0.1/src/GDSPainter.py` & `pysvg-cl3-0.0.2/src/GDSPainter.py`

 * *Files identical despite different names*

### Comparing `pysvg-cl3-0.0.1/src/Painter.py` & `pysvg-cl3-0.0.2/src/Painter.py`

 * *Files identical despite different names*

### Comparing `pysvg-cl3-0.0.1/src/Path.py` & `pysvg-cl3-0.0.2/src/Path.py`

 * *Files identical despite different names*

### Comparing `pysvg-cl3-0.0.1/src/matrix.py` & `pysvg-cl3-0.0.2/src/matrix.py`

 * *Files identical despite different names*

### Comparing `pysvg-cl3-0.0.1/src/pysvg_cl3.egg-info/PKG-INFO` & `pysvg-cl3-0.0.2/src/pysvg_cl3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysvg-cl3
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python class to build SVG and 'paint' them as DXF or GDS.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pysvg-cl3-0.0.1/src/svg.py` & `pysvg-cl3-0.0.2/src/svg.py`

 * *Files identical despite different names*

