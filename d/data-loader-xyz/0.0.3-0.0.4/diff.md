# Comparing `tmp/data_loader_xyz-0.0.3.tar.gz` & `tmp/data_loader_xyz-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_loader_xyz-0.0.3.tar", last modified: Tue May 16 14:42:40 2023, max compression
+gzip compressed data, was "data_loader_xyz-0.0.4.tar", last modified: Tue May 16 16:12:07 2023, max compression
```

## Comparing `data_loader_xyz-0.0.3.tar` & `data_loader_xyz-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 14:42:40.324062 data_loader_xyz-0.0.3/
--rw-rw-r--   0 zied      (1000) zied      (1000)     1073 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.3/LICENCE
--rw-rw-r--   0 zied      (1000) zied      (1000)     4061 2023-05-16 14:42:40.324062 data_loader_xyz-0.0.3/PKG-INFO
--rw-rw-r--   0 zied      (1000) zied      (1000)     3357 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.3/README.md
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 14:42:40.320062 data_loader_xyz-0.0.3/configs/
--rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.3/configs/__init__.py
--rw-rw-r--   0 zied      (1000) zied      (1000)      237 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.3/configs/base_config.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 14:42:40.320062 data_loader_xyz-0.0.3/data_loader_xyz/
--rw-rw-r--   0 zied      (1000) zied      (1000)       51 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.3/data_loader_xyz/__init__.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 14:42:40.324062 data_loader_xyz-0.0.3/data_loader_xyz/src/
--rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.3/data_loader_xyz/src/__init__.py
--rw-rw-r--   0 zied      (1000) zied      (1000)     2807 2023-05-16 14:41:10.000000 data_loader_xyz-0.0.3/data_loader_xyz/src/mount.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 14:42:40.324062 data_loader_xyz-0.0.3/data_loader_xyz.egg-info/
--rw-rw-r--   0 zied      (1000) zied      (1000)     4061 2023-05-16 14:42:40.000000 data_loader_xyz-0.0.3/data_loader_xyz.egg-info/PKG-INFO
--rw-rw-r--   0 zied      (1000) zied      (1000)      444 2023-05-16 14:42:40.000000 data_loader_xyz-0.0.3/data_loader_xyz.egg-info/SOURCES.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)        1 2023-05-16 14:42:40.000000 data_loader_xyz-0.0.3/data_loader_xyz.egg-info/dependency_links.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       62 2023-05-16 14:42:40.000000 data_loader_xyz-0.0.3/data_loader_xyz.egg-info/entry_points.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       34 2023-05-16 14:42:40.000000 data_loader_xyz-0.0.3/data_loader_xyz.egg-info/requires.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       82 2023-05-16 14:42:40.000000 data_loader_xyz-0.0.3/data_loader_xyz.egg-info/top_level.txt
--rw-rw-r--   0 zied      (1000) zied      (1000)       79 2023-05-16 14:42:40.324062 data_loader_xyz-0.0.3/setup.cfg
--rw-rw-r--   0 zied      (1000) zied      (1000)     2019 2023-05-16 13:44:07.000000 data_loader_xyz-0.0.3/setup.py
-drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 14:42:40.320062 data_loader_xyz-0.0.3/utils/
--rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.3/utils/__init__.py
--rw-rw-r--   0 zied      (1000) zied      (1000)     1758 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.3/utils/util.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 16:12:07.901656 data_loader_xyz-0.0.4/
+-rw-rw-r--   0 zied      (1000) zied      (1000)     1073 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.4/LICENCE
+-rw-rw-r--   0 zied      (1000) zied      (1000)     4061 2023-05-16 16:12:07.901656 data_loader_xyz-0.0.4/PKG-INFO
+-rw-rw-r--   0 zied      (1000) zied      (1000)     3357 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.4/README.md
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 16:12:07.897656 data_loader_xyz-0.0.4/configs/
+-rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.4/configs/__init__.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)      237 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.4/configs/base_config.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 16:12:07.897656 data_loader_xyz-0.0.4/data_loader_xyz/
+-rw-rw-r--   0 zied      (1000) zied      (1000)       51 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.4/data_loader_xyz/__init__.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 16:12:07.901656 data_loader_xyz-0.0.4/data_loader_xyz/src/
+-rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.4/data_loader_xyz/src/__init__.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)     4877 2023-05-16 16:11:56.000000 data_loader_xyz-0.0.4/data_loader_xyz/src/mount.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 16:12:07.901656 data_loader_xyz-0.0.4/data_loader_xyz.egg-info/
+-rw-rw-r--   0 zied      (1000) zied      (1000)     4061 2023-05-16 16:12:07.000000 data_loader_xyz-0.0.4/data_loader_xyz.egg-info/PKG-INFO
+-rw-rw-r--   0 zied      (1000) zied      (1000)      444 2023-05-16 16:12:07.000000 data_loader_xyz-0.0.4/data_loader_xyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)        1 2023-05-16 16:12:07.000000 data_loader_xyz-0.0.4/data_loader_xyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       62 2023-05-16 16:12:07.000000 data_loader_xyz-0.0.4/data_loader_xyz.egg-info/entry_points.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       34 2023-05-16 16:12:07.000000 data_loader_xyz-0.0.4/data_loader_xyz.egg-info/requires.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       82 2023-05-16 16:12:07.000000 data_loader_xyz-0.0.4/data_loader_xyz.egg-info/top_level.txt
+-rw-rw-r--   0 zied      (1000) zied      (1000)       79 2023-05-16 16:12:07.901656 data_loader_xyz-0.0.4/setup.cfg
+-rw-rw-r--   0 zied      (1000) zied      (1000)     2019 2023-05-16 13:44:07.000000 data_loader_xyz-0.0.4/setup.py
+drwxrwxr-x   0 zied      (1000) zied      (1000)        0 2023-05-16 16:12:07.897656 data_loader_xyz-0.0.4/utils/
+-rw-rw-r--   0 zied      (1000) zied      (1000)        0 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.4/utils/__init__.py
+-rw-rw-r--   0 zied      (1000) zied      (1000)     1758 2023-05-16 13:34:50.000000 data_loader_xyz-0.0.4/utils/util.py
```

### Comparing `data_loader_xyz-0.0.3/LICENCE` & `data_loader_xyz-0.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `data_loader_xyz-0.0.3/PKG-INFO` & `data_loader_xyz-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_loader_xyz
-Version: 0.0.3
+Version: 0.0.4
 Summary: to work with aws S3
 Home-page: https://github.com/Proxia-ai/data_loader
 Author: Zied
 Author-email: ziedici@gmail.com
 License: BSD
 Project-URL: url0, https://github.com/Proxia-ai/
 Keywords: working with aws S3
```

### Comparing `data_loader_xyz-0.0.3/README.md` & `data_loader_xyz-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `data_loader_xyz-0.0.3/data_loader_xyz.egg-info/PKG-INFO` & `data_loader_xyz-0.0.4/data_loader_xyz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-loader-xyz
-Version: 0.0.3
+Version: 0.0.4
 Summary: to work with aws S3
 Home-page: https://github.com/Proxia-ai/data_loader
 Author: Zied
 Author-email: ziedici@gmail.com
 License: BSD
 Project-URL: url0, https://github.com/Proxia-ai/
 Keywords: working with aws S3
```

### Comparing `data_loader_xyz-0.0.3/setup.py` & `data_loader_xyz-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `data_loader_xyz-0.0.3/utils/util.py` & `data_loader_xyz-0.0.4/utils/util.py`

 * *Files identical despite different names*

