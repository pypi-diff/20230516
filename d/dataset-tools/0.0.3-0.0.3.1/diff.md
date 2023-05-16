# Comparing `tmp/dataset-tools-0.0.3.tar.gz` & `tmp/dataset-tools-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset-tools-0.0.3.tar", last modified: Tue May 16 12:23:19 2023, max compression
+gzip compressed data, was "dataset-tools-0.0.3.1.tar", last modified: Tue May 16 12:46:58 2023, max compression
```

## Comparing `dataset-tools-0.0.3.tar` & `dataset-tools-0.0.3.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:23:19.570404 dataset-tools-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-16 12:23:19.570404 dataset-tools-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:23:19.566403 dataset-tools-0.0.3/dataset_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:23:19.566403 dataset-tools-0.0.3/dataset_tools/image/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:23:19.566403 dataset-tools-0.0.3/dataset_tools/image/renders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/renders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/renders/poster.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/renders/previews.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/renders/separated_anns_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/renders/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:23:19.566403 dataset-tools-0.0.3/dataset_tools/image/stats/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/stats/class_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/stats/class_cooccurrence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/stats/classes_per_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/stats/heatmaps_for_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/stats/object_and_class_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/stats/objects_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/dataset_tools/image/stats/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:23:19.566403 dataset-tools-0.0.3/dataset_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-16 12:23:19.000000 dataset-tools-0.0.3/dataset_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-16 12:23:19.000000 dataset-tools-0.0.3/dataset_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:23:19.000000 dataset-tools-0.0.3/dataset_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-16 12:23:19.000000 dataset-tools-0.0.3/dataset_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 12:23:19.000000 dataset-tools-0.0.3/dataset_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 12:23:19.570404 dataset-tools-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-16 12:20:26.000000 dataset-tools-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:46:58.017188 dataset-tools-0.0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 12:44:15.000000 dataset-tools-0.0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-16 12:46:58.017188 dataset-tools-0.0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 12:44:15.000000 dataset-tools-0.0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:46:58.013188 dataset-tools-0.0.3.1/dataset_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-16 12:44:15.000000 dataset-tools-0.0.3.1/dataset_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:46:58.013188 dataset-tools-0.0.3.1/dataset_tools/image/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-16 12:44:15.000000 dataset-tools-0.0.3.1/dataset_tools/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:46:58.013188 dataset-tools-0.0.3.1/dataset_tools/image/renders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:44:15.000000 dataset-tools-0.0.3.1/dataset_tools/image/renders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-05-16 12:44:15.000000 dataset-tools-0.0.3.1/dataset_tools/image/renders/poster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-16 12:44:15.000000 dataset-tools-0.0.3.1/dataset_tools/image/renders/previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-16 12:44:15.000000 dataset-tools-0.0.3.1/dataset_tools/image/renders/separated_anns_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-16 12:44:15.000000 dataset-tools-0.0.3.1/dataset_tools/image/renders/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:46:58.017188 dataset-tools-0.0.3.1/dataset_tools/image/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 12:44:15.000000 dataset-tools-0.0.3.1/dataset_tools/image/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-05-16 12:44:15.000000 dataset-tools-0.0.3.1/dataset_tools/image/stats/class_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-16 12:44:15.000000 dataset-tools-0.0.3.1/dataset_tools/image/stats/class_cooccurrence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-16 12:44:15.000000 dataset-tools-0.0.3.1/dataset_tools/image/stats/classes_per_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-16 12:44:15.000000 dataset-tools-0.0.3.1/dataset_tools/image/stats/heatmaps_for_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-05-16 12:44:15.000000 dataset-tools-0.0.3.1/dataset_tools/image/stats/object_and_class_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-16 12:44:15.000000 dataset-tools-0.0.3.1/dataset_tools/image/stats/objects_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-16 12:44:15.000000 dataset-tools-0.0.3.1/dataset_tools/image/stats/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:46:58.013188 dataset-tools-0.0.3.1/dataset_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-16 12:46:58.000000 dataset-tools-0.0.3.1/dataset_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-16 12:46:58.000000 dataset-tools-0.0.3.1/dataset_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:46:58.000000 dataset-tools-0.0.3.1/dataset_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-16 12:46:58.000000 dataset-tools-0.0.3.1/dataset_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 12:46:58.000000 dataset-tools-0.0.3.1/dataset_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-16 12:44:15.000000 dataset-tools-0.0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 12:46:58.017188 dataset-tools-0.0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-16 12:44:15.000000 dataset-tools-0.0.3.1/setup.py
```

### Comparing `dataset-tools-0.0.3/LICENSE` & `dataset-tools-0.0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.3/PKG-INFO` & `dataset-tools-0.0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-tools
-Version: 0.0.3
+Version: 0.0.3.1
 Summary: Dataset tools for dataset ninja made by Supervisely team.
 Home-page: https://github.com/supervisely/dataset-tools
 Author: Supervisely
 Author-email: support@supervise.ly
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dataset-tools-0.0.3/dataset_tools/__init__.py` & `dataset-tools-0.0.3.1/dataset_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.3/dataset_tools/image/renders/poster.py` & `dataset-tools-0.0.3.1/dataset_tools/image/renders/poster.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.3/dataset_tools/image/renders/previews.py` & `dataset-tools-0.0.3.1/dataset_tools/image/renders/previews.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.3/dataset_tools/image/renders/separated_anns_grid.py` & `dataset-tools-0.0.3.1/dataset_tools/image/renders/separated_anns_grid.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.3/dataset_tools/image/renders/wrapper.py` & `dataset-tools-0.0.3.1/dataset_tools/image/renders/wrapper.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.3/dataset_tools/image/stats/class_balance.py` & `dataset-tools-0.0.3.1/dataset_tools/image/stats/class_balance.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.3/dataset_tools/image/stats/class_cooccurrence.py` & `dataset-tools-0.0.3.1/dataset_tools/image/stats/class_cooccurrence.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.3/dataset_tools/image/stats/classes_per_image.py` & `dataset-tools-0.0.3.1/dataset_tools/image/stats/classes_per_image.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.3/dataset_tools/image/stats/heatmaps_for_classes.py` & `dataset-tools-0.0.3.1/dataset_tools/image/stats/heatmaps_for_classes.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.3/dataset_tools/image/stats/object_and_class_sizes.py` & `dataset-tools-0.0.3.1/dataset_tools/image/stats/object_and_class_sizes.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.3/dataset_tools/image/stats/objects_distribution.py` & `dataset-tools-0.0.3.1/dataset_tools/image/stats/objects_distribution.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.3/dataset_tools/image/stats/wrapper.py` & `dataset-tools-0.0.3.1/dataset_tools/image/stats/wrapper.py`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.3/dataset_tools.egg-info/PKG-INFO` & `dataset-tools-0.0.3.1/dataset_tools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-tools
-Version: 0.0.3
+Version: 0.0.3.1
 Summary: Dataset tools for dataset ninja made by Supervisely team.
 Home-page: https://github.com/supervisely/dataset-tools
 Author: Supervisely
 Author-email: support@supervise.ly
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dataset-tools-0.0.3/dataset_tools.egg-info/SOURCES.txt` & `dataset-tools-0.0.3.1/dataset_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataset-tools-0.0.3/setup.py` & `dataset-tools-0.0.3.1/setup.py`

 * *Files identical despite different names*

