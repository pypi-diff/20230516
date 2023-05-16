# Comparing `tmp/pxgrid-api-0.2.1.tar.gz` & `tmp/pxgrid-api-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxgrid-api-0.2.1.tar", last modified: Tue May 16 03:17:42 2023, max compression
+gzip compressed data, was "pxgrid-api-0.2.2.tar", last modified: Tue May 16 03:38:00 2023, max compression
```

## Comparing `pxgrid-api-0.2.1.tar` & `pxgrid-api-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-16 03:17:42.110445 pxgrid-api-0.2.1/
--rw-r--r--   0 vibobrov   (503) staff       (20)    11357 2023-05-10 01:50:25.000000 pxgrid-api-0.2.1/LICENSE
--rw-r--r--   0 vibobrov   (503) staff       (20)       24 2023-05-13 01:43:48.000000 pxgrid-api-0.2.1/MANIFEST.in
--rw-r--r--   0 vibobrov   (503) staff       (20)    13504 2023-05-16 03:17:42.109964 pxgrid-api-0.2.1/PKG-INFO
--rw-r--r--   0 vibobrov   (503) staff       (20)    16166 2023-05-16 03:15:00.000000 pxgrid-api-0.2.1/README.rst
--rw-r--r--   0 vibobrov   (503) staff       (20)      765 2023-05-16 03:15:00.000000 pxgrid-api-0.2.1/pyproject.toml
--rw-r--r--   0 vibobrov   (503) staff       (20)       38 2023-05-16 03:17:42.110600 pxgrid-api-0.2.1/setup.cfg
-drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-16 03:17:42.101294 pxgrid-api-0.2.1/src/
-drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-16 03:17:42.105332 pxgrid-api-0.2.1/src/pxapi/
--rw-r--r--   0 vibobrov   (503) staff       (20)       82 2023-05-16 03:15:00.000000 pxgrid-api-0.2.1/src/pxapi/__init__.py
--rwxr-xr-x   0 vibobrov   (503) staff       (20)    20358 2023-05-16 03:15:00.000000 pxgrid-api-0.2.1/src/pxapi/__main__.py
--rw-r--r--   0 vibobrov   (503) staff       (20)    29184 2023-05-16 03:15:00.000000 pxgrid-api-0.2.1/src/pxapi/pxapi.py
--rw-r--r--   0 vibobrov   (503) staff       (20)     1488 2023-05-16 03:15:00.000000 pxgrid-api-0.2.1/src/pxapi/stompframe.py
-drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-16 03:17:42.109079 pxgrid-api-0.2.1/src/pxgrid_api.egg-info/
--rw-r--r--   0 vibobrov   (503) staff       (20)    13504 2023-05-16 03:17:42.000000 pxgrid-api-0.2.1/src/pxgrid_api.egg-info/PKG-INFO
--rw-r--r--   0 vibobrov   (503) staff       (20)      362 2023-05-16 03:17:42.000000 pxgrid-api-0.2.1/src/pxgrid_api.egg-info/SOURCES.txt
--rw-r--r--   0 vibobrov   (503) staff       (20)        1 2023-05-16 03:17:42.000000 pxgrid-api-0.2.1/src/pxgrid_api.egg-info/dependency_links.txt
--rw-r--r--   0 vibobrov   (503) staff       (20)       48 2023-05-16 03:17:42.000000 pxgrid-api-0.2.1/src/pxgrid_api.egg-info/entry_points.txt
--rw-r--r--   0 vibobrov   (503) staff       (20)       42 2023-05-16 03:17:42.000000 pxgrid-api-0.2.1/src/pxgrid_api.egg-info/requires.txt
--rw-r--r--   0 vibobrov   (503) staff       (20)       14 2023-05-16 03:17:42.000000 pxgrid-api-0.2.1/src/pxgrid_api.egg-info/top_level.txt
+drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-16 03:38:00.106985 pxgrid-api-0.2.2/
+-rw-r--r--   0 vibobrov   (503) staff       (20)    11357 2023-05-10 01:50:25.000000 pxgrid-api-0.2.2/LICENSE
+-rw-r--r--   0 vibobrov   (503) staff       (20)       24 2023-05-13 01:43:48.000000 pxgrid-api-0.2.2/MANIFEST.in
+-rw-r--r--   0 vibobrov   (503) staff       (20)    29667 2023-05-16 03:38:00.106573 pxgrid-api-0.2.2/PKG-INFO
+-rw-r--r--   0 vibobrov   (503) staff       (20)    16165 2023-05-16 03:25:57.000000 pxgrid-api-0.2.2/README.rst
+-rw-r--r--   0 vibobrov   (503) staff       (20)      766 2023-05-16 03:20:09.000000 pxgrid-api-0.2.2/pyproject.toml
+-rw-r--r--   0 vibobrov   (503) staff       (20)       38 2023-05-16 03:38:00.107105 pxgrid-api-0.2.2/setup.cfg
+drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-16 03:38:00.095313 pxgrid-api-0.2.2/src/
+drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-16 03:38:00.100781 pxgrid-api-0.2.2/src/pxapi/
+-rw-r--r--   0 vibobrov   (503) staff       (20)       82 2023-05-16 03:37:17.000000 pxgrid-api-0.2.2/src/pxapi/__init__.py
+-rwxr-xr-x   0 vibobrov   (503) staff       (20)    20358 2023-05-16 03:15:00.000000 pxgrid-api-0.2.2/src/pxapi/__main__.py
+-rw-r--r--   0 vibobrov   (503) staff       (20)    29184 2023-05-16 03:33:24.000000 pxgrid-api-0.2.2/src/pxapi/pxapi.py
+-rw-r--r--   0 vibobrov   (503) staff       (20)     1488 2023-05-16 03:15:00.000000 pxgrid-api-0.2.2/src/pxapi/stompframe.py
+drwxr-xr-x   0 vibobrov   (503) staff       (20)        0 2023-05-16 03:38:00.105744 pxgrid-api-0.2.2/src/pxgrid_api.egg-info/
+-rw-r--r--   0 vibobrov   (503) staff       (20)    29667 2023-05-16 03:38:00.000000 pxgrid-api-0.2.2/src/pxgrid_api.egg-info/PKG-INFO
+-rw-r--r--   0 vibobrov   (503) staff       (20)      362 2023-05-16 03:38:00.000000 pxgrid-api-0.2.2/src/pxgrid_api.egg-info/SOURCES.txt
+-rw-r--r--   0 vibobrov   (503) staff       (20)        1 2023-05-16 03:38:00.000000 pxgrid-api-0.2.2/src/pxgrid_api.egg-info/dependency_links.txt
+-rw-r--r--   0 vibobrov   (503) staff       (20)       48 2023-05-16 03:38:00.000000 pxgrid-api-0.2.2/src/pxgrid_api.egg-info/entry_points.txt
+-rw-r--r--   0 vibobrov   (503) staff       (20)       42 2023-05-16 03:38:00.000000 pxgrid-api-0.2.2/src/pxgrid_api.egg-info/requires.txt
+-rw-r--r--   0 vibobrov   (503) staff       (20)       14 2023-05-16 03:38:00.000000 pxgrid-api-0.2.2/src/pxgrid_api.egg-info/top_level.txt
```

### Comparing `pxgrid-api-0.2.1/LICENSE` & `pxgrid-api-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pxgrid-api-0.2.1/README.rst` & `pxgrid-api-0.2.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 REST API
 ~~~~~~~~
 
 These are fairly straight forward. Review the comments in the code for reference.
 
 .. code-block:: python
