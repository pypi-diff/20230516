# Comparing `tmp/pyskema-0.4.0.tar.gz` & `tmp/pyskema-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyskema-0.4.0.tar", last modified: Thu Mar  9 16:08:04 2023, max compression
+gzip compressed data, was "pyskema-0.4.1.tar", last modified: Tue May 16 13:06:04 2023, max compression
```

## Comparing `pyskema-0.4.0.tar` & `pyskema-0.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-03-09 16:08:04.824824 pyskema-0.4.0/
--rw-r--r--   0 theo      (1000) theo      (1000)       34 2023-03-08 16:07:43.000000 pyskema-0.4.0/.gitignore
--rw-r--r--   0 theo      (1000) theo      (1000)      593 2023-03-07 17:09:35.000000 pyskema-0.4.0/.readthedocs.yaml
--rw-r--r--   0 theo      (1000) theo      (1000)     1493 2023-03-07 14:21:36.000000 pyskema-0.4.0/LICENSE
--rw-r--r--   0 theo      (1000) theo      (1000)     2625 2023-03-09 16:08:04.824824 pyskema-0.4.0/PKG-INFO
--rw-r--r--   0 theo      (1000) theo      (1000)      349 2023-03-08 15:03:31.000000 pyskema-0.4.0/README.md
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-03-09 16:08:04.818158 pyskema-0.4.0/docs/
--rw-r--r--   0 theo      (1000) theo      (1000)        7 2023-03-07 16:59:45.000000 pyskema-0.4.0/docs/.gitignore
--rw-r--r--   0 theo      (1000) theo      (1000)      804 2023-03-08 15:50:36.000000 pyskema-0.4.0/docs/Makefile
--rw-r--r--   0 theo      (1000) theo      (1000)      365 2023-03-08 16:02:39.000000 pyskema-0.4.0/docs/conf.py
--rw-r--r--   0 theo      (1000) theo      (1000)     2919 2023-03-09 15:59:02.000000 pyskema-0.4.0/docs/index.rst
--rw-r--r--   0 theo      (1000) theo      (1000)      800 2023-03-07 13:56:46.000000 pyskema-0.4.0/docs/make.bat
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-03-09 16:08:04.821491 pyskema-0.4.0/docs/ref/
--rw-r--r--   0 theo      (1000) theo      (1000)     1093 2023-03-09 15:59:05.000000 pyskema-0.4.0/docs/ref/pyskema.rst
--rw-r--r--   0 theo      (1000) theo      (1000)      906 2023-03-08 16:24:48.000000 pyskema-0.4.0/pyproject.toml
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-03-09 16:08:04.821491 pyskema-0.4.0/pyskema/
--rw-r--r--   0 theo      (1000) theo      (1000)      243 2023-03-09 15:16:02.000000 pyskema-0.4.0/pyskema/__init__.py
--rw-r--r--   0 theo      (1000) theo      (1000)     5469 2023-03-09 15:25:54.000000 pyskema-0.4.0/pyskema/describe.py
--rw-r--r--   0 theo      (1000) theo      (1000)     4034 2023-03-09 15:48:40.000000 pyskema-0.4.0/pyskema/edit.py
--rw-r--r--   0 theo      (1000) theo      (1000)     1902 2023-03-07 14:03:21.000000 pyskema-0.4.0/pyskema/misc.py
--rw-r--r--   0 theo      (1000) theo      (1000)     9616 2023-03-09 15:46:33.000000 pyskema-0.4.0/pyskema/schema.py
--rw-r--r--   0 theo      (1000) theo      (1000)     1651 2023-03-07 14:03:21.000000 pyskema-0.4.0/pyskema/template.py
--rw-r--r--   0 theo      (1000) theo      (1000)     8330 2023-03-07 14:05:01.000000 pyskema-0.4.0/pyskema/validate.py
--rw-r--r--   0 theo      (1000) theo      (1000)     2794 2023-03-09 15:03:59.000000 pyskema-0.4.0/pyskema/visitor.py
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-03-09 16:08:04.824824 pyskema-0.4.0/pyskema.egg-info/
--rw-r--r--   0 theo      (1000) theo      (1000)     2625 2023-03-09 16:08:04.000000 pyskema-0.4.0/pyskema.egg-info/PKG-INFO
--rw-r--r--   0 theo      (1000) theo      (1000)      474 2023-03-09 16:08:04.000000 pyskema-0.4.0/pyskema.egg-info/SOURCES.txt
--rw-r--r--   0 theo      (1000) theo      (1000)        1 2023-03-09 16:08:04.000000 pyskema-0.4.0/pyskema.egg-info/dependency_links.txt
--rw-r--r--   0 theo      (1000) theo      (1000)       18 2023-03-09 16:08:04.000000 pyskema-0.4.0/pyskema.egg-info/top_level.txt
--rw-r--r--   0 theo      (1000) theo      (1000)       38 2023-03-09 16:08:04.824824 pyskema-0.4.0/setup.cfg
-drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-03-09 16:08:04.824824 pyskema-0.4.0/tests/
--rw-r--r--   0 theo      (1000) theo      (1000)     1692 2023-03-08 16:23:20.000000 pyskema-0.4.0/tests/test_pyschema.py
--rw-r--r--   0 theo      (1000) theo      (1000)     6977 2023-03-08 16:23:20.000000 pyskema-0.4.0/tests/test_real_file.py
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-05-16 13:06:04.465505 pyskema-0.4.1/
+-rw-r--r--   0 theo      (1000) theo      (1000)       34 2023-03-08 16:07:43.000000 pyskema-0.4.1/.gitignore
+-rw-r--r--   0 theo      (1000) theo      (1000)      593 2023-03-07 17:09:35.000000 pyskema-0.4.1/.readthedocs.yaml
+-rw-r--r--   0 theo      (1000) theo      (1000)     1493 2023-03-07 14:21:36.000000 pyskema-0.4.1/LICENSE
+-rw-r--r--   0 theo      (1000) theo      (1000)     2625 2023-05-16 13:06:04.462171 pyskema-0.4.1/PKG-INFO
+-rw-r--r--   0 theo      (1000) theo      (1000)      349 2023-03-08 15:03:31.000000 pyskema-0.4.1/README.md
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-05-16 13:06:04.458838 pyskema-0.4.1/docs/
+-rw-r--r--   0 theo      (1000) theo      (1000)        7 2023-03-07 16:59:45.000000 pyskema-0.4.1/docs/.gitignore
+-rw-r--r--   0 theo      (1000) theo      (1000)      804 2023-03-08 15:50:36.000000 pyskema-0.4.1/docs/Makefile
+-rw-r--r--   0 theo      (1000) theo      (1000)      365 2023-03-08 16:02:39.000000 pyskema-0.4.1/docs/conf.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     2919 2023-03-09 15:59:02.000000 pyskema-0.4.1/docs/index.rst
+-rw-r--r--   0 theo      (1000) theo      (1000)      800 2023-03-07 13:56:46.000000 pyskema-0.4.1/docs/make.bat
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-05-16 13:06:04.458838 pyskema-0.4.1/docs/ref/
+-rw-r--r--   0 theo      (1000) theo      (1000)     1093 2023-03-09 15:59:05.000000 pyskema-0.4.1/docs/ref/pyskema.rst
+-rw-r--r--   0 theo      (1000) theo      (1000)      906 2023-03-08 16:24:48.000000 pyskema-0.4.1/pyproject.toml
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-05-16 13:06:04.462171 pyskema-0.4.1/pyskema/
+-rw-r--r--   0 theo      (1000) theo      (1000)      243 2023-05-16 13:02:51.000000 pyskema-0.4.1/pyskema/__init__.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     5469 2023-03-09 15:25:54.000000 pyskema-0.4.1/pyskema/describe.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     4034 2023-03-09 15:48:40.000000 pyskema-0.4.1/pyskema/edit.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     1902 2023-03-07 14:03:21.000000 pyskema-0.4.1/pyskema/misc.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     9616 2023-03-09 15:46:33.000000 pyskema-0.4.1/pyskema/schema.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     1651 2023-03-07 14:03:21.000000 pyskema-0.4.1/pyskema/template.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     8337 2023-05-16 13:01:32.000000 pyskema-0.4.1/pyskema/validate.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     2794 2023-03-09 15:03:59.000000 pyskema-0.4.1/pyskema/visitor.py
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-05-16 13:06:04.462171 pyskema-0.4.1/pyskema.egg-info/
+-rw-r--r--   0 theo      (1000) theo      (1000)     2625 2023-05-16 13:06:04.000000 pyskema-0.4.1/pyskema.egg-info/PKG-INFO
+-rw-r--r--   0 theo      (1000) theo      (1000)      474 2023-05-16 13:06:04.000000 pyskema-0.4.1/pyskema.egg-info/SOURCES.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)        1 2023-05-16 13:06:04.000000 pyskema-0.4.1/pyskema.egg-info/dependency_links.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)       24 2023-05-16 13:06:04.000000 pyskema-0.4.1/pyskema.egg-info/top_level.txt
+-rw-r--r--   0 theo      (1000) theo      (1000)       38 2023-05-16 13:06:04.465505 pyskema-0.4.1/setup.cfg
+drwxr-xr-x   0 theo      (1000) theo      (1000)        0 2023-05-16 13:06:04.462171 pyskema-0.4.1/tests/
+-rw-r--r--   0 theo      (1000) theo      (1000)     1692 2023-03-08 16:23:20.000000 pyskema-0.4.1/tests/test_pyschema.py
+-rw-r--r--   0 theo      (1000) theo      (1000)     6977 2023-03-08 16:23:20.000000 pyskema-0.4.1/tests/test_real_file.py
```

### Comparing `pyskema-0.4.0/.readthedocs.yaml` & `pyskema-0.4.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pyskema-0.4.0/LICENSE` & `pyskema-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyskema-0.4.0/PKG-INFO` & `pyskema-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyskema
-Version: 0.4.0
+Version: 0.4.1
 Summary: A schema definition module for validation and documentation of structured data.
 Author-email: Théo Cavignac <theo.cavignac+dev@gmail.com>
 License: Copyright 2023 Théo Cavignac <theo.cavignac+dev@gmail.com>
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `pyskema-0.4.0/docs/Makefile` & `pyskema-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyskema-0.4.0/docs/index.rst` & `pyskema-0.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyskema-0.4.0/docs/make.bat` & `pyskema-0.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyskema-0.4.0/docs/ref/pyskema.rst` & `pyskema-0.4.1/docs/ref/pyskema.rst`

 * *Files identical despite different names*

