# Comparing `tmp/devgoldyutils-2.5.tar.gz` & `tmp/devgoldyutils-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devgoldyutils-2.5.tar", last modified: Sun May 14 19:34:38 2023, max compression
+gzip compressed data, was "devgoldyutils-2.5.1.tar", last modified: Tue May 16 19:41:30 2023, max compression
```

## Comparing `devgoldyutils-2.5.tar` & `devgoldyutils-2.5.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-05-14 19:34:38.527313 devgoldyutils-2.5/
--rw-r--r--   0 goldy     (1001) goldy     (1001)       53 2023-05-14 16:10:00.000000 devgoldyutils-2.5/.gitignore
--rw-r--r--   0 goldy     (1001) goldy     (1001)    35148 2023-05-14 16:10:00.000000 devgoldyutils-2.5/LICENSE
--rwxr-xr-x   0 goldy     (1001) goldy     (1001)       32 2023-02-01 17:19:33.000000 devgoldyutils-2.5/MANIFEST.in
--rw-r--r--   0 goldy     (1001) goldy     (1001)       23 2023-05-14 16:10:00.000000 devgoldyutils-2.5/Makefile
--rw-r--r--   0 goldy     (1001) goldy     (1001)    41573 2023-05-14 19:34:38.527313 devgoldyutils-2.5/PKG-INFO
--rwxr-xr-x   0 goldy     (1001) goldy     (1001)     1670 2023-05-14 16:51:09.000000 devgoldyutils-2.5/demo.py
-drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-05-14 19:34:38.525313 devgoldyutils-2.5/devgoldyutils/
--rw-r--r--   0 goldy     (1001) goldy     (1001)      467 2023-05-14 16:40:15.000000 devgoldyutils-2.5/devgoldyutils/__init__.py
--rw-r--r--   0 goldy     (1001) goldy     (1001)     1497 2023-05-14 19:34:30.000000 devgoldyutils-2.5/devgoldyutils/better_get.py
--rw-r--r--   0 goldy     (1001) goldy     (1001)     1520 2023-05-14 16:10:00.000000 devgoldyutils-2.5/devgoldyutils/colours.py
-drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-05-14 19:34:38.526313 devgoldyutils-2.5/devgoldyutils/console/
--rw-r--r--   0 goldy     (1001) goldy     (1001)      340 2023-05-14 16:10:00.000000 devgoldyutils-2.5/devgoldyutils/console/__init__.py
--rw-r--r--   0 goldy     (1001) goldy     (1001)      326 2023-05-14 16:10:00.000000 devgoldyutils-2.5/devgoldyutils/console/colours.py
--rw-r--r--   0 goldy     (1001) goldy     (1001)     1295 2023-05-14 16:10:00.000000 devgoldyutils-2.5/devgoldyutils/console/legacy_colours.py
--rw-r--r--   0 goldy     (1001) goldy     (1001)     4376 2023-05-14 16:52:57.000000 devgoldyutils-2.5/devgoldyutils/dict_classes.py
--rw-r--r--   0 goldy     (1001) goldy     (1001)      382 2023-05-14 16:10:00.000000 devgoldyutils-2.5/devgoldyutils/errors.py
--rw-r--r--   0 goldy     (1001) goldy     (1001)     1634 2023-05-14 16:52:08.000000 devgoldyutils-2.5/devgoldyutils/file_configs.py
--rw-r--r--   0 goldy     (1001) goldy     (1001)     1715 2023-05-14 16:10:00.000000 devgoldyutils-2.5/devgoldyutils/logging.py
-drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-05-14 19:34:38.526313 devgoldyutils-2.5/devgoldyutils.egg-info/
--rw-r--r--   0 goldy     (1001) goldy     (1001)    41573 2023-05-14 19:34:38.000000 devgoldyutils-2.5/devgoldyutils.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1001) goldy     (1001)      551 2023-05-14 19:34:38.000000 devgoldyutils-2.5/devgoldyutils.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1001) goldy     (1001)        1 2023-05-14 19:34:38.000000 devgoldyutils-2.5/devgoldyutils.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1001) goldy     (1001)       14 2023-05-14 19:34:38.000000 devgoldyutils-2.5/devgoldyutils.egg-info/requires.txt
--rw-r--r--   0 goldy     (1001) goldy     (1001)       14 2023-05-14 19:34:38.000000 devgoldyutils-2.5/devgoldyutils.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1001) goldy     (1001)     1250 2023-05-14 16:30:05.000000 devgoldyutils-2.5/pyproject.toml
--rw-r--r--   0 goldy     (1001) goldy     (1001)      441 2023-05-14 16:10:00.000000 devgoldyutils-2.5/readme.md
--rw-r--r--   0 goldy     (1001) goldy     (1001)       38 2023-05-14 19:34:38.527313 devgoldyutils-2.5/setup.cfg
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-05-16 19:41:30.764266 devgoldyutils-2.5.1/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       53 2023-05-14 16:10:00.000000 devgoldyutils-2.5.1/.gitignore
+-rw-r--r--   0 goldy     (1001) goldy     (1001)    35148 2023-05-14 16:10:00.000000 devgoldyutils-2.5.1/LICENSE
+-rwxr-xr-x   0 goldy     (1001) goldy     (1001)       32 2023-02-01 17:19:33.000000 devgoldyutils-2.5.1/MANIFEST.in
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       23 2023-05-14 16:10:00.000000 devgoldyutils-2.5.1/Makefile
+-rw-r--r--   0 goldy     (1001) goldy     (1001)    42017 2023-05-16 19:41:30.764266 devgoldyutils-2.5.1/PKG-INFO
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      441 2023-05-14 16:10:00.000000 devgoldyutils-2.5.1/README.md
+-rwxr-xr-x   0 goldy     (1001) goldy     (1001)     1670 2023-05-14 16:51:09.000000 devgoldyutils-2.5.1/demo.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-05-16 19:41:30.762266 devgoldyutils-2.5.1/devgoldyutils/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      467 2023-05-14 16:40:15.000000 devgoldyutils-2.5.1/devgoldyutils/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1497 2023-05-14 19:34:30.000000 devgoldyutils-2.5.1/devgoldyutils/better_get.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1520 2023-05-14 16:10:00.000000 devgoldyutils-2.5.1/devgoldyutils/colours.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-05-16 19:41:30.764266 devgoldyutils-2.5.1/devgoldyutils/console/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      340 2023-05-14 16:10:00.000000 devgoldyutils-2.5.1/devgoldyutils/console/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      326 2023-05-14 16:10:00.000000 devgoldyutils-2.5.1/devgoldyutils/console/colours.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1295 2023-05-14 16:10:00.000000 devgoldyutils-2.5.1/devgoldyutils/console/legacy_colours.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     4376 2023-05-14 16:52:57.000000 devgoldyutils-2.5.1/devgoldyutils/dict_classes.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      382 2023-05-14 16:10:00.000000 devgoldyutils-2.5.1/devgoldyutils/errors.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1634 2023-05-14 16:52:08.000000 devgoldyutils-2.5.1/devgoldyutils/file_configs.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1715 2023-05-14 16:10:00.000000 devgoldyutils-2.5.1/devgoldyutils/logging.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-05-16 19:41:30.763266 devgoldyutils-2.5.1/devgoldyutils.egg-info/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)    42017 2023-05-16 19:41:30.000000 devgoldyutils-2.5.1/devgoldyutils.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      551 2023-05-16 19:41:30.000000 devgoldyutils-2.5.1/devgoldyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1001) goldy     (1001)        1 2023-05-16 19:41:30.000000 devgoldyutils-2.5.1/devgoldyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       14 2023-05-16 19:41:30.000000 devgoldyutils-2.5.1/devgoldyutils.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       14 2023-05-16 19:41:30.000000 devgoldyutils-2.5.1/devgoldyutils.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1252 2023-05-16 19:40:59.000000 devgoldyutils-2.5.1/pyproject.toml
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       38 2023-05-16 19:41:30.764266 devgoldyutils-2.5.1/setup.cfg
```

### Comparing `devgoldyutils-2.5/LICENSE` & `devgoldyutils-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `devgoldyutils-2.5/PKG-INFO` & `devgoldyutils-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devgoldyutils
-Version: 2.5
+Version: 2.5.1
 Summary: My own utils library I use throughout all my python projects.
 Author-email: Goldy <goldy@devgoldy.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -689,7 +689,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+<div align="center">
+
+  # ⚒ devgoldyutils
+  
+  <sub>My own utils library I use throughout all my python projects.</sub>
+  
+  [![Pypi Badge](https://img.shields.io/pypi/v/devgoldyutils?style=flat)](https://pypi.org/project/devgoldyutils "We're on pypi!")
+  [![Python Badge](https://img.shields.io/pypi/pyversions/devgoldyutils?style=flat)](https://pypi.org/project/devgoldyutils "Supported python versions.")
+  
+</div>
+
+> whoo hooo, yeahhh
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `devgoldyutils-2.5/demo.py` & `devgoldyutils-2.5.1/demo.py`

 * *Files identical despite different names*

### Comparing `devgoldyutils-2.5/devgoldyutils/better_get.py` & `devgoldyutils-2.5.1/devgoldyutils/better_get.py`

 * *Files identical despite different names*

### Comparing `devgoldyutils-2.5/devgoldyutils/colours.py` & `devgoldyutils-2.5.1/devgoldyutils/colours.py`

 * *Files identical despite different names*

### Comparing `devgoldyutils-2.5/devgoldyutils/console/legacy_colours.py` & `devgoldyutils-2.5.1/devgoldyutils/console/legacy_colours.py`

 * *Files identical despite different names*

### Comparing `devgoldyutils-2.5/devgoldyutils/dict_classes.py` & `devgoldyutils-2.5.1/devgoldyutils/dict_classes.py`

 * *Files identical despite different names*

### Comparing `devgoldyutils-2.5/devgoldyutils/file_configs.py` & `devgoldyutils-2.5.1/devgoldyutils/file_configs.py`

 * *Files identical despite different names*

### Comparing `devgoldyutils-2.5/devgoldyutils/logging.py` & `devgoldyutils-2.5.1/devgoldyutils/logging.py`

 * *Files identical despite different names*

### Comparing `devgoldyutils-2.5/devgoldyutils.egg-info/PKG-INFO` & `devgoldyutils-2.5.1/devgoldyutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devgoldyutils
-Version: 2.5
+Version: 2.5.1
 Summary: My own utils library I use throughout all my python projects.
 Author-email: Goldy <goldy@devgoldy.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -689,7 +689,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+<div align="center">
