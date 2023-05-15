# Comparing `tmp/rcmpy-1.4.0.tar.gz` & `tmp/rcmpy-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcmpy-1.4.0.tar", last modified: Sun May  7 21:30:24 2023, max compression
+gzip compressed data, was "rcmpy-1.4.1.tar", last modified: Mon May 15 22:36:03 2023, max compression
```

## Comparing `rcmpy-1.4.0.tar` & `rcmpy-1.4.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.536857 rcmpy-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-07 21:28:52.000000 rcmpy-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-05-07 21:30:24.536857 rcmpy-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-05-07 21:28:52.000000 rcmpy-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-07 21:28:52.000000 rcmpy-1.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.524857 rcmpy-1.4.0/rcmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.528857 rcmpy-1.4.0/rcmpy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/commands/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/commands/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/commands/use.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/commands/variant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/commands/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.528857 rcmpy-1.4.0/rcmpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/config/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.524857 rcmpy-1.4.0/rcmpy/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.528857 rcmpy-1.4.0/rcmpy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/data/schemas/ManagedFile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/data/schemas/State.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.532857 rcmpy-1.4.0/rcmpy/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/environment/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/environment/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.532857 rcmpy-1.4.0/rcmpy/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.532857 rcmpy-1.4.0/rcmpy/state/
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/state/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.532857 rcmpy-1.4.0/rcmpy/xdg/
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/xdg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.528857 rcmpy-1.4.0/rcmpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-05-07 21:30:24.000000 rcmpy-1.4.0/rcmpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-07 21:30:24.000000 rcmpy-1.4.0/rcmpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 21:30:24.000000 rcmpy-1.4.0/rcmpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-07 21:30:24.000000 rcmpy-1.4.0/rcmpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-07 21:30:24.000000 rcmpy-1.4.0/rcmpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 21:30:24.000000 rcmpy-1.4.0/rcmpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 21:30:24.536857 rcmpy-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-07 21:28:52.000000 rcmpy-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.532857 rcmpy-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-07 21:28:52.000000 rcmpy-1.4.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-07 21:28:52.000000 rcmpy-1.4.0/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-07 21:28:52.000000 rcmpy-1.4.0/tests/test_xdg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:36:03.738680 rcmpy-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 22:34:50.000000 rcmpy-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-05-15 22:36:03.738680 rcmpy-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-05-15 22:34:50.000000 rcmpy-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-15 22:34:50.000000 rcmpy-1.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:36:03.734680 rcmpy-1.4.1/rcmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:36:03.738680 rcmpy-1.4.1/rcmpy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/commands/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/commands/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/commands/use.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/commands/variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/commands/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:36:03.738680 rcmpy-1.4.1/rcmpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/config/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:36:03.734680 rcmpy-1.4.1/rcmpy/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:36:03.738680 rcmpy-1.4.1/rcmpy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/data/schemas/ManagedFile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/data/schemas/State.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:36:03.738680 rcmpy-1.4.1/rcmpy/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/environment/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/environment/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:36:03.738680 rcmpy-1.4.1/rcmpy/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:36:03.738680 rcmpy-1.4.1/rcmpy/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/state/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:36:03.738680 rcmpy-1.4.1/rcmpy/xdg/
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-15 22:34:50.000000 rcmpy-1.4.1/rcmpy/xdg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:36:03.734680 rcmpy-1.4.1/rcmpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-05-15 22:36:03.000000 rcmpy-1.4.1/rcmpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-15 22:36:03.000000 rcmpy-1.4.1/rcmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:36:03.000000 rcmpy-1.4.1/rcmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 22:36:03.000000 rcmpy-1.4.1/rcmpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-15 22:36:03.000000 rcmpy-1.4.1/rcmpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 22:36:03.000000 rcmpy-1.4.1/rcmpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:36:03.738680 rcmpy-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-15 22:34:50.000000 rcmpy-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:36:03.738680 rcmpy-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-15 22:34:50.000000 rcmpy-1.4.1/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-15 22:34:50.000000 rcmpy-1.4.1/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-15 22:34:50.000000 rcmpy-1.4.1/tests/test_xdg.py
```

### Comparing `rcmpy-1.4.0/LICENSE` & `rcmpy-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rcmpy-1.4.0/PKG-INFO` & `rcmpy-1.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 1.4.0
+Version: 1.4.1
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=c1786731fe10b81b6b18afa242c53257
+    hash=a3c34cf886cf3dbc2f8bf336f6b2d7b5
     =====================================
 -->
 
