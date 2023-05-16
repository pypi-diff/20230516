# Comparing `tmp/triglav-1.0.0.tar.gz` & `tmp/triglav-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triglav-1.0.0.tar", last modified: Fri May 12 08:29:36 2023, max compression
+gzip compressed data, was "triglav-1.0.1.tar", last modified: Tue May 16 14:47:39 2023, max compression
```

## Comparing `triglav-1.0.0.tar` & `triglav-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:29:36.447559 triglav-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-12 08:29:25.000000 triglav-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-05-12 08:29:36.447559 triglav-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-12 08:29:25.000000 triglav-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-12 08:29:25.000000 triglav-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:29:36.447559 triglav-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:29:36.443559 triglav-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-12 08:29:25.000000 triglav-1.0.0/tests/test_triglav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:29:36.443559 triglav-1.0.0/triglav.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-05-12 08:29:36.000000 triglav-1.0.0/triglav.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-12 08:29:36.000000 triglav-1.0.0/triglav.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:29:36.000000 triglav-1.0.0/triglav.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-12 08:29:36.000000 triglav-1.0.0/triglav.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 08:29:36.000000 triglav-1.0.0/triglav.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:47:39.829107 triglav-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-16 14:47:23.000000 triglav-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-05-16 14:47:39.829107 triglav-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-16 14:47:23.000000 triglav-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-16 14:47:23.000000 triglav-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 14:47:39.829107 triglav-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:47:39.829107 triglav-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-16 14:47:23.000000 triglav-1.0.1/tests/test_triglav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:47:39.829107 triglav-1.0.1/triglav.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-05-16 14:47:39.000000 triglav-1.0.1/triglav.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-16 14:47:39.000000 triglav-1.0.1/triglav.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 14:47:39.000000 triglav-1.0.1/triglav.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-16 14:47:39.000000 triglav-1.0.1/triglav.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 14:47:39.000000 triglav-1.0.1/triglav.egg-info/top_level.txt
```

### Comparing `triglav-1.0.0/LICENSE` & `triglav-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `triglav-1.0.0/PKG-INFO` & `triglav-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triglav
-Version: 1.0.0
+Version: 1.0.1
 Summary: Triglav: Iterative Refinement and Selection of Stable Features Using Shapley Values
 Author: Peter Kruczkiewicz, G. Brian Golding, Oliver Lung
 Author-email: Josip Rudar <rudarj@uoguelph.ca>, Mehrdad Hajibabaei <mhajibab@uoguelph.ca>
 License: MIT License
         
         Copyright (c) 2023 Josip Rudar, Peter Kruczkiewicz, Oliver Lung, G.Brian Golding, Mehrdad Hajibabaei
         
@@ -36,15 +36,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: <=3.11,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # Triglav - Feature Selection Using Iterative Refinement
```

### Comparing `triglav-1.0.0/README.md` & `triglav-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `triglav-1.0.0/pyproject.toml` & `triglav-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "triglav"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     {name = "Josip Rudar", email = "rudarj@uoguelph.ca"},
     {name = "Peter Kruczkiewicz"},
     {name = "G. Brian Golding"},
     {name = "Oliver Lung"},
     {name = "Mehrdad Hajibabaei", email = "mhajibab@uoguelph.ca"}
 ]
@@ -13,15 +13,15 @@
     "ecology",
     "multivariate statistics",
     "feature selection",
     "stability selection"
 ]
 license = {file = "LICENSE"}
 readme = "README.md"
-requires-python = ">=3.8,<=3.11"
+requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
```

### Comparing `triglav-1.0.0/tests/test_triglav.py` & `triglav-1.0.1/tests/test_triglav.py`

 * *Files identical despite different names*

### Comparing `triglav-1.0.0/triglav.egg-info/PKG-INFO` & `triglav-1.0.1/triglav.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triglav
-Version: 1.0.0
+Version: 1.0.1
 Summary: Triglav: Iterative Refinement and Selection of Stable Features Using Shapley Values
 Author: Peter Kruczkiewicz, G. Brian Golding, Oliver Lung
 Author-email: Josip Rudar <rudarj@uoguelph.ca>, Mehrdad Hajibabaei <mhajibab@uoguelph.ca>
 License: MIT License
         
         Copyright (c) 2023 Josip Rudar, Peter Kruczkiewicz, Oliver Lung, G.Brian Golding, Mehrdad Hajibabaei
         
@@ -36,15 +36,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: <=3.11,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # Triglav - Feature Selection Using Iterative Refinement
```

