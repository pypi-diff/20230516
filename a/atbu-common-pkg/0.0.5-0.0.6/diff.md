# Comparing `tmp/atbu-common-pkg-0.0.5.tar.gz` & `tmp/atbu-common-pkg-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atbu-common-pkg-0.0.5.tar", last modified: Tue Jul 26 04:37:42 2022, max compression
+gzip compressed data, was "atbu-common-pkg-0.0.6.tar", last modified: Tue May 16 05:31:43 2023, max compression
```

## Comparing `atbu-common-pkg-0.0.5.tar` & `atbu-common-pkg-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxrwx   0        0        0        0 2022-07-26 04:37:42.353415 atbu-common-pkg-0.0.5/
--rw-rw-rw-   0        0        0    11560 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     2419 2022-07-26 04:37:42.352410 atbu-common-pkg-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1718 2022-06-09 04:50:33.000000 atbu-common-pkg-0.0.5/README.md
--rw-rw-rw-   0        0        0      110 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-07-26 04:37:42.353415 atbu-common-pkg-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1782 2022-07-26 01:54:34.000000 atbu-common-pkg-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-26 04:37:42.288420 atbu-common-pkg-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2022-07-26 04:37:42.287416 atbu-common-pkg-0.0.5/src/atbu/
-drwxrwxrwx   0        0        0        0 2022-07-26 04:37:42.330413 atbu-common-pkg-0.0.5/src/atbu/common/
--rw-rw-rw-   0        0        0        2 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.5/src/atbu/common/__init__.py
--rw-rw-rw-   0        0        0     6142 2022-06-08 21:42:34.000000 atbu-common-pkg-0.0.5/src/atbu/common/aes_cbc.py
--rw-rw-rw-   0        0        0     8076 2022-06-09 03:13:12.000000 atbu-common-pkg-0.0.5/src/atbu/common/exception.py
--rw-rw-rw-   0        0        0     2503 2022-06-09 03:47:47.000000 atbu-common-pkg-0.0.5/src/atbu/common/hasher.py
--rw-rw-rw-   0        0        0     4223 2022-06-01 12:51:45.000000 atbu-common-pkg-0.0.5/src/atbu/common/multi_json_enc_dec.py
--rw-rw-rw-   0        0        0     3946 2022-07-26 01:57:07.000000 atbu-common-pkg-0.0.5/src/atbu/common/profile.py
--rw-rw-rw-   0        0        0     2745 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.5/src/atbu/common/simple_report.py
--rw-rw-rw-   0        0        0     1330 2022-06-01 12:51:45.000000 atbu-common-pkg-0.0.5/src/atbu/common/singleton.py
--rw-rw-rw-   0        0        0     8362 2022-07-26 01:49:30.000000 atbu-common-pkg-0.0.5/src/atbu/common/util_helpers.py
-drwxrwxrwx   0        0        0        0 2022-07-26 04:37:42.350409 atbu-common-pkg-0.0.5/src/atbu_common_pkg.egg-info/
--rw-rw-rw-   0        0        0     2419 2022-07-26 04:37:42.000000 atbu-common-pkg-0.0.5/src/atbu_common_pkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      524 2022-07-26 04:37:42.000000 atbu-common-pkg-0.0.5/src/atbu_common_pkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-26 04:37:42.000000 atbu-common-pkg-0.0.5/src/atbu_common_pkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2022-07-26 04:37:42.000000 atbu-common-pkg-0.0.5/src/atbu_common_pkg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-07-26 04:37:42.000000 atbu-common-pkg-0.0.5/src/atbu_common_pkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 05:31:43.812369 atbu-common-pkg-0.0.6/
+-rw-rw-rw-   0        0        0    11560 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2419 2023-05-16 05:31:43.811370 atbu-common-pkg-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1718 2022-06-09 04:50:33.000000 atbu-common-pkg-0.0.6/README.md
+-rw-rw-rw-   0        0        0      110 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 05:31:43.812369 atbu-common-pkg-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1782 2023-05-16 05:29:05.000000 atbu-common-pkg-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 05:31:43.762422 atbu-common-pkg-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 05:31:43.762422 atbu-common-pkg-0.0.6/src/atbu/
+drwxrwxrwx   0        0        0        0 2023-05-16 05:31:43.786374 atbu-common-pkg-0.0.6/src/atbu/common/
+-rw-rw-rw-   0        0        0        2 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.6/src/atbu/common/__init__.py
+-rw-rw-rw-   0        0        0     6142 2022-06-08 21:42:34.000000 atbu-common-pkg-0.0.6/src/atbu/common/aes_cbc.py
+-rw-rw-rw-   0        0        0     8076 2022-06-09 03:13:12.000000 atbu-common-pkg-0.0.6/src/atbu/common/exception.py
+-rw-rw-rw-   0        0        0     2503 2022-06-09 03:47:47.000000 atbu-common-pkg-0.0.6/src/atbu/common/hasher.py
+-rw-rw-rw-   0        0        0     4223 2022-06-01 12:51:45.000000 atbu-common-pkg-0.0.6/src/atbu/common/multi_json_enc_dec.py
+-rw-rw-rw-   0        0        0     3946 2022-07-26 01:57:07.000000 atbu-common-pkg-0.0.6/src/atbu/common/profile.py
+-rw-rw-rw-   0        0        0     2745 2022-06-01 12:51:37.000000 atbu-common-pkg-0.0.6/src/atbu/common/simple_report.py
+-rw-rw-rw-   0        0        0     1330 2022-06-01 12:51:45.000000 atbu-common-pkg-0.0.6/src/atbu/common/singleton.py
+-rw-rw-rw-   0        0        0     8660 2022-10-12 15:50:13.000000 atbu-common-pkg-0.0.6/src/atbu/common/util_helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-16 05:31:43.808381 atbu-common-pkg-0.0.6/src/atbu_common_pkg.egg-info/
+-rw-rw-rw-   0        0        0     2419 2023-05-16 05:31:43.000000 atbu-common-pkg-0.0.6/src/atbu_common_pkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      546 2023-05-16 05:31:43.000000 atbu-common-pkg-0.0.6/src/atbu_common_pkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 05:31:43.000000 atbu-common-pkg-0.0.6/src/atbu_common_pkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-05-16 05:31:43.000000 atbu-common-pkg-0.0.6/src/atbu_common_pkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-16 05:31:43.000000 atbu-common-pkg-0.0.6/src/atbu_common_pkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 05:31:43.809372 atbu-common-pkg-0.0.6/tests/
+-rw-rw-rw-   0        0        0     3282 2022-06-01 12:51:45.000000 atbu-common-pkg-0.0.6/tests/test_enc_dec.py
```

### Comparing `atbu-common-pkg-0.0.5/LICENSE` & `atbu-common-pkg-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.5/PKG-INFO` & `atbu-common-pkg-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atbu-common-pkg
-Version: 0.0.5
+Version: 0.0.6
 Summary: ATBU common package, common modules used by atbu.backup and atbu.mp_pipeline.
 Home-page: https://github.com/AshleyT3/atbu-common
 Author: Ashley R. Thomas
 Author-email: ashley.r.thomas.701@gmail.com
 Project-URL: Bug Tracker, https://github.com/AshleyT3/atbu-common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `atbu-common-pkg-0.0.5/README.md` & `atbu-common-pkg-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.5/setup.py` & `atbu-common-pkg-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 # read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="atbu-common-pkg",
