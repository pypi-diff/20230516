# Comparing `tmp/python-barn-0.6.0.tar.gz` & `tmp/python-barn-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-barn-0.6.0.tar", last modified: Tue May 16 15:06:29 2023, max compression
+gzip compressed data, was "python-barn-0.7.0.tar", last modified: Tue May 16 18:02:31 2023, max compression
```

## Comparing `python-barn-0.6.0.tar` & `python-barn-0.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:06:29.543465 python-barn-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-16 15:06:29.543465 python-barn-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-16 15:06:17.000000 python-barn-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:06:29.539465 python-barn-0.6.0/python_barn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-16 15:06:29.000000 python-barn-0.6.0/python_barn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-16 15:06:29.000000 python-barn-0.6.0/python_barn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 15:06:29.000000 python-barn-0.6.0/python_barn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 15:06:29.000000 python-barn-0.6.0/python_barn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 15:06:29.000000 python-barn-0.6.0/python_barn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-16 15:06:29.000000 python-barn-0.6.0/python_barn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 15:06:29.543465 python-barn-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-16 15:06:17.000000 python-barn-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:06:29.539465 python-barn-0.6.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-16 15:06:17.000000 python-barn-0.6.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:06:29.539465 python-barn-0.6.0/src/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-16 15:06:17.000000 python-barn-0.6.0/src/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-16 15:06:17.000000 python-barn-0.6.0/src/actions/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-16 15:06:17.000000 python-barn-0.6.0/src/actions/execute_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-16 15:06:17.000000 python-barn-0.6.0/src/actions/init.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-16 15:06:17.000000 python-barn-0.6.0/src/actions/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-16 15:06:17.000000 python-barn-0.6.0/src/actions/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-16 15:06:17.000000 python-barn-0.6.0/src/actions/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-16 15:06:17.000000 python-barn-0.6.0/src/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-16 15:06:17.000000 python-barn-0.6.0/src/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-16 15:06:17.000000 python-barn-0.6.0/src/logging_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:02:31.115624 python-barn-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-16 18:02:31.115624 python-barn-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-16 18:02:19.000000 python-barn-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:02:31.111624 python-barn-0.7.0/python_barn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-16 18:02:31.000000 python-barn-0.7.0/python_barn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-16 18:02:31.000000 python-barn-0.7.0/python_barn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:02:31.000000 python-barn-0.7.0/python_barn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 18:02:31.000000 python-barn-0.7.0/python_barn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 18:02:31.000000 python-barn-0.7.0/python_barn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-16 18:02:31.000000 python-barn-0.7.0/python_barn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 18:02:31.115624 python-barn-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-16 18:02:19.000000 python-barn-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:02:31.111624 python-barn-0.7.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-16 18:02:19.000000 python-barn-0.7.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:02:31.115624 python-barn-0.7.0/src/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-16 18:02:19.000000 python-barn-0.7.0/src/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-16 18:02:19.000000 python-barn-0.7.0/src/actions/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-16 18:02:19.000000 python-barn-0.7.0/src/actions/execute_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-16 18:02:19.000000 python-barn-0.7.0/src/actions/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-16 18:02:19.000000 python-barn-0.7.0/src/actions/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-16 18:02:19.000000 python-barn-0.7.0/src/actions/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-16 18:02:19.000000 python-barn-0.7.0/src/actions/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-16 18:02:19.000000 python-barn-0.7.0/src/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-16 18:02:19.000000 python-barn-0.7.0/src/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-16 18:02:19.000000 python-barn-0.7.0/src/logging_utils.py
```

### Comparing `python-barn-0.6.0/PKG-INFO` & `python-barn-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-barn
-Version: 0.6.0
+Version: 0.7.0
 Summary: A wrapper for pip, to give better utils to python projects dependency management
 Home-page: https://github.com/JacopoMadaluni/barn
 Author: Jacopo Madaluni
 Author-email: jacopo.madaluni@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `python-barn-0.6.0/README.md` & `python-barn-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `python-barn-0.6.0/python_barn.egg-info/PKG-INFO` & `python-barn-0.7.0/python_barn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-barn
-Version: 0.6.0
+Version: 0.7.0
 Summary: A wrapper for pip, to give better utils to python projects dependency management
 Home-page: https://github.com/JacopoMadaluni/barn
 Author: Jacopo Madaluni
 Author-email: jacopo.madaluni@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `python-barn-0.6.0/setup.py` & `python-barn-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="python-barn",
-    version="0.6.0",
+    version="0.7.0",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "barn=src.cli:main",
         ],
     },
     package_data={
```

### Comparing `python-barn-0.6.0/src/actions/add.py` & `python-barn-0.7.0/src/actions/add.py`

 * *Files identical despite different names*

### Comparing `python-barn-0.6.0/src/actions/execute_script.py` & `python-barn-0.7.0/src/actions/execute_script.py`

 * *Files identical despite different names*

### Comparing `python-barn-0.6.0/src/actions/init.py` & `python-barn-0.7.0/src/actions/init.py`

 * *Files identical despite different names*

### Comparing `python-barn-0.6.0/src/actions/install.py` & `python-barn-0.7.0/src/actions/install.py`

 * *Files identical despite different names*

### Comparing `python-barn-0.6.0/src/cli.py` & `python-barn-0.7.0/src/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     # subparsers.add_parser('test')
 
     # Parse the arguments
  
     args, unknown_args = parser.parse_known_args()
 
     exit_code = 0
-    if len(unknown_args) and args.command is None > 0:
+    if len(unknown_args) > 0 and args.command is None:
         _, exit_code = execute_script(unknown_args[0], unknown_args[1:])
     # If no command is given, print help and exit
     elif args.command is None:
         _, exit_code = install()
     elif args.command == 'show':
         _, exit_code = show(args.package_name, verbose=args.verbose, files=args.files)
     elif args.command == 'install':
```

### Comparing `python-barn-0.6.0/src/core.py` & `python-barn-0.7.0/src/core.py`

 * *Files identical despite different names*

### Comparing `python-barn-0.6.0/src/logging_utils.py` & `python-barn-0.7.0/src/logging_utils.py`

 * *Files identical despite different names*

