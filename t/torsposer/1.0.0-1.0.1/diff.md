# Comparing `tmp/torsposer-1.0.0.tar.gz` & `tmp/torsposer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torsposer-1.0.0.tar", max compression
+gzip compressed data, was "torsposer-1.0.1.tar", max compression
```

## Comparing `torsposer-1.0.0.tar` & `torsposer-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1900 2023-05-14 19:20:52.604608 torsposer-1.0.0/README.md
--rw-r--r--   0        0        0      729 2023-05-14 19:24:01.708535 torsposer-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-14 10:44:54.667172 torsposer-1.0.0/torsposer/__init__.py
--rw-r--r--   0        0        0     1874 2023-05-14 18:57:17.103999 torsposer-1.0.0/torsposer/__main__.py
--rw-r--r--   0        0        0     6445 2023-05-14 19:17:42.926054 torsposer-1.0.0/torsposer/exposer.py
--rw-r--r--   0        0        0     1675 2023-05-14 13:05:18.790297 torsposer-1.0.0/torsposer/utils.py
--rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 torsposer-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1943 2023-05-16 10:14:44.603605 torsposer-1.0.1/README.md
+-rw-r--r--   0        0        0      729 2023-05-16 10:14:44.603605 torsposer-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 10:14:44.603605 torsposer-1.0.1/torsposer/__init__.py
+-rw-r--r--   0        0        0     2122 2023-05-16 10:14:44.607605 torsposer-1.0.1/torsposer/__main__.py
+-rw-r--r--   0        0        0     6445 2023-05-16 10:14:44.607605 torsposer-1.0.1/torsposer/exposer.py
+-rw-r--r--   0        0        0     1675 2023-05-16 10:14:44.607605 torsposer-1.0.1/torsposer/utils.py
+-rw-r--r--   0        0        0     2843 1970-01-01 00:00:00.000000 torsposer-1.0.1/PKG-INFO
```

### Comparing `torsposer-1.0.0/README.md` & `torsposer-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -52,11 +52,11 @@
     usage: torsposer [-h] -s SERVICE_NAME [-sp SERVICE_PORT] [-tp TOR_PORT]
     torsposer: error: the following arguments are required: -s/--service
     ```
 
 - expose localhost server running on port 80 to tor network on tor host port 80
 
     ```bash
-
+    torsposer -s http_service -sp 80 -tp 80
     ```
 
 > Note: if `torsposer` doesn't work try replacing it with `python3 -m torsposer`
```

### Comparing `torsposer-1.0.0/pyproject.toml` & `torsposer-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "torsposer"
-version = "1.0.0"
+version = "1.0.1"
 description = "Expose Services to the TOR network automatically"
 authors = ["Dhrumil Mistry <56185972+dmdhrumilmistry@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
```

### Comparing `torsposer-1.0.0/torsposer/__main__.py` & `torsposer-1.0.1/torsposer/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 from argparse import ArgumentParser
-from .exposer import TorServiceExposer
 from textwrap import dedent
+import logging
 
 
+logger = logging.getLogger(__name__)
+logging.basicConfig(level=logging.INFO,
+                    format='[%(asctime)s] [%(levelname)s] - %(message)s')
+
+
+try:
+    from .exposer import TorServiceExposer
+except ImportError:
+    logger.error('Windows is not supported yet!')
+
 def start():
     '''Starts torsposer cli tool
     
     Arguments:
         None
 
     Returns:
```

### Comparing `torsposer-1.0.0/torsposer/exposer.py` & `torsposer-1.0.1/torsposer/exposer.py`

 * *Files identical despite different names*

### Comparing `torsposer-1.0.0/torsposer/utils.py` & `torsposer-1.0.1/torsposer/utils.py`

 * *Files identical despite different names*

### Comparing `torsposer-1.0.0/PKG-INFO` & `torsposer-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torsposer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Expose Services to the TOR network automatically
 License: MIT
 Author: Dhrumil Mistry
 Author-email: 56185972+dmdhrumilmistry@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -73,12 +73,12 @@
     usage: torsposer [-h] -s SERVICE_NAME [-sp SERVICE_PORT] [-tp TOR_PORT]
     torsposer: error: the following arguments are required: -s/--service
     ```
 
 - expose localhost server running on port 80 to tor network on tor host port 80
 
     ```bash
-
+    torsposer -s http_service -sp 80 -tp 80
     ```
 
 > Note: if `torsposer` doesn't work try replacing it with `python3 -m torsposer`
```

