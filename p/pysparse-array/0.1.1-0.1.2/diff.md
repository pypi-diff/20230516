# Comparing `tmp/pysparse-array-0.1.1.tar.gz` & `tmp/pysparse-array-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparse-array-0.1.1.tar", last modified: Mon May 15 18:01:54 2023, max compression
+gzip compressed data, was "pysparse-array-0.1.2.tar", last modified: Mon May 15 22:09:44 2023, max compression
```

## Comparing `pysparse-array-0.1.1.tar` & `pysparse-array-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-15 18:01:54.372942 pysparse-array-0.1.1/
--rw-r--r--   0 thomasfrost   (502) staff       (20)     1060 2023-05-15 14:53:09.000000 pysparse-array-0.1.1/LICENSE.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)     2289 2023-05-15 18:01:54.371185 pysparse-array-0.1.1/PKG-INFO
--rw-r--r--   0 thomasfrost   (502) staff       (20)     1584 2023-05-15 17:35:02.000000 pysparse-array-0.1.1/README.md
--rw-r--r--   0 thomasfrost   (502) staff       (20)      772 2023-05-15 18:00:38.000000 pysparse-array-0.1.1/pyproject.toml
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-15 18:01:54.368489 pysparse-array-0.1.1/pysparse_array.egg-info/
--rw-r--r--   0 thomasfrost   (502) staff       (20)     2289 2023-05-15 18:01:54.000000 pysparse-array-0.1.1/pysparse_array.egg-info/PKG-INFO
--rw-r--r--   0 thomasfrost   (502) staff       (20)      234 2023-05-15 18:01:54.000000 pysparse-array-0.1.1/pysparse_array.egg-info/SOURCES.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-05-15 18:01:54.000000 pysparse-array-0.1.1/pysparse_array.egg-info/dependency_links.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       41 2023-05-15 18:01:54.000000 pysparse-array-0.1.1/pysparse_array.egg-info/requires.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-05-15 18:01:54.000000 pysparse-array-0.1.1/pysparse_array.egg-info/top_level.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       38 2023-05-15 18:01:54.373178 pysparse-array-0.1.1/setup.cfg
--rw-r--r--   0 thomasfrost   (502) staff       (20)      815 2023-05-15 17:31:05.000000 pysparse-array-0.1.1/setup.py
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-15 22:09:44.422214 pysparse-array-0.1.2/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     1060 2023-05-15 14:53:09.000000 pysparse-array-0.1.2/LICENSE.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     2289 2023-05-15 22:09:44.418936 pysparse-array-0.1.2/PKG-INFO
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     1584 2023-05-15 17:35:02.000000 pysparse-array-0.1.2/README.md
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      772 2023-05-15 22:08:03.000000 pysparse-array-0.1.2/pyproject.toml
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-15 22:09:44.370005 pysparse-array-0.1.2/pysparse_array.egg-info/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     2289 2023-05-15 22:09:44.000000 pysparse-array-0.1.2/pysparse_array.egg-info/PKG-INFO
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      270 2023-05-15 22:09:44.000000 pysparse-array-0.1.2/pysparse_array.egg-info/SOURCES.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-05-15 22:09:44.000000 pysparse-array-0.1.2/pysparse_array.egg-info/dependency_links.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       41 2023-05-15 22:09:44.000000 pysparse-array-0.1.2/pysparse_array.egg-info/requires.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)        7 2023-05-15 22:09:44.000000 pysparse-array-0.1.2/pysparse_array.egg-info/top_level.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       38 2023-05-15 22:09:44.422659 pysparse-array-0.1.2/setup.cfg
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      815 2023-05-15 22:08:34.000000 pysparse-array-0.1.2/setup.py
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-15 22:09:44.389824 pysparse-array-0.1.2/sparse/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       49 2023-05-15 14:51:01.000000 pysparse-array-0.1.2/sparse/__init__.py
+-rw-r--r--   0 thomasfrost   (502) staff       (20)    14885 2023-05-15 16:10:49.000000 pysparse-array-0.1.2/sparse/sparse.py
```

### Comparing `pysparse-array-0.1.1/LICENSE.txt` & `pysparse-array-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysparse-array-0.1.1/PKG-INFO` & `pysparse-array-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparse-array
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries.
 Home-page: https://github.com/tdgfrost/PySparse
 Download-URL: https://pypi.org/project/pysparse-array/
 Author: Thomas Frost
 Author-email: Thomas Frost <tdgfrost@gmail.com>
 Project-URL: Homepage, https://github.com/tdgfrost/PySparse
 Project-URL: Bug Tracker, https://github.com/tdgfrost/PySparse/issues
```

### Comparing `pysparse-array-0.1.1/README.md` & `pysparse-array-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pysparse-array-0.1.1/pyproject.toml` & `pysparse-array-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pysparse-array"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
 	{ name="Thomas Frost", email="tdgfrost@gmail.com" },
 ]
 description = "A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries."
 readme = "README.md"
 requires-python = ">=3.8.0"
 classifiers = [
```

### Comparing `pysparse-array-0.1.1/pysparse_array.egg-info/PKG-INFO` & `pysparse-array-0.1.2/pysparse_array.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparse-array
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries.
 Home-page: https://github.com/tdgfrost/PySparse
 Download-URL: https://pypi.org/project/pysparse-array/
 Author: Thomas Frost
 Author-email: Thomas Frost <tdgfrost@gmail.com>
 Project-URL: Homepage, https://github.com/tdgfrost/PySparse
 Project-URL: Bug Tracker, https://github.com/tdgfrost/PySparse/issues
```

### Comparing `pysparse-array-0.1.1/setup.py` & `pysparse-array-0.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     README = readme_file.read()
 
 with open('/Users/thomasfrost/Documents/Github/pysparse/PySparse/HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='pysparse-array',
-    version='0.1.0',
+    version='0.1.2',
     description='Package to encode and decode large OOM numpy arrays as Sparse binaries',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     packages=find_packages(),
     author='Thomas Frost',
     author_email='tdgfrost@gmail.com',
     url='https://github.com/tdgfrost/PySparse',
```