+
+  # ⚒ devgoldyutils
+  
+  <sub>My own utils library I use throughout all my python projects.</sub>
+  
+  [![Pypi Badge](https://img.shields.io/pypi/v/devgoldyutils?style=flat)](https://pypi.org/project/devgoldyutils "We're on pypi!")
+  [![Python Badge](https://img.shields.io/pypi/pyversions/devgoldyutils?style=flat)](https://pypi.org/project/devgoldyutils "Supported python versions.")
+  
+</div>
+
+> whoo hooo, yeahhh
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `devgoldyutils-2.5/devgoldyutils.egg-info/SOURCES.txt` & `devgoldyutils-2.5.1/devgoldyutils.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .gitignore
 LICENSE
 MANIFEST.in
 Makefile
+README.md
 demo.py
 pyproject.toml
-readme.md
 devgoldyutils/__init__.py
 devgoldyutils/better_get.py
 devgoldyutils/colours.py
 devgoldyutils/dict_classes.py
 devgoldyutils/errors.py
 devgoldyutils/file_configs.py
 devgoldyutils/logging.py
```

### Comparing `devgoldyutils-2.5/pyproject.toml` & `devgoldyutils-2.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     'Programming Language :: Python :: 3.10',
 	'Programming Language :: Python :: 3.11'
 ]
 dependencies = [
     "prettyprinter"
 ]
 
-version = "2.5"
+version = "2.5.1"
 
 [project.urls]
 GitHub = "https://github.com/THEGOLDENPRO/devgoldyutils"
 BugTracker = "https://github.com/THEGOLDENPRO/devgoldyutils/issues"
 ChangeLog = "https://github.com/THEGOLDENPRO/devgoldyutils/master/CHANGELOG.md"
 
 [build-system]
```