-    version="0.0.5",
+    version="0.0.6",
     author="Ashley R. Thomas",
     author_email="ashley.r.thomas.701@gmail.com",
     description= (
         "ATBU common package, common modules used by atbu.backup and atbu.mp_pipeline."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `atbu-common-pkg-0.0.5/src/atbu/common/aes_cbc.py` & `atbu-common-pkg-0.0.6/src/atbu/common/aes_cbc.py`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.5/src/atbu/common/exception.py` & `atbu-common-pkg-0.0.6/src/atbu/common/exception.py`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.5/src/atbu/common/hasher.py` & `atbu-common-pkg-0.0.6/src/atbu/common/hasher.py`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.5/src/atbu/common/multi_json_enc_dec.py` & `atbu-common-pkg-0.0.6/src/atbu/common/multi_json_enc_dec.py`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.5/src/atbu/common/profile.py` & `atbu-common-pkg-0.0.6/src/atbu/common/profile.py`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.5/src/atbu/common/simple_report.py` & `atbu-common-pkg-0.0.6/src/atbu/common/simple_report.py`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.5/src/atbu/common/singleton.py` & `atbu-common-pkg-0.0.6/src/atbu/common/singleton.py`

 * *Files identical despite different names*

### Comparing `atbu-common-pkg-0.0.5/src/atbu/common/util_helpers.py` & `atbu-common-pkg-0.0.6/src/atbu/common/util_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,14 +132,21 @@
     if p is None:
         return p
     if not isinstance(p, str):
         p = str(p)
     return p
 
 
+def pathlib_splitdrive(path: Union[str, Path]):
+    if not isinstance(path, (str, Path)):
+        raise ValueError(f"pathlib_splitdrive: path must be str or Path: {type(path)}")
+    path_drive, path_wo_drive = os.path.splitdrive(str(path))
+    return Path(path_drive), Path(path_wo_drive)
+
+
 def is_absolute_path(path_to_dir: Union[str, Path]):
     if isinstance(path_to_dir, Path):
         path_to_dir = str(path_to_dir)
     converted_to_abs = os.path.normcase(os.path.abspath(path_to_dir).rstrip("\\/"))
     original_path = os.path.normcase(path_to_dir.rstrip("\\/"))
     return converted_to_abs == original_path
```

### Comparing `atbu-common-pkg-0.0.5/src/atbu_common_pkg.egg-info/PKG-INFO` & `atbu-common-pkg-0.0.6/src/atbu_common_pkg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atbu-common-pkg
-Version: 0.0.5
+Version: 0.0.6
 Summary: ATBU common package, common modules used by atbu.backup and atbu.mp_pipeline.
 Home-page: https://github.com/AshleyT3/atbu-common
 Author: Ashley R. Thomas
 Author-email: ashley.r.thomas.701@gmail.com
 Project-URL: Bug Tracker, https://github.com/AshleyT3/atbu-common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