-  
+
   #!/usr/bin/env python3
   from pxapi import PXAPI
 
   # Instatiate object. Root CA argument can be omitted to disable server certificate verification.
   api=PXAPI('pxgridnode.example.com','client-name','client.cer','client.key','root.cer')
 
   # Check account activation status. This will connect to pxGrid node and check if our account is in approved and enabled state
@@ -207,14 +207,15 @@
 
 Examples
 ~~~~~~~~
 
 Check if account is approved in ISE
 
 .. code-block:: console
+
   pxshell> activate
   {'accountState': 'ENABLED', 'version': '2.0'}
 
 Using password based authentication
 
 .. code-block:: console
```

### Comparing `pxgrid-api-0.2.1/pyproject.toml` & `pxgrid-api-0.2.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires=["setuptools","wheel"]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "pxgrid-api"
-version = "0.2.1"
+version = "0.2.2"
 description = "pxGrid API library and command line tool"
-readme = "README.md"
+readme = "README.rst"
 authors = [{ name = "Viktor Bobrov", email = "vibobrov@cisco.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
```

### Comparing `pxgrid-api-0.2.1/src/pxapi/__main__.py` & `pxgrid-api-0.2.2/src/pxapi/__main__.py`

 * *Files identical despite different names*

### Comparing `pxgrid-api-0.2.1/src/pxapi/pxapi.py` & `pxgrid-api-0.2.2/src/pxapi/pxapi.py`

 * *Files identical despite different names*

### Comparing `pxgrid-api-0.2.1/src/pxapi/stompframe.py` & `pxgrid-api-0.2.2/src/pxapi/stompframe.py`

 * *Files identical despite different names*