-# rcmpy ([1.4.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.4.1](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
 
@@ -229,26 +229,28 @@
 ```
 
 ### `watch`
 
 ```
 $ ./venv3.11/bin/rcmpy watch -h
 
-usage: rcmpy watch [-h] [-p POLL_RATE] [-s] [-i] directory cmd [cmd ...]
+usage: rcmpy watch [-h] [-p POLL_RATE] [-s] [-i] [-n] directory cmd [cmd ...]
 
 positional arguments:
   directory             directory to watch for file changes
   cmd                   command to run
 
 options:
   -h, --help            show this help message and exit
   -p POLL_RATE, --poll-rate POLL_RATE
                         poll period in seconds (default: 0.1s)
   -s, --shell           set to run a shell command
   -i, --single-pass     only run a single iteration
+  -n, --no-change       don't act on changed files, only the overall set of
+                        files changing (added or removed)
 
 ```
 
 # Internal Dependency Graph
 
 A coarse view of the internal structure and scale of
 `rcmpy`'s source.
```

### Comparing `rcmpy-1.4.0/README.md` & `rcmpy-1.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=c1786731fe10b81b6b18afa242c53257
+    hash=a3c34cf886cf3dbc2f8bf336f6b2d7b5
     =====================================
 -->
 
-# rcmpy ([1.4.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.4.1](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
 
@@ -205,26 +205,28 @@
 ```
 
 ### `watch`
 
 ```
 $ ./venv3.11/bin/rcmpy watch -h
 
-usage: rcmpy watch [-h] [-p POLL_RATE] [-s] [-i] directory cmd [cmd ...]
+usage: rcmpy watch [-h] [-p POLL_RATE] [-s] [-i] [-n] directory cmd [cmd ...]
 
 positional arguments:
   directory             directory to watch for file changes
   cmd                   command to run
 
 options:
   -h, --help            show this help message and exit
   -p POLL_RATE, --poll-rate POLL_RATE
                         poll period in seconds (default: 0.1s)
   -s, --shell           set to run a shell command
   -i, --single-pass     only run a single iteration
+  -n, --no-change       don't act on changed files, only the overall set of
+                        files changing (added or removed)
 
 ```
 
 # Internal Dependency Graph
 
 A coarse view of the internal structure and scale of
 `rcmpy`'s source.
```

### Comparing `rcmpy-1.4.0/pyproject.toml` & `rcmpy-1.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "rcmpy"
-version = "1.4.0"
+version = "1.4.1"
 description = "A configuration-file management system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `rcmpy-1.4.0/rcmpy/app.py` & `rcmpy-1.4.1/rcmpy/app.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.4.0/rcmpy/commands/all.py` & `rcmpy-1.4.1/rcmpy/commands/all.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.4.0/rcmpy/commands/apply.py` & `rcmpy-1.4.1/rcmpy/commands/apply.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.4.0/rcmpy/commands/common.py` & `rcmpy-1.4.1/rcmpy/commands/common.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.4.0/rcmpy/commands/dump.py` & `rcmpy-1.4.1/rcmpy/commands/dump.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.4.0/rcmpy/commands/use.py` & `rcmpy-1.4.1/rcmpy/commands/use.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.4.0/rcmpy/commands/variant.py` & `rcmpy-1.4.1/rcmpy/commands/variant.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.4.0/rcmpy/commands/watch.py` & `rcmpy-1.4.1/rcmpy/commands/watch.py`

 * *Files 15% similar despite different names*

