# Comparing `tmp/mmlab_lightning-1.0.4.tar.gz` & `tmp/mmlab_lightning-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmlab_lightning-1.0.4.tar", last modified: Wed May  3 05:34:25 2023, max compression
+gzip compressed data, was "mmlab_lightning-1.0.5.tar", last modified: Tue May 16 09:41:54 2023, max compression
```

## Comparing `mmlab_lightning-1.0.4.tar` & `mmlab_lightning-1.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:34:25.743048 mmlab_lightning-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-03 05:34:12.000000 mmlab_lightning-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-03 05:34:25.739047 mmlab_lightning-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-03 05:34:12.000000 mmlab_lightning-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:34:25.739047 mmlab_lightning-1.0.4/mmlab_lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-03 05:34:12.000000 mmlab_lightning-1.0.4/mmlab_lightning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:34:25.739047 mmlab_lightning-1.0.4/mmlab_lightning/datasets/
--rwxr-xr-x   0 runner    (1001) docker     (123)       78 2023-05-03 05:34:12.000000 mmlab_lightning-1.0.4/mmlab_lightning/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-03 05:34:12.000000 mmlab_lightning-1.0.4/mmlab_lightning/datasets/mmlab_dataset_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:34:25.739047 mmlab_lightning-1.0.4/mmlab_lightning/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-05-03 05:34:12.000000 mmlab_lightning-1.0.4/mmlab_lightning/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-03 05:34:12.000000 mmlab_lightning-1.0.4/mmlab_lightning/models/mmlab_model_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:34:25.739047 mmlab_lightning-1.0.4/mmlab_lightning/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-03 05:34:12.000000 mmlab_lightning-1.0.4/mmlab_lightning/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:34:25.739047 mmlab_lightning-1.0.4/mmlab_lightning/tools/config/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 05:34:12.000000 mmlab_lightning-1.0.4/mmlab_lightning/tools/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-03 05:34:12.000000 mmlab_lightning-1.0.4/mmlab_lightning/tools/config/get_mmconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 05:34:25.739047 mmlab_lightning-1.0.4/mmlab_lightning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-03 05:34:25.000000 mmlab_lightning-1.0.4/mmlab_lightning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-03 05:34:25.000000 mmlab_lightning-1.0.4/mmlab_lightning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 05:34:25.000000 mmlab_lightning-1.0.4/mmlab_lightning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 05:34:25.000000 mmlab_lightning-1.0.4/mmlab_lightning.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-03 05:34:25.000000 mmlab_lightning-1.0.4/mmlab_lightning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 05:34:25.000000 mmlab_lightning-1.0.4/mmlab_lightning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 05:34:25.743048 mmlab_lightning-1.0.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1647 2023-05-03 05:34:12.000000 mmlab_lightning-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:41:54.200824 mmlab_lightning-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-16 09:41:43.000000 mmlab_lightning-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-16 09:41:54.200824 mmlab_lightning-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-16 09:41:43.000000 mmlab_lightning-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:41:54.196824 mmlab_lightning-1.0.5/mmlab_lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-16 09:41:43.000000 mmlab_lightning-1.0.5/mmlab_lightning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:41:54.200824 mmlab_lightning-1.0.5/mmlab_lightning/datasets/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       78 2023-05-16 09:41:43.000000 mmlab_lightning-1.0.5/mmlab_lightning/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-16 09:41:43.000000 mmlab_lightning-1.0.5/mmlab_lightning/datasets/mmlab_dataset_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:41:54.200824 mmlab_lightning-1.0.5/mmlab_lightning/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-05-16 09:41:43.000000 mmlab_lightning-1.0.5/mmlab_lightning/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-16 09:41:43.000000 mmlab_lightning-1.0.5/mmlab_lightning/models/mmlab_model_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:41:54.200824 mmlab_lightning-1.0.5/mmlab_lightning/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 09:41:43.000000 mmlab_lightning-1.0.5/mmlab_lightning/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:41:54.200824 mmlab_lightning-1.0.5/mmlab_lightning/tools/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 09:41:43.000000 mmlab_lightning-1.0.5/mmlab_lightning/tools/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-16 09:41:43.000000 mmlab_lightning-1.0.5/mmlab_lightning/tools/config/get_mmconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:41:54.196824 mmlab_lightning-1.0.5/mmlab_lightning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-16 09:41:54.000000 mmlab_lightning-1.0.5/mmlab_lightning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-16 09:41:54.000000 mmlab_lightning-1.0.5/mmlab_lightning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:41:54.000000 mmlab_lightning-1.0.5/mmlab_lightning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-16 09:41:54.000000 mmlab_lightning-1.0.5/mmlab_lightning.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 09:41:54.000000 mmlab_lightning-1.0.5/mmlab_lightning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 09:41:54.000000 mmlab_lightning-1.0.5/mmlab_lightning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 09:41:54.200824 mmlab_lightning-1.0.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1647 2023-05-16 09:41:43.000000 mmlab_lightning-1.0.5/setup.py
```

### Comparing `mmlab_lightning-1.0.4/LICENSE` & `mmlab_lightning-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mmlab_lightning-1.0.4/PKG-INFO` & `mmlab_lightning-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmlab_lightning
-Version: 1.0.4
+Version: 1.0.5
 Summary: A wrapper for mmlab repos to use in project_template.
 Home-page: https://github.com/shenmishajing/mmlab_lightning
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/mmlab_lightning
 Project-URL: Issue tracker, https://github.com/shenmishajing/mmlab_lightning/issues
```

### Comparing `mmlab_lightning-1.0.4/README.md` & `mmlab_lightning-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mmlab_lightning-1.0.4/mmlab_lightning/datasets/mmlab_dataset_adapter.py` & `mmlab_lightning-1.0.5/mmlab_lightning/datasets/mmlab_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `mmlab_lightning-1.0.4/mmlab_lightning.egg-info/PKG-INFO` & `mmlab_lightning-1.0.5/mmlab_lightning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmlab-lightning
-Version: 1.0.4
+Version: 1.0.5
 Summary: A wrapper for mmlab repos to use in project_template.
 Home-page: https://github.com/shenmishajing/mmlab_lightning
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/mmlab_lightning
 Project-URL: Issue tracker, https://github.com/shenmishajing/mmlab_lightning/issues
```

### Comparing `mmlab_lightning-1.0.4/mmlab_lightning.egg-info/SOURCES.txt` & `mmlab_lightning-1.0.5/mmlab_lightning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmlab_lightning-1.0.4/setup.py` & `mmlab_lightning-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="mmlab_lightning",
-    version="1.0.4",
+    version="1.0.5",
     description="A wrapper for mmlab repos to use in project_template.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="shenmishajing",
     author_email="shenmishajing@gmail.com",
     url="https://github.com/shenmishajing/mmlab_lightning",
     project_urls={
```

