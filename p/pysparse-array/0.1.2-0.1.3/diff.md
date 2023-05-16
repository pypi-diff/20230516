# Comparing `tmp/pysparse-array-0.1.2.tar.gz` & `tmp/pysparse-array-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparse-array-0.1.2.tar", last modified: Mon May 15 22:09:44 2023, max compression
+gzip compressed data, was "pysparse-array-0.1.3.tar", last modified: Tue May 16 11:49:38 2023, max compression
```

## Comparing `pysparse-array-0.1.2.tar` & `pysparse-array-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-15 22:09:44.422214 pysparse-array-0.1.2/
--rw-r--r--   0 thomasfrost   (502) staff       (20)     1060 2023-05-15 14:53:09.000000 pysparse-array-0.1.2/LICENSE.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)     2289 2023-05-15 22:09:44.418936 pysparse-array-0.1.2/PKG-INFO
--rw-r--r--   0 thomasfrost   (502) staff       (20)     1584 2023-05-15 17:35:02.000000 pysparse-array-0.1.2/README.md
--rw-r--r--   0 thomasfrost   (502) staff       (20)      772 2023-05-15 22:08:03.000000 pysparse-array-0.1.2/pyproject.toml
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-15 22:09:44.370005 pysparse-array-0.1.2/pysparse_array.egg-info/
--rw-r--r--   0 thomasfrost   (502) staff       (20)     2289 2023-05-15 22:09:44.000000 pysparse-array-0.1.2/pysparse_array.egg-info/PKG-INFO
--rw-r--r--   0 thomasfrost   (502) staff       (20)      270 2023-05-15 22:09:44.000000 pysparse-array-0.1.2/pysparse_array.egg-info/SOURCES.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-05-15 22:09:44.000000 pysparse-array-0.1.2/pysparse_array.egg-info/dependency_links.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       41 2023-05-15 22:09:44.000000 pysparse-array-0.1.2/pysparse_array.egg-info/requires.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)        7 2023-05-15 22:09:44.000000 pysparse-array-0.1.2/pysparse_array.egg-info/top_level.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       38 2023-05-15 22:09:44.422659 pysparse-array-0.1.2/setup.cfg
--rw-r--r--   0 thomasfrost   (502) staff       (20)      815 2023-05-15 22:08:34.000000 pysparse-array-0.1.2/setup.py
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-15 22:09:44.389824 pysparse-array-0.1.2/sparse/
--rw-r--r--   0 thomasfrost   (502) staff       (20)       49 2023-05-15 14:51:01.000000 pysparse-array-0.1.2/sparse/__init__.py
--rw-r--r--   0 thomasfrost   (502) staff       (20)    14885 2023-05-15 16:10:49.000000 pysparse-array-0.1.2/sparse/sparse.py
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-16 11:49:38.673487 pysparse-array-0.1.3/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      834 2023-05-16 11:39:55.000000 pysparse-array-0.1.3/HISTORY.md
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     1060 2023-05-15 14:53:09.000000 pysparse-array-0.1.3/LICENSE.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       19 2023-05-16 11:11:47.000000 pysparse-array-0.1.3/MANIFEST.in
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     2289 2023-05-16 11:49:38.667941 pysparse-array-0.1.3/PKG-INFO
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     1584 2023-05-15 17:35:02.000000 pysparse-array-0.1.3/README.md
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      779 2023-05-15 22:23:50.000000 pysparse-array-0.1.3/pyproject.toml
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-16 11:49:38.626472 pysparse-array-0.1.3/pysparse_array.egg-info/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     2289 2023-05-16 11:49:38.000000 pysparse-array-0.1.3/pysparse_array.egg-info/PKG-INFO
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      311 2023-05-16 11:49:38.000000 pysparse-array-0.1.3/pysparse_array.egg-info/SOURCES.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-05-16 11:49:38.000000 pysparse-array-0.1.3/pysparse_array.egg-info/dependency_links.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       47 2023-05-16 11:49:38.000000 pysparse-array-0.1.3/pysparse_array.egg-info/requires.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)        7 2023-05-16 11:49:38.000000 pysparse-array-0.1.3/pysparse_array.egg-info/top_level.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       38 2023-05-16 11:49:38.674045 pysparse-array-0.1.3/setup.cfg
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      708 2023-05-16 11:12:23.000000 pysparse-array-0.1.3/setup.py
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-16 11:49:38.662705 pysparse-array-0.1.3/sparse/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      113 2023-05-16 11:47:08.000000 pysparse-array-0.1.3/sparse/__init__.py
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     8471 2023-05-16 11:46:30.000000 pysparse-array-0.1.3/sparse/array_api.py
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     6846 2023-05-16 11:46:59.000000 pysparse-array-0.1.3/sparse/core.py
```

### Comparing `pysparse-array-0.1.2/LICENSE.txt` & `pysparse-array-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysparse-array-0.1.2/PKG-INFO` & `pysparse-array-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparse-array
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries.
 Home-page: https://github.com/tdgfrost/PySparse
 Download-URL: https://pypi.org/project/pysparse-array/
 Author: Thomas Frost
 Author-email: Thomas Frost <tdgfrost@gmail.com>
 Project-URL: Homepage, https://github.com/tdgfrost/PySparse
 Project-URL: Bug Tracker, https://github.com/tdgfrost/PySparse/issues
```

### Comparing `pysparse-array-0.1.2/README.md` & `pysparse-array-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pysparse-array-0.1.2/pyproject.toml` & `pysparse-array-0.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pysparse-array"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
 	{ name="Thomas Frost", email="tdgfrost@gmail.com" },
 ]
 description = "A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries."
 readme = "README.md"
 requires-python = ">=3.8.0"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
 	"Operating System :: OS Independent",
 ]
-dependencies = ['numpy>=1.18.0', 'tqdm>=4.46.0', 'numba>=0.49.0']
+dependencies = ['numpy>=1.18.0', 'tqdm>=4.46.0', 'numba>=0.49.0, <0.57']
 
 [dynamic]
 keywords = ["PySparse", "SparseArray"]
 license = "MIT"
 
 [project.urls]
 "Homepage" = "https://github.com/tdgfrost/PySparse"
```

### Comparing `pysparse-array-0.1.2/pysparse_array.egg-info/PKG-INFO` & `pysparse-array-0.1.3/pysparse_array.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparse-array
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries.
 Home-page: https://github.com/tdgfrost/PySparse
 Download-URL: https://pypi.org/project/pysparse-array/
 Author: Thomas Frost
 Author-email: Thomas Frost <tdgfrost@gmail.com>
 Project-URL: Homepage, https://github.com/tdgfrost/PySparse
 Project-URL: Bug Tracker, https://github.com/tdgfrost/PySparse/issues
```

