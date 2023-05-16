# Comparing `tmp/dynamic-yaml-1.3.3.tar.gz` & `tmp/dynamic-yaml-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-yaml-1.3.3.tar", last modified: Wed Oct 19 21:01:33 2022, max compression
+gzip compressed data, was "dynamic-yaml-1.3.4.tar", last modified: Tue May 16 13:13:32 2023, max compression
```

## Comparing `dynamic-yaml-1.3.3.tar` & `dynamic-yaml-1.3.4.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 21:01:33.504850 dynamic-yaml-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-10-19 21:01:22.000000 dynamic-yaml-1.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6434 2022-10-19 21:01:33.504850 dynamic-yaml-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4699 2022-10-19 21:01:22.000000 dynamic-yaml-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 21:01:33.504850 dynamic-yaml-1.3.3/dynamic_yaml/
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-10-19 21:01:22.000000 dynamic-yaml-1.3.3/dynamic_yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3187 2022-10-19 21:01:22.000000 dynamic-yaml-1.3.3/dynamic_yaml/yaml_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 21:01:33.504850 dynamic-yaml-1.3.3/dynamic_yaml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6434 2022-10-19 21:01:33.000000 dynamic-yaml-1.3.3/dynamic_yaml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-10-19 21:01:33.000000 dynamic-yaml-1.3.3/dynamic_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 21:01:33.000000 dynamic-yaml-1.3.3/dynamic_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-19 21:01:33.000000 dynamic-yaml-1.3.3/dynamic_yaml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-19 21:01:33.000000 dynamic-yaml-1.3.3/dynamic_yaml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-10-19 21:01:22.000000 dynamic-yaml-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-19 21:01:33.504850 dynamic-yaml-1.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:32.198892 dynamic-yaml-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 13:13:04.000000 dynamic-yaml-1.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-05-16 13:13:32.198892 dynamic-yaml-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-16 13:13:04.000000 dynamic-yaml-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:32.194893 dynamic-yaml-1.3.4/dynamic_yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-16 13:13:04.000000 dynamic-yaml-1.3.4/dynamic_yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-16 13:13:04.000000 dynamic-yaml-1.3.4/dynamic_yaml/yaml_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:32.194893 dynamic-yaml-1.3.4/dynamic_yaml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-05-16 13:13:32.000000 dynamic-yaml-1.3.4/dynamic_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-16 13:13:32.000000 dynamic-yaml-1.3.4/dynamic_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:13:32.000000 dynamic-yaml-1.3.4/dynamic_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 13:13:32.000000 dynamic-yaml-1.3.4/dynamic_yaml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 13:13:32.000000 dynamic-yaml-1.3.4/dynamic_yaml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-16 13:13:04.000000 dynamic-yaml-1.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:13:32.198892 dynamic-yaml-1.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:32.194893 dynamic-yaml-1.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-05-16 13:13:04.000000 dynamic-yaml-1.3.4/tests/test_dynamic_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-16 13:13:04.000000 dynamic-yaml-1.3.4/tests/test_representations.py
```

### Comparing `dynamic-yaml-1.3.3/LICENSE.txt` & `dynamic-yaml-1.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dynamic-yaml-1.3.3/PKG-INFO` & `dynamic-yaml-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-yaml
-Version: 1.3.3
+Version: 1.3.4
 Summary: Enables self referential yaml entries
 Author-email: "Liam H. Childs" <liam.h.childs@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Liam H. Childs
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dynamic-yaml-1.3.3/README.md` & `dynamic-yaml-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `dynamic-yaml-1.3.3/dynamic_yaml/__init__.py` & `dynamic-yaml-1.3.4/dynamic_yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `dynamic-yaml-1.3.3/dynamic_yaml/yaml_wrappers.py` & `dynamic-yaml-1.3.4/dynamic_yaml/yaml_wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,17 @@
         if key in self:
             return self[key]
         return super().__getattribute__(key)
 
     def __setattr__(self, key, value):
         self[key] = value
 
+    def __delattr__(self, key):
+        del self[key]
+
     def _values(self):
         return super().__getattribute__('_collection').values()
 
 
 class YamlList(DynamicYamlObject, MutableSequence):
     ROOT_NAME = 'root'
```

### Comparing `dynamic-yaml-1.3.3/dynamic_yaml.egg-info/PKG-INFO` & `dynamic-yaml-1.3.4/dynamic_yaml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-yaml
-Version: 1.3.3
+Version: 1.3.4
 Summary: Enables self referential yaml entries
 Author-email: "Liam H. Childs" <liam.h.childs@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Liam H. Childs
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dynamic-yaml-1.3.3/pyproject.toml` & `dynamic-yaml-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dynamic-yaml"
-version = "1.3.3"
+version = "1.3.4"
 description = "Enables self referential yaml entries"
 readme = "README.md"
 authors = [{ name = "Liam H. Childs", email = "liam.h.childs@gmail.com" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