```diff
@@ -46,15 +46,17 @@
     def poll_cb(_: FileChanged) -> bool:
         """Method to run when any watched file changes."""
 
         nonlocal count
         count += 1
         return True
 
-    with file_info_cache(cache_file, poll_cb, logger=LOG) as files:
+    with file_info_cache(
+        cache_file, poll_cb, logger=LOG, check_contents=not args.no_change
+    ) as files:
         while not stop_sig.is_set():
             files.poll_directory(args.directory, base=args.dir)
             files.poll_existing(base=args.dir)
 
             if count > 0:
                 # Run the command, return True if it exits 0.
                 await command(*args.cmd, shell=args.shell)
@@ -96,12 +98,21 @@
     parser.add_argument(
         "-i",
         "--single-pass",
         action="store_true",
         help="only run a single iteration",
     )
     parser.add_argument(
+        "-n",
+        "--no-change",
+        action="store_true",
+        help=(
+            "don't act on changed files, only the overall "
+            "set of files changing (added or removed)"
+        ),
+    )
+    parser.add_argument(
         "directory", type=Path, help="directory to watch for file changes"
     )
     parser.add_argument("cmd", nargs="+", help="command to run")
 
     return watch_cmd
```

### Comparing `rcmpy-1.4.0/rcmpy/config/__init__.py` & `rcmpy-1.4.1/rcmpy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.4.0/rcmpy/config/file.py` & `rcmpy-1.4.1/rcmpy/config/file.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.4.0/rcmpy/data/schemas/ManagedFile.yaml` & `rcmpy-1.4.1/rcmpy/data/schemas/ManagedFile.yaml`

 * *Files identical despite different names*

### Comparing `rcmpy-1.4.0/rcmpy/entry.py` & `rcmpy-1.4.1/rcmpy/entry.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.4.0/rcmpy/environment/__init__.py` & `rcmpy-1.4.1/rcmpy/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.4.0/rcmpy/environment/base.py` & `rcmpy-1.4.1/rcmpy/environment/base.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.4.0/rcmpy/environment/data.py` & `rcmpy-1.4.1/rcmpy/environment/data.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.4.0/rcmpy/environment/template.py` & `rcmpy-1.4.1/rcmpy/environment/template.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.4.0/rcmpy/paths/__init__.py` & `rcmpy-1.4.1/rcmpy/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.4.0/rcmpy/schemas.py` & `rcmpy-1.4.1/rcmpy/schemas.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.4.0/rcmpy/state/__init__.py` & `rcmpy-1.4.1/rcmpy/state/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.4.0/rcmpy/xdg/__init__.py` & `rcmpy-1.4.1/rcmpy/xdg/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.4.0/rcmpy.egg-info/PKG-INFO` & `rcmpy-1.4.1/rcmpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 1.4.0
+Version: 1.4.1
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=c1786731fe10b81b6b18afa242c53257
+    hash=a3c34cf886cf3dbc2f8bf336f6b2d7b5
     =====================================
 -->
 
-# rcmpy ([1.4.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.4.1](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
 
@@ -229,26 +229,28 @@
 ```
 
 ### `watch`
 
 ```
 $ ./venv3.11/bin/rcmpy watch -h
 
-usage: rcmpy watch [-h] [-p POLL_RATE] [-s] [-i] directory cmd [cmd ...]
+usage: rcmpy watch [-h] [-p POLL_RATE] [-s] [-i] [-n] directory cmd [cmd ...]
 
 positional arguments:
   directory             directory to watch for file changes
   cmd                   command to run
 
 options:
   -h, --help            show this help message and exit
   -p POLL_RATE, --poll-rate POLL_RATE
                         poll period in seconds (default: 0.1s)
   -s, --shell           set to run a shell command
   -i, --single-pass     only run a single iteration
+  -n, --no-change       don't act on changed files, only the overall set of
+                        files changing (added or removed)
 
 ```
 
 # Internal Dependency Graph
 
 A coarse view of the internal structure and scale of
 `rcmpy`'s source.
```

### Comparing `rcmpy-1.4.0/rcmpy.egg-info/SOURCES.txt` & `rcmpy-1.4.1/rcmpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcmpy-1.4.0/setup.py` & `rcmpy-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.4.0/tests/test_entry.py` & `rcmpy-1.4.1/tests/test_entry.py`

 * *Files identical despite different names*

