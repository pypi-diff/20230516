# Comparing `tmp/sinetstream-type-image-1.7.0.tar.gz` & `tmp/sinetstream-type-image-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinetstream-type-image-1.7.0.tar", last modified: Fri Sep 16 07:09:25 2022, max compression
+gzip compressed data, was "sinetstream-type-image-1.8.0.tar", last modified: Tue May 16 06:36:43 2023, max compression
```

## Comparing `sinetstream-type-image-1.7.0.tar` & `sinetstream-type-image-1.8.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2022-09-16 07:09:25.645435 sinetstream-type-image-1.7.0/
--rw-rw-r--   0 koie      (1004) koie      (1004)      596 2022-09-16 07:09:25.645435 sinetstream-type-image-1.7.0/PKG-INFO
--rw-rw-r--   0 koie      (1004) koie      (1004)     1523 2022-09-16 07:09:25.645435 sinetstream-type-image-1.7.0/setup.cfg
--rw-rw-r--   0 koie      (1004) koie      (1004)       39 2022-09-15 07:30:59.000000 sinetstream-type-image-1.7.0/setup.py
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2022-09-16 07:09:25.641435 sinetstream-type-image-1.7.0/src/
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2022-09-16 07:09:25.645435 sinetstream-type-image-1.7.0/src/sinetstream_type_image.egg-info/
--rw-rw-r--   0 koie      (1004) koie      (1004)      596 2022-09-16 07:09:25.000000 sinetstream-type-image-1.7.0/src/sinetstream_type_image.egg-info/PKG-INFO
--rw-rw-r--   0 koie      (1004) koie      (1004)      469 2022-09-16 07:09:25.000000 sinetstream-type-image-1.7.0/src/sinetstream_type_image.egg-info/SOURCES.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)        1 2022-09-16 07:09:25.000000 sinetstream-type-image-1.7.0/src/sinetstream_type_image.egg-info/dependency_links.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)       83 2022-09-16 07:09:25.000000 sinetstream-type-image-1.7.0/src/sinetstream_type_image.egg-info/entry_points.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)       18 2022-09-16 07:09:25.000000 sinetstream-type-image-1.7.0/src/sinetstream_type_image.egg-info/namespace_packages.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)        1 2022-09-16 07:07:24.000000 sinetstream-type-image-1.7.0/src/sinetstream_type_image.egg-info/not-zip-safe
--rw-rw-r--   0 koie      (1004) koie      (1004)      107 2022-09-16 07:09:25.000000 sinetstream-type-image-1.7.0/src/sinetstream_type_image.egg-info/requires.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)       18 2022-09-16 07:09:25.000000 sinetstream-type-image-1.7.0/src/sinetstream_type_image.egg-info/top_level.txt
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2022-09-16 07:09:25.641435 sinetstream-type-image-1.7.0/src/sinetstreamplugin/
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2022-09-16 07:09:25.645435 sinetstream-type-image-1.7.0/src/sinetstreamplugin/valuetype/
--rw-rw-r--   0 koie      (1004) koie      (1004)     1934 2022-09-15 07:30:59.000000 sinetstream-type-image-1.7.0/src/sinetstreamplugin/valuetype/image.py
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:36:43.434529 sinetstream-type-image-1.8.0/
+-rw-rw-r--   0 koie      (1004) koie      (1004)      557 2023-05-16 06:36:43.434529 sinetstream-type-image-1.8.0/PKG-INFO
+-rw-rw-r--   0 koie      (1004) koie      (1004)     1530 2023-05-16 06:36:43.434529 sinetstream-type-image-1.8.0/setup.cfg
+-rw-rw-r--   0 koie      (1004) koie      (1004)       39 2023-01-12 00:12:25.000000 sinetstream-type-image-1.8.0/setup.py
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:36:43.430529 sinetstream-type-image-1.8.0/src/
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:36:43.434529 sinetstream-type-image-1.8.0/src/sinetstream_type_image.egg-info/
+-rw-rw-r--   0 koie      (1004) koie      (1004)      557 2023-05-16 06:36:43.000000 sinetstream-type-image-1.8.0/src/sinetstream_type_image.egg-info/PKG-INFO
+-rw-rw-r--   0 koie      (1004) koie      (1004)      469 2023-05-16 06:36:43.000000 sinetstream-type-image-1.8.0/src/sinetstream_type_image.egg-info/SOURCES.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-05-16 06:36:43.000000 sinetstream-type-image-1.8.0/src/sinetstream_type_image.egg-info/dependency_links.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)       82 2023-05-16 06:36:43.000000 sinetstream-type-image-1.8.0/src/sinetstream_type_image.egg-info/entry_points.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)       18 2023-05-16 06:36:43.000000 sinetstream-type-image-1.8.0/src/sinetstream_type_image.egg-info/namespace_packages.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-01-12 00:15:53.000000 sinetstream-type-image-1.8.0/src/sinetstream_type_image.egg-info/not-zip-safe
+-rw-rw-r--   0 koie      (1004) koie      (1004)      107 2023-05-16 06:36:43.000000 sinetstream-type-image-1.8.0/src/sinetstream_type_image.egg-info/requires.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)       18 2023-05-16 06:36:43.000000 sinetstream-type-image-1.8.0/src/sinetstream_type_image.egg-info/top_level.txt
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:36:43.430529 sinetstream-type-image-1.8.0/src/sinetstreamplugin/
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:36:43.434529 sinetstream-type-image-1.8.0/src/sinetstreamplugin/valuetype/
+-rw-rw-r--   0 koie      (1004) koie      (1004)     1934 2023-01-12 00:12:25.000000 sinetstream-type-image-1.8.0/src/sinetstreamplugin/valuetype/image.py
```

### Comparing `sinetstream-type-image-1.7.0/PKG-INFO` & `sinetstream-type-image-1.8.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: sinetstream-type-image
-Version: 1.7.0
+Version: 1.8.0
 Summary: Image Type plugin for SINETStream library
 Home-page: https://github.com/nii-gakunin-cloud/sinetstream
 License: Apache License, Version 2.0
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
```

### Comparing `sinetstream-type-image-1.7.0/setup.cfg` & `sinetstream-type-image-1.8.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sinetstream-type-image
-version = 1.7.0
+version = 1.8.0
 description = Image Type plugin for SINETStream library
 license = Apache License, Version 2.0
 license_files = 
 	../../../../LICENSE
 url = https://github.com/nii-gakunin-cloud/sinetstream
 classifiers = 
 	Development Status :: 4 - Beta