### Comparing `pyskema-0.4.0/pyproject.toml` & `pyskema-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyskema-0.4.0/pyskema/describe.py` & `pyskema-0.4.1/pyskema/describe.py`

 * *Files identical despite different names*

### Comparing `pyskema-0.4.0/pyskema/edit.py` & `pyskema-0.4.1/pyskema/edit.py`

 * *Files identical despite different names*

### Comparing `pyskema-0.4.0/pyskema/misc.py` & `pyskema-0.4.1/pyskema/misc.py`

 * *Files identical despite different names*

### Comparing `pyskema-0.4.0/pyskema/schema.py` & `pyskema-0.4.1/pyskema/schema.py`

 * *Files identical despite different names*

### Comparing `pyskema-0.4.0/pyskema/template.py` & `pyskema-0.4.1/pyskema/template.py`

 * *Files identical despite different names*

### Comparing `pyskema-0.4.0/pyskema/validate.py` & `pyskema-0.4.1/pyskema/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                 return Result.ok(data)
             elif isinstance(data, float):
                 if int(data) == data:
                     return Result.ok(int(data))
 
         elif atom.type_ == AtomType.FLOAT:
             if isinstance(data, (float, int)):
-                return Result.ok(data)
+                return Result.ok(float(data))
 
         elif atom.type_ == AtomType.STR:
             if isinstance(data, str):
                 return Result.ok(data)
 
         elif atom.type_ == AtomType.OPTION:
             assert atom.options is not None, "atom.options must be set"
```

### Comparing `pyskema-0.4.0/pyskema/visitor.py` & `pyskema-0.4.1/pyskema/visitor.py`

 * *Files identical despite different names*

### Comparing `pyskema-0.4.0/pyskema.egg-info/PKG-INFO` & `pyskema-0.4.1/pyskema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyskema
-Version: 0.4.0
+Version: 0.4.1
 Summary: A schema definition module for validation and documentation of structured data.
 Author-email: Théo Cavignac <theo.cavignac+dev@gmail.com>
 License: Copyright 2023 Théo Cavignac <theo.cavignac+dev@gmail.com>
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `pyskema-0.4.0/tests/test_pyschema.py` & `pyskema-0.4.1/tests/test_pyschema.py`

 * *Files identical despite different names*

### Comparing `pyskema-0.4.0/tests/test_real_file.py` & `pyskema-0.4.1/tests/test_real_file.py`

 * *Files identical despite different names*