@@ -16,24 +16,24 @@
 
 [options]
 package_dir = 
 	=src
 packages = find_namespace:
 zip_safe = False
 install_requires = 
-	sinetstream>=1.7.0
+	sinetstream>=1.8.0
 	opencv-python
 	numpy<1.22.0;python_version<'3.8'
 	numpy;python_version>='3.8'
 tests_require = 
 	pytest
 	pytest-cov
 	pytest-flake8
 	pytest-timeout
-	pytest-html
+	pytest-html==3.2.0
 	flake8>=4.0.0,<5.0.0  # workaround: https://github.com/tholo/pytest-flake8/issues/87
 setup_requires = 
 	pytest-runner
 namespace_packages = 
 	sinetstreamplugin
 python_requires = >= 3.7
```

### Comparing `sinetstream-type-image-1.7.0/src/sinetstream_type_image.egg-info/PKG-INFO` & `sinetstream-type-image-1.8.0/src/sinetstream_type_image.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: sinetstream-type-image
-Version: 1.7.0
+Version: 1.8.0
 Summary: Image Type plugin for SINETStream library
 Home-page: https://github.com/nii-gakunin-cloud/sinetstream
 License: Apache License, Version 2.0
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
```

### Comparing `sinetstream-type-image-1.7.0/src/sinetstreamplugin/valuetype/image.py` & `sinetstream-type-image-1.8.0/src/sinetstreamplugin/valuetype/image.py`

 * *Files identical despite different names*

